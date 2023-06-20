# Comparing `tmp/np2mcpl-0.0.1.tar.gz` & `tmp/np2mcpl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np2mcpl-0.0.1.tar", last modified: Mon Apr 17 18:49:19 2023, max compression
+gzip compressed data, was "np2mcpl-0.1.0.tar", last modified: Tue Jun 20 14:30:42 2023, max compression
```

## Comparing `np2mcpl-0.0.1.tar` & `np2mcpl-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-17 18:49:19.149048 np2mcpl-0.0.1/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2023-04-12 09:17:40.000000 np2mcpl-0.0.1/LICENSE
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1664 2023-04-17 18:49:19.149048 np2mcpl-0.0.1/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1089 2023-04-17 08:54:19.000000 np2mcpl-0.0.1/README.md
--rw-r--r--   0 erkn      (1000) erkn      (1000)     5301 2023-04-14 08:27:36.000000 np2mcpl-0.0.1/np2mcplmodule.c
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1172 2023-04-17 18:27:21.000000 np2mcpl-0.0.1/pyproject.toml
--rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2023-04-17 18:49:19.149048 np2mcpl-0.0.1/setup.cfg
--rw-r--r--   0 erkn      (1000) erkn      (1000)      477 2023-04-17 15:11:19.000000 np2mcpl-0.0.1/setup.py
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-17 18:49:19.145715 np2mcpl-0.0.1/src/
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-17 18:49:19.145715 np2mcpl-0.0.1/src/np2mcpl.egg-info/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1664 2023-04-17 18:49:19.000000 np2mcpl-0.0.1/src/np2mcpl.egg-info/PKG-INFO
--rw-r--r--   0 erkn      (1000) erkn      (1000)      244 2023-04-17 18:49:19.000000 np2mcpl-0.0.1/src/np2mcpl.egg-info/SOURCES.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2023-04-17 18:49:19.000000 np2mcpl-0.0.1/src/np2mcpl.egg-info/dependency_links.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)        6 2023-04-17 18:49:19.000000 np2mcpl-0.0.1/src/np2mcpl.egg-info/requires.txt
--rw-r--r--   0 erkn      (1000) erkn      (1000)        8 2023-04-17 18:49:19.000000 np2mcpl-0.0.1/src/np2mcpl.egg-info/top_level.txt
-drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-04-17 18:49:19.149048 np2mcpl-0.0.1/test/
--rw-r--r--   0 erkn      (1000) erkn      (1000)     1209 2023-04-14 08:22:49.000000 np2mcpl-0.0.1/test/test.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-20 14:30:42.956117 np2mcpl-0.1.0/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1071 2023-06-20 13:12:15.000000 np2mcpl-0.1.0/LICENSE
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1956 2023-06-20 14:30:42.952783 np2mcpl-0.1.0/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1381 2023-06-20 13:12:15.000000 np2mcpl-0.1.0/README.md
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-20 14:30:42.952783 np2mcpl-0.1.0/np2mcpl.egg-info/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1956 2023-06-20 14:30:42.000000 np2mcpl-0.1.0/np2mcpl.egg-info/PKG-INFO
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      228 2023-06-20 14:30:42.000000 np2mcpl-0.1.0/np2mcpl.egg-info/SOURCES.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)        1 2023-06-20 14:30:42.000000 np2mcpl-0.1.0/np2mcpl.egg-info/dependency_links.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)        6 2023-06-20 14:30:42.000000 np2mcpl-0.1.0/np2mcpl.egg-info/requires.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)        8 2023-06-20 14:30:42.000000 np2mcpl-0.1.0/np2mcpl.egg-info/top_level.txt
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1043 2023-06-20 13:36:40.000000 np2mcpl-0.1.0/pyproject.toml
+-rw-r--r--   0 erkn      (1000) erkn      (1000)       38 2023-06-20 14:30:42.956117 np2mcpl-0.1.0/setup.cfg
+-rw-r--r--   0 erkn      (1000) erkn      (1000)      481 2023-06-20 14:23:56.000000 np2mcpl-0.1.0/setup.py
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-20 14:30:42.952783 np2mcpl-0.1.0/src/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     6117 2023-06-20 13:12:25.000000 np2mcpl-0.1.0/src/np2mcplmodule.c
+drwxr-xr-x   0 erkn      (1000) erkn      (1000)        0 2023-06-20 14:30:42.952783 np2mcpl-0.1.0/test/
+-rw-r--r--   0 erkn      (1000) erkn      (1000)     1209 2023-06-20 13:12:15.000000 np2mcpl-0.1.0/test/test.py
```

### Comparing `np2mcpl-0.0.1/LICENSE` & `np2mcpl-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `np2mcpl-0.0.1/PKG-INFO` & `np2mcpl-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: np2mcpl
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to convert a Monte Carlo particle in the form of a numpy-array to a MCPL-file.
 Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
 Project-URL: Homepage, https://github.com/ebknudsen/np2mcpl
 Project-URL: Bug Tracker, https://github.com/ebknudsen/np2mcpl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # np2mcpl
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 np2mcpl is a low-key tool to help write mcpl-files directly from numpy-arrays.
 
 ## Build/Install/Use
 1. Make sure you have installed the MCPL-library (and NumPy)
 2. Build the python/c module: ```python setup.py build```
 3. Add the build directory to PYTHONPATH _or_ run: ```python setup.py install```
@@ -24,10 +25,11 @@
 5. Create a numpy array and save it. E.g. : ```np2mcpl.save("output",M)```
 
 ## Notes and limitations
 - np2mcpl takes as input a 2D NumPy array with 10 or 13 columns, where the columns are assumed to be:
 ```
 PDG-code  x y z   ux uy uz   t e_kin weight    [ px py pz ]
 ```
- where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... 
+ where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... as documented here: [Particle Numbering Scheme](https://pdg.lbl.gov/2023/mcdata/mc_particle_id_contents.html)
 - The vector ux,uy,uz must have unit length. The optional vector px,py,pz is the polarisation vector associated with the Monte Carlo-particle.
+- Units follow the MCPL-standard. I.e. x,y,z in cm, e_kin in MeV, t in ms.
 - The input array is expected to be made of floating point numbers (including the PDG-code) in either double or single precision. If the numpy array is in single precision, this will be reflected in the mcpl-file.
```

