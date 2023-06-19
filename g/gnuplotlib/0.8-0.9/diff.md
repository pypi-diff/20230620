# Comparing `tmp/gnuplotlib-0.8.tar.gz` & `tmp/gnuplotlib-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gnuplotlib-0.8.tar", last modified: Thu Oct 15 03:11:03 2015, max compression
+gzip compressed data, was "dist/gnuplotlib-0.9.tar", last modified: Sun Nov 15 05:59:52 2015, max compression
```

## Comparing `gnuplotlib-0.8.tar` & `gnuplotlib-0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2015-10-15 03:11:03.000000 gnuplotlib-0.8/
--rw-r--r--   0 dima      (1000) dima      (1000)    23791 2015-10-15 03:10:24.000000 gnuplotlib-0.8/README.org
--rw-r--r--   0 dima      (1000) dima      (1000)      251 2015-10-15 03:11:03.000000 gnuplotlib-0.8/PKG-INFO
--rwxr-xr-x   0 dima      (1000) dima      (1000)      662 2015-10-15 03:10:45.000000 gnuplotlib-0.8/setup.py
-lrwxrwxrwx   0 dima      (1000) dima      (1000)        0 2015-10-13 19:48:06.000000 gnuplotlib-0.8/README -> README.org
--rwxr-xr-x   0 dima      (1000) dima      (1000)    70698 2015-10-15 03:10:03.000000 gnuplotlib-0.8/gnuplotlib.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2015-11-15 05:59:52.000000 gnuplotlib-0.9/
+-rw-r--r--   0 dima      (1000) dima      (1000)    26535 2015-11-14 10:46:48.000000 gnuplotlib-0.9/README.org
+-rw-r--r--   0 dima      (1000) dima      (1000)      251 2015-11-15 05:59:52.000000 gnuplotlib-0.9/PKG-INFO
+-rwxr-xr-x   0 dima      (1000) dima      (1000)      662 2015-11-14 10:23:33.000000 gnuplotlib-0.9/setup.py
+lrwxrwxrwx   0 dima      (1000) dima      (1000)        0 2015-11-14 10:46:48.000000 gnuplotlib-0.9/README -> README.org
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    74120 2015-11-14 10:23:33.000000 gnuplotlib-0.9/gnuplotlib.py
```

### Comparing `gnuplotlib-0.8/README.org` & `gnuplotlib-0.9/README.org`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,16 @@
 
 Plot generation is controlled by two sets of options:
 
 - Plot options: parameters that affect the whole plot, like the title of the
   plot, the axis labels, the extents, 2d/3d selection, etc. All the plot options
   are described below in "Plot options".
 
-- Curve options: parameters that affect only a single curve
+- Curve options: parameters that affect only a single curve. Each is described
+  below in "Curve options".
 
 ** Data arguments
 
 The 'curve' arguments in the plot(...) argument list represent the actual data
 being plotted. Each output data point is a tuple (set of values, not a python
 "tuple") whose size varies depending on what is being plotted. For example if
 we're making a simple 2D x-y plot, each tuple has 2 values; if we're making a 3d
@@ -217,14 +218,77 @@
 
 Also note that the 'tuplesize' curve option is independent of implicit domains.
 This option specifies not how many data arrays we have, but how many values
 represent each data point. For example, if we want a 2D line plot with varying
 colors plotted with an implicit domain, set tuplesize=3 as before (x,y,color),
 but pass in only 2 arrays (y, color).
 
+** Symbolic equations
+
+Gnuplot can plot both data and equations. This module exists largely for the
+data-plotting case, but sometimes it can be useful to plot equations together
+with some data. This is supported by the 'equation' plot option. This plot
+option is either a string (for a single equation) or a list/tuple containing
+multiple strings for multiple equations. Note that plotting only equations
+without data is not supported (and generally is better done with gnuplot
+directly). An example:
+
+#+BEGIN_SRC python
+ import numpy as np
+ import numpy.random as nr
+ import numpy.linalg
+ import gnuplotlib as gp
+
+ # generate data
+ x     = np.arange(100)
+ c     = np.array([1, 1800, -100, 0.8])   # coefficients
+ m     = x[:, np.newaxis] ** np.arange(4) # 1, x, x**2, ...
+ noise = 1e4 * nr.random(x.shape)
+ y     = np.dot( m, c) + noise            # polynomial corrupted by noise
+
+ c_fit = np.dot(numpy.linalg.pinv(m), y)  # coefficients obtained by a curve fit
+
+ # generate a string that describes the curve-fitted equation
+ fit_equation = '+'.join( '{} * {}'.format(c,m) for c,m in zip( c_fit.tolist(), ('x**0','x**1','x**2','x**3')))
+
+ # plot the data points and the fitted curve
+ gp.plot(x, y, _with='points', equation = fit_equation)
+#+END_SRC
+
+Here I generated some data, performed a curve fit to it, and plotted the data
+points together with the best-fitting curve. Here the best-fitting curve was
+plotted by gnuplot as an equation, so gnuplot was free to choose the proper
+sampling frequency. And as we zoom around the plot, the sampling frequency is
+adjusted to keep things looking nice.
+
+Note that the various styles and options set by the other options do NOT apply
+to these equation plots. Instead, the string is passed to gnuplot directly, and
+any styling can be applied there. For instance, to plot a parabola with thick
+lines, you can issue
+
+#+BEGIN_SRC python
+ gp.plot( ....., equation = 'x**2 with lines linewidth 2')
+#+END_SRC
+
+As before, see the gnuplot documentation for details. You can also do fancy
+things:
+
+#+BEGIN_SRC python
+ x   = np.arange(100, dtype=float) / 100 * np.pi * 2;
+ c,s = np.cos(x), np.sin(x)
+
+ gp.plot( c,s,
+          square=1, _with='points',
+          set = ('parametric', 'trange [0:2*3.14]'),
+          equation = "sin(t),cos(t)" )
+#+END_SRC
+
+Here the data are points evently spaced around a unit circle. Along with these
+points we plot a unit circle as a parametric equation.
+
 ** Interactivity
 
 The graphical backends of Gnuplot are interactive, allowing the user to pan,
 zoom, rotate and measure the data in the plot window. See the Gnuplot
 documentation for details about how to do this. Some terminals (such as wxt) are
 persistently interactive, and the rest of this section does not apply to them.
 Other terminals (such as x11) have the downside described here.
@@ -299,14 +363,21 @@
 The 'cb' axis represents the color axis, used when color-coded plots are being
 generated
 
 - xlabel, ylabel, zlabel, y2label
 
 These specify axis labels
 
+- equation
+
+This option allows equations represented as formula strings to be plotted along
+with data passed in as numpy arrays. This can be a string (for a single
+equation) or an array/tuple of strings (for multiple equations). See the
+"Symbolic equations" section above.
+
 - hardcopy
 
 Instead of drawing a plot on screen, plot into a file instead. The output
 filename is the value associated with this key. The output format is inferred
 from the filename. Currently only eps, ps, pdf, png, svg are supported with some
 default sets of options. This option is simply a shorthand for the 'terminal'
 and 'output' options. If the defaults provided by the 'hardcopy' option are
```

