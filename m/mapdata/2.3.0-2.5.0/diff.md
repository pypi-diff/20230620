# Comparing `tmp/mapdata-2.3.0.tar.gz` & `tmp/mapdata-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.3.0.tar", last modified: Sun Jun 18 15:44:26 2023, max compression
+gzip compressed data, was "mapdata-2.5.0.tar", last modified: Tue Jun 20 15:30:25 2023, max compression
```

## Comparing `mapdata-2.3.0.tar` & `mapdata-2.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.3.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.3.0/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-18 15:44:26.192525 mapdata-2.3.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2385 2023-06-15 03:39:51.000000 mapdata-2.3.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   168929 2023-06-18 14:39:13.000000 mapdata-2.3.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-18 15:44:26.192525 mapdata-2.3.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-17 22:05:15.000000 mapdata-2.3.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.5.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.5.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3742 2023-06-20 15:30:25.252635 mapdata-2.5.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2544 2023-06-19 13:37:21.000000 mapdata-2.5.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   176187 2023-06-20 15:03:06.000000 mapdata-2.5.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-20 15:30:25.252635 mapdata-2.5.0/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3742 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-20 15:30:25.000000 mapdata-2.5.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-20 15:30:25.252635 mapdata-2.5.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-20 15:18:57.000000 mapdata-2.5.0/setup.py
```

### Comparing `mapdata-2.3.0/LICENSE.txt` & `mapdata-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.3.0/PKG-INFO` & `mapdata-2.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.3.0
+Version: 2.5.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -35,14 +35,16 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
     OpenStreetMap.  Several alternatives are provided, and other tile servers
@@ -73,9 +75,11 @@
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
 