### Comparing `np2mcpl-0.0.1/README.md` & `np2mcpl-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # np2mcpl
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 np2mcpl is a low-key tool to help write mcpl-files directly from numpy-arrays.
 
 ## Build/Install/Use
 1. Make sure you have installed the MCPL-library (and NumPy)
 2. Build the python/c module: ```python setup.py build```
 3. Add the build directory to PYTHONPATH _or_ run: ```python setup.py install```
@@ -10,10 +11,11 @@
 5. Create a numpy array and save it. E.g. : ```np2mcpl.save("output",M)```
 
 ## Notes and limitations
 - np2mcpl takes as input a 2D NumPy array with 10 or 13 columns, where the columns are assumed to be:
 ```
 PDG-code  x y z   ux uy uz   t e_kin weight    [ px py pz ]
 ```
- where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... 
+ where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... as documented here: [Particle Numbering Scheme](https://pdg.lbl.gov/2023/mcdata/mc_particle_id_contents.html)
 - The vector ux,uy,uz must have unit length. The optional vector px,py,pz is the polarisation vector associated with the Monte Carlo-particle.
+- Units follow the MCPL-standard. I.e. x,y,z in cm, e_kin in MeV, t in ms.
 - The input array is expected to be made of floating point numbers (including the PDG-code) in either double or single precision. If the numpy array is in single precision, this will be reflected in the mcpl-file.
```

### Comparing `np2mcpl-0.0.1/np2mcplmodule.c` & `np2mcpl-0.1.0/src/np2mcplmodule.c`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
   PyArrayObject *particle_bank;
     
   mcpl_outfile_t outputfile;
 
   int sts,i,nparticles,m;
   int dims[2];
-  int polarised,double_prec;
+  int polarised,userflags,double_prec;
 
   if (!PyArg_ParseTuple(args, "sO!", &filename, &PyArray_Type, &particle_bank))
     return failure(PyExc_RuntimeError, "np2mcpl: Failed to parse parameters.");
   /* We should Check that object input is 'double' type and a matrix
      Also, ideally should allow 'float'*/
   if ( not_matrix(particle_bank) || not_floating_point_array(particle_bank) ){
     return NULL;
@@ -61,26 +61,44 @@
   if (particle_bank->descr->type_num==NPY_DOUBLE){
     mcpl_enable_doubleprec(outputfile);
     double_prec=1;
   } else {
     double_prec=0;
   }
 
-  /* check if dims match polaized or not */
-  if (m==13) {
-    printf("INFO: polarization enabled.\n");
-    polarised=1;
-    mcpl_enable_polarisation(outputfile);
-  } else if (m==10){
-    printf("INFO: polarization disabled.\n");
-    polarised=0;
-
-  } else {
-    printf("ERROR: wrong number of columns in numpy array");
-    return failure(PyExc_RuntimeError, "Wrong number of of columns: ({m}. Expected 9 or 12.");
+  polarised=0;
+  userflags=0;
+  /* check if dims match polarised and userflags or not */
+  switch (m) {
+    case 14:
+      printf("INFO: polarization enabled.\n");
+      polarised=1;
+      mcpl_enable_polarisation(outputfile);
+      printf("INFO: integer userflags enabled.\n");
+      userflags=1;
+      mcpl_enable_userflags(outputfile);
+      break;
+    case 13:
+      printf("INFO: polarization enabled.\n");
+      polarised=1;
+      mcpl_enable_polarisation(outputfile);
+      break;
+    case 11:
+      printf("INFO: polarization disabled.\n");
+      printf("INFO: integer userflags enabled.\n");
+      userflags=1;
+      mcpl_enable_userflags(outputfile);
+      break;
+    case 10:
+      printf("INFO: polarization disabled.\n");
+      printf("INFO: integer userflag disabled.\n");
+      break;
+    default:
+      printf("ERROR: wrong number of columns in numpy array");
+      return failure(PyExc_RuntimeError, "Wrong number of of columns: ({m}. Expected 10,11,13, or 14.");
   }
 
   /* loop over rows in the numpy array and drop everything to an mcpl-file*/
   for (i=0;i<nparticles;i++){
     mcpl_particle_t p;
     if(double_prec){
       p.pdgcode=(int) rint( *( (double *) PyArray_GETPTR2(particle_bank,i,0)) );
@@ -94,14 +112,17 @@
       p.ekin=*( (double *) PyArray_GETPTR2(particle_bank,i,8));
       p.weight=*( (double *) PyArray_GETPTR2(particle_bank,i,9));
       if(polarised){
         p.polarisation[0]=*( (double *) PyArray_GETPTR2(particle_bank,i,10));
         p.polarisation[1]=*( (double *) PyArray_GETPTR2(particle_bank,i,11));
         p.polarisation[2]=*( (double *) PyArray_GETPTR2(particle_bank,i,12));
       }
+      if(userflags){
+        p.userflags=(uint32_t) rint( *( (double *) PyArray_GETPTR2(particle_bank,i,13)) );
+      }
     }else{
       p.pdgcode=(int) rint( *( (float *) PyArray_GETPTR2(particle_bank,i,0)) );
       p.position[0]=*( (float *) PyArray_GETPTR2(particle_bank,i,1));
       p.position[1]=*( (float *) PyArray_GETPTR2(particle_bank,i,2));
       p.position[2]=*( (float *) PyArray_GETPTR2(particle_bank,i,3));
       p.direction[0]=*( (float *) PyArray_GETPTR2(particle_bank,i,4));
       p.direction[1]=*( (float *) PyArray_GETPTR2(particle_bank,i,5));
@@ -110,14 +131,17 @@
       p.ekin=*( (float *) PyArray_GETPTR2(particle_bank,i,8));
       p.weight=*( (float *) PyArray_GETPTR2(particle_bank,i,9));
       if(polarised){
         p.polarisation[0]=*( (float *) PyArray_GETPTR2(particle_bank,i,10));
         p.polarisation[1]=*( (float *) PyArray_GETPTR2(particle_bank,i,11));
         p.polarisation[2]=*( (float *) PyArray_GETPTR2(particle_bank,i,12));
       }
+      if(userflags){
+        p.userflags=(uint32_t) rint( *( (double *) PyArray_GETPTR2(particle_bank,i,13)) );
+      }
     }
     /*write the particle*/
     mcpl_add_particle(outputfile,&p);
   }  
   mcpl_closeandgzip_outfile(outputfile);
   sts = m;
   return PyLong_FromLong(sts);
```

### Comparing `np2mcpl-0.0.1/pyproject.toml` & `np2mcpl-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 [project]
 name="np2mcpl"
-version="0.0.1"
+version="0.1.0"
 authors = [
   { name="Erik B Knudsen", email="erik.knudsen@copenhagenatomics.com" },
 ]
 description = "Package to convert a Monte Carlo particle in the form of a numpy-array to a MCPL-file."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies=[
-    'numpy', 
+    'numpy',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ebknudsen/np2mcpl"
 "Bug Tracker" = "https://github.com/ebknudsen/np2mcpl/issues"
 
 [build-system]
 requires = ["setuptools>=61.0", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+py-modules=[]
+
 [tool.cibuildwheel]
 manylinux-x86_64-image = "manylinux_2_24"
-#before-all = [
-#  "yum install -y git",
-#  "git clone https://github.com/mctools/mcpl",
-#  "cd mcpl",
-#  "cmake --build . --target install --config Release"
-#]
 before-all = [
   "apt-get -y install curl",
   "curl --output mcpl.tar.gz -L https://github.com/mctools/mcpl/tarball/master",
   "mkdir mcpl",
   "tar -xvf mcpl.tar.gz -C mcpl --strip-components=1",
   "cd mcpl",
   "cmake .","make","make install",
```

### Comparing `np2mcpl-0.0.1/src/np2mcpl.egg-info/PKG-INFO` & `np2mcpl-0.1.0/np2mcpl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: np2mcpl
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to convert a Monte Carlo particle in the form of a numpy-array to a MCPL-file.
 Author-email: Erik B Knudsen <erik.knudsen@copenhagenatomics.com>
 Project-URL: Homepage, https://github.com/ebknudsen/np2mcpl
 Project-URL: Bug Tracker, https://github.com/ebknudsen/np2mcpl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # np2mcpl
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 np2mcpl is a low-key tool to help write mcpl-files directly from numpy-arrays.
 
 ## Build/Install/Use
 1. Make sure you have installed the MCPL-library (and NumPy)
 2. Build the python/c module: ```python setup.py build```
 3. Add the build directory to PYTHONPATH _or_ run: ```python setup.py install```
@@ -24,10 +25,11 @@
 5. Create a numpy array and save it. E.g. : ```np2mcpl.save("output",M)```
 
 ## Notes and limitations
 - np2mcpl takes as input a 2D NumPy array with 10 or 13 columns, where the columns are assumed to be:
 ```
 PDG-code  x y z   ux uy uz   t e_kin weight    [ px py pz ]
 ```
- where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... 
+ where the PDG-code denotes which kind of particle it is, e.g. 2112 for neutrons, 22 for photon, ... as documented here: [Particle Numbering Scheme](https://pdg.lbl.gov/2023/mcdata/mc_particle_id_contents.html)
 - The vector ux,uy,uz must have unit length. The optional vector px,py,pz is the polarisation vector associated with the Monte Carlo-particle.
+- Units follow the MCPL-standard. I.e. x,y,z in cm, e_kin in MeV, t in ms.
 - The input array is expected to be made of floating point numbers (including the PDG-code) in either double or single precision. If the numpy array is in single precision, this will be reflected in the mcpl-file.
```

### Comparing `np2mcpl-0.0.1/test/test.py` & `np2mcpl-0.1.0/test/test.py`

 * *Files identical despite different names*