### Comparing `gnuplotlib-0.8/setup.py` & `gnuplotlib-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class MoreClean(clean):
     def run(self):
         clean.run(self)
         subprocess.call( ['make', 'clean'] )
 
 
 setup(name         = 'gnuplotlib',
-      version      = '0.8',
+      version      = '0.9',
       author       = 'Dima Kogan',
       author_email = 'dima@secretsauce.net',
       url          = 'http://github.com/dkogan/gnuplotlib',
       description  = 'Gnuplot-based plotting for numpy',
       license      = 'LGPL-3+',
       py_modules   = ['gnuplotlib'],
       cmdclass     = {'clean': MoreClean})
```

### Comparing `gnuplotlib-0.8/gnuplotlib.py` & `gnuplotlib-0.9/gnuplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 
 Plot generation is controlled by two sets of options:
 
 - Plot options: parameters that affect the whole plot, like the title of the
   plot, the axis labels, the extents, 2d/3d selection, etc. All the plot options
   are described below in "Plot options".
 
-- Curve options: parameters that affect only a single curve
+- Curve options: parameters that affect only a single curve. Each is described
+  below in "Curve options".
 
 ** Data arguments
 
 The 'curve' arguments in the plot(...) argument list represent the actual data
 being plotted. Each output data point is a tuple (set of values, not a python
 "tuple") whose size varies depending on what is being plotted. For example if
 we're making a simple 2D x-y plot, each tuple has 2 values; if we're making a 3d