+[![Downloads](https://pepy.tech/badge/mapdata)](https://pypi.org/project/mapdata/)  
+
```

### Comparing `mapdata-2.3.0/README.md` & `mapdata-2.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
     OpenStreetMap.  Several alternatives are provided, and other tile servers
@@ -39,7 +41,9 @@
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
 
+[![Downloads](https://pepy.tech/badge/mapdata)](https://pypi.org/project/mapdata/)  
+
```

### Comparing `mapdata-2.3.0/mapdata/mapdata.py` & `mapdata-2.5.0/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.3.0"
-vdate = "2023-06-17"
+version = "2.5.0"
+vdate = "2023-06-20"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -44,14 +44,15 @@
 import math
 import collections
 import webbrowser
 import threading
 import queue
 import sqlite3
 import tempfile
+import subprocess
 import tkinter as tk
 import tkinter.ttk as ttk
 import tkinter.font as tkfont
 import tkinter.filedialog as tkfiledialog
 import tkintermapview as tkmv
 from PIL import ImageGrab
 import odf.opendocument
@@ -91,14 +92,17 @@
 label_color = "black"
 label_font = "Liberation Sans"
 label_size = 10
 label_bold = False
 label_position = "below"	# above or below
 
 
+# Name of editor, read from environment if it exists
+editor = os.environ.get("EDITOR")
+
 #-- Operational configuration
 # Whether to use a temporary file for Sqlite (as opposed to memory).
 temp_dbfile = False
 
 
 # Patch the tkintermapview CanvasPositionMarker 'calculate_text_y_offset()' function to
 # allow labeling below the icon.  The icon anchor position is always "center" for this app.
@@ -1191,17 +1195,17 @@
 		res = [[] for _ in column_list]
 		indices = [self.headers.index(c) for c in column_list]
 		for sel_row in self.tbl.selection():
 			datarow = self.tbl.item(sel_row)["values"]
 			for i, index in enumerate(indices):
 				res[i].append(datarow[index])
 		return res
-	def update_plot_data(self, all_data=False):
+	def update_plot_data(self):
 		for plot in self.plot_list:
-			if all_data or plot.sel_only_var.get() == "1":
+			if plot.sel_only_var.get() == "1" and plot.auto_update:
 				plot.q_redraw()
 	def remove_plot(self, plot_obj):
 		# For use by the plot 'do_close()' method.
 		try:
 			self.plot_list.remove(plot_obj)
 		except:
 			pass
@@ -1455,14 +1459,18 @@
 				f.write("select_symbol=%s\n" % select_symbol)
 				f.write("select_color=%s\n" % select_color)
 				f.write("label_color=%s\n" % label_color)
 				f.write("label_font=%s\n" % label_font)
 				f.write("label_size=%s\n" % label_size)
 				f.write("label_bold=%s\n" % ('No' if not label_bold else 'Yes'))
 				f.write("label_position=%s\n" % label_position)
+				if editor is not None:
+					f.write("\n[config]\n")
+					f.write("editor=%s\n" % editor)
+
 		def show_data_types():
 			dlg = MsgDialog("Data Types", "Data types, data completeness, and number of unique\nnon-missing values for columns of the data table:")
 			tframe, tdata = treeview_table(dlg.content_frame, self.data_types, ["Column", "Type", "Missing", "Unique"], "browse")
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 		def run_query():
 			dlg = QueryDialog(self.headers, self.db, self.whereclause)
@@ -1721,15 +1729,15 @@
 			return (self.symbol_var.get(), self.color_var.get())
 		else:
 			return (None, None)
 
 
 class ImportSymbolDialog(object):
 	def __init__(self):
-		def get_fn():
+		def get_fn(*args):
 			fn = tkfiledialog.askopenfilename(filetypes=([('X11 bitmaps', '.xbm')]))
 			if fn != '':
 				self.fn_var.set(fn)
 		def check_enable(*args):
 			if self.fn_var.get() != '' and self.symbol_var.get() != '':
 				self.ok_btn["state"] = tk.NORMAL
 			else:
@@ -1944,15 +1952,15 @@
 		else:
 			return (None, None, None, None, None, None, None, None, None, None)
 
 
 
 class ImportSpreadsheetDialog(object):
 	def __init__(self):
-		def get_fn():
+		def get_fn(*args):
 			fn = tkfiledialog.askopenfilename(filetypes=([('Spreadsheets', '.ods .xlsx .xls')]), parent=self.dlg)
 			if fn != '':
 				self.fn_var.set(fn)
 		def check_w1enable(*args):
 			if self.fn_var.get() != '':
 				if os.path.isfile(self.fn_var.get()):
 					w1next_btn["state"] = tk.NORMAL
@@ -2013,69 +2021,77 @@
 		fn_label = ttk.Label(fn_frame, text="File:")
 		fn_label.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.fn_var = tk.StringVar(fn_frame, '')
 		self.fn_var.trace('w', new_fn)
 		fn_entry = ttk.Entry(fn_frame, textvariable=self.fn_var)
 		fn_entry.configure(width=64)
 		fn_entry.grid(row=0, column=1, sticky=tk.EW, padx=(3,3))
-		fn_btn = ttk.Button(fn_frame, text="Browse", command=get_fn)
+		fn_btn = ttk.Button(fn_frame, text="Browse", command=get_fn, underline=0)
 		fn_btn.grid(row=0, column=2, sticky=tk.W, padx=(3,3))
+		self.dlg.bind("<Alt-b>", get_fn)
 
 		w1opt_frame = ttk.LabelFrame(wiz1_frame, text="Optional")
 		w1opt_frame.grid(row=1, column=0, sticky=tk.EW, padx=(6,3), pady=(9,3))
 		w1opt_frame.columnconfigure(0, weight=1)
 		desc_label = ttk.Label(w1opt_frame, text="Description:")
 		desc_label.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.desc_var = tk.StringVar(w1opt_frame, '')
 		desc_entry = ttk.Entry(w1opt_frame, width=60, textvariable=self.desc_var)
 		desc_entry.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
 
-		def w1_next():
-			# Open spreadsheet, get sheet names
-			fn, ext = os.path.splitext(self.fn_var.get())
-			ext = ext.lower()
-			try:
-				if ext == '.ods':
-					sso = OdsFile()
-				elif ext == '.xlsx':
-					sso = XlsxFile()
-				else:
-					sso = XlsFile()
-			except:
-				warning("Could not open %s" % self.fn_var.get(), kwargs={'parent': self.dlg})
-			else:
-				sso.open(self.fn_var.get())
-				self.sheet_list = sso.sheetnames()
-				self.sheet_sel["values"] = self.sheet_list
-				if ext in ('.ods', '.xlsx'):
-					try:
-						sso.close()
-					except:
-						pass
+		def w1_next(*args):
+			if self.fn_var.get() != '':
+				# Open spreadsheet, get sheet names
+				fn, ext = os.path.splitext(self.fn_var.get())
+				ext = ext.lower()
+				try:
+					if ext == '.ods':
+						sso = OdsFile()
+					elif ext == '.xlsx':
+						sso = XlsxFile()
+					else:
+						sso = XlsFile()
+				except:
+					warning("Could not open %s" % self.fn_var.get(), kwargs={'parent': self.dlg})
 				else:
-					try:
-						sso.release_resources()
-						del sso
-					except:
-						pass
-				wiz2_frame.lift()
+					sso.open(self.fn_var.get())
+					self.sheet_list = sso.sheetnames()
+					self.sheet_sel["values"] = self.sheet_list
+					if ext in ('.ods', '.xlsx'):
+						try:
+							sso.close()
+						except:
+							pass
+					else:
+						try:
+							sso.release_resources()
+							del sso
+						except:
+							pass
+					self.dlg.bind("<Alt-b>")
+					self.dlg.bind("<Alt-n>")
+					wiz2_frame.lift()
+					self.dlg.bind("<Alt-b>", w2_back)
+					self.dlg.bind("<Alt-n>", w2_next)
 
 		w1btn_frame = tk.Frame(wiz1_frame, borderwidth=3, relief=tk.RIDGE)
 		w1btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w1btn_frame.columnconfigure(0, weight=1)
 		self.canceled = False
 		#
 		w1help_btn = ttk.Button(w1btn_frame, text="Help", command=self.do_help, underline=0)
 		w1help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
-		w1next_btn = ttk.Button(w1btn_frame, text="Next", command=w1_next)
+		w1next_btn = ttk.Button(w1btn_frame, text="Next", command=w1_next, underline=0)
 		w1next_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w1cancel_btn = ttk.Button(w1btn_frame, text="Cancel", command=self.do_cancel)
+		self.dlg.bind("<Alt-n>", w1_next)
+		w1cancel_btn = ttk.Button(w1btn_frame, text="Cancel", command=self.do_cancel, underline=0)
 		w1cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		w1next_btn["state"] = tk.DISABLED
+		self.dlg.bind("<Alt-c>", self.do_cancel)
 		self.dlg.bind("<Escape>", self.do_cancel)
 
 
 		# Populate wiz2_frame
 		w2req_frame = ttk.LabelFrame(wiz2_frame, text="Required")
 		w2req_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
 		w2req_frame.columnconfigure(0, weight=1)
@@ -2092,51 +2108,60 @@
 		xrows_label = ttk.Label(w2inner_frame, text="Initial rows to skip:")
 		xrows_label.grid(row=1, column=0, sticky=tk.E, padx=(3,3))
 		self.xrows_var = tk.IntVar(w2req_frame, 0)
 		self.xrows_var.trace('w', check_w2enable)
 		xrows_entry = ttk.Entry(w2inner_frame, textvariable=self.xrows_var, width=6)
 		xrows_entry.grid(row=1, column=1, sticky=tk.W, padx=(3,3))
 
-		def w2_back():
+		def w2_back(*args):
+			self.dlg.bind("<Alt-b>")
+			self.dlg.bind("<Alt-n>")
 			wiz1_frame.lift()
+			self.dlg.bind("<Alt-n>", w1_next)
+			self.dlg.bind("<Alt-b>", get_fn)
 
-		def w2_next():
-			fn, ext = os.path.splitext(self.fn_var.get())
-			try:
-				if ext.lower() == '.ods':
-					hdrs, data = ods_data(self.fn_var.get(), self.sheet_var.get(), junk_header_rows=self.xrows_var.get())
+		def w2_next(*args):
+			# Open spreadsheet, get column names
+			if self.fn_var.get() != '' and self.sheet_var.get() != '':
+				fn, ext = os.path.splitext(self.fn_var.get())
+				try:
+					if ext.lower() == '.ods':
+						hdrs, data = ods_data(self.fn_var.get(), self.sheet_var.get(), junk_header_rows=self.xrows_var.get())
+					else:
+						hdrs, data = xls_data(self.fn_var.get(), self.sheet_var.get(), junk_header_rows=self.xrows_var.get())
+				except:
+					warning("Could not read table from %s, sheet %s" % (self.fn_var.get(), self.sheet_var.get()), 
+							kwargs={'parent': self.dlg})
 				else:
-					hdrs, data = xls_data(self.fn_var.get(), self.sheet_var.get(), junk_header_rows=self.xrows_var.get())
-			except:
-				warning("Could not read table from %s, sheet %s" % (self.fn_var.get(), self.sheet_var.get()), 
-						kwargs={'parent': self.dlg})
-			else:
-				self.headers = hdrs
-				self.header_list = list(hdrs)
-				self.rows = data
-				# Set list box values
-				self.id_sel["values"] = self.header_list
-				self.lat_sel["values"] = self.header_list
-				self.lon_sel["values"] = self.header_list
-				self.sym_sel["values"] = self.header_list
-				self.col_sel["values"] = self.header_list
-				wiz3_frame.lift()
+					self.headers = hdrs
+					self.header_list = list(hdrs)
+					self.rows = data
+					# Set list box values
+					self.id_sel["values"] = self.header_list
+					self.lat_sel["values"] = self.header_list
+					self.lon_sel["values"] = self.header_list
+					self.sym_sel["values"] = self.header_list
+					self.col_sel["values"] = self.header_list
+					self.dlg.bind("<Alt-b>")
+					self.dlg.bind("<Alt-n>")
+					wiz3_frame.lift()
+					self.dlg.bind("<Alt-b>", w3_back)
 
 		w2btn_frame = tk.Frame(wiz2_frame, borderwidth=3, relief=tk.RIDGE)
 		w2btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w2btn_frame.columnconfigure(0, weight=1)
 		#
 		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help, underline=0)
 		w2help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
-		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back)
+		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back, underline=0)
 		w2prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w2next_btn = ttk.Button(w2btn_frame, text="Next", command=w2_next)
+		w2next_btn = ttk.Button(w2btn_frame, text="Next", command=w2_next, underline=0)
 		w2next_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
-		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel)
+		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel, underline=0)
 		w2cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
 		w2next_btn["state"] = tk.DISABLED
 	
 		# Populate wiz3_frame
 		w3req_frame = ttk.LabelFrame(wiz3_frame, text="Required")
 		w3req_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
 		w3req_frame.columnconfigure(0, weight=1)
@@ -2181,30 +2206,33 @@
 		#
 		col_label = ttk.Label(w3opt_frame, text="Color column:")
 		col_label.grid(row=1, column=2, sticky=tk.E, padx=(3,3), pady=(3,3))
 		self.col_var = tk.StringVar(w3opt_frame, '')
 		self.col_sel = ttk.Combobox(w3opt_frame, state="readonly", textvariable=self.col_var, values=self.header_list, width=12)
 		self.col_sel.grid(row=1, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
 
-		def w3_back():
+		def w3_back(*args):
+			self.dlg.bind("<Alt-b>")
 			wiz2_frame.lift()
+			self.dlg.bind("<Alt-b>", w2_back)
+			self.dlg.bind("<Alt-n>", w2_next)
 
 		w3btn_frame = tk.Frame(wiz3_frame, borderwidth=3, relief=tk.RIDGE)
 		w3btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w3btn_frame.columnconfigure(0, weight=1)
 		#
 		w3help_btn = ttk.Button(w3btn_frame, text="Help", command=self.do_help, underline=0)
 		w3help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
 		w3prev_btn = ttk.Button(w3btn_frame, text="Back", command=w3_back)
 		w3prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
 		w3ok_btn = ttk.Button(w3btn_frame, text="OK", command=self.do_select, underline=0)
 		w3ok_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
 		self.dlg.bind('<Alt-o>', self.do_select)
-		w3cancel_btn = ttk.Button(w3btn_frame, text="Cancel", command=self.do_cancel)
+		w3cancel_btn = ttk.Button(w3btn_frame, text="Cancel", command=self.do_cancel, underline=0)
 		w3cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
 		w3ok_btn["state"] = tk.DISABLED
 	
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#open-spreadsheet-data-file", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
@@ -2231,42 +2259,47 @@
 	FILE, SERVER, FILE_PW = range(3)
 	def __init__(self):
 		self.exit_status = 0	# Canceled
 		self.exit_svr = None	# For caller
 		self.exit_db = None	# For caller
 		self.xpos = None
 		self.ypos = None
+		self.scriptfilepath = None
 		# Values of db_params indicate whether server information is needed.
 		self.db_params = {u"PostgreSQL": self.SERVER, u"SQLite": self.FILE, u"DuckDB": self.FILE,
 							u"SQL Server": self.SERVER, u"MySQL": self.SERVER, u"Firebird": self.SERVER,
 							u"MariaDB": self.SERVER, u"Oracle": self.SERVER}
 		self.dlg = tk.Toplevel()
 		self.title = "Database Table for Map Display"
 		self.dlg.title(self.title)
 		self.dlg.protocol("WM_DELETE_WINDOW", self.do_cancel)
-		self.dlg.geometry("650x245")
+		self.dlg.geometry("650x260")
 		self.headers = None
 		self.header_list = None
 		self.datarows = None
 
 		# Main frames
 		msgframe = tk.Frame(self.dlg)
-		msgframe.grid(column=0, row=0, padx=6, pady=3, sticky=tk.EW)
-		# Database and table selection are in one wizard pane, column selection is in a second wizard pane
+		msgframe.grid(column=0, row=0, padx=6, pady=2, sticky=tk.EW)
+		# Database selection is in one wizard pane, table and script selection are in a second, and column selection is in a third wizard pane
 		wiz1_frame = tk.Frame(self.dlg)
 		wiz1_frame.grid(column=0, row=1, sticky=tk.NSEW)
 		wiz2_frame = tk.Frame(self.dlg)
 		wiz2_frame.grid(column=0, row=1, sticky=tk.NSEW)
+		wiz3_frame = tk.Frame(self.dlg)
+		wiz3_frame.grid(column=0, row=1, sticky=tk.NSEW)
 		self.dlg.rowconfigure(0, weight=0)
 		self.dlg.rowconfigure(1, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		wiz1_frame.rowconfigure(0, weight=1)
 		wiz1_frame.columnconfigure(0, weight=1)
 		wiz2_frame.rowconfigure(0, weight=1)
 		wiz2_frame.columnconfigure(0, weight=1)
+		wiz3_frame.rowconfigure(0, weight=1)
+		wiz3_frame.columnconfigure(0, weight=1)
 
 		# Populate message frame
 		msg_label = ttk.Label(msgframe, text="The database, table, and columns to be used for mapping must be specified.", anchor=tk.W, justify=tk.LEFT, wraplength=500)
 		msg_label.grid(column=0, row=0, sticky=tk.EW)
 
 		# Wizard page 1
 		# Database selector
@@ -2279,15 +2312,14 @@
 		dbframe = tk.Frame(wiz1_frame)
 		dbtypeframe = tk.Frame(dbframe)
 		rightframe = tk.Frame(dbframe)
 		paramframe = tk.Frame(rightframe)
 		self.serverparamframe = tk.Frame(paramframe)
 		self.fileparamframe = tk.Frame(paramframe)
 		self.filepwparamframe = tk.Frame(paramframe)
-		tableframe = tk.Frame(paramframe)
 		w1btnframe = tk.Frame(wiz1_frame, borderwidth=3, relief=tk.RIDGE)
 
 		# Grid wiz1 frame widgets
 		def param_choices(*args, **kwargs):
 			svr_params = self.db_params[self.db_type_var.get()]
 			if svr_params == self.SERVER:
 				self.fileparamframe.grid_remove()
@@ -2304,34 +2336,33 @@
 			check_w1enable()
 
 		def check_w1enable(*args):
 			dbms = self.db_type_var.get()
 			if dbms != '':
 				dbtype = self.db_params[dbms]
 				if dbtype == self.SERVER:
-					if self.server.get() != '' and self.db.get != '' and self.table_var.get() != '':
+					if self.server.get() != '' and self.db.get != '':
 						w1next_btn["state"] = tk.NORMAL
 					else:
 						w1next_btn["state"] = tk.DISABLED
 				elif dbtype == self.FILE_PW:
-					if self.db_file.get() != '' and self.user.get() != '' and self.pw.get() != '' and self.table_var.get() != '':
+					if self.db_file.get() != '' and self.user.get() != '' and self.pw.get() != '':
 						w1next_btn["state"] = tk.NORMAL
 					else:
 						w1next_btn["state"] = tk.DISABLED
 				else:	# self.FILE
-					if self.db_file.get() != '' and self.table_var.get() != '':
+					if self.db_file.get() != '':
 						w1next_btn["state"] = tk.NORMAL
 					else:
 						w1next_btn["state"] = tk.DISABLED
 
 		dbframe.grid(column=0, row=0, sticky=tk.NSEW)
 		dbtypeframe.grid(column=0, row=0, padx=5, sticky=tk.NW)
 		rightframe.grid(column=1, row=0, padx=5, sticky=tk.N + tk.EW)
 		paramframe.grid(column=0, row=0, padx=5, sticky=tk.N + tk.EW)
-		tableframe.grid(column=0, row=1, sticky=tk.NW)
 		# Put serverparamframe, fileparamframe, and filepwparamframe in the same place in paramframe.
 		# Leave only serverparamframe visible.
 		self.fileparamframe.grid(row=0, column=0, sticky=tk.N + tk.EW)
 		self.fileparamframe.grid_remove()
 		self.filepwparamframe.grid(row=0, column=0, sticky=tk.N + tk.EW)
 		self.filepwparamframe.grid_remove()
 		self.serverparamframe.grid(row=0, column=0, sticky=tk.N + tk.EW)
@@ -2402,272 +2433,392 @@
 		self.fileparamframe.grid(row=0, column=0, sticky=tk.NW)
 		self.fileparamframe.grid_remove()
 		self.filepwparamframe.grid(row=0, column=0, sticky=tk.NW)
 		self.filepwparamframe.grid_remove()
 		self.serverparamframe.grid(row=0, column=0, sticky=tk.NW)
 		self.db_type_var.set(u"PostgreSQL")
 
-		# Populate tableframe
-		ttk.Label(tableframe, text="Table:").grid(column=0, row=0, padx=(28,3), pady=3, sticky=tk.E)
-		ttk.Entry(tableframe, width=30, textvariable=self.table_var).grid(column=1, row=0, padx=3, pady=3, sticky=tk.W)
+		def w1_next(*args):
+			self.dlg.bind("<Alt-p>", load_script)
+			self.dlg.bind("<Alt-s>", save_script)
+			self.dlg.bind("<Alt-e>", edit_sql)
+			wiz2_frame.lift()
+			# The following conditional fails
+			#if w1next_btn["state"] == tk.NORMAL:
+			#	wiz2_frame.lift()
+			self.dlg.bind("<Alt-n>")
+			self.dlg.bind("<Alt-n>", w2_next)
+			self.dlg.bind("<Alt-b>")
+			self.dlg.bind("<Alt-b>", w2_back)
 
 		# Populate w1btnframe
-		def w1_next():
-			sql = "select * from %s;" % self.table_var.get()
-			conn = None
-			# Open database, get table data and column headers, populate wiz2 comboboxes
-			dbms = self.db_type_var.get()
-			if dbms == 'PostgreSQL':
-				try:
-					import psycopg2
-				except:
-					warning("The Python package 'psycopg2' must be installed.", kwargs={'parent': self.dlg})
-				else:
+		w1help_btn = ttk.Button(w1btnframe, text="Help", command=self.do_help, underline=0)
+		w1help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		w1next_btn = ttk.Button(w1btnframe, text="Next", command=w1_next, underline=0)
+		w1next_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
+		w1cancel_btn = ttk.Button(w1btnframe, text="Cancel", command=self.do_cancel, underline=0)
+		w1cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
+		w1next_btn["state"] = tk.DISABLED
+		self.dlg.bind("<Alt-n>", w1_next)
+		self.dlg.bind("<Alt-c>", self.do_cancel)
+		self.dlg.bind("<Escape>", self.do_cancel)
+		
+
+		# Wizard page 2
+		# Database table and optional query
+		def check_w2enable(*args):
+			if self.table_var.get() != '':
+				w2next_btn["state"] = tk.NORMAL
+			else:
+				w2next_btn["state"] = tk.DISABLED
+		def w2_back(*args):
+			self.dlg.unbind("<Alt-p>")
+			self.dlg.unbind("<Alt-s>")
+			self.dlg.unbind("<Alt-e>")
+			wiz1_frame.lift()
+			self.dlg.bind("<Alt-n>", w1_next)
+			self.dlg.bind("<Alt-b>")
+		def w2_next(*args):
+			if self.table_var.get() != '':
+				sql = "select * from %s;" % self.table_var.get()
+				conn = None
+				# Open database, get table data and column headers, populate wiz2 comboboxes
+				dbms = self.db_type_var.get()
+				if dbms == 'PostgreSQL':
 					try:
-						port = '5432' if self.port.get() == '' else self.port.get()
-						if self.user.get() != '' and self.pw != '':
-							conn = psycopg2.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
-						else:
-							conn = psycopg2.connect(host=self.server.get(), database=self.db.get(), port=port)
+						import psycopg2
 					except:
-						warning("Cannot open the Postgres database.", kwargs={'parent': self.dlg})
-
-			elif dbms == 'SQLite':
-				import sqlite3
-				try:
-					conn = sqlite3.connect(self.db_file.get())
-				except:
-					warning("Cannot open the file %s as a SQLite database." % self.db_file.get(), kwargs={'parent': self.dlg})
+						warning("The Python package 'psycopg2' must be installed.", kwargs={'parent': self.dlg})
+					else:
+						try:
+							port = '5432' if self.port.get() == '' else self.port.get()
+							if self.user.get() != '' and self.pw != '':
+								conn = psycopg2.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
+							else:
+								conn = psycopg2.connect(host=self.server.get(), database=self.db.get(), port=port)
+						except:
+							warning("Cannot open the Postgres database.", kwargs={'parent': self.dlg})
 
-			elif dbms == 'DuckDB':
-				try:
-					import duckdb
-				except:
-					warning("The Python package 'duckdb' must be installed.", kwargs={'parent': self.dlg})
-				else:
+				elif dbms == 'SQLite':
+					import sqlite3
 					try:
-						conn = duckdb.connect(self.db_file.get(), read_only=True)
+						conn = sqlite3.connect(self.db_file.get())
 					except:
-						warning("Cannot open the file %s as a DuckDB database." % self.db_file.get(), kwargs={'parent': self.dlg})
+						warning("Cannot open the file %s as a SQLite database." % self.db_file.get(), kwargs={'parent': self.dlg})
 
-			elif dbms == 'MariaDB' or dbms == 'MySQL':
-				try:
-					import pymysql
-				except:
-					warning("The Python package 'pymysql' must be installed.", kwargs={'parent': self.dlg})
-				else:
+				elif dbms == 'DuckDB':
 					try:
-						port = '3306' if self.port.get() == '' else self.port.get()
-						if self.user.get() != '' and self.pw != '':
-							conn = pymysql.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
-						else:
-							conn = pymysql.connect(host=self.server.get(), database=self.db.get(), port=port)
+						import duckdb
 					except:
-						warning("Cannot open the MariaDB/MySQL database.", kwargs={'parent': self.dlg})
+						warning("The Python package 'duckdb' must be installed.", kwargs={'parent': self.dlg})
+					else:
+						try:
+							conn = duckdb.connect(self.db_file.get(), read_only=True)
+						except:
+							warning("Cannot open the file %s as a DuckDB database." % self.db_file.get(), kwargs={'parent': self.dlg})
 
-			elif dbms == 'SQL Server':
-				try:
-					import pyodbc
-				except:
-					warning("The Python package 'pyodbc' must be installed.", kwargs={'parent': self.dlg})
-				else:
-					ssdrivers = ('ODBC Driver 17 for SQL Server', 'ODBC Driver 13.1 for SQL Server',
-						'ODBC Driver 13 for SQL Server', 'ODBC Driver 11 for SQL Server',
-						'SQL Server Native Client 11.0', 'SQL Server Native Client 10.0',
-						'SQL Native Client', 'SQL Server')
-					for drv in ssdrivers:
-						if self.user.get() != '':
-							if self.pw.get() != '':
-								connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Uid=%s;Pwd=%s" % (drv, self.server.get(), self.db.get(), self.user.get(), self.pw.get())
-							else:
-								connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Uid=%s;Pwd=%s" % (drv, self.server.get(), self.db.get(), self.user.get())
-						else:
-							connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Trusted_Connection=yes" % (drv, self.server.get(), self.db.get())
+				elif dbms == 'MariaDB' or dbms == 'MySQL':
+					try:
+						import pymysql
+					except:
+						warning("The Python package 'pymysql' must be installed.", kwargs={'parent': self.dlg})
+					else:
 						try:
-							conn = pyodbc.connect(connstr)
+							port = '3306' if self.port.get() == '' else self.port.get()
+							if self.user.get() != '' and self.pw != '':
+								conn = pymysql.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
+							else:
+								conn = pymysql.connect(host=self.server.get(), database=self.db.get(), port=port)
 						except:
-							conn = None
-						else:
-							break
-					if conn == None:
-						warning("Cannot open the SQL Server database.", kwargs={'parent': self.dlg})
+							warning("Cannot open the MariaDB/MySQL database.", kwargs={'parent': self.dlg})
 
-			elif dbms == 'Oracle':
-				port = '1521' if self.port.get() == '' else self.port.get()
-				try:
-					import cx_Oracle as orc
-				except:
-					warning("The Python package 'cx-Oracle' must be installed.", kwargs={'parent': self.dlg})
-				else:
+				elif dbms == 'SQL Server':
 					try:
-						dsn = orc.makedsn(self.server.get(), port, service_name=self.db.get())
-						if self.user.get() != '' and self.pw != '':
-							conn = orc.connect(user=self.user.get(), password=self.pw.get(), dsn=dsn)
-						else:
-							conn = orc.connect(dsn=dsn)
+						import pyodbc
 					except:
-						warning("Cannot open the Oracle database.", kwargs={'parent': self.dlg})
+						warning("The Python package 'pyodbc' must be installed.", kwargs={'parent': self.dlg})
+					else:
+						ssdrivers = ('ODBC Driver 17 for SQL Server', 'ODBC Driver 13.1 for SQL Server',
+							'ODBC Driver 13 for SQL Server', 'ODBC Driver 11 for SQL Server',
+							'SQL Server Native Client 11.0', 'SQL Server Native Client 10.0',
+							'SQL Native Client', 'SQL Server')
+						for drv in ssdrivers:
+							if self.user.get() != '':
+								if self.pw.get() != '':
+									connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Uid=%s;Pwd=%s" % (drv, self.server.get(), self.db.get(), self.user.get(), self.pw.get())
+								else:
+									connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Uid=%s;Pwd=%s" % (drv, self.server.get(), self.db.get(), self.user.get())
+							else:
+								connstr = "DRIVER={%s};SERVER=%s;MARS_Connection=Yes; DATABASE=%s;Trusted_Connection=yes" % (drv, self.server.get(), self.db.get())
+							try:
+								conn = pyodbc.connect(connstr)
+							except:
+								conn = None
+							else:
+								break
+						if conn == None:
+							warning("Cannot open the SQL Server database.", kwargs={'parent': self.dlg})
 
-			elif dbms == 'Firebird':
-				port = '3050' if self.port.get == '' else self.port.get()
-				try:
-					import fdb
-				except:
-					warning("The Python package 'fdb' must be installed.", kwargs={'parent': self.dlg})
-				else:
+				elif dbms == 'Oracle':
+					port = '1521' if self.port.get() == '' else self.port.get()
 					try:
-						if self.user.get() != '' and self.pw != '':
-							return fdb.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
-						else:
-							return fdb.connect(host=self.server.get(), database=self.db.get(), port=port)
+						import cx_Oracle as orc
 					except:
-						warning("Cannot open the Firebird database.", kwargs={'parent': self.dlg})
+						warning("The Python package 'cx-Oracle' must be installed.", kwargs={'parent': self.dlg})
+					else:
+						try:
+							dsn = orc.makedsn(self.server.get(), port, service_name=self.db.get())
+							if self.user.get() != '' and self.pw != '':
+								conn = orc.connect(user=self.user.get(), password=self.pw.get(), dsn=dsn)
+							else:
+								conn = orc.connect(dsn=dsn)
+						except:
+							warning("Cannot open the Oracle database.", kwargs={'parent': self.dlg})
 
-			else:
-				warning("Unrecognized DBMS type", kwargs={'parent': self.dlg})
+				elif dbms == 'Firebird':
+					port = '3050' if self.port.get == '' else self.port.get()
+					try:
+						import fdb
+					except:
+						warning("The Python package 'fdb' must be installed.", kwargs={'parent': self.dlg})
+					else:
+						try:
+							if self.user.get() != '' and self.pw != '':
+								return fdb.connect(host=self.server.get(), database=self.db.get(), port=port, user=self.user.get(), password=self.pw.get())
+							else:
+								return fdb.connect(host=self.server.get(), database=self.db.get(), port=port)
+						except:
+							warning("Cannot open the Firebird database.", kwargs={'parent': self.dlg})
 
-			if conn is not None:
-				curs = conn.cursor()
-				try:
-					curs.execute(sql)
-				except:
-					warning("Cannot select data from table %s." % self.table_var.get(), kwargs={'parent':self.dlg})
 				else:
-					self.headers = [d[0] for d in curs.description]
-					self.rows = curs.fetchall()
-					self.header_list = list(self.headers)
-					# Set list box values
-					self.id_sel["values"] = self.header_list
-					self.lat_sel["values"] = self.header_list
-					self.lon_sel["values"] = self.header_list
-					self.sym_sel["values"] = self.header_list
-					self.col_sel["values"] = self.header_list
-					wiz2_frame.lift()
-				conn.close()
+					warning("Unrecognized DBMS type", kwargs={'parent': self.dlg})
 
+				if conn is not None:
+					curs = conn.cursor()
+					sqlscript = self.script_text.get("1.0", "end-1c")
+					run_ok = True
+					if sqlscript != '':
+						try:
+							curs.execute(sqlscript)
+						except:
+							run_ok = False
+							warning("Execution of the SQL script failed.", kwargs={'parent':self.dlg})
+					if run_ok:
+						try:
+							curs.execute(sql)
+						except:
+							warning("Cannot select data from table %s." % self.table_var.get(), kwargs={'parent':self.dlg})
+						else:
+							self.headers = [d[0] for d in curs.description]
+							self.rows = curs.fetchall()
+							self.header_list = list(self.headers)
+							# Set list box values
+							self.id_sel["values"] = self.header_list
+							self.lat_sel["values"] = self.header_list
+							self.lon_sel["values"] = self.header_list
+							self.sym_sel["values"] = self.header_list
+							self.col_sel["values"] = self.header_list
+							self.dlg.unbind("<Alt-p>")
+							self.dlg.unbind("<Alt-s>")
+							self.dlg.unbind("Alt-e>")
+							wiz3_frame.lift()
+							self.dlg.bind("<Alt-n>")
+							self.dlg.bind("<Alt-b>")
+							self.dlg.bind("<Alt-b>", w3_back)
+							self.dlg.bind('<Alt-o>', self.do_select)
+					conn.close()
+
+		def load_script(*args):
+			fn = tkfiledialog.askopenfilename(parent=self.dlg, title="SQL script file to open", filetypes=([('SQL script files', '.sql')]))
+			if not (fn is None or fn == ''):
+				path, filename = os.path.split(os.path.abspath(fn))
+				self.scriptfilepath = path
+				with open(fn, "r") as f:
+					sql = f.read()
+				self.script_text.insert("end", sql)
+		def save_script(*args):
+			outfile = tkfiledialog.asksaveasfilename(initialdir=self.scriptfilepath, parent=self.dlg, title="SQL script file to save", filetypes=[('SQL script files', '.sql')])
+			if not (outfile is None or outfile == ''):
+				sql = self.script_text.get("1.0", "end")
+				with open(outfile, "w") as f:
+					f.write(sql)
+		def edit_sql(*args):
+			td = tempfile.TemporaryDirectory()
+			edit_fn = os.path.join(td.name, "mapfile_temp.sql")
+			with open(edit_fn, "w") as f:
+				f.write(self.script_text.get("1.0", "end"))
+			returncode = subprocess.call([editor, edit_fn])
+			if returncode == 0:
+				with open(edit_fn, "r") as f:
+					sql = f.read()
+				self.script_text.delete("1.0", "end")
+				self.script_text.insert("end", sql)
+			else:
+				warning("Failure attempting to edit the SQL with %s" % editor)
 
-		w1help_btn = ttk.Button(w1btnframe, text="Help", command=self.do_help, underline=0)
-		w1help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		self.dlg.bind("<Alt-h>", self.do_help)
-		w1next_btn = ttk.Button(w1btnframe, text="Next", command=w1_next)
-		w1next_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w1cancel_btn = ttk.Button(w1btnframe, text="Cancel", command=self.do_cancel)
-		w1cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
-		w1next_btn["state"] = tk.DISABLED
-		self.dlg.bind("<Escape>", self.do_cancel)
-		
+		w2req_frame = ttk.LabelFrame(wiz2_frame, text="Required")
+		w2req_frame.grid(row=0, column=0, sticky=tk.EW+tk.N, padx=(6,6), pady=(3,3))
+		w2req_frame.columnconfigure(1, weight=1)
+		#
+		tbl_label = ttk.Label(w2req_frame, text="Table:")
+		tbl_label.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.table_var = tk.StringVar(w2req_frame, '')
+		self.table_var.trace('w', check_w2enable)
+		ttk.Entry(w2req_frame, width=30, textvariable=self.table_var).grid(row=0, column=1, padx=(3,6), pady=3, sticky=tk.W)
+		#
+		w2opt_frame = ttk.LabelFrame(wiz2_frame, text="Optional")
+		w2opt_frame.grid(row=1, column=0, sticky=tk.EW+tk.N, padx=(6,6), pady=(3,3))
+		w2opt_frame.columnconfigure(1, weight=1)
+		#
+		self.script_text = tk.Text(w2opt_frame, width=40, height=4)
+		self.script_text.grid(row=0, column=1, columnspan=2, rowspan=4, sticky=tk.NSEW, padx=(3,0), pady=(3,3))
+		scr_label = ttk.Label(w2opt_frame, text="Script:")
+		scr_label.grid(row=0, column=0, sticky=tk.NE, padx=(6,3), pady=(2,2))
+		load_btn = ttk.Button(w2opt_frame, text="Open", command=load_script, underline=1)
+		load_btn.grid(row=1, column=0, sticky=tk.E, padx=(6,3))
+		save_btn = ttk.Button(w2opt_frame, text="Save", command=save_script, underline=0)
+		save_btn.grid(row=2, column=0, sticky=tk.E, padx=(3,3))
+		edit_btn = ttk.Button(w2opt_frame, text="Edit", command=edit_sql, underline=0)
+		edit_btn.grid(row=3, column=0, sticky=tk.E, padx=(3,3), pady=(0,2))
+		if editor is None:
+			edit_btn["state"] = tk.DISABLED
+		else:
+			edit_btn["state"] = tk.NORMAL
+		sbar = tk.Scrollbar(w2opt_frame)
+		sbar.grid(row=0, column=2, rowspan=4, sticky=tk.NS, padx=(0,3), pady=(3,3))
+		sbar.config(command=self.script_text.yview)
+		self.script_text.config(yscrollcommand = sbar.set)
+		#
+		w2btn_frame = tk.Frame(wiz2_frame, borderwidth=3, relief=tk.RIDGE)
+		w2btn_frame.grid(row=2, column=0, sticky=tk.S+tk.EW, padx=(3,3), pady=(2,2))
+		w2btn_frame.columnconfigure(0, weight=1)
+		#
+		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help, underline=0)
+		w2help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back, underline=0)
+		w2prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
+		w2next_btn = ttk.Button(w2btn_frame, text="Next", command=w2_next, underline=0)
+		w2next_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
+		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel, underline=0)
+		w2cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
+		w2next_btn["state"] = tk.DISABLED
 