@@ -220,14 +221,77 @@
 
 Also note that the 'tuplesize' curve option is independent of implicit domains.
 This option specifies not how many data arrays we have, but how many values
 represent each data point. For example, if we want a 2D line plot with varying
 colors plotted with an implicit domain, set tuplesize=3 as before (x,y,color),
 but pass in only 2 arrays (y, color).
 
+** Symbolic equations
+
+Gnuplot can plot both data and equations. This module exists largely for the
+data-plotting case, but sometimes it can be useful to plot equations together
+with some data. This is supported by the 'equation' plot option. This plot
+option is either a string (for a single equation) or a list/tuple containing
+multiple strings for multiple equations. Note that plotting only equations
+without data is not supported (and generally is better done with gnuplot
+directly). An example:
+
+#+BEGIN_SRC python
+ import numpy as np
+ import numpy.random as nr
+ import numpy.linalg
+ import gnuplotlib as gp
+
+ # generate data
+ x     = np.arange(100)
+ c     = np.array([1, 1800, -100, 0.8])   # coefficients
+ m     = x[:, np.newaxis] ** np.arange(4) # 1, x, x**2, ...
+ noise = 1e4 * nr.random(x.shape)
+ y     = np.dot( m, c) + noise            # polynomial corrupted by noise
+
+ c_fit = np.dot(numpy.linalg.pinv(m), y)  # coefficients obtained by a curve fit
+
+ # generate a string that describes the curve-fitted equation
+ fit_equation = '+'.join( '{} * {}'.format(c,m) for c,m in zip( c_fit.tolist(), ('x**0','x**1','x**2','x**3')))
+
+ # plot the data points and the fitted curve
+ gp.plot(x, y, _with='points', equation = fit_equation)
+#+END_SRC
+
+Here I generated some data, performed a curve fit to it, and plotted the data
+points together with the best-fitting curve. Here the best-fitting curve was
+plotted by gnuplot as an equation, so gnuplot was free to choose the proper
+sampling frequency. And as we zoom around the plot, the sampling frequency is
+adjusted to keep things looking nice.
+
+Note that the various styles and options set by the other options do NOT apply
+to these equation plots. Instead, the string is passed to gnuplot directly, and
+any styling can be applied there. For instance, to plot a parabola with thick
+lines, you can issue
+
+#+BEGIN_SRC python
+ gp.plot( ....., equation = 'x**2 with lines linewidth 2')
+#+END_SRC
+
+As before, see the gnuplot documentation for details. You can also do fancy
+things:
+
+#+BEGIN_SRC python
+ x   = np.arange(100, dtype=float) / 100 * np.pi * 2;
+ c,s = np.cos(x), np.sin(x)
+
+ gp.plot( c,s,
+          square=1, _with='points',
+          set = ('parametric', 'trange [0:2*3.14]'),
+          equation = "sin(t),cos(t)" )
+#+END_SRC
+
+Here the data are points evently spaced around a unit circle. Along with these
+points we plot a unit circle as a parametric equation.
+
 ** Interactivity
 
 The graphical backends of Gnuplot are interactive, allowing the user to pan,
 zoom, rotate and measure the data in the plot window. See the Gnuplot
 documentation for details about how to do this. Some terminals (such as wxt) are
 persistently interactive, and the rest of this section does not apply to them.
 Other terminals (such as x11) have the downside described here.