-		# Wizard page 2
+
+		# Wizard page 3
 		# Column selectors
-		def check_w2enable(*args):
+		def check_w3enable(*args):
 			if self.lat_var.get() != '' and self.lon_var.get() != '':
-				w2ok_btn["state"] = tk.NORMAL
+				w3ok_btn["state"] = tk.NORMAL
 			else:
-				w2ok_btn["state"] = tk.DISABLED
-		w2req_frame = ttk.LabelFrame(wiz2_frame, text="Required")
-		w2req_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
-		w2req_frame.columnconfigure(0, weight=1)
+				w3ok_btn["state"] = tk.DISABLED
+		w3req_frame = ttk.LabelFrame(wiz3_frame, text="Required")
+		w3req_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
+		w3req_frame.columnconfigure(0, weight=1)
 		#
-		lat_label = ttk.Label(w2req_frame, text="Latitude column:")
+		lat_label = ttk.Label(w3req_frame, text="Latitude column:")
 		lat_label.grid(row=0, column=0, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.lat_var = tk.StringVar(w2req_frame, '')
-		self.lat_var.trace('w', check_w2enable)
-		self.lat_sel = ttk.Combobox(w2req_frame, state="readonly", textvariable=self.lat_var, values=self.header_list, width=15)
+		self.lat_var = tk.StringVar(w3req_frame, '')
+		self.lat_var.trace('w', check_w3enable)
+		self.lat_sel = ttk.Combobox(w3req_frame, state="readonly", textvariable=self.lat_var, values=self.header_list, width=15)
 		self.lat_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,30), pady=(3,3))
 		#
-		lon_label = ttk.Label(w2req_frame, text="Longitude column:")
+		lon_label = ttk.Label(w3req_frame, text="Longitude column:")
 		lon_label.grid(row=0, column=2, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.lon_var = tk.StringVar(w2req_frame, '')
-		self.lon_var.trace('w', check_w2enable)
-		self.lon_sel = ttk.Combobox(w2req_frame, state="readonly", textvariable=self.lon_var, values=self.header_list, width=15)
+		self.lon_var = tk.StringVar(w3req_frame, '')
+		self.lon_var.trace('w', check_w3enable)
+		self.lon_sel = ttk.Combobox(w3req_frame, state="readonly", textvariable=self.lon_var, values=self.header_list, width=15)
 		self.lon_sel.grid(row=0, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
 
-		w2opt_frame = ttk.LabelFrame(wiz2_frame, text="Optional")
-		w2opt_frame.grid(row=1, column=0, sticky=tk.EW, padx=(6,6), pady=(6,3))
-		w2opt_frame.columnconfigure(0, weight=1)
+		w3opt_frame = ttk.LabelFrame(wiz3_frame, text="Optional")
+		w3opt_frame.grid(row=1, column=0, sticky=tk.EW, padx=(6,6), pady=(6,3))
+		w3opt_frame.columnconfigure(0, weight=1)
 		#
-		id_label = ttk.Label(w2opt_frame, text="Label column:")
+		id_label = ttk.Label(w3opt_frame, text="Label column:")
 		id_label.grid(row=0, column=0, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.id_var = tk.StringVar(w2opt_frame, '')
-		self.id_sel = ttk.Combobox(w2opt_frame, state="readonly", textvariable=self.id_var, values=self.header_list, width=12)
+		self.id_var = tk.StringVar(w3opt_frame, '')
+		self.id_sel = ttk.Combobox(w3opt_frame, state="readonly", textvariable=self.id_var, values=self.header_list, width=12)
 		self.id_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,30), pady=(3,3))
 		#
-		crs_label = ttk.Label(w2opt_frame, text="CRS:")
+		crs_label = ttk.Label(w3opt_frame, text="CRS:")
 		crs_label.grid(row=0, column=2, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.crs_var = tk.IntVar(w2opt_frame, 4326)
-		self.crs_var.trace('w', check_w2enable)
-		self.crs_sel = ttk.Entry(w2opt_frame, width=8, textvariable=self.crs_var)
+		self.crs_var = tk.IntVar(w3opt_frame, 4326)
+		self.crs_var.trace('w', check_w3enable)
+		self.crs_sel = ttk.Entry(w3opt_frame, width=8, textvariable=self.crs_var)
 		self.crs_sel.grid(row=0, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
 		#
-		sym_label = ttk.Label(w2opt_frame, text="Symbol column:")
+		sym_label = ttk.Label(w3opt_frame, text="Symbol column:")
 		sym_label.grid(row=1, column=0, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.sym_var = tk.StringVar(w2opt_frame, '')
-		self.sym_sel = ttk.Combobox(w2opt_frame, state="readonly", textvariable=self.sym_var, values=self.header_list, width=12)
+		self.sym_var = tk.StringVar(w3opt_frame, '')
+		self.sym_sel = ttk.Combobox(w3opt_frame, state="readonly", textvariable=self.sym_var, values=self.header_list, width=12)
 		self.sym_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,30), pady=(3,3))
 		#
-		col_label = ttk.Label(w2opt_frame, text="Color column:")
+		col_label = ttk.Label(w3opt_frame, text="Color column:")
 		col_label.grid(row=1, column=2, sticky=tk.E, padx=(3,3), pady=(3,3))
-		self.col_var = tk.StringVar(w2opt_frame, '')
-		self.col_sel = ttk.Combobox(w2opt_frame, state="readonly", textvariable=self.col_var, values=self.header_list, width=12)
+		self.col_var = tk.StringVar(w3opt_frame, '')
+		self.col_sel = ttk.Combobox(w3opt_frame, state="readonly", textvariable=self.col_var, values=self.header_list, width=12)
 		self.col_sel.grid(row=1, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
 		#
-		desc_label = ttk.Label(w2opt_frame, text="Description:")
+		desc_label = ttk.Label(w3opt_frame, text="Description:")
 		desc_label.grid(row=2, column=0, sticky=tk.E, padx=(3,3), pady=(3,6))
-		self.desc_var = tk.StringVar(w2opt_frame, '')
-		desc_entry = ttk.Entry(w2opt_frame, width=60, textvariable=self.desc_var)
+		self.desc_var = tk.StringVar(w3opt_frame, '')
+		desc_entry = ttk.Entry(w3opt_frame, width=60, textvariable=self.desc_var)
 		desc_entry.grid(row=2, column=1, columnspan=3, sticky=tk.W, padx=(3,3), pady=(3,6))
 
-		def w2_back():
-			wiz1_frame.lift()
+		def w3_back(*args):
+			self.dlg.bind("<Alt-p>", load_script)
+			self.dlg.bind("<Alt-s>", save_script)
+			self.dlg.bind("<Alt-e>", edit_sql)
+			self.dlg.bind("<Alt-o>")
+			wiz2_frame.lift()
+			self.dlg.bind("<Alt-n>", w2_next)
+			self.dlg.bind("<Alt-b>")
+			self.dlg.bind("<Alt-b>", w2_back)
 
-		w2btn_frame = tk.Frame(wiz2_frame, borderwidth=3, relief=tk.RIDGE)
-		w2btn_frame.grid(row=2, column=0, sticky=tk.S+tk.EW, padx=(3,3), pady=(3,3))
-		w2btn_frame.columnconfigure(0, weight=1)
+		w3btn_frame = tk.Frame(wiz3_frame, borderwidth=3, relief=tk.RIDGE)
+		w3btn_frame.grid(row=2, column=0, sticky=tk.S+tk.EW, padx=(3,3), pady=(3,3))
+		w3btn_frame.columnconfigure(0, weight=1)
 		#
-		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help, underline=0)
-		w2help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		w3help_btn = ttk.Button(w3btn_frame, text="Help", command=self.do_help, underline=0)
+		w3help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
-		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back)
-		w2prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w2ok_btn = ttk.Button(w2btn_frame, text="OK", command=self.do_select, underline=0)
-		w2ok_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
-		self.dlg.bind('<Alt-o>', self.do_select)
-		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel)
-		w2cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
-		w2ok_btn["state"] = tk.DISABLED
-	
-
-		# Bindings
-		self.dlg.bind('<Return>', self.do_select)
-		self.dlg.bind('<Escape>', self.do_cancel)
+		w3prev_btn = ttk.Button(w3btn_frame, text="Back", command=w3_back, underline=0)
+		w3prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
+		w3ok_btn = ttk.Button(w3btn_frame, text="OK", command=self.do_select, underline=0)
+		w3ok_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
+		w3cancel_btn = ttk.Button(w3btn_frame, text="Cancel", command=self.do_cancel, underline=0)
+		w3cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
+		w3ok_btn["state"] = tk.DISABLED
 
 		wiz1_frame.lift()
 