@@ -302,14 +366,21 @@
 The 'cb' axis represents the color axis, used when color-coded plots are being
 generated
 
 - xlabel, ylabel, zlabel, y2label
 
 These specify axis labels
 
+- equation
+
+This option allows equations represented as formula strings to be plotted along
+with data passed in as numpy arrays. This can be a string (for a single
+equation) or an array/tuple of strings (for multiple equations). See the
+"Symbolic equations" section above.
+
 - hardcopy
 
 Instead of drawing a plot on screen, plot into a file instead. The output
 filename is the value associated with this key. The output format is inferred
 from the filename. Currently only eps, ps, pdf, png, svg are supported with some
 default sets of options. This option is simply a shorthand for the 'terminal'
 and 'output' options. If the defaults provided by the 'hardcopy' option are
@@ -713,15 +784,15 @@
 import numpy as np
 
 
 # note that 'with' is both a known plot and curve option
 knownPlotOptions = frozenset(('3d', 'dump', 'ascii', 'log',
                               'cmds', 'set', 'unset', 'square', 'square_xy', 'title',
                               'hardcopy', 'terminal', 'output',
-                              'with',
+                              'with', 'equation',
                               'xmax',  'xmin',  'xrange',  'xinv',  'xlabel',
                               'y2max', 'y2min', 'y2range', 'y2inv', 'y2label',
                               'ymax',  'ymin',  'yrange',  'yinv',  'ylabel',
                               'zmax',  'zmin',  'zrange',  'zinv',  'zlabel',
                               'cbmin', 'cbmax', 'cbrange'))
 
 knownCurveOptions = frozenset(('legend', 'y2', 'with', 'tuplesize'))
@@ -970,16 +1041,21 @@
                              'png': 'png size 1280,1024',
                              'svg': 'svg enhanced solid'}
 
             self.plotOptions['terminal'] = terminalOpts[outputfileType]
             self.plotOptions['output']   = outputfile
 
 
-        if 'terminal' in self.plotOptions and not 'output' in self.plotOptions:
-            sys.stderr.write('Warning: defined gnuplot terminal, but NOT an output file. Is this REALLY what you want?\n')
+        if 'terminal' in self.plotOptions:
+            if self.plotOptions['terminal'] in ('x11', 'wxt', 'qt', 'aquaterm'):
+                if 'output' in self.plotOptions:
+                    sys.stderr.write("Warning: requested a known-interactive gnuplot terminal AND an output file. Is this REALLY what you want?\n")
+            else:
+                if not 'output' in self.plotOptions:
+                    sys.stderr.write("Warning: requested a gnuplot terminal (not a known-interactive one), but NOT an output file. Is this REALLY what you want?\n")
 
         # add the extra global options
         if 'cmds' in self.plotOptions:
             # if there's a single cmds option, put it into a 1-element list to
             # make the processing work
             if isinstance(self.plotOptions['cmds'], (list, tuple)):
                 cmds += self.plotOptions['cmds']
@@ -1319,14 +1395,21 @@
 
             basecmd += "set ytics nomirror\n"
             basecmd += "set y2tics\n"
 
         if self.plotOptions.get('3d'): basecmd += 'splot '
         else:                          basecmd += 'plot '
 
+        # send all equations
+        if 'equation' in self.plotOptions:
+            if isinstance(self.plotOptions['equation'], (list, tuple)):
+                basecmd += ''.join( eq + ', ' for eq in self.plotOptions['equation'])
+            else:
+                basecmd += self.plotOptions['equation'] + ', '
+
         plotCurveCmds        = []
         plotCurveCmdsMinimal = [] # same as above, but with a single data point per plot only
         testData             = '' # data to make a minimal plot
 
         for curve in curves:
             optioncmds = optioncmd(curve)
```