+		self.canceled = True
 		# Limit resizing
 		self.dlg.resizable(False, False)
 		center_window(self.dlg)
 	def set_sel_fn(self):
 		fn = tkfiledialog.askopenfilename(parent=self.fileparamframe, title=self.title)
 		if fn:
 			self.db_file.set(fn)
 			#self.clearstatus()
 	def do_select(self, *args):
-		self.exit_status = 1
-		self.dlg.destroy()
-		#self.dlg.update_idletasks()
+		if self.table_var.get() != '' and self.lat_var.get() != '' and self.lon_var.get() != '':
+			self.canceled = False
+			self.dlg.destroy()
 	def do_cancel(self, *args):
+		self.canceled = True
 		self.dlg.destroy()
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#open-database-data-source", new=2, autoraise=True)
 	def get_data(self):
 		self.dlg.grab_set()
 		self.dlg.focus_force()
 		self.db_choices.focus()
 		self.dlg.wait_window(self.dlg)
-		if self.headers is None:
+		if self.canceled:
 			return (None, None, None, None, None, None, None, None, None, None)
 		else:
 			return self.table_var.get(), self.id_var.get(), self.lat_var.get(), self.lon_var.get(), \
 					self.crs_var.get(), self.sym_var.get(), self.col_var.get(), self.desc_var.get(), \
 					self.headers, self.rows
 
 
@@ -2838,14 +2989,22 @@
 		self.dataset = None
 		self.data_labels = None
 		self.plot_data = None
 		self.plot_data_labels = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Plot")
 		self.dlg.columnconfigure(0, weight=1)
+		self.auto_update = True
+
+		def set_autoupdate():
+			if self.autoupdate_var.get() == "1":
+				self.auto_update = True
+				self.q_redraw()
+			else:
+				self.auto_update = False
 
 		# Message
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		prompt_frame.columnconfigure(0, weight=1)
 		msg_lbl = ttk.Label(prompt_frame, width=70, text="Select the type of plot, columns for X and Y data, and whether to show all data or only selected data.")
 		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
@@ -2858,45 +3017,50 @@
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.type_var = tk.StringVar(ctrl_frame, "")
 		type_lbl = ttk.Label(ctrl_frame, text="Plot type:")
 		type_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.type_sel = ttk.Combobox(ctrl_frame, state="readonly", textvariable=self.type_var, width=20,
 				values=["Box plot", "Category counts", "Empirical CDF", "Histogram", "Line plot", "Scatter plot", "Y range plot"])
-		self.type_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.type_sel.grid(row=0, column=1, columnspan=2, sticky=tk.W, padx=(3,6), pady=(3,3))
 		self.type_sel.bind("<<ComboboxSelected>>", self.set_xy)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_redraw, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
-		self.sel_only_ck.grid(row=1, column=0, columnspan=2, sticky=tk.W, padx=(6,6), pady=(3,3))
+		self.sel_only_ck.grid(row=1, column=0, columnspan=2, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
+		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=set_autoupdate, variable=self.autoupdate_var,
+				onvalue="1", offvalue="0")
+		self.autoupdate_ck.grid(row=1, column=2, sticky=tk.W, padx=(3,3), pady=(3,3))
 
 		self.x_var = tk.StringVar(ctrl_frame, "")
 		x_lbl = ttk.Label(ctrl_frame, text="X column:")
-		x_lbl.grid(row=0, column=2, sticky=tk.E, padx=(6,3), pady=(3,3))
+		x_lbl.grid(row=0, column=3, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.x_sel = ttk.Combobox(ctrl_frame, state="disabled", textvariable=self.x_var, width=20)
-		self.x_sel.grid(row=0, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.x_sel.grid(row=0, column=4, sticky=tk.W, padx=(3,6), pady=(3,3))
 		self.x_sel.bind("<<ComboboxSelected>>", self.q_redraw)
 
 		self.y_var = tk.StringVar(ctrl_frame, "")
 		y_lbl = ttk.Label(ctrl_frame, text="Y column:")
-		y_lbl.grid(row=1, column=2, sticky=tk.E, padx=(6,3), pady=(3,3))
+		y_lbl.grid(row=1, column=3, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.y_sel = ttk.Combobox(ctrl_frame, state="disabled", textvariable=self.y_var, width=20)
-		self.y_sel.grid(row=1, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.y_sel.grid(row=1, column=4, sticky=tk.W, padx=(3,6), pady=(3,3))
 		self.y_sel.bind("<<ComboboxSelected>>", self.q_redraw)
 
 		self.xlog_var = tk.StringVar(ctrl_frame, "0")
 		self.xlog_ck = ttk.Checkbutton(ctrl_frame, text="Log X", state="disabled", command=self.q_redraw, variable=self.xlog_var,
 				onvalue="1", offvalue="0")
-		self.xlog_ck.grid(row=0, column=4, sticky=tk.W, padx=(6,6), pady=(3,3))
+		self.xlog_ck.grid(row=0, column=5, sticky=tk.W, padx=(6,6), pady=(3,3))
 
 		self.ylog_var = tk.StringVar(ctrl_frame, "0")
 		self.ylog_ck = ttk.Checkbutton(ctrl_frame, text="Log Y", state="disabled", command=self.q_redraw, variable=self.ylog_var,
 				onvalue="1", offvalue="0")
-		self.ylog_ck.grid(row=1, column=4, sticky=tk.W, padx=(6,6), pady=(3,3))
+		self.ylog_ck.grid(row=1, column=5, sticky=tk.W, padx=(6,6), pady=(3,3))
 
 		# Plot
 		self.content_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
@@ -2917,44 +3081,44 @@
 		btn_frame.columnconfigure(1, weight=0)
 		btn_frame.columnconfigure(2, weight=0)
 		btn_frame.columnconfigure(3, weight=1)
 		self.canceled = False
 		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
-		self.data_btn = ttk.Button(btn_frame, text="Source Data", state="disabled", command=self.show_data)
+		self.data_btn = ttk.Button(btn_frame, text="Source Data", state="disabled", command=self.show_data, underline=0)
 		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
-		self.plot_data_btn = ttk.Button(btn_frame, text="Plot Data", state="disabled", command=self.show_plot_data)
+		self.plot_data_btn = ttk.Button(btn_frame, text="Plot Data", state="disabled", command=self.show_plot_data, underline=0)
 		self.plot_data_btn.grid(row=0, column=2, sticky=tk.W, padx=(3,6))
 		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
 		close_btn.grid(row=0, column=3, sticky=tk.E, padx=(6,6))
 		self.dlg.bind("<Alt-c>", self.do_close)
 		self.dlg.bind("<Escape>", self.do_close)
 		center_window(self.dlg)
 		raise_window(self.dlg)
 
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#plot-dialog", new=2, autoraise=True)
 
-	def show_data(self):
+	def show_data(self, *args):
 		# Show data that have been collected for plotting, but not summarized as needed for a particular plot type.
 		if self.dataset is not None:
 			dlg = MsgDialog("Source Data", "Original data:")
 			variables = len(self.dataset)
 			rowwise_data = []
 			for i in range(len(self.dataset[0])):
 				row = []
 				for j in range(variables):
 					row.append(self.dataset[j][i])
 				rowwise_data.append(row)
 			tframe, tdata = treeview_table(dlg.content_frame, rowwise_data, self.data_labels)
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 
-	def show_plot_data(self):
+	def show_plot_data(self, *args):
 		# Show data as summarized for a particular plot type.
 		if self.plot_data is not None:
 			dlg = MsgDialog("Data for Plotting", "Data to be plotted:")
 			variables = len(self.plot_data)
 			rowwise_data = []
 			max_data_len = max([len(self.plot_data[i]) for i in range(variables)])
 			for i in range(max_data_len):
@@ -3943,15 +4107,15 @@
 
 
 def read_config(configfile):
 	_BASEMAP_SECTION = "basemap_tile_servers"
 	_APIKEYS_SECTION = "api_keys"
 	_SYMBOL_SECTION = "symbols"
 	_DEFAULTS_SECTION = "defaults"
-	_CONFIG_SECTION = "config"
+	_MISC_SECTION = "misc"
 	cp = ConfigParser()
 	cp.read(configfile)
 	# Tile servers
 	if cp.has_section(_BASEMAP_SECTION):
 		basemap_sources = cp.items(_BASEMAP_SECTION)
 		for name, url in basemap_sources:
 			if url is None:
@@ -4073,24 +4237,35 @@
 		lbl_position = cp.get(_DEFAULTS_SECTION, "label_position")
 		if lbl_position is not None:
 			lbl_position = lbl_position.lower()
 			if lbl_position not in ("above", "below"):
 				warning("Invalid argument to the 'label_position' configuration option", kwargs={})
 			else:
 				label_position = lbl_position
-	if cp.has_option(_CONFIG_SECTION, "temp_dbfile"):
+	if cp.has_option(_MISC_SECTION, "temp_dbfile"):
 		global temp_dbfile
 		err = False
 		try:
-			dbfile = cp.getboolean(_CONFIG_SECTION, "temp_dbfile")
+			dbfile = cp.getboolean(_MISC_SECTION, "temp_dbfile")
 		except:
 			err = True
 			warning("Invalid argument to the 'temp_dbfile' configuration option", kwargs={})
 		if not err:
 			temp_dbfile = dbfile
+	if cp.has_option(_MISC_SECTION, "editor"):
+		global editor
+		err = False
+		try:
+			ed = cp.get(_MISC_SECTION, "editor")
+		except:
+			err = True
+			warning("Invalid argument to the 'editor' configuration option", kwargs={})
+		if not err:
+			editor = ed
+
 
 
 def import_symbol(symbol_name, filename):
 	with open(filename, mode='r') as f:
 		symbol_def = f.read()
 	icon_xbm[symbol_name] = symbol_def
```

### Comparing `mapdata-2.3.0/mapdata.egg-info/PKG-INFO` & `mapdata-2.5.0/mapdata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.3.0
+Version: 2.5.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
@@ -35,14 +35,16 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
+![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png)
+
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
     OpenStreetMap.  Several alternatives are provided, and other tile servers
@@ -73,9 +75,11 @@
 
 Complete documentation is at [https://mapdata.osdn.io](https://mapdata.osdn.io).
 
 A configuration file template, application icons for Linux and Windows, a .desktop
 file for Linux, and additional bitmap symbols, are available for download from
 [OSDN](https://osdn.net/projects/mapdata/releases/).
 
+[![Downloads](https://pepy.tech/badge/mapdata)](https://pypi.org/project/mapdata/)  
+
```

### Comparing `mapdata-2.3.0/setup.py` & `mapdata-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.3.0',
+	version='2.5.0',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

