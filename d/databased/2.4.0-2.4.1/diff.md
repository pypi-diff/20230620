# Comparing `tmp/databased-2.4.0.tar.gz` & `tmp/databased-2.4.1.tar.gz`

## Comparing `databased-2.4.0.tar` & `databased-2.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 databased-2.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.4.0/docs/index.html
--rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.4.0/docs/search.js
--rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/customshell.html
--rw-r--r--   0        0        0   428406 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/databased.html
--rw-r--r--   0        0        0   127332 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/dbparsers.html
--rw-r--r--   0        0        0   318210 2020-02-02 00:00:00.000000 databased-2.4.0/docs/databased/dbshell.html
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/customshell.py
--rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/databased.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/dbparsers.py
--rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 databased-2.4.0/src/databased/dbshell.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.4.0/LICENSE.txt
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.4.0/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 databased-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 databased-2.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.4.1/docs/index.html
+-rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.4.1/docs/search.js
+-rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/customshell.html
+-rw-r--r--   0        0        0   428406 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/databased.html
+-rw-r--r--   0        0        0   127330 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0   320438 2020-02-02 00:00:00.000000 databased-2.4.1/docs/databased/dbshell.html
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/customshell.py
+-rw-r--r--   0        0        0    21943 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/databased.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 databased-2.4.1/src/databased/dbshell.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.4.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.4.1/README.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 databased-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 databased-2.4.1/PKG-INFO
```

### Comparing `databased-2.4.0/CHANGELOG.md` & `databased-2.4.1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 # Changelog
 
-## 2.3.0 (2023-05-13)
+## v2.4.0 (2023-05-21)
+
+#### Refactorings
+
+* do_query() will attempt to use griddy to display results
+#### Others
+
+* add missing tag prefix
+
+
+## v2.3.0 (2023-05-13)
 
 #### Refactorings
 
 * use griddle.griddy in data_to_string()
 
 
 ## v2.2.1 (2023-05-08)
 
 #### Fixes
 
 * do_vacuum actually calls vacuum function now smh
-#### Others
-
-* build v2.2.1
-* update changelog
 
 
 ## v2.2.0 (2023-05-08)
 
 #### New Features
 
 * add backup parser
 #### Refactorings
 
 * add timestamp option to dbshell backup command
-#### Others
-
-* build v2.2.0
-* update changelog
 
 
 ## v2.1.0 (2023-05-08)
 
 #### New Features
 
 * add _disconnect decorator
 * add vacuum()
 * add connection_timeout property
-#### Others
-
-* build v2.1.0
-* update changelog
 
 
 ## v2.0.1 (2023-05-07)
 
 #### Fixes
 
 * wrap table names in query statements in [] so things like colons don't trigger syntax errors
-#### Others
-
-* build v2.0.1
-* update changelog
 
 
 ## v2.0.0 (2023-05-04)
 
 #### Refactorings
 
 * change dbmanager names to dbshell
 * rename dbmanager cli script to dbshell
-#### Others
-
-* build v2.0.0
-* update changelog
 
 
 ## v1.7.0 (2023-05-04)
 
 #### New Features
 
 * add add_rows()
@@ -82,36 +72,28 @@
 * do_add_row() prints addition success status
 * add_rows() returns number of successes and number of failures
 * add_row() returns whether the addition was successful
 * delete() returns number of deleted rows via cursor.rowcount
 #### Refactorings
 
 * update() returns number of affected rows
-#### Others
-
-* build v1.7.0
-* update changelog
 
 
 ## v1.6.0 (2023-05-03)
 
 #### New Features
 
 * add do_scan_dbs()
 * add new column functionality to dbmanager
 #### Refactorings
 
 * change do_create_table to do_add_table in dbmanager for consistency
 #### Docs
 
 * update readme
-#### Others
-
-* build v1.6.0
-* update changelog
 
 
 ## v1.5.1 (2023-05-02)
 
 #### Fixes
 
 * fix add_column() not updating existing rows to default value, if given
@@ -119,18 +101,14 @@
 * fix data_to_string hanging in an infinite loop when current_width==terminal_width
 #### Refactorings
 
 * change do_find command to do_show
 #### Docs
 
 * update formatting and fix typos
-#### Others
-
-* build v1.5.1
-* update changelog
 
 
 ## v1.5.0 (2023-04-27)
 
 #### New Features
 
 * add do_add_row()
@@ -190,19 +168,15 @@
 
 * prune changelog
 * improve type annotations
 * update readme
 * fix doc string
 #### Others
 
-* test build
-* build v1.5.0
 * add imports to custom_manager.py
-* update imports
-* update imports
 * add dbmanager to project.scripts
 * cleanup testing lines
 * remove unused import
 * update ignores
 * add dbshell import statement
 * update ignores
 * revert changing do_find() to do_find_rows()
@@ -215,97 +189,66 @@
 #### Fixes
 
 * fix condition causing infinite loop in data_to_string
 #### Refactorings
 
 * add print statements to data_to_string
 * remove uneeded lambda in data_to_string
-#### Others
-
-* build v1.4.5
-* update changelog
 
 
 ## v1.4.4 (2023-04-02)
 
 #### Fixes
 
 * return statement was indented one level too many
-#### Others
-
-* build v1.4.4
-* update changelog
 
 
 ## v1.4.3 (2023-04-02)
 
 #### Performance improvements
 
 * rewrite data_to_string() with a different resizing algo
-#### Others
-
-* build v1.4.3
-* update changelog
 
 
 ## v1.4.2 (2023-03-31)
 
 #### Fixes
 
 * fix dbmanager switching back to default dbname after user sets it with -db/--dbname switch
-#### Others
-
-* build v1.4.2
-* update changelog
 
 
 ## v1.4.1 (2023-03-22)
 
-#### Others
-
-* build v1.4.1
-
 
 ## v1.4.0 (2023-03-17)
 
 #### New Features
 
 * set -db switch default in dbmanager to in-use dbname when it's  created
 #### Fixes
 
 * print results directly in dbmanager find() func when results are too wide for tabulator
-#### Others
-
-* build v1.4.0
-* update changelog
 
 
 ## v1.3.0 (2023-03-13)
 
 #### New Features
 
 * add option to return a pandas.DataFrame from get_rows()
 #### Others
 
-* build v1.3.0
-* update changelog
 * update test for get_rows
 * remove duplicate dependency
 
 
 ## v1.2.0 (2023-03-11)
 
 #### New Features
 
 * add query switch
-#### Others
-
-* build v1.2.0
-* update changelog
-
 
 ## v1.1.0 (2023-03-11)
 
 #### New Features
 
 * add cleanup func
 * add query function
@@ -321,30 +264,25 @@
 * add tests
 * copy dbmanager with shutil.copyfile
 #### Refactorings
 
 * move connection decorator outside of DataBased
 #### Others
 
-* build v1.1.0
-* update changelog
 * add tests
 
 
 ## v1.0.6 (2023-03-03)
 
 #### Refactorings
 
 * change return type to list
 #### Others
 
-* build v1.0.6
-* update changelog
 * update readme
 
 
 ## v1.0.5 (2023-02-04)
 
 #### Others
 
-* update to build v1.0.5
 * add files
```

### Comparing `databased-2.4.0/docs/databased.html` & `databased-2.4.1/docs/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/docs/search.js` & `databased-2.4.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/docs/databased/customshell.html` & `databased-2.4.1/docs/databased/customshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/docs/databased/databased.html` & `databased-2.4.1/docs/databased/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/docs/databased/dbparsers.html` & `databased-2.4.1/docs/databased/dbparsers.html`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 </span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>        <span class="s2">&quot;--tables&quot;</span><span class="p">,</span>
 </span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
 </span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
 </span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
 </span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Only display info for this table(s). &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="p">)</span>
 </span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="s2">&quot;-rc&quot;</span><span class="p">,</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="s2">&quot;-c&quot;</span><span class="p">,</span>
 </span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="s2">&quot;--rowcount&quot;</span><span class="p">,</span>
 </span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Count and display the number of rows for each table. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="p">)</span>
 </span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
 </span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
@@ -321,15 +321,15 @@
 </span><span id="get_info_parser-45"><a href="#get_info_parser-45"><span class="linenos">45</span></a>        <span class="s2">&quot;--tables&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-46"><a href="#get_info_parser-46"><span class="linenos">46</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
 </span><span id="get_info_parser-47"><a href="#get_info_parser-47"><span class="linenos">47</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-48"><a href="#get_info_parser-48"><span class="linenos">48</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
 </span><span id="get_info_parser-49"><a href="#get_info_parser-49"><span class="linenos">49</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Only display info for this table(s). &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-50"><a href="#get_info_parser-50"><span class="linenos">50</span></a>    <span class="p">)</span>
 </span><span id="get_info_parser-51"><a href="#get_info_parser-51"><span class="linenos">51</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_info_parser-52"><a href="#get_info_parser-52"><span class="linenos">52</span></a>        <span class="s2">&quot;-rc&quot;</span><span class="p">,</span>
+</span><span id="get_info_parser-52"><a href="#get_info_parser-52"><span class="linenos">52</span></a>        <span class="s2">&quot;-c&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-53"><a href="#get_info_parser-53"><span class="linenos">53</span></a>        <span class="s2">&quot;--rowcount&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-54"><a href="#get_info_parser-54"><span class="linenos">54</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-55"><a href="#get_info_parser-55"><span class="linenos">55</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Count and display the number of rows for each table. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="get_info_parser-56"><a href="#get_info_parser-56"><span class="linenos">56</span></a>    <span class="p">)</span>
 </span><span id="get_info_parser-57"><a href="#get_info_parser-57"><span class="linenos">57</span></a>    <span class="k">return</span> <span class="n">parser</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -69,15 +69,15 @@
 _44        "--tables",
 _45        type=str,
 _46        nargs="*",
 _47        default=[],
 _48        help=""" Only display info for this table(s). """,
 _49    )
 _50    parser.add_argument(
-_51        "-rc",
+_51        "-c",
 _52        "--rowcount",
 _53        action="store_true",
 _54        help=""" Count and display the number of rows for each table. """,
 _55    )
 _56    return parser
 _57
 _58
@@ -262,15 +262,15 @@
 45        "--tables",
 46        type=str,
 47        nargs="*",
 48        default=[],
 49        help=""" Only display info for this table(s). """,
 50    )
 51    parser.add_argument(
-52        "-rc",
+52        "-c",
 53        "--rowcount",
 54        action="store_true",
 55        help=""" Count and display the number of rows for each table. """,
 56    )
 57    return parser
 Returns info parser.
   ⁰
```

### Comparing `databased-2.4.0/docs/databased/dbshell.html` & `databased-2.4.1/docs/databased/dbshell.html`

 * *Files 0% similar despite different names*

```diff
@@ -217,222 +217,224 @@
 </span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
 </span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
 </span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
 </span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
 </span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>                <span class="p">)</span>
 </span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>                <span class="k">try</span><span class="p">:</span>
 </span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
 </span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>                <span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                    <span class="k">continue</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                <span class="p">)</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>                <span class="k">if</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>                <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>                <span class="p">)</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>                <span class="p">)</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>                    <span class="k">continue</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                <span class="p">)</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DBShell">
                             <input id="DBShell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -534,218 +536,220 @@
 </span><span id="DBShell-96"><a href="#DBShell-96"><span class="linenos"> 96</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
 </span><span id="DBShell-97"><a href="#DBShell-97"><span class="linenos"> 97</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
 </span><span id="DBShell-98"><a href="#DBShell-98"><span class="linenos"> 98</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
 </span><span id="DBShell-99"><a href="#DBShell-99"><span class="linenos"> 99</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
 </span><span id="DBShell-100"><a href="#DBShell-100"><span class="linenos">100</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
 </span><span id="DBShell-101"><a href="#DBShell-101"><span class="linenos">101</span></a>                <span class="p">)</span>
 </span><span id="DBShell-102"><a href="#DBShell-102"><span class="linenos">102</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DBShell-103"><a href="#DBShell-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="DBShell-103"><a href="#DBShell-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span><span id="DBShell-104"><a href="#DBShell-104"><span class="linenos">104</span></a>                <span class="k">try</span><span class="p">:</span>
 </span><span id="DBShell-105"><a href="#DBShell-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
 </span><span id="DBShell-106"><a href="#DBShell-106"><span class="linenos">106</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DBShell-107"><a href="#DBShell-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
 </span><span id="DBShell-108"><a href="#DBShell-108"><span class="linenos">108</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-109"><a href="#DBShell-109"><span class="linenos">109</span></a>                <span class="nb">print</span><span class="p">()</span>
-</span><span id="DBShell-110"><a href="#DBShell-110"><span class="linenos">110</span></a>
-</span><span id="DBShell-111"><a href="#DBShell-111"><span class="linenos">111</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="DBShell-112"><a href="#DBShell-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-113"><a href="#DBShell-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="DBShell-114"><a href="#DBShell-114"><span class="linenos">114</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="DBShell-115"><a href="#DBShell-115"><span class="linenos">115</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="DBShell-116"><a href="#DBShell-116"><span class="linenos">116</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-117"><a href="#DBShell-117"><span class="linenos">117</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-118"><a href="#DBShell-118"><span class="linenos">118</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-119"><a href="#DBShell-119"><span class="linenos">119</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-120"><a href="#DBShell-120"><span class="linenos">120</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DBShell-121"><a href="#DBShell-121"><span class="linenos">121</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DBShell-122"><a href="#DBShell-122"><span class="linenos">122</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="DBShell-123"><a href="#DBShell-123"><span class="linenos">123</span></a>                <span class="p">)</span>
-</span><span id="DBShell-124"><a href="#DBShell-124"><span class="linenos">124</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DBShell-125"><a href="#DBShell-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DBShell-126"><a href="#DBShell-126"><span class="linenos">126</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DBShell-127"><a href="#DBShell-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-128"><a href="#DBShell-128"><span class="linenos">128</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="DBShell-129"><a href="#DBShell-129"><span class="linenos">129</span></a>
-</span><span id="DBShell-130"><a href="#DBShell-130"><span class="linenos">130</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-131"><a href="#DBShell-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-132"><a href="#DBShell-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="DBShell-133"><a href="#DBShell-133"><span class="linenos">133</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="DBShell-134"><a href="#DBShell-134"><span class="linenos">134</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="DBShell-135"><a href="#DBShell-135"><span class="linenos">135</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-136"><a href="#DBShell-136"><span class="linenos">136</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell-137"><a href="#DBShell-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-138"><a href="#DBShell-138"><span class="linenos">138</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-139"><a href="#DBShell-139"><span class="linenos">139</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-140"><a href="#DBShell-140"><span class="linenos">140</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-141"><a href="#DBShell-141"><span class="linenos">141</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell-142"><a href="#DBShell-142"><span class="linenos">142</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-143"><a href="#DBShell-143"><span class="linenos">143</span></a>
-</span><span id="DBShell-144"><a href="#DBShell-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-145"><a href="#DBShell-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="DBShell-146"><a href="#DBShell-146"><span class="linenos">146</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-147"><a href="#DBShell-147"><span class="linenos">147</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-148"><a href="#DBShell-148"><span class="linenos">148</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell-149"><a href="#DBShell-149"><span class="linenos">149</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-150"><a href="#DBShell-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-151"><a href="#DBShell-151"><span class="linenos">151</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="DBShell-152"><a href="#DBShell-152"><span class="linenos">152</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-153"><a href="#DBShell-153"><span class="linenos">153</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="DBShell-154"><a href="#DBShell-154"><span class="linenos">154</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="DBShell-155"><a href="#DBShell-155"><span class="linenos">155</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-156"><a href="#DBShell-156"><span class="linenos">156</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-157"><a href="#DBShell-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
-</span><span id="DBShell-158"><a href="#DBShell-158"><span class="linenos">158</span></a>
-</span><span id="DBShell-159"><a href="#DBShell-159"><span class="linenos">159</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-160"><a href="#DBShell-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-161"><a href="#DBShell-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="DBShell-162"><a href="#DBShell-162"><span class="linenos">162</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="DBShell-163"><a href="#DBShell-163"><span class="linenos">163</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="DBShell-164"><a href="#DBShell-164"><span class="linenos">164</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="DBShell-165"><a href="#DBShell-165"><span class="linenos">165</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-166"><a href="#DBShell-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="DBShell-167"><a href="#DBShell-167"><span class="linenos">167</span></a>
-</span><span id="DBShell-168"><a href="#DBShell-168"><span class="linenos">168</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell-169"><a href="#DBShell-169"><span class="linenos">169</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-170"><a href="#DBShell-170"><span class="linenos">170</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-171"><a href="#DBShell-171"><span class="linenos">171</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-172"><a href="#DBShell-172"><span class="linenos">172</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-173"><a href="#DBShell-173"><span class="linenos">173</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="DBShell-174"><a href="#DBShell-174"><span class="linenos">174</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell-175"><a href="#DBShell-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="DBShell-176"><a href="#DBShell-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="DBShell-177"><a href="#DBShell-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell-178"><a href="#DBShell-178"><span class="linenos">178</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell-179"><a href="#DBShell-179"><span class="linenos">179</span></a>                <span class="p">)</span>
-</span><span id="DBShell-180"><a href="#DBShell-180"><span class="linenos">180</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-181"><a href="#DBShell-181"><span class="linenos">181</span></a>
-</span><span id="DBShell-182"><a href="#DBShell-182"><span class="linenos">182</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell-183"><a href="#DBShell-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-184"><a href="#DBShell-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="DBShell-185"><a href="#DBShell-185"><span class="linenos">185</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="DBShell-186"><a href="#DBShell-186"><span class="linenos">186</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="DBShell-187"><a href="#DBShell-187"><span class="linenos">187</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell-188"><a href="#DBShell-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="DBShell-189"><a href="#DBShell-189"><span class="linenos">189</span></a>
-</span><span id="DBShell-190"><a href="#DBShell-190"><span class="linenos">190</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell-191"><a href="#DBShell-191"><span class="linenos">191</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-192"><a href="#DBShell-192"><span class="linenos">192</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-193"><a href="#DBShell-193"><span class="linenos">193</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-194"><a href="#DBShell-194"><span class="linenos">194</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-195"><a href="#DBShell-195"><span class="linenos">195</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell-196"><a href="#DBShell-196"><span class="linenos">196</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-197"><a href="#DBShell-197"><span class="linenos">197</span></a>
-</span><span id="DBShell-198"><a href="#DBShell-198"><span class="linenos">198</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="DBShell-199"><a href="#DBShell-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell-200"><a href="#DBShell-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="DBShell-201"><a href="#DBShell-201"><span class="linenos">201</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-202"><a href="#DBShell-202"><span class="linenos">202</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell-203"><a href="#DBShell-203"><span class="linenos">203</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell-204"><a href="#DBShell-204"><span class="linenos">204</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
-</span><span id="DBShell-205"><a href="#DBShell-205"><span class="linenos">205</span></a>
-</span><span id="DBShell-206"><a href="#DBShell-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-207"><a href="#DBShell-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="DBShell-208"><a href="#DBShell-208"><span class="linenos">208</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="DBShell-209"><a href="#DBShell-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-210"><a href="#DBShell-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-211"><a href="#DBShell-211"><span class="linenos">211</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-212"><a href="#DBShell-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-213"><a href="#DBShell-213"><span class="linenos">213</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="DBShell-214"><a href="#DBShell-214"><span class="linenos">214</span></a>
-</span><span id="DBShell-215"><a href="#DBShell-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-216"><a href="#DBShell-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="DBShell-217"><a href="#DBShell-217"><span class="linenos">217</span></a>
-</span><span id="DBShell-218"><a href="#DBShell-218"><span class="linenos">218</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-219"><a href="#DBShell-219"><span class="linenos">219</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-220"><a href="#DBShell-220"><span class="linenos">220</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="DBShell-221"><a href="#DBShell-221"><span class="linenos">221</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell-222"><a href="#DBShell-222"><span class="linenos">222</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-223"><a href="#DBShell-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell-224"><a href="#DBShell-224"><span class="linenos">224</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-225"><a href="#DBShell-225"><span class="linenos">225</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
-</span><span id="DBShell-226"><a href="#DBShell-226"><span class="linenos">226</span></a>
-</span><span id="DBShell-227"><a href="#DBShell-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-228"><a href="#DBShell-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="DBShell-229"><a href="#DBShell-229"><span class="linenos">229</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="DBShell-230"><a href="#DBShell-230"><span class="linenos">230</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell-231"><a href="#DBShell-231"><span class="linenos">231</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell-232"><a href="#DBShell-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
-</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>
-</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>
-</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>            <span class="p">)</span>
-</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>                    <span class="k">continue</span>
-</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>
-</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                <span class="p">)</span>
-</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell-303"><a href="#DBShell-303"><span class="linenos">303</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-304"><a href="#DBShell-304"><span class="linenos">304</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-305"><a href="#DBShell-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell-306"><a href="#DBShell-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-109"><a href="#DBShell-109"><span class="linenos">109</span></a>                <span class="k">if</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell-110"><a href="#DBShell-110"><span class="linenos">110</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-111"><a href="#DBShell-111"><span class="linenos">111</span></a>                <span class="nb">print</span><span class="p">()</span>
+</span><span id="DBShell-112"><a href="#DBShell-112"><span class="linenos">112</span></a>
+</span><span id="DBShell-113"><a href="#DBShell-113"><span class="linenos">113</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="DBShell-114"><a href="#DBShell-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-115"><a href="#DBShell-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="DBShell-116"><a href="#DBShell-116"><span class="linenos">116</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="DBShell-117"><a href="#DBShell-117"><span class="linenos">117</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="DBShell-118"><a href="#DBShell-118"><span class="linenos">118</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-119"><a href="#DBShell-119"><span class="linenos">119</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-120"><a href="#DBShell-120"><span class="linenos">120</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-121"><a href="#DBShell-121"><span class="linenos">121</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-122"><a href="#DBShell-122"><span class="linenos">122</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DBShell-123"><a href="#DBShell-123"><span class="linenos">123</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DBShell-124"><a href="#DBShell-124"><span class="linenos">124</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="DBShell-125"><a href="#DBShell-125"><span class="linenos">125</span></a>                <span class="p">)</span>
+</span><span id="DBShell-126"><a href="#DBShell-126"><span class="linenos">126</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DBShell-127"><a href="#DBShell-127"><span class="linenos">127</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DBShell-128"><a href="#DBShell-128"><span class="linenos">128</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DBShell-129"><a href="#DBShell-129"><span class="linenos">129</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-130"><a href="#DBShell-130"><span class="linenos">130</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell-131"><a href="#DBShell-131"><span class="linenos">131</span></a>
+</span><span id="DBShell-132"><a href="#DBShell-132"><span class="linenos">132</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-133"><a href="#DBShell-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-134"><a href="#DBShell-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="DBShell-135"><a href="#DBShell-135"><span class="linenos">135</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="DBShell-136"><a href="#DBShell-136"><span class="linenos">136</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="DBShell-137"><a href="#DBShell-137"><span class="linenos">137</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-138"><a href="#DBShell-138"><span class="linenos">138</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell-139"><a href="#DBShell-139"><span class="linenos">139</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-140"><a href="#DBShell-140"><span class="linenos">140</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-141"><a href="#DBShell-141"><span class="linenos">141</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-142"><a href="#DBShell-142"><span class="linenos">142</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-143"><a href="#DBShell-143"><span class="linenos">143</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell-144"><a href="#DBShell-144"><span class="linenos">144</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-145"><a href="#DBShell-145"><span class="linenos">145</span></a>
+</span><span id="DBShell-146"><a href="#DBShell-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-147"><a href="#DBShell-147"><span class="linenos">147</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="DBShell-148"><a href="#DBShell-148"><span class="linenos">148</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-149"><a href="#DBShell-149"><span class="linenos">149</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-150"><a href="#DBShell-150"><span class="linenos">150</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell-151"><a href="#DBShell-151"><span class="linenos">151</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-152"><a href="#DBShell-152"><span class="linenos">152</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-153"><a href="#DBShell-153"><span class="linenos">153</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell-154"><a href="#DBShell-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-155"><a href="#DBShell-155"><span class="linenos">155</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell-156"><a href="#DBShell-156"><span class="linenos">156</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="DBShell-157"><a href="#DBShell-157"><span class="linenos">157</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-158"><a href="#DBShell-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-159"><a href="#DBShell-159"><span class="linenos">159</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
+</span><span id="DBShell-160"><a href="#DBShell-160"><span class="linenos">160</span></a>
+</span><span id="DBShell-161"><a href="#DBShell-161"><span class="linenos">161</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-162"><a href="#DBShell-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-163"><a href="#DBShell-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="DBShell-164"><a href="#DBShell-164"><span class="linenos">164</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="DBShell-165"><a href="#DBShell-165"><span class="linenos">165</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="DBShell-166"><a href="#DBShell-166"><span class="linenos">166</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="DBShell-167"><a href="#DBShell-167"><span class="linenos">167</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-168"><a href="#DBShell-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="DBShell-169"><a href="#DBShell-169"><span class="linenos">169</span></a>
+</span><span id="DBShell-170"><a href="#DBShell-170"><span class="linenos">170</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell-171"><a href="#DBShell-171"><span class="linenos">171</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-172"><a href="#DBShell-172"><span class="linenos">172</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-173"><a href="#DBShell-173"><span class="linenos">173</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-174"><a href="#DBShell-174"><span class="linenos">174</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-175"><a href="#DBShell-175"><span class="linenos">175</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="DBShell-176"><a href="#DBShell-176"><span class="linenos">176</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell-177"><a href="#DBShell-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="DBShell-178"><a href="#DBShell-178"><span class="linenos">178</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="DBShell-179"><a href="#DBShell-179"><span class="linenos">179</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell-180"><a href="#DBShell-180"><span class="linenos">180</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell-181"><a href="#DBShell-181"><span class="linenos">181</span></a>                <span class="p">)</span>
+</span><span id="DBShell-182"><a href="#DBShell-182"><span class="linenos">182</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-183"><a href="#DBShell-183"><span class="linenos">183</span></a>
+</span><span id="DBShell-184"><a href="#DBShell-184"><span class="linenos">184</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell-185"><a href="#DBShell-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-186"><a href="#DBShell-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="DBShell-187"><a href="#DBShell-187"><span class="linenos">187</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="DBShell-188"><a href="#DBShell-188"><span class="linenos">188</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="DBShell-189"><a href="#DBShell-189"><span class="linenos">189</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell-190"><a href="#DBShell-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="DBShell-191"><a href="#DBShell-191"><span class="linenos">191</span></a>
+</span><span id="DBShell-192"><a href="#DBShell-192"><span class="linenos">192</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell-193"><a href="#DBShell-193"><span class="linenos">193</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-194"><a href="#DBShell-194"><span class="linenos">194</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-195"><a href="#DBShell-195"><span class="linenos">195</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-196"><a href="#DBShell-196"><span class="linenos">196</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-197"><a href="#DBShell-197"><span class="linenos">197</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell-198"><a href="#DBShell-198"><span class="linenos">198</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-199"><a href="#DBShell-199"><span class="linenos">199</span></a>
+</span><span id="DBShell-200"><a href="#DBShell-200"><span class="linenos">200</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="DBShell-201"><a href="#DBShell-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell-202"><a href="#DBShell-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="DBShell-203"><a href="#DBShell-203"><span class="linenos">203</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-204"><a href="#DBShell-204"><span class="linenos">204</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell-205"><a href="#DBShell-205"><span class="linenos">205</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell-206"><a href="#DBShell-206"><span class="linenos">206</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+</span><span id="DBShell-207"><a href="#DBShell-207"><span class="linenos">207</span></a>
+</span><span id="DBShell-208"><a href="#DBShell-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-209"><a href="#DBShell-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="DBShell-210"><a href="#DBShell-210"><span class="linenos">210</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="DBShell-211"><a href="#DBShell-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-212"><a href="#DBShell-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-213"><a href="#DBShell-213"><span class="linenos">213</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-214"><a href="#DBShell-214"><span class="linenos">214</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-215"><a href="#DBShell-215"><span class="linenos">215</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="DBShell-216"><a href="#DBShell-216"><span class="linenos">216</span></a>
+</span><span id="DBShell-217"><a href="#DBShell-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-218"><a href="#DBShell-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="DBShell-219"><a href="#DBShell-219"><span class="linenos">219</span></a>
+</span><span id="DBShell-220"><a href="#DBShell-220"><span class="linenos">220</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-221"><a href="#DBShell-221"><span class="linenos">221</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-222"><a href="#DBShell-222"><span class="linenos">222</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="DBShell-223"><a href="#DBShell-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell-224"><a href="#DBShell-224"><span class="linenos">224</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-225"><a href="#DBShell-225"><span class="linenos">225</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell-226"><a href="#DBShell-226"><span class="linenos">226</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-227"><a href="#DBShell-227"><span class="linenos">227</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+</span><span id="DBShell-228"><a href="#DBShell-228"><span class="linenos">228</span></a>
+</span><span id="DBShell-229"><a href="#DBShell-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-230"><a href="#DBShell-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="DBShell-231"><a href="#DBShell-231"><span class="linenos">231</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="DBShell-232"><a href="#DBShell-232"><span class="linenos">232</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="DBShell-233"><a href="#DBShell-233"><span class="linenos">233</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="DBShell-234"><a href="#DBShell-234"><span class="linenos">234</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-235"><a href="#DBShell-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>
+</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>
+</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>            <span class="p">)</span>
+</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>                    <span class="k">continue</span>
+</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>
+</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                <span class="p">)</span>
+</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-303"><a href="#DBShell-303"><span class="linenos">303</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-304"><a href="#DBShell-304"><span class="linenos">304</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell-305"><a href="#DBShell-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-306"><a href="#DBShell-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-307"><a href="#DBShell-307"><span class="linenos">307</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell-308"><a href="#DBShell-308"><span class="linenos">308</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -994,21 +998,23 @@
 </span><span id="DBShell.do_show-96"><a href="#DBShell.do_show-96"><span class="linenos"> 96</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
 </span><span id="DBShell.do_show-97"><a href="#DBShell.do_show-97"><span class="linenos"> 97</span></a>                    <span class="n">columns_to_return</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">columns</span><span class="p">,</span>
 </span><span id="DBShell.do_show-98"><a href="#DBShell.do_show-98"><span class="linenos"> 98</span></a>                    <span class="n">order_by</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">order_by</span><span class="p">,</span>
 </span><span id="DBShell.do_show-99"><a href="#DBShell.do_show-99"><span class="linenos"> 99</span></a>                    <span class="n">limit</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">limit</span><span class="p">,</span>
 </span><span id="DBShell.do_show-100"><a href="#DBShell.do_show-100"><span class="linenos">100</span></a>                    <span class="n">exact_match</span><span class="o">=</span><span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
 </span><span id="DBShell.do_show-101"><a href="#DBShell.do_show-101"><span class="linenos">101</span></a>                <span class="p">)</span>
 </span><span id="DBShell.do_show-102"><a href="#DBShell.do_show-102"><span class="linenos">102</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">close</span><span class="p">()</span>
-</span><span id="DBShell.do_show-103"><a href="#DBShell.do_show-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table:&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-103"><a href="#DBShell.do_show-103"><span class="linenos">103</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span><span id="DBShell.do_show-104"><a href="#DBShell.do_show-104"><span class="linenos">104</span></a>                <span class="k">try</span><span class="p">:</span>
 </span><span id="DBShell.do_show-105"><a href="#DBShell.do_show-105"><span class="linenos">105</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>  <span class="c1"># type: ignore</span>
 </span><span id="DBShell.do_show-106"><a href="#DBShell.do_show-106"><span class="linenos">106</span></a>                <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DBShell.do_show-107"><a href="#DBShell.do_show-107"><span class="linenos">107</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t fit data into a grid.&quot;</span><span class="p">)</span>
 </span><span id="DBShell.do_show-108"><a href="#DBShell.do_show-108"><span class="linenos">108</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">results</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_show-109"><a href="#DBShell.do_show-109"><span class="linenos">109</span></a>                <span class="nb">print</span><span class="p">()</span>
+</span><span id="DBShell.do_show-109"><a href="#DBShell.do_show-109"><span class="linenos">109</span></a>                <span class="k">if</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell.do_show-110"><a href="#DBShell.do_show-110"><span class="linenos">110</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_show-111"><a href="#DBShell.do_show-111"><span class="linenos">111</span></a>                <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Find and print rows from the database.
 Use the -t/--tables, -m/--match_pairs, and -l/--limit flags to limit the search.
 Use the -c/--columns flag to limit what columns are printed.
 Use the -o/--order_by flag to order the results.
@@ -1026,32 +1032,32 @@
         <span class="def">def</span>
         <span class="name">do_search</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_search-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_search"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_search-111"><a href="#DBShell.do_search-111"><span class="linenos">111</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_search-112"><a href="#DBShell.do_search-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_search-113"><a href="#DBShell.do_search-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
-</span><span id="DBShell.do_search-114"><a href="#DBShell.do_search-114"><span class="linenos">114</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
-</span><span id="DBShell.do_search-115"><a href="#DBShell.do_search-115"><span class="linenos">115</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_search-116"><a href="#DBShell.do_search-116"><span class="linenos">116</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_search-117"><a href="#DBShell.do_search-117"><span class="linenos">117</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_search-118"><a href="#DBShell.do_search-118"><span class="linenos">118</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_search-119"><a href="#DBShell.do_search-119"><span class="linenos">119</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_search-120"><a href="#DBShell.do_search-120"><span class="linenos">120</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
-</span><span id="DBShell.do_search-121"><a href="#DBShell.do_search-121"><span class="linenos">121</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="DBShell.do_search-122"><a href="#DBShell.do_search-122"><span class="linenos">122</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
-</span><span id="DBShell.do_search-123"><a href="#DBShell.do_search-123"><span class="linenos">123</span></a>                <span class="p">)</span>
-</span><span id="DBShell.do_search-124"><a href="#DBShell.do_search-124"><span class="linenos">124</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
-</span><span id="DBShell.do_search-125"><a href="#DBShell.do_search-125"><span class="linenos">125</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
-</span><span id="DBShell.do_search-126"><a href="#DBShell.do_search-126"><span class="linenos">126</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
-</span><span id="DBShell.do_search-127"><a href="#DBShell.do_search-127"><span class="linenos">127</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_search-128"><a href="#DBShell.do_search-128"><span class="linenos">128</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_search-113"><a href="#DBShell.do_search-113"><span class="linenos">113</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_search_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_search-114"><a href="#DBShell.do_search-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">do_search</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_search-115"><a href="#DBShell.do_search-115"><span class="linenos">115</span></a>        <span class="sd">&quot;&quot;&quot;Search and return any rows containg the searched substring in any of its columns.</span>
+</span><span id="DBShell.do_search-116"><a href="#DBShell.do_search-116"><span class="linenos">116</span></a><span class="sd">        Use the -t/--tables flag to limit the search to a specific table(s).</span>
+</span><span id="DBShell.do_search-117"><a href="#DBShell.do_search-117"><span class="linenos">117</span></a><span class="sd">        Use the -c/--columns flag to limit the search to a specific column(s).&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_search-118"><a href="#DBShell.do_search-118"><span class="linenos">118</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Searching for </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s2">...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_search-119"><a href="#DBShell.do_search-119"><span class="linenos">119</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_search-120"><a href="#DBShell.do_search-120"><span class="linenos">120</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_search-121"><a href="#DBShell.do_search-121"><span class="linenos">121</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_search-122"><a href="#DBShell.do_search-122"><span class="linenos">122</span></a>                <span class="n">columns</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">columns</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_column_names</span><span class="p">(</span><span class="n">table</span><span class="p">)</span>
+</span><span id="DBShell.do_search-123"><a href="#DBShell.do_search-123"><span class="linenos">123</span></a>                <span class="n">matcher</span> <span class="o">=</span> <span class="s2">&quot; OR &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="DBShell.do_search-124"><a href="#DBShell.do_search-124"><span class="linenos">124</span></a>                    <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1"> LIKE &quot;%</span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">search_string</span><span class="si">}</span><span class="s1">%&quot;&#39;</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span>
+</span><span id="DBShell.do_search-125"><a href="#DBShell.do_search-125"><span class="linenos">125</span></a>                <span class="p">)</span>
+</span><span id="DBShell.do_search-126"><a href="#DBShell.do_search-126"><span class="linenos">126</span></a>                <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;SELECT * FROM </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> WHERE </span><span class="si">{</span><span class="n">matcher</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DBShell.do_search-127"><a href="#DBShell.do_search-127"><span class="linenos">127</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
+</span><span id="DBShell.do_search-128"><a href="#DBShell.do_search-128"><span class="linenos">128</span></a>                <span class="n">results</span> <span class="o">=</span> <span class="p">[</span><span class="n">db</span><span class="o">.</span><span class="n">_get_dict</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">]</span>
+</span><span id="DBShell.do_search-129"><a href="#DBShell.do_search-129"><span class="linenos">129</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">results</span><span class="p">)</span><span class="si">}</span><span class="s2"> results in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_search-130"><a href="#DBShell.do_search-130"><span class="linenos">130</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">DataBased</span><span class="o">.</span><span class="n">data_to_string</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Search and return any rows containg the searched substring in any of its columns.
 Use the -t/--tables flag to limit the search to a specific table(s).
 Use the -c/--columns flag to limit the search to a specific column(s).</p>
 </div>
@@ -1066,27 +1072,27 @@
         <span class="def">def</span>
         <span class="name">do_count</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_count-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_count"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_count-130"><a href="#DBShell.do_count-130"><span class="linenos">130</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_count-131"><a href="#DBShell.do_count-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_count-132"><a href="#DBShell.do_count-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
-</span><span id="DBShell.do_count-133"><a href="#DBShell.do_count-133"><span class="linenos">133</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
-</span><span id="DBShell.do_count-134"><a href="#DBShell.do_count-134"><span class="linenos">134</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
-</span><span id="DBShell.do_count-135"><a href="#DBShell.do_count-135"><span class="linenos">135</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_count-136"><a href="#DBShell.do_count-136"><span class="linenos">136</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_count-137"><a href="#DBShell.do_count-137"><span class="linenos">137</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_count-138"><a href="#DBShell.do_count-138"><span class="linenos">138</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_count-139"><a href="#DBShell.do_count-139"><span class="linenos">139</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_count-140"><a href="#DBShell.do_count-140"><span class="linenos">140</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_count-141"><a href="#DBShell.do_count-141"><span class="linenos">141</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell.do_count-142"><a href="#DBShell.do_count-142"><span class="linenos">142</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_count-132"><a href="#DBShell.do_count-132"><span class="linenos">132</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_count-133"><a href="#DBShell.do_count-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">do_count</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_count-134"><a href="#DBShell.do_count-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Print the number of rows in the database.</span>
+</span><span id="DBShell.do_count-135"><a href="#DBShell.do_count-135"><span class="linenos">135</span></a><span class="sd">        Use the -t/--tables flag to limit results to a specific table(s).</span>
+</span><span id="DBShell.do_count-136"><a href="#DBShell.do_count-136"><span class="linenos">136</span></a><span class="sd">        Use the -m/--match_pairs flag to limit the results to rows matching these criteria.</span>
+</span><span id="DBShell.do_count-137"><a href="#DBShell.do_count-137"><span class="linenos">137</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_count-138"><a href="#DBShell.do_count-138"><span class="linenos">138</span></a><span class="sd">        Pass -h/--help flag for parser help.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_count-139"><a href="#DBShell.do_count-139"><span class="linenos">139</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Counting rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_count-140"><a href="#DBShell.do_count-140"><span class="linenos">140</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_count-141"><a href="#DBShell.do_count-141"><span class="linenos">141</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_count-142"><a href="#DBShell.do_count-142"><span class="linenos">142</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_count-143"><a href="#DBShell.do_count-143"><span class="linenos">143</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">count</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell.do_count-144"><a href="#DBShell.do_count-144"><span class="linenos">144</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> matching rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print the number of rows in the database.
 Use the -t/--tables flag to limit results to a specific table(s).
 Use the -m/--match_pairs flag to limit the results to rows matching these criteria.
 Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.
@@ -1102,28 +1108,28 @@
         <span class="def">def</span>
         <span class="name">do_query</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_query-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_query"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_query-144"><a href="#DBShell.do_query-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_query-145"><a href="#DBShell.do_query-145"><span class="linenos">145</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_query-146"><a href="#DBShell.do_query-146"><span class="linenos">146</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-147"><a href="#DBShell.do_query-147"><span class="linenos">147</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_query-148"><a href="#DBShell.do_query-148"><span class="linenos">148</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
-</span><span id="DBShell.do_query-149"><a href="#DBShell.do_query-149"><span class="linenos">149</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell.do_query-150"><a href="#DBShell.do_query-150"><span class="linenos">150</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell.do_query-151"><a href="#DBShell.do_query-151"><span class="linenos">151</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
-</span><span id="DBShell.do_query-152"><a href="#DBShell.do_query-152"><span class="linenos">152</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell.do_query-153"><a href="#DBShell.do_query-153"><span class="linenos">153</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
-</span><span id="DBShell.do_query-154"><a href="#DBShell.do_query-154"><span class="linenos">154</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-155"><a href="#DBShell.do_query-155"><span class="linenos">155</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell.do_query-156"><a href="#DBShell.do_query-156"><span class="linenos">156</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_query-157"><a href="#DBShell.do_query-157"><span class="linenos">157</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_query-146"><a href="#DBShell.do_query-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">do_query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_query-147"><a href="#DBShell.do_query-147"><span class="linenos">147</span></a>        <span class="sd">&quot;&quot;&quot;Execute a query against the current database.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_query-148"><a href="#DBShell.do_query-148"><span class="linenos">148</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Executing </span><span class="si">{</span><span class="n">arg</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-149"><a href="#DBShell.do_query-149"><span class="linenos">149</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_query-150"><a href="#DBShell.do_query-150"><span class="linenos">150</span></a>            <span class="n">results</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span>
+</span><span id="DBShell.do_query-151"><a href="#DBShell.do_query-151"><span class="linenos">151</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_query-152"><a href="#DBShell.do_query-152"><span class="linenos">152</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell.do_query-153"><a href="#DBShell.do_query-153"><span class="linenos">153</span></a>                <span class="nb">print</span><span class="p">(</span><span class="n">griddy</span><span class="p">(</span><span class="n">results</span><span class="p">))</span>
+</span><span id="DBShell.do_query-154"><a href="#DBShell.do_query-154"><span class="linenos">154</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_query-155"><a href="#DBShell.do_query-155"><span class="linenos">155</span></a>                <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="n">results</span><span class="p">:</span>
+</span><span id="DBShell.do_query-156"><a href="#DBShell.do_query-156"><span class="linenos">156</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">result</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;|-|&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-157"><a href="#DBShell.do_query-157"><span class="linenos">157</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell.do_query-158"><a href="#DBShell.do_query-158"><span class="linenos">158</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_query-159"><a href="#DBShell.do_query-159"><span class="linenos">159</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">db</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span><span class="si">}</span><span class="s2"> affected rows&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute a query against the current database.</p>
 </div>
 
 
@@ -1136,36 +1142,36 @@
         <span class="def">def</span>
         <span class="name">do_update</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_update-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_update"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_update-159"><a href="#DBShell.do_update-159"><span class="linenos">159</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_update-160"><a href="#DBShell.do_update-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_update-161"><a href="#DBShell.do_update-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
-</span><span id="DBShell.do_update-162"><a href="#DBShell.do_update-162"><span class="linenos">162</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
-</span><span id="DBShell.do_update-163"><a href="#DBShell.do_update-163"><span class="linenos">163</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
-</span><span id="DBShell.do_update-164"><a href="#DBShell.do_update-164"><span class="linenos">164</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
-</span><span id="DBShell.do_update-165"><a href="#DBShell.do_update-165"><span class="linenos">165</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_update-166"><a href="#DBShell.do_update-166"><span class="linenos">166</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
-</span><span id="DBShell.do_update-167"><a href="#DBShell.do_update-167"><span class="linenos">167</span></a>
-</span><span id="DBShell.do_update-168"><a href="#DBShell.do_update-168"><span class="linenos">168</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_update-169"><a href="#DBShell.do_update-169"><span class="linenos">169</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_update-170"><a href="#DBShell.do_update-170"><span class="linenos">170</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_update-171"><a href="#DBShell.do_update-171"><span class="linenos">171</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_update-172"><a href="#DBShell.do_update-172"><span class="linenos">172</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_update-173"><a href="#DBShell.do_update-173"><span class="linenos">173</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
-</span><span id="DBShell.do_update-174"><a href="#DBShell.do_update-174"><span class="linenos">174</span></a>                    <span class="n">table</span><span class="p">,</span>
-</span><span id="DBShell.do_update-175"><a href="#DBShell.do_update-175"><span class="linenos">175</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
-</span><span id="DBShell.do_update-176"><a href="#DBShell.do_update-176"><span class="linenos">176</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
-</span><span id="DBShell.do_update-177"><a href="#DBShell.do_update-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
-</span><span id="DBShell.do_update-178"><a href="#DBShell.do_update-178"><span class="linenos">178</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
-</span><span id="DBShell.do_update-179"><a href="#DBShell.do_update-179"><span class="linenos">179</span></a>                <span class="p">)</span>
-</span><span id="DBShell.do_update-180"><a href="#DBShell.do_update-180"><span class="linenos">180</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_update-161"><a href="#DBShell.do_update-161"><span class="linenos">161</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_update_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_update-162"><a href="#DBShell.do_update-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">do_update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_update-163"><a href="#DBShell.do_update-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Update a column to a new value.</span>
+</span><span id="DBShell.do_update-164"><a href="#DBShell.do_update-164"><span class="linenos">164</span></a><span class="sd">        Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.</span>
+</span><span id="DBShell.do_update-165"><a href="#DBShell.do_update-165"><span class="linenos">165</span></a><span class="sd">        Use the -t/--tables flag to limit what tables are updated.</span>
+</span><span id="DBShell.do_update-166"><a href="#DBShell.do_update-166"><span class="linenos">166</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are updated.</span>
+</span><span id="DBShell.do_update-167"><a href="#DBShell.do_update-167"><span class="linenos">167</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_update-168"><a href="#DBShell.do_update-168"><span class="linenos">168</span></a><span class="sd">        &gt;&gt;&gt; based&gt;update -c username -v big_chungus -t users -m username lil_chungus</span>
+</span><span id="DBShell.do_update-169"><a href="#DBShell.do_update-169"><span class="linenos">169</span></a>
+</span><span id="DBShell.do_update-170"><a href="#DBShell.do_update-170"><span class="linenos">170</span></a><span class="sd">        ^will update the username in the users &#39;table&#39; to &#39;big_chungus&#39; where the username is currently &#39;lil_chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_update-171"><a href="#DBShell.do_update-171"><span class="linenos">171</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Updating rows...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_update-172"><a href="#DBShell.do_update-172"><span class="linenos">172</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_update-173"><a href="#DBShell.do_update-173"><span class="linenos">173</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_update-174"><a href="#DBShell.do_update-174"><span class="linenos">174</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_update-175"><a href="#DBShell.do_update-175"><span class="linenos">175</span></a>                <span class="n">num_updates</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">update</span><span class="p">(</span>
+</span><span id="DBShell.do_update-176"><a href="#DBShell.do_update-176"><span class="linenos">176</span></a>                    <span class="n">table</span><span class="p">,</span>
+</span><span id="DBShell.do_update-177"><a href="#DBShell.do_update-177"><span class="linenos">177</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">column</span><span class="p">,</span>
+</span><span id="DBShell.do_update-178"><a href="#DBShell.do_update-178"><span class="linenos">178</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">new_value</span><span class="p">,</span>
+</span><span id="DBShell.do_update-179"><a href="#DBShell.do_update-179"><span class="linenos">179</span></a>                    <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span>
+</span><span id="DBShell.do_update-180"><a href="#DBShell.do_update-180"><span class="linenos">180</span></a>                    <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">,</span>
+</span><span id="DBShell.do_update-181"><a href="#DBShell.do_update-181"><span class="linenos">181</span></a>                <span class="p">)</span>
+</span><span id="DBShell.do_update-182"><a href="#DBShell.do_update-182"><span class="linenos">182</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Updated </span><span class="si">{</span><span class="n">num_updates</span><span class="si">}</span><span class="s2"> rows in </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Update a column to a new value.
 Two required args: the column (-c/--column) to update and the value (-v/--value) to update to.
 Use the -t/--tables flag to limit what tables are updated.
 Use the -m/--match_pairs flag to specify which rows are updated.
@@ -1189,29 +1195,29 @@
         <span class="def">def</span>
         <span class="name">do_delete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_delete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_delete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_delete-182"><a href="#DBShell.do_delete-182"><span class="linenos">182</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
-</span><span id="DBShell.do_delete-183"><a href="#DBShell.do_delete-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_delete-184"><a href="#DBShell.do_delete-184"><span class="linenos">184</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
-</span><span id="DBShell.do_delete-185"><a href="#DBShell.do_delete-185"><span class="linenos">185</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
-</span><span id="DBShell.do_delete-186"><a href="#DBShell.do_delete-186"><span class="linenos">186</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
-</span><span id="DBShell.do_delete-187"><a href="#DBShell.do_delete-187"><span class="linenos">187</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
-</span><span id="DBShell.do_delete-188"><a href="#DBShell.do_delete-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
-</span><span id="DBShell.do_delete-189"><a href="#DBShell.do_delete-189"><span class="linenos">189</span></a>
-</span><span id="DBShell.do_delete-190"><a href="#DBShell.do_delete-190"><span class="linenos">190</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_delete-191"><a href="#DBShell.do_delete-191"><span class="linenos">191</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_delete-192"><a href="#DBShell.do_delete-192"><span class="linenos">192</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_delete-193"><a href="#DBShell.do_delete-193"><span class="linenos">193</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_delete-194"><a href="#DBShell.do_delete-194"><span class="linenos">194</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_delete-195"><a href="#DBShell.do_delete-195"><span class="linenos">195</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
-</span><span id="DBShell.do_delete-196"><a href="#DBShell.do_delete-196"><span class="linenos">196</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_delete-184"><a href="#DBShell.do_delete-184"><span class="linenos">184</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_lookup_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">convert_match_pairs</span><span class="p">])</span>
+</span><span id="DBShell.do_delete-185"><a href="#DBShell.do_delete-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_delete</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_delete-186"><a href="#DBShell.do_delete-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Delete rows from the database.</span>
+</span><span id="DBShell.do_delete-187"><a href="#DBShell.do_delete-187"><span class="linenos">187</span></a><span class="sd">        Use the -t/--tables flag to limit what tables rows are deleted from.</span>
+</span><span id="DBShell.do_delete-188"><a href="#DBShell.do_delete-188"><span class="linenos">188</span></a><span class="sd">        Use the -m/--match_pairs flag to specify which rows are deleted.</span>
+</span><span id="DBShell.do_delete-189"><a href="#DBShell.do_delete-189"><span class="linenos">189</span></a><span class="sd">        Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</span>
+</span><span id="DBShell.do_delete-190"><a href="#DBShell.do_delete-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; based&gt;delete -t users -m username chungus -p</span>
+</span><span id="DBShell.do_delete-191"><a href="#DBShell.do_delete-191"><span class="linenos">191</span></a>
+</span><span id="DBShell.do_delete-192"><a href="#DBShell.do_delete-192"><span class="linenos">192</span></a><span class="sd">        ^will delete all rows in the &#39;users&#39; table whose username contains &#39;chungus&#39;^&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_delete-193"><a href="#DBShell.do_delete-193"><span class="linenos">193</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Deleting records...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_delete-194"><a href="#DBShell.do_delete-194"><span class="linenos">194</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_delete-195"><a href="#DBShell.do_delete-195"><span class="linenos">195</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_delete-196"><a href="#DBShell.do_delete-196"><span class="linenos">196</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_delete-197"><a href="#DBShell.do_delete-197"><span class="linenos">197</span></a>                <span class="n">num_rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">match_pairs</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">partial_matching</span><span class="p">)</span>
+</span><span id="DBShell.do_delete-198"><a href="#DBShell.do_delete-198"><span class="linenos">198</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">num_rows</span><span class="si">}</span><span class="s2"> rows from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> table.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete rows from the database.
 Use the -t/--tables flag to limit what tables rows are deleted from.
 Use the -m/--match_pairs flag to specify which rows are deleted.
 Use the -p/--partial_matching flag to enable substring matching on -m/--match_pairs.</p>
@@ -1234,21 +1240,21 @@
         <span class="def">def</span>
         <span class="name">do_add_column</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_add_column-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_add_column"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_column-198"><a href="#DBShell.do_add_column-198"><span class="linenos">198</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
-</span><span id="DBShell.do_add_column-199"><a href="#DBShell.do_add_column-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
-</span><span id="DBShell.do_add_column-200"><a href="#DBShell.do_add_column-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_add_column-201"><a href="#DBShell.do_add_column-201"><span class="linenos">201</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_add_column-202"><a href="#DBShell.do_add_column-202"><span class="linenos">202</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
-</span><span id="DBShell.do_add_column-203"><a href="#DBShell.do_add_column-203"><span class="linenos">203</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
-</span><span id="DBShell.do_add_column-204"><a href="#DBShell.do_add_column-204"><span class="linenos">204</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_add_column-200"><a href="#DBShell.do_add_column-200"><span class="linenos">200</span></a>    <span class="nd">@argshell</span><span class="o">.</span><span class="n">with_parser</span><span class="p">(</span><span class="n">dbparsers</span><span class="o">.</span><span class="n">get_add_column_parser</span><span class="p">)</span>
+</span><span id="DBShell.do_add_column-201"><a href="#DBShell.do_add_column-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">do_add_column</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span><span class="p">):</span>
+</span><span id="DBShell.do_add_column-202"><a href="#DBShell.do_add_column-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Add a new column to the specified tables.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_add_column-203"><a href="#DBShell.do_add_column-203"><span class="linenos">203</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_add_column-204"><a href="#DBShell.do_add_column-204"><span class="linenos">204</span></a>            <span class="n">tables</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">tables</span> <span class="ow">or</span> <span class="n">db</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
+</span><span id="DBShell.do_add_column-205"><a href="#DBShell.do_add_column-205"><span class="linenos">205</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">tables</span><span class="p">:</span>
+</span><span id="DBShell.do_add_column-206"><a href="#DBShell.do_add_column-206"><span class="linenos">206</span></a>                <span class="n">db</span><span class="o">.</span><span class="n">add_column</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">column_name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">type</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">default_value</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new column to the specified tables.</p>
 </div>
 
 
@@ -1260,22 +1266,22 @@
         <span class="def">def</span>
         <span class="name">do_flush_log</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_flush_log-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_flush_log"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_flush_log-206"><a href="#DBShell.do_flush_log-206"><span class="linenos">206</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_flush_log-207"><a href="#DBShell.do_flush_log-207"><span class="linenos">207</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_flush_log-208"><a href="#DBShell.do_flush_log-208"><span class="linenos">208</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-209"><a href="#DBShell.do_flush_log-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_flush_log-210"><a href="#DBShell.do_flush_log-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-211"><a href="#DBShell.do_flush_log-211"><span class="linenos">211</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_flush_log-212"><a href="#DBShell.do_flush_log-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_flush_log-213"><a href="#DBShell.do_flush_log-213"><span class="linenos">213</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_flush_log-208"><a href="#DBShell.do_flush_log-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_flush_log</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_flush_log-209"><a href="#DBShell.do_flush_log-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Clear the log file for this database.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_flush_log-210"><a href="#DBShell.do_flush_log-210"><span class="linenos">210</span></a>        <span class="n">log_path</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">with_name</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">stem</span> <span class="o">+</span> <span class="s2">&quot;db.log&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-211"><a href="#DBShell.do_flush_log-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">log_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.do_flush_log-212"><a href="#DBShell.do_flush_log-212"><span class="linenos">212</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;No log file at path </span><span class="si">{</span><span class="n">log_path</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-213"><a href="#DBShell.do_flush_log-213"><span class="linenos">213</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_flush_log-214"><a href="#DBShell.do_flush_log-214"><span class="linenos">214</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Flushing log...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_flush_log-215"><a href="#DBShell.do_flush_log-215"><span class="linenos">215</span></a>            <span class="n">log_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Clear the log file for this database.</p>
 </div>
 
 
@@ -1287,25 +1293,25 @@
         <span class="def">def</span>
         <span class="name">do_scan_dbs</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_scan_dbs-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_scan_dbs"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_scan_dbs-215"><a href="#DBShell.do_scan_dbs-215"><span class="linenos">215</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_scan_dbs-216"><a href="#DBShell.do_scan_dbs-216"><span class="linenos">216</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
-</span><span id="DBShell.do_scan_dbs-217"><a href="#DBShell.do_scan_dbs-217"><span class="linenos">217</span></a>
-</span><span id="DBShell.do_scan_dbs-218"><a href="#DBShell.do_scan_dbs-218"><span class="linenos">218</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_scan_dbs-219"><a href="#DBShell.do_scan_dbs-219"><span class="linenos">219</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.do_scan_dbs-220"><a href="#DBShell.do_scan_dbs-220"><span class="linenos">220</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-221"><a href="#DBShell.do_scan_dbs-221"><span class="linenos">221</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_scan_dbs-222"><a href="#DBShell.do_scan_dbs-222"><span class="linenos">222</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-223"><a href="#DBShell.do_scan_dbs-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_scan_dbs-224"><a href="#DBShell.do_scan_dbs-224"><span class="linenos">224</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.do_scan_dbs-225"><a href="#DBShell.do_scan_dbs-225"><span class="linenos">225</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_scan_dbs-217"><a href="#DBShell.do_scan_dbs-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_scan_dbs</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_scan_dbs-218"><a href="#DBShell.do_scan_dbs-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current working directory for `*.db` files and display them.</span>
+</span><span id="DBShell.do_scan_dbs-219"><a href="#DBShell.do_scan_dbs-219"><span class="linenos">219</span></a>
+</span><span id="DBShell.do_scan_dbs-220"><a href="#DBShell.do_scan_dbs-220"><span class="linenos">220</span></a><span class="sd">        If the command is entered as `based&gt;scan_dbs r`, the scan will be performed recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_scan_dbs-221"><a href="#DBShell.do_scan_dbs-221"><span class="linenos">221</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.do_scan_dbs-222"><a href="#DBShell.do_scan_dbs-222"><span class="linenos">222</span></a>        <span class="k">if</span> <span class="n">arg</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;r&quot;</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-223"><a href="#DBShell.do_scan_dbs-223"><span class="linenos">223</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_scan_dbs-224"><a href="#DBShell.do_scan_dbs-224"><span class="linenos">224</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-225"><a href="#DBShell.do_scan_dbs-225"><span class="linenos">225</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_scan_dbs-226"><a href="#DBShell.do_scan_dbs-226"><span class="linenos">226</span></a>        <span class="k">for</span> <span class="n">db</span> <span class="ow">in</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.do_scan_dbs-227"><a href="#DBShell.do_scan_dbs-227"><span class="linenos">227</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current working directory for <code>*.db</code> files and display them.</p>
 
 <p>If the command is entered as <code>based&gt;scan_dbs r</code>, the scan will be performed recursively.</p>
 </div>
@@ -1319,28 +1325,28 @@
         <span class="def">def</span>
         <span class="name">do_customize</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_customize-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_customize"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_customize-227"><a href="#DBShell.do_customize-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_customize-228"><a href="#DBShell.do_customize-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
-</span><span id="DBShell.do_customize-229"><a href="#DBShell.do_customize-229"><span class="linenos">229</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
-</span><span id="DBShell.do_customize-230"><a href="#DBShell.do_customize-230"><span class="linenos">230</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_customize-231"><a href="#DBShell.do_customize-231"><span class="linenos">231</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-232"><a href="#DBShell.do_customize-232"><span class="linenos">232</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="DBShell.do_customize-237"><a href="#DBShell.do_customize-237"><span class="linenos">237</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
-</span><span id="DBShell.do_customize-238"><a href="#DBShell.do_customize-238"><span class="linenos">238</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-239"><a href="#DBShell.do_customize-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
-</span><span id="DBShell.do_customize-240"><a href="#DBShell.do_customize-240"><span class="linenos">240</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_customize-229"><a href="#DBShell.do_customize-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_customize</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_customize-230"><a href="#DBShell.do_customize-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Generate a template file in the current working directory for creating a custom DBShell class.</span>
+</span><span id="DBShell.do_customize-231"><a href="#DBShell.do_customize-231"><span class="linenos">231</span></a><span class="sd">        Expects one argument: the name of the custom dbshell.</span>
+</span><span id="DBShell.do_customize-232"><a href="#DBShell.do_customize-232"><span class="linenos">232</span></a><span class="sd">        This will be used to name the generated file as well as several components in the file content.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_customize-233"><a href="#DBShell.do_customize-233"><span class="linenos">233</span></a>        <span class="n">custom_file</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span> <span class="o">/</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot; &quot;</span><span class="p">,</span> <span class="s2">&quot;_&quot;</span><span class="p">))</span><span class="o">.</span><span class="n">with_suffix</span><span class="p">(</span><span class="s2">&quot;.py&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-234"><a href="#DBShell.do_customize-234"><span class="linenos">234</span></a>        <span class="k">if</span> <span class="n">custom_file</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.do_customize-235"><a href="#DBShell.do_customize-235"><span class="linenos">235</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error: </span><span class="si">{</span><span class="n">custom_file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2"> already exists in this location.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-236"><a href="#DBShell.do_customize-236"><span class="linenos">236</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.do_customize-237"><a href="#DBShell.do_customize-237"><span class="linenos">237</span></a>            <span class="n">variable_name</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell.do_customize-238"><a href="#DBShell.do_customize-238"><span class="linenos">238</span></a>            <span class="n">class_name</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">word</span><span class="o">.</span><span class="n">capitalize</span><span class="p">()</span> <span class="k">for</span> <span class="n">word</span> <span class="ow">in</span> <span class="n">arg</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="DBShell.do_customize-239"><a href="#DBShell.do_customize-239"><span class="linenos">239</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span><span class="o">.</span><span class="n">parent</span> <span class="o">/</span> <span class="s2">&quot;customshell.py&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">read_text</span><span class="p">()</span>
+</span><span id="DBShell.do_customize-240"><a href="#DBShell.do_customize-240"><span class="linenos">240</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;CustomShell&quot;</span><span class="p">,</span> <span class="n">class_name</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-241"><a href="#DBShell.do_customize-241"><span class="linenos">241</span></a>            <span class="n">content</span> <span class="o">=</span> <span class="n">content</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;customshell&quot;</span><span class="p">,</span> <span class="n">variable_name</span><span class="p">)</span>
+</span><span id="DBShell.do_customize-242"><a href="#DBShell.do_customize-242"><span class="linenos">242</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Generate a template file in the current working directory for creating a custom DBShell class.
 Expects one argument: the name of the custom dbshell.
 This will be used to name the generated file as well as several components in the file content.</p>
 </div>
@@ -1354,23 +1360,23 @@
         <span class="def">def</span>
         <span class="name">do_vacuum</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">arg</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.do_vacuum-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.do_vacuum"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-242"><a href="#DBShell.do_vacuum-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
-</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-247"><a href="#DBShell.do_vacuum-247"><span class="linenos">247</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
-</span><span id="DBShell.do_vacuum-248"><a href="#DBShell.do_vacuum-248"><span class="linenos">248</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
-</span><span id="DBShell.do_vacuum-249"><a href="#DBShell.do_vacuum-249"><span class="linenos">249</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-250"><a href="#DBShell.do_vacuum-250"><span class="linenos">250</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
+</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-247"><a href="#DBShell.do_vacuum-247"><span class="linenos">247</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-248"><a href="#DBShell.do_vacuum-248"><span class="linenos">248</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-249"><a href="#DBShell.do_vacuum-249"><span class="linenos">249</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_vacuum-250"><a href="#DBShell.do_vacuum-250"><span class="linenos">250</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-251"><a href="#DBShell.do_vacuum-251"><span class="linenos">251</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-252"><a href="#DBShell.do_vacuum-252"><span class="linenos">252</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce database disk memory.</p>
 </div>
 
 
@@ -1382,51 +1388,51 @@
         <span class="def">def</span>
         <span class="name">preloop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.preloop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.preloop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                <span class="p">)</span>
-</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-303"><a href="#DBShell.preloop-303"><span class="linenos">303</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.preloop-304"><a href="#DBShell.preloop-304"><span class="linenos">304</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-305"><a href="#DBShell.preloop-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell.preloop-306"><a href="#DBShell.preloop-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                <span class="p">)</span>
+</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-303"><a href="#DBShell.preloop-303"><span class="linenos">303</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-304"><a href="#DBShell.preloop-304"><span class="linenos">304</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-305"><a href="#DBShell.preloop-305"><span class="linenos">305</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.preloop-306"><a href="#DBShell.preloop-306"><span class="linenos">306</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-307"><a href="#DBShell.preloop-307"><span class="linenos">307</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell.preloop-308"><a href="#DBShell.preloop-308"><span class="linenos">308</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current directory for a .db file to use.
 If not found, prompt the user for one or to try again recursively.</p>
 </div>
 
@@ -1470,16 +1476,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-309"><a href="#main-309"><span class="linenos">309</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-310"><a href="#main-310"><span class="linenos">310</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-311"><a href="#main-311"><span class="linenos">311</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-312"><a href="#main-312"><span class="linenos">312</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -132,252 +132,254 @@
 _95                    args.match_pairs,
 _96                    columns_to_return=args.columns,
 _97                    order_by=args.order_by,
 _98                    limit=args.limit,
 _99                    exact_match=not args.partial_matching,
 100                )
 101                db.close()
-102                print(f"{len(results)} matching rows in {table} table:")
+102                print(f"{len(results)} matching rows in {table} table.")
 103                try:
 104                    print(DataBased.data_to_string(results))  # type: ignore
 105                except Exception as e:
 106                    print("Couldn't fit data into a grid.")
 107                    print(*results, sep="\n")
-108                print()
-109
-110    @argshell.with_parser(dbparsers.get_search_parser)
-111    def do_search(self, args: argshell.Namespace):
-112        """Search and return any rows containg the searched substring in any
+108                if results:
+109                    print(f"{len(results)} matching rows in {table} table.")
+110                print()
+111
+112    @argshell.with_parser(dbparsers.get_search_parser)
+113    def do_search(self, args: argshell.Namespace):
+114        """Search and return any rows containg the searched substring in any
 of its columns.
-113        Use the -t/--tables flag to limit the search to a specific table(s).
-114        Use the -c/--columns flag to limit the search to a specific column
+115        Use the -t/--tables flag to limit the search to a specific table(s).
+116        Use the -c/--columns flag to limit the search to a specific column
 (s)."""
-115        print(f"Searching for {args.search_string}...")
-116        with DataBased(self.dbpath) as db:
-117            tables = args.tables or db.get_table_names()
-118            for table in tables:
-119                columns = args.columns or db.get_column_names(table)
-120                matcher = " OR ".join(
-121                    f'{column} LIKE "%{args.search_string}%"' for column in
+117        print(f"Searching for {args.search_string}...")
+118        with DataBased(self.dbpath) as db:
+119            tables = args.tables or db.get_table_names()
+120            for table in tables:
+121                columns = args.columns or db.get_column_names(table)
+122                matcher = " OR ".join(
+123                    f'{column} LIKE "%{args.search_string}%"' for column in
 columns
-122                )
-123                query = f"SELECT * FROM {table} WHERE {matcher};"
-124                results = db.query(query)
-125                results = [db._get_dict(table, result) for result in
+124                )
+125                query = f"SELECT * FROM {table} WHERE {matcher};"
+126                results = db.query(query)
+127                results = [db._get_dict(table, result) for result in
 results]
-126                print(f"Found {len(results)} results in {table} table.")
-127                print(DataBased.data_to_string(results))
-128
-129    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-130    def do_count(self, args: argshell.Namespace):
-131        """Print the number of rows in the database.
-132        Use the -t/--tables flag to limit results to a specific table(s).
-133        Use the -m/--match_pairs flag to limit the results to rows matching
+128                print(f"Found {len(results)} results in {table} table.")
+129                print(DataBased.data_to_string(results))
+130
+131    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+132    def do_count(self, args: argshell.Namespace):
+133        """Print the number of rows in the database.
+134        Use the -t/--tables flag to limit results to a specific table(s).
+135        Use the -m/--match_pairs flag to limit the results to rows matching
 these criteria.
-134        Use the -p/--partial_matching flag to enable substring matching on -
+136        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-135        Pass -h/--help flag for parser help."""
-136        print("Counting rows...")
-137        with DataBased(self.dbpath) as db:
-138            tables = args.tables or db.get_table_names()
-139            for table in tables:
-140                num_rows = db.count(table, args.match_pairs, not
+137        Pass -h/--help flag for parser help."""
+138        print("Counting rows...")
+139        with DataBased(self.dbpath) as db:
+140            tables = args.tables or db.get_table_names()
+141            for table in tables:
+142                num_rows = db.count(table, args.match_pairs, not
 args.partial_matching)
-141                print(f"{num_rows} matching rows in {table} table.")
-142
-143    def do_query(self, arg: str):
-144        """Execute a query against the current database."""
-145        print(f"Executing {arg}")
-146        with DataBased(self.dbpath) as db:
-147            results = db.query(arg)
-148        try:
-149            try:
-150                print(griddy(results))
-151            except Exception as e:
-152                for result in results:
-153                    print(*result, sep="|-|")
-154        except Exception as e:
-155            print(f"{type(e).__name__}: {e}")
-156        print(f"{db.cursor.rowcount} affected rows")
-157
-158    @argshell.with_parser(dbparsers.get_update_parser,
-[dbparsers.convert_match_pairs])
-159    def do_update(self, args: argshell.Namespace):
-160        """Update a column to a new value.
-161        Two required args: the column (-c/--column) to update and the value
+143                print(f"{num_rows} matching rows in {table} table.")
+144
+145    def do_query(self, arg: str):
+146        """Execute a query against the current database."""
+147        print(f"Executing {arg}")
+148        with DataBased(self.dbpath) as db:
+149            results = db.query(arg)
+150        try:
+151            try:
+152                print(griddy(results))
+153            except Exception as e:
+154                for result in results:
+155                    print(*result, sep="|-|")
+156        except Exception as e:
+157            print(f"{type(e).__name__}: {e}")
+158        print(f"{db.cursor.rowcount} affected rows")
+159
+160    @argshell.with_parser(dbparsers.get_update_parser,
+[dbparsers.convert_match_pairs])
+161    def do_update(self, args: argshell.Namespace):
+162        """Update a column to a new value.
+163        Two required args: the column (-c/--column) to update and the value
 (-v/--value) to update to.
-162        Use the -t/--tables flag to limit what tables are updated.
-163        Use the -m/--match_pairs flag to specify which rows are updated.
-164        Use the -p/--partial_matching flag to enable substring matching on -
+164        Use the -t/--tables flag to limit what tables are updated.
+165        Use the -m/--match_pairs flag to specify which rows are updated.
+166        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-165        >>> based>update -c username -v big_chungus -t users -m username
+167        >>> based>update -c username -v big_chungus -t users -m username
 lil_chungus
-166
-167        ^will update the username in the users 'table' to 'big_chungus'
+168
+169        ^will update the username in the users 'table' to 'big_chungus'
 where the username is currently 'lil_chungus'^"""
-168        print("Updating rows...")
-169        with DataBased(self.dbpath) as db:
-170            tables = args.tables or db.get_table_names()
-171            for table in tables:
-172                num_updates = db.update(
-173                    table,
-174                    args.column,
-175                    args.new_value,
-176                    args.match_pairs,
-177                    not args.partial_matching,
-178                )
-179                print(f"Updated {num_updates} rows in {table} table.")
-180
-181    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-182    def do_delete(self, args: argshell.Namespace):
-183        """Delete rows from the database.
-184        Use the -t/--tables flag to limit what tables rows are deleted from.
-185        Use the -m/--match_pairs flag to specify which rows are deleted.
-186        Use the -p/--partial_matching flag to enable substring matching on -
+170        print("Updating rows...")
+171        with DataBased(self.dbpath) as db:
+172            tables = args.tables or db.get_table_names()
+173            for table in tables:
+174                num_updates = db.update(
+175                    table,
+176                    args.column,
+177                    args.new_value,
+178                    args.match_pairs,
+179                    not args.partial_matching,
+180                )
+181                print(f"Updated {num_updates} rows in {table} table.")
+182
+183    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+184    def do_delete(self, args: argshell.Namespace):
+185        """Delete rows from the database.
+186        Use the -t/--tables flag to limit what tables rows are deleted from.
+187        Use the -m/--match_pairs flag to specify which rows are deleted.
+188        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-187        >>> based>delete -t users -m username chungus -p
-188
-189        ^will delete all rows in the 'users' table whose username contains
+189        >>> based>delete -t users -m username chungus -p
+190
+191        ^will delete all rows in the 'users' table whose username contains
 'chungus'^"""
-190        print("Deleting records...")
-191        with DataBased(self.dbpath) as db:
-192            tables = args.tables or db.get_table_names()
-193            for table in tables:
-194                num_rows = db.delete(table, args.match_pairs, not
+192        print("Deleting records...")
+193        with DataBased(self.dbpath) as db:
+194            tables = args.tables or db.get_table_names()
+195            for table in tables:
+196                num_rows = db.delete(table, args.match_pairs, not
 args.partial_matching)
-195                print(f"Deleted {num_rows} rows from {table} table.")
-196
-197    @argshell.with_parser(dbparsers.get_add_column_parser)
-198    def do_add_column(self, args: argshell.Namespace):
-199        """Add a new column to the specified tables."""
-200        with DataBased(self.dbpath) as db:
-201            tables = args.tables or db.get_table_names()
-202            for table in tables:
-203                db.add_column(table, args.column_name, args.type,
+197                print(f"Deleted {num_rows} rows from {table} table.")
+198
+199    @argshell.with_parser(dbparsers.get_add_column_parser)
+200    def do_add_column(self, args: argshell.Namespace):
+201        """Add a new column to the specified tables."""
+202        with DataBased(self.dbpath) as db:
+203            tables = args.tables or db.get_table_names()
+204            for table in tables:
+205                db.add_column(table, args.column_name, args.type,
 args.default_value)
-204
-205    def do_flush_log(self, arg: str):
-206        """Clear the log file for this database."""
-207        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-208        if not log_path.exists():
-209            print(f"No log file at path {log_path}")
-210        else:
-211            print(f"Flushing log...")
-212            log_path.write_text("")
-213
-214    def do_scan_dbs(self, arg: str):
-215        """Scan the current working directory for `*.db` files and display
+206
+207    def do_flush_log(self, arg: str):
+208        """Clear the log file for this database."""
+209        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+210        if not log_path.exists():
+211            print(f"No log file at path {log_path}")
+212        else:
+213            print(f"Flushing log...")
+214            log_path.write_text("")
+215
+216    def do_scan_dbs(self, arg: str):
+217        """Scan the current working directory for `*.db` files and display
 them.
-216
-217        If the command is entered as `based>scan_dbs r`, the scan will be
+218
+219        If the command is entered as `based>scan_dbs r`, the scan will be
 performed recursively."""
-218        cwd = Pathier.cwd()
-219        if arg.strip() == "r":
-220            dbs = cwd.rglob("*.db")
-221        else:
-222            dbs = cwd.glob("*.db")
-223        for db in dbs:
-224            print(db.separate(cwd.stem))
-225
-226    def do_customize(self, arg: str):
-227        """Generate a template file in the current working directory for
+220        cwd = Pathier.cwd()
+221        if arg.strip() == "r":
+222            dbs = cwd.rglob("*.db")
+223        else:
+224            dbs = cwd.glob("*.db")
+225        for db in dbs:
+226            print(db.separate(cwd.stem))
+227
+228    def do_customize(self, arg: str):
+229        """Generate a template file in the current working directory for
 creating a custom DBShell class.
-228        Expects one argument: the name of the custom dbshell.
-229        This will be used to name the generated file as well as several
+230        Expects one argument: the name of the custom dbshell.
+231        This will be used to name the generated file as well as several
 components in the file content."""
-230        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+232        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
 (".py")
-231        if custom_file.exists():
-232            print(f"Error: {custom_file.name} already exists in this
+233        if custom_file.exists():
+234            print(f"Error: {custom_file.name} already exists in this
 location.")
-233        else:
-234            variable_name = "_".join(word for word in arg.lower().split())
-235            class_name = "".join(word.capitalize() for word in arg.split())
-236            content = (Pathier(__file__).parent /
+235        else:
+236            variable_name = "_".join(word for word in arg.lower().split())
+237            class_name = "".join(word.capitalize() for word in arg.split())
+238            content = (Pathier(__file__).parent /
 "customshell.py").read_text()
-237            content = content.replace("CustomShell", class_name)
-238            content = content.replace("customshell", variable_name)
-239            custom_file.write_text(content)
-240
-241    def do_vacuum(self, arg: str):
-242        """Reduce database disk memory."""
-243        starting_size = self.dbpath.size()
-244        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-245        print("Vacuuming database...")
-246        with DataBased(self.dbpath) as db:
-247            db.vacuum()
-248        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-249        print(f"Freed up {Pathier.format_size(starting_size -
+239            content = content.replace("CustomShell", class_name)
+240            content = content.replace("customshell", variable_name)
+241            custom_file.write_text(content)
+242
+243    def do_vacuum(self, arg: str):
+244        """Reduce database disk memory."""
+245        starting_size = self.dbpath.size()
+246        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+247        print("Vacuuming database...")
+248        with DataBased(self.dbpath) as db:
+249            db.vacuum()
+250        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+251        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
-250
-251    def _choose_db(self, options: list[Pathier]) -> Pathier:
-252        """Prompt the user to select from a list of files."""
-253        cwd = Pathier.cwd()
-254        paths = [path.separate(cwd.stem) for path in options]
-255        while True:
-256            print(
-257                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+252
+253    def _choose_db(self, options: list[Pathier]) -> Pathier:
+254        """Prompt the user to select from a list of files."""
+255        cwd = Pathier.cwd()
+256        paths = [path.separate(cwd.stem) for path in options]
+257        while True:
+258            print(
+259                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-258            )
-259            choice = input("Enter the number of the option to use: ")
-260            try:
-261                index = int(choice)
-262                if not 1 <= index <= len(options):
-263                    print("Choice out of range.")
-264                    continue
-265                return options[index - 1]
-266            except Exception as e:
-267                print(f"{choice} is not a valid option.")
-268
-269    def preloop(self):
-270        """Scan the current directory for a .db file to use.
-271        If not found, prompt the user for one or to try again
+260            )
+261            choice = input("Enter the number of the option to use: ")
+262            try:
+263                index = int(choice)
+264                if not 1 <= index <= len(options):
+265                    print("Choice out of range.")
+266                    continue
+267                return options[index - 1]
+268            except Exception as e:
+269                print(f"{choice} is not a valid option.")
+270
+271    def preloop(self):
+272        """Scan the current directory for a .db file to use.
+273        If not found, prompt the user for one or to try again
 recursively."""
-272        if self.dbpath:
-273            self.dbpath = Pathier(self.dbpath)
-274            print(f"Defaulting to database {self.dbpath}")
-275        else:
-276            print("Searching for database...")
-277            cwd = Pathier.cwd()
-278            dbs = list(cwd.glob("*.db"))
-279            if len(dbs) == 1:
-280                self.dbpath = dbs[0]
-281                print(f"Using database {self.dbpath}.")
-282            elif dbs:
-283                self.dbpath = self._choose_db(dbs)
-284            else:
-285                print(f"Could not find a .db file in {cwd}.")
-286                path = input(
-287                    "Enter path to .db file to use or press enter to search
+274        if self.dbpath:
+275            self.dbpath = Pathier(self.dbpath)
+276            print(f"Defaulting to database {self.dbpath}")
+277        else:
+278            print("Searching for database...")
+279            cwd = Pathier.cwd()
+280            dbs = list(cwd.glob("*.db"))
+281            if len(dbs) == 1:
+282                self.dbpath = dbs[0]
+283                print(f"Using database {self.dbpath}.")
+284            elif dbs:
+285                self.dbpath = self._choose_db(dbs)
+286            else:
+287                print(f"Could not find a .db file in {cwd}.")
+288                path = input(
+289                    "Enter path to .db file to use or press enter to search
 again recursively: "
-288                )
-289                if path:
-290                    self.dbpath = Pathier(path)
-291                elif not path:
-292                    print("Searching recursively...")
-293                    dbs = list(cwd.rglob("*.db"))
-294                    if len(dbs) == 1:
-295                        self.dbpath = dbs[0]
-296                        print(f"Using database {self.dbpath}.")
-297                    elif dbs:
-298                        self.dbpath = self._choose_db(dbs)
-299                    else:
-300                        print("Could not find a .db file.")
-301                        self.dbpath = Pathier(input("Enter path to a .db
+290                )
+291                if path:
+292                    self.dbpath = Pathier(path)
+293                elif not path:
+294                    print("Searching recursively...")
+295                    dbs = list(cwd.rglob("*.db"))
+296                    if len(dbs) == 1:
+297                        self.dbpath = dbs[0]
+298                        print(f"Using database {self.dbpath}.")
+299                    elif dbs:
+300                        self.dbpath = self._choose_db(dbs)
+301                    else:
+302                        print("Could not find a .db file.")
+303                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-302        if not self.dbpath.exists():
-303            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-304        if not self.dbpath.is_file():
-305            raise ValueError(f"{self.dbpath} is not a file.")
-306
-307
-308def main():
-309    DBShell().cmdloop()
+304        if not self.dbpath.exists():
+305            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+306        if not self.dbpath.is_file():
+307            raise ValueError(f"{self.dbpath} is not a file.")
+308
+309
+310def main():
+311    DBShell().cmdloop()
   ⁰
 class DBShell(argshell.argshell.ArgShell): View Source
 __9class DBShell(argshell.ArgShell):
 _10    intro = "Starting dbshell (enter help or ? for arg info)..."
 _11    prompt = "based>"
 _12    dbpath: Pathier = None  # type: ignore
 _13
@@ -472,248 +474,250 @@
 _96                    args.match_pairs,
 _97                    columns_to_return=args.columns,
 _98                    order_by=args.order_by,
 _99                    limit=args.limit,
 100                    exact_match=not args.partial_matching,
 101                )
 102                db.close()
-103                print(f"{len(results)} matching rows in {table} table:")
+103                print(f"{len(results)} matching rows in {table} table.")
 104                try:
 105                    print(DataBased.data_to_string(results))  # type: ignore
 106                except Exception as e:
 107                    print("Couldn't fit data into a grid.")
 108                    print(*results, sep="\n")
-109                print()
-110
-111    @argshell.with_parser(dbparsers.get_search_parser)
-112    def do_search(self, args: argshell.Namespace):
-113        """Search and return any rows containg the searched substring in any
+109                if results:
+110                    print(f"{len(results)} matching rows in {table} table.")
+111                print()
+112
+113    @argshell.with_parser(dbparsers.get_search_parser)
+114    def do_search(self, args: argshell.Namespace):
+115        """Search and return any rows containg the searched substring in any
 of its columns.
-114        Use the -t/--tables flag to limit the search to a specific table(s).
-115        Use the -c/--columns flag to limit the search to a specific column
+116        Use the -t/--tables flag to limit the search to a specific table(s).
+117        Use the -c/--columns flag to limit the search to a specific column
 (s)."""
-116        print(f"Searching for {args.search_string}...")
-117        with DataBased(self.dbpath) as db:
-118            tables = args.tables or db.get_table_names()
-119            for table in tables:
-120                columns = args.columns or db.get_column_names(table)
-121                matcher = " OR ".join(
-122                    f'{column} LIKE "%{args.search_string}%"' for column in
+118        print(f"Searching for {args.search_string}...")
+119        with DataBased(self.dbpath) as db:
+120            tables = args.tables or db.get_table_names()
+121            for table in tables:
+122                columns = args.columns or db.get_column_names(table)
+123                matcher = " OR ".join(
+124                    f'{column} LIKE "%{args.search_string}%"' for column in
 columns
-123                )
-124                query = f"SELECT * FROM {table} WHERE {matcher};"
-125                results = db.query(query)
-126                results = [db._get_dict(table, result) for result in
+125                )
+126                query = f"SELECT * FROM {table} WHERE {matcher};"
+127                results = db.query(query)
+128                results = [db._get_dict(table, result) for result in
 results]
-127                print(f"Found {len(results)} results in {table} table.")
-128                print(DataBased.data_to_string(results))
-129
-130    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-131    def do_count(self, args: argshell.Namespace):
-132        """Print the number of rows in the database.
-133        Use the -t/--tables flag to limit results to a specific table(s).
-134        Use the -m/--match_pairs flag to limit the results to rows matching
+129                print(f"Found {len(results)} results in {table} table.")
+130                print(DataBased.data_to_string(results))
+131
+132    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+133    def do_count(self, args: argshell.Namespace):
+134        """Print the number of rows in the database.
+135        Use the -t/--tables flag to limit results to a specific table(s).
+136        Use the -m/--match_pairs flag to limit the results to rows matching
 these criteria.
-135        Use the -p/--partial_matching flag to enable substring matching on -
+137        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-136        Pass -h/--help flag for parser help."""
-137        print("Counting rows...")
-138        with DataBased(self.dbpath) as db:
-139            tables = args.tables or db.get_table_names()
-140            for table in tables:
-141                num_rows = db.count(table, args.match_pairs, not
+138        Pass -h/--help flag for parser help."""
+139        print("Counting rows...")
+140        with DataBased(self.dbpath) as db:
+141            tables = args.tables or db.get_table_names()
+142            for table in tables:
+143                num_rows = db.count(table, args.match_pairs, not
 args.partial_matching)
-142                print(f"{num_rows} matching rows in {table} table.")
-143
-144    def do_query(self, arg: str):
-145        """Execute a query against the current database."""
-146        print(f"Executing {arg}")
-147        with DataBased(self.dbpath) as db:
-148            results = db.query(arg)
-149        try:
-150            try:
-151                print(griddy(results))
-152            except Exception as e:
-153                for result in results:
-154                    print(*result, sep="|-|")
-155        except Exception as e:
-156            print(f"{type(e).__name__}: {e}")
-157        print(f"{db.cursor.rowcount} affected rows")
-158
-159    @argshell.with_parser(dbparsers.get_update_parser,
-[dbparsers.convert_match_pairs])
-160    def do_update(self, args: argshell.Namespace):
-161        """Update a column to a new value.
-162        Two required args: the column (-c/--column) to update and the value
+144                print(f"{num_rows} matching rows in {table} table.")
+145
+146    def do_query(self, arg: str):
+147        """Execute a query against the current database."""
+148        print(f"Executing {arg}")
+149        with DataBased(self.dbpath) as db:
+150            results = db.query(arg)
+151        try:
+152            try:
+153                print(griddy(results))
+154            except Exception as e:
+155                for result in results:
+156                    print(*result, sep="|-|")
+157        except Exception as e:
+158            print(f"{type(e).__name__}: {e}")
+159        print(f"{db.cursor.rowcount} affected rows")
+160
+161    @argshell.with_parser(dbparsers.get_update_parser,
+[dbparsers.convert_match_pairs])
+162    def do_update(self, args: argshell.Namespace):
+163        """Update a column to a new value.
+164        Two required args: the column (-c/--column) to update and the value
 (-v/--value) to update to.
-163        Use the -t/--tables flag to limit what tables are updated.
-164        Use the -m/--match_pairs flag to specify which rows are updated.
-165        Use the -p/--partial_matching flag to enable substring matching on -
+165        Use the -t/--tables flag to limit what tables are updated.
+166        Use the -m/--match_pairs flag to specify which rows are updated.
+167        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-166        >>> based>update -c username -v big_chungus -t users -m username
+168        >>> based>update -c username -v big_chungus -t users -m username
 lil_chungus
-167
-168        ^will update the username in the users 'table' to 'big_chungus'
+169
+170        ^will update the username in the users 'table' to 'big_chungus'
 where the username is currently 'lil_chungus'^"""
-169        print("Updating rows...")
-170        with DataBased(self.dbpath) as db:
-171            tables = args.tables or db.get_table_names()
-172            for table in tables:
-173                num_updates = db.update(
-174                    table,
-175                    args.column,
-176                    args.new_value,
-177                    args.match_pairs,
-178                    not args.partial_matching,
-179                )
-180                print(f"Updated {num_updates} rows in {table} table.")
-181
-182    @argshell.with_parser(dbparsers.get_lookup_parser,
-[dbparsers.convert_match_pairs])
-183    def do_delete(self, args: argshell.Namespace):
-184        """Delete rows from the database.
-185        Use the -t/--tables flag to limit what tables rows are deleted from.
-186        Use the -m/--match_pairs flag to specify which rows are deleted.
-187        Use the -p/--partial_matching flag to enable substring matching on -
+171        print("Updating rows...")
+172        with DataBased(self.dbpath) as db:
+173            tables = args.tables or db.get_table_names()
+174            for table in tables:
+175                num_updates = db.update(
+176                    table,
+177                    args.column,
+178                    args.new_value,
+179                    args.match_pairs,
+180                    not args.partial_matching,
+181                )
+182                print(f"Updated {num_updates} rows in {table} table.")
+183
+184    @argshell.with_parser(dbparsers.get_lookup_parser,
+[dbparsers.convert_match_pairs])
+185    def do_delete(self, args: argshell.Namespace):
+186        """Delete rows from the database.
+187        Use the -t/--tables flag to limit what tables rows are deleted from.
+188        Use the -m/--match_pairs flag to specify which rows are deleted.
+189        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-188        >>> based>delete -t users -m username chungus -p
-189
-190        ^will delete all rows in the 'users' table whose username contains
+190        >>> based>delete -t users -m username chungus -p
+191
+192        ^will delete all rows in the 'users' table whose username contains
 'chungus'^"""
-191        print("Deleting records...")
-192        with DataBased(self.dbpath) as db:
-193            tables = args.tables or db.get_table_names()
-194            for table in tables:
-195                num_rows = db.delete(table, args.match_pairs, not
+193        print("Deleting records...")
+194        with DataBased(self.dbpath) as db:
+195            tables = args.tables or db.get_table_names()
+196            for table in tables:
+197                num_rows = db.delete(table, args.match_pairs, not
 args.partial_matching)
-196                print(f"Deleted {num_rows} rows from {table} table.")
-197
-198    @argshell.with_parser(dbparsers.get_add_column_parser)
-199    def do_add_column(self, args: argshell.Namespace):
-200        """Add a new column to the specified tables."""
-201        with DataBased(self.dbpath) as db:
-202            tables = args.tables or db.get_table_names()
-203            for table in tables:
-204                db.add_column(table, args.column_name, args.type,
+198                print(f"Deleted {num_rows} rows from {table} table.")
+199
+200    @argshell.with_parser(dbparsers.get_add_column_parser)
+201    def do_add_column(self, args: argshell.Namespace):
+202        """Add a new column to the specified tables."""
+203        with DataBased(self.dbpath) as db:
+204            tables = args.tables or db.get_table_names()
+205            for table in tables:
+206                db.add_column(table, args.column_name, args.type,
 args.default_value)
-205
-206    def do_flush_log(self, arg: str):
-207        """Clear the log file for this database."""
-208        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-209        if not log_path.exists():
-210            print(f"No log file at path {log_path}")
-211        else:
-212            print(f"Flushing log...")
-213            log_path.write_text("")
-214
-215    def do_scan_dbs(self, arg: str):
-216        """Scan the current working directory for `*.db` files and display
+207
+208    def do_flush_log(self, arg: str):
+209        """Clear the log file for this database."""
+210        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+211        if not log_path.exists():
+212            print(f"No log file at path {log_path}")
+213        else:
+214            print(f"Flushing log...")
+215            log_path.write_text("")
+216
+217    def do_scan_dbs(self, arg: str):
+218        """Scan the current working directory for `*.db` files and display
 them.
-217
-218        If the command is entered as `based>scan_dbs r`, the scan will be
+219
+220        If the command is entered as `based>scan_dbs r`, the scan will be
 performed recursively."""
-219        cwd = Pathier.cwd()
-220        if arg.strip() == "r":
-221            dbs = cwd.rglob("*.db")
-222        else:
-223            dbs = cwd.glob("*.db")
-224        for db in dbs:
-225            print(db.separate(cwd.stem))
-226
-227    def do_customize(self, arg: str):
-228        """Generate a template file in the current working directory for
+221        cwd = Pathier.cwd()
+222        if arg.strip() == "r":
+223            dbs = cwd.rglob("*.db")
+224        else:
+225            dbs = cwd.glob("*.db")
+226        for db in dbs:
+227            print(db.separate(cwd.stem))
+228
+229    def do_customize(self, arg: str):
+230        """Generate a template file in the current working directory for
 creating a custom DBShell class.
-229        Expects one argument: the name of the custom dbshell.
-230        This will be used to name the generated file as well as several
+231        Expects one argument: the name of the custom dbshell.
+232        This will be used to name the generated file as well as several
 components in the file content."""
-231        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+233        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
 (".py")
-232        if custom_file.exists():
-233            print(f"Error: {custom_file.name} already exists in this
+234        if custom_file.exists():
+235            print(f"Error: {custom_file.name} already exists in this
 location.")
-234        else:
-235            variable_name = "_".join(word for word in arg.lower().split())
-236            class_name = "".join(word.capitalize() for word in arg.split())
-237            content = (Pathier(__file__).parent /
+236        else:
+237            variable_name = "_".join(word for word in arg.lower().split())
+238            class_name = "".join(word.capitalize() for word in arg.split())
+239            content = (Pathier(__file__).parent /
 "customshell.py").read_text()
-238            content = content.replace("CustomShell", class_name)
-239            content = content.replace("customshell", variable_name)
-240            custom_file.write_text(content)
-241
-242    def do_vacuum(self, arg: str):
-243        """Reduce database disk memory."""
-244        starting_size = self.dbpath.size()
-245        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-246        print("Vacuuming database...")
-247        with DataBased(self.dbpath) as db:
-248            db.vacuum()
-249        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-250        print(f"Freed up {Pathier.format_size(starting_size -
+240            content = content.replace("CustomShell", class_name)
+241            content = content.replace("customshell", variable_name)
+242            custom_file.write_text(content)
+243
+244    def do_vacuum(self, arg: str):
+245        """Reduce database disk memory."""
+246        starting_size = self.dbpath.size()
+247        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+248        print("Vacuuming database...")
+249        with DataBased(self.dbpath) as db:
+250            db.vacuum()
+251        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+252        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
-251
-252    def _choose_db(self, options: list[Pathier]) -> Pathier:
-253        """Prompt the user to select from a list of files."""
-254        cwd = Pathier.cwd()
-255        paths = [path.separate(cwd.stem) for path in options]
-256        while True:
-257            print(
-258                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+253
+254    def _choose_db(self, options: list[Pathier]) -> Pathier:
+255        """Prompt the user to select from a list of files."""
+256        cwd = Pathier.cwd()
+257        paths = [path.separate(cwd.stem) for path in options]
+258        while True:
+259            print(
+260                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-259            )
-260            choice = input("Enter the number of the option to use: ")
-261            try:
-262                index = int(choice)
-263                if not 1 <= index <= len(options):
-264                    print("Choice out of range.")
-265                    continue
-266                return options[index - 1]
-267            except Exception as e:
-268                print(f"{choice} is not a valid option.")
-269
-270    def preloop(self):
-271        """Scan the current directory for a .db file to use.
-272        If not found, prompt the user for one or to try again
+261            )
+262            choice = input("Enter the number of the option to use: ")
+263            try:
+264                index = int(choice)
+265                if not 1 <= index <= len(options):
+266                    print("Choice out of range.")
+267                    continue
+268                return options[index - 1]
+269            except Exception as e:
+270                print(f"{choice} is not a valid option.")
+271
+272    def preloop(self):
+273        """Scan the current directory for a .db file to use.
+274        If not found, prompt the user for one or to try again
 recursively."""
-273        if self.dbpath:
-274            self.dbpath = Pathier(self.dbpath)
-275            print(f"Defaulting to database {self.dbpath}")
-276        else:
-277            print("Searching for database...")
-278            cwd = Pathier.cwd()
-279            dbs = list(cwd.glob("*.db"))
-280            if len(dbs) == 1:
-281                self.dbpath = dbs[0]
-282                print(f"Using database {self.dbpath}.")
-283            elif dbs:
-284                self.dbpath = self._choose_db(dbs)
-285            else:
-286                print(f"Could not find a .db file in {cwd}.")
-287                path = input(
-288                    "Enter path to .db file to use or press enter to search
+275        if self.dbpath:
+276            self.dbpath = Pathier(self.dbpath)
+277            print(f"Defaulting to database {self.dbpath}")
+278        else:
+279            print("Searching for database...")
+280            cwd = Pathier.cwd()
+281            dbs = list(cwd.glob("*.db"))
+282            if len(dbs) == 1:
+283                self.dbpath = dbs[0]
+284                print(f"Using database {self.dbpath}.")
+285            elif dbs:
+286                self.dbpath = self._choose_db(dbs)
+287            else:
+288                print(f"Could not find a .db file in {cwd}.")
+289                path = input(
+290                    "Enter path to .db file to use or press enter to search
 again recursively: "
-289                )
-290                if path:
-291                    self.dbpath = Pathier(path)
-292                elif not path:
-293                    print("Searching recursively...")
-294                    dbs = list(cwd.rglob("*.db"))
-295                    if len(dbs) == 1:
-296                        self.dbpath = dbs[0]
-297                        print(f"Using database {self.dbpath}.")
-298                    elif dbs:
-299                        self.dbpath = self._choose_db(dbs)
-300                    else:
-301                        print("Could not find a .db file.")
-302                        self.dbpath = Pathier(input("Enter path to a .db
+291                )
+292                if path:
+293                    self.dbpath = Pathier(path)
+294                elif not path:
+295                    print("Searching recursively...")
+296                    dbs = list(cwd.rglob("*.db"))
+297                    if len(dbs) == 1:
+298                        self.dbpath = dbs[0]
+299                        print(f"Using database {self.dbpath}.")
+300                    elif dbs:
+301                        self.dbpath = self._choose_db(dbs)
+302                    else:
+303                        print("Could not find a .db file.")
+304                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-303        if not self.dbpath.exists():
-304            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-305        if not self.dbpath.is_file():
-306            raise ValueError(f"{self.dbpath} is not a file.")
+305        if not self.dbpath.exists():
+306            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+307        if not self.dbpath.is_file():
+308            raise ValueError(f"{self.dbpath} is not a file.")
 Subclass this to create custom ArgShells.
 ⁰
 def do_use_db(self, arg: str): View Source
 14    def do_use_db(self, arg: str):
 15        """Set which database file to use."""
 16        dbpath = Pathier(arg)
 17        if not dbpath.exists():
@@ -828,287 +832,289 @@
 _96                    args.match_pairs,
 _97                    columns_to_return=args.columns,
 _98                    order_by=args.order_by,
 _99                    limit=args.limit,
 100                    exact_match=not args.partial_matching,
 101                )
 102                db.close()
-103                print(f"{len(results)} matching rows in {table} table:")
+103                print(f"{len(results)} matching rows in {table} table.")
 104                try:
 105                    print(DataBased.data_to_string(results))  # type: ignore
 106                except Exception as e:
 107                    print("Couldn't fit data into a grid.")
 108                    print(*results, sep="\n")
-109                print()
+109                if results:
+110                    print(f"{len(results)} matching rows in {table} table.")
+111                print()
 Find and print rows from the database. Use the -t/--tables, -m/--match_pairs,
 and -l/--limit flags to limit the search. Use the -c/--columns flag to limit
 what columns are printed. Use the -o/--order_by flag to order the results. Use
 the -p/--partial_matching flag to enable substring matching on -m/--match_pairs
 Pass -h/--help flag for parser help.
 ⁰
 @argshell.with_parser(dbparsers.get_search_parser)
 def do_search(self, args: argshell.argshell.Namespace): View Source
-111    @argshell.with_parser(dbparsers.get_search_parser)
-112    def do_search(self, args: argshell.Namespace):
-113        """Search and return any rows containg the searched substring in any
+113    @argshell.with_parser(dbparsers.get_search_parser)
+114    def do_search(self, args: argshell.Namespace):
+115        """Search and return any rows containg the searched substring in any
 of its columns.
-114        Use the -t/--tables flag to limit the search to a specific table(s).
-115        Use the -c/--columns flag to limit the search to a specific column
+116        Use the -t/--tables flag to limit the search to a specific table(s).
+117        Use the -c/--columns flag to limit the search to a specific column
 (s)."""
-116        print(f"Searching for {args.search_string}...")
-117        with DataBased(self.dbpath) as db:
-118            tables = args.tables or db.get_table_names()
-119            for table in tables:
-120                columns = args.columns or db.get_column_names(table)
-121                matcher = " OR ".join(
-122                    f'{column} LIKE "%{args.search_string}%"' for column in
+118        print(f"Searching for {args.search_string}...")
+119        with DataBased(self.dbpath) as db:
+120            tables = args.tables or db.get_table_names()
+121            for table in tables:
+122                columns = args.columns or db.get_column_names(table)
+123                matcher = " OR ".join(
+124                    f'{column} LIKE "%{args.search_string}%"' for column in
 columns
-123                )
-124                query = f"SELECT * FROM {table} WHERE {matcher};"
-125                results = db.query(query)
-126                results = [db._get_dict(table, result) for result in
+125                )
+126                query = f"SELECT * FROM {table} WHERE {matcher};"
+127                results = db.query(query)
+128                results = [db._get_dict(table, result) for result in
 results]
-127                print(f"Found {len(results)} results in {table} table.")
-128                print(DataBased.data_to_string(results))
+129                print(f"Found {len(results)} results in {table} table.")
+130                print(DataBased.data_to_string(results))
 Search and return any rows containg the searched substring in any of its
 columns. Use the -t/--tables flag to limit the search to a specific table(s).
 Use the -c/--columns flag to limit the search to a specific column(s).
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
 def do_count(self, args: argshell.argshell.Namespace): View Source
-130    @argshell.with_parser(dbparsers.get_lookup_parser,
+132    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-131    def do_count(self, args: argshell.Namespace):
-132        """Print the number of rows in the database.
-133        Use the -t/--tables flag to limit results to a specific table(s).
-134        Use the -m/--match_pairs flag to limit the results to rows matching
+133    def do_count(self, args: argshell.Namespace):
+134        """Print the number of rows in the database.
+135        Use the -t/--tables flag to limit results to a specific table(s).
+136        Use the -m/--match_pairs flag to limit the results to rows matching
 these criteria.
-135        Use the -p/--partial_matching flag to enable substring matching on -
+137        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-136        Pass -h/--help flag for parser help."""
-137        print("Counting rows...")
-138        with DataBased(self.dbpath) as db:
-139            tables = args.tables or db.get_table_names()
-140            for table in tables:
-141                num_rows = db.count(table, args.match_pairs, not
+138        Pass -h/--help flag for parser help."""
+139        print("Counting rows...")
+140        with DataBased(self.dbpath) as db:
+141            tables = args.tables or db.get_table_names()
+142            for table in tables:
+143                num_rows = db.count(table, args.match_pairs, not
 args.partial_matching)
-142                print(f"{num_rows} matching rows in {table} table.")
+144                print(f"{num_rows} matching rows in {table} table.")
 Print the number of rows in the database. Use the -t/--tables flag to limit
 results to a specific table(s). Use the -m/--match_pairs flag to limit the
 results to rows matching these criteria. Use the -p/--partial_matching flag to
 enable substring matching on -m/--match_pairs. Pass -h/--help flag for parser
 help.
 ⁰
 def do_query(self, arg: str): View Source
-144    def do_query(self, arg: str):
-145        """Execute a query against the current database."""
-146        print(f"Executing {arg}")
-147        with DataBased(self.dbpath) as db:
-148            results = db.query(arg)
-149        try:
-150            try:
-151                print(griddy(results))
-152            except Exception as e:
-153                for result in results:
-154                    print(*result, sep="|-|")
-155        except Exception as e:
-156            print(f"{type(e).__name__}: {e}")
-157        print(f"{db.cursor.rowcount} affected rows")
+146    def do_query(self, arg: str):
+147        """Execute a query against the current database."""
+148        print(f"Executing {arg}")
+149        with DataBased(self.dbpath) as db:
+150            results = db.query(arg)
+151        try:
+152            try:
+153                print(griddy(results))
+154            except Exception as e:
+155                for result in results:
+156                    print(*result, sep="|-|")
+157        except Exception as e:
+158            print(f"{type(e).__name__}: {e}")
+159        print(f"{db.cursor.rowcount} affected rows")
 Execute a query against the current database.
 ⁰
 @argshell.with_parser(dbparsers.get_update_parser,
 [dbparsers.convert_match_pairs])
 def do_update(self, args: argshell.argshell.Namespace): View Source
-159    @argshell.with_parser(dbparsers.get_update_parser,
+161    @argshell.with_parser(dbparsers.get_update_parser,
 [dbparsers.convert_match_pairs])
-160    def do_update(self, args: argshell.Namespace):
-161        """Update a column to a new value.
-162        Two required args: the column (-c/--column) to update and the value
+162    def do_update(self, args: argshell.Namespace):
+163        """Update a column to a new value.
+164        Two required args: the column (-c/--column) to update and the value
 (-v/--value) to update to.
-163        Use the -t/--tables flag to limit what tables are updated.
-164        Use the -m/--match_pairs flag to specify which rows are updated.
-165        Use the -p/--partial_matching flag to enable substring matching on -
+165        Use the -t/--tables flag to limit what tables are updated.
+166        Use the -m/--match_pairs flag to specify which rows are updated.
+167        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-166        >>> based>update -c username -v big_chungus -t users -m username
+168        >>> based>update -c username -v big_chungus -t users -m username
 lil_chungus
-167
-168        ^will update the username in the users 'table' to 'big_chungus'
+169
+170        ^will update the username in the users 'table' to 'big_chungus'
 where the username is currently 'lil_chungus'^"""
-169        print("Updating rows...")
-170        with DataBased(self.dbpath) as db:
-171            tables = args.tables or db.get_table_names()
-172            for table in tables:
-173                num_updates = db.update(
-174                    table,
-175                    args.column,
-176                    args.new_value,
-177                    args.match_pairs,
-178                    not args.partial_matching,
-179                )
-180                print(f"Updated {num_updates} rows in {table} table.")
+171        print("Updating rows...")
+172        with DataBased(self.dbpath) as db:
+173            tables = args.tables or db.get_table_names()
+174            for table in tables:
+175                num_updates = db.update(
+176                    table,
+177                    args.column,
+178                    args.new_value,
+179                    args.match_pairs,
+180                    not args.partial_matching,
+181                )
+182                print(f"Updated {num_updates} rows in {table} table.")
 Update a column to a new value. Two required args: the column (-c/--column) to
 update and the value (-v/--value) to update to. Use the -t/--tables flag to
 limit what tables are updated. Use the -m/--match_pairs flag to specify which
 rows are updated. Use the -p/--partial_matching flag to enable substring
 matching on -m/--match_pairs.
 >>> based>update -c username -v big_chungus -t users -m username lil_chungus
 ^will update the username in the users 'table' to 'big_chungus' where the
 username is currently 'lil_chungus'^
 ⁰
 @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
 def do_delete(self, args: argshell.argshell.Namespace): View Source
-182    @argshell.with_parser(dbparsers.get_lookup_parser,
+184    @argshell.with_parser(dbparsers.get_lookup_parser,
 [dbparsers.convert_match_pairs])
-183    def do_delete(self, args: argshell.Namespace):
-184        """Delete rows from the database.
-185        Use the -t/--tables flag to limit what tables rows are deleted from.
-186        Use the -m/--match_pairs flag to specify which rows are deleted.
-187        Use the -p/--partial_matching flag to enable substring matching on -
+185    def do_delete(self, args: argshell.Namespace):
+186        """Delete rows from the database.
+187        Use the -t/--tables flag to limit what tables rows are deleted from.
+188        Use the -m/--match_pairs flag to specify which rows are deleted.
+189        Use the -p/--partial_matching flag to enable substring matching on -
 m/--match_pairs.
-188        >>> based>delete -t users -m username chungus -p
-189
-190        ^will delete all rows in the 'users' table whose username contains
+190        >>> based>delete -t users -m username chungus -p
+191
+192        ^will delete all rows in the 'users' table whose username contains
 'chungus'^"""
-191        print("Deleting records...")
-192        with DataBased(self.dbpath) as db:
-193            tables = args.tables or db.get_table_names()
-194            for table in tables:
-195                num_rows = db.delete(table, args.match_pairs, not
+193        print("Deleting records...")
+194        with DataBased(self.dbpath) as db:
+195            tables = args.tables or db.get_table_names()
+196            for table in tables:
+197                num_rows = db.delete(table, args.match_pairs, not
 args.partial_matching)
-196                print(f"Deleted {num_rows} rows from {table} table.")
+198                print(f"Deleted {num_rows} rows from {table} table.")
 Delete rows from the database. Use the -t/--tables flag to limit what tables
 rows are deleted from. Use the -m/--match_pairs flag to specify which rows are
 deleted. Use the -p/--partial_matching flag to enable substring matching on -m/
 --match_pairs.
 >>> based>delete -t users -m username chungus -p
 ^will delete all rows in the 'users' table whose username contains 'chungus'^
 ⁰
 @argshell.with_parser(dbparsers.get_add_column_parser)
 def do_add_column(self, args: argshell.argshell.Namespace): View Source
-198    @argshell.with_parser(dbparsers.get_add_column_parser)
-199    def do_add_column(self, args: argshell.Namespace):
-200        """Add a new column to the specified tables."""
-201        with DataBased(self.dbpath) as db:
-202            tables = args.tables or db.get_table_names()
-203            for table in tables:
-204                db.add_column(table, args.column_name, args.type,
+200    @argshell.with_parser(dbparsers.get_add_column_parser)
+201    def do_add_column(self, args: argshell.Namespace):
+202        """Add a new column to the specified tables."""
+203        with DataBased(self.dbpath) as db:
+204            tables = args.tables or db.get_table_names()
+205            for table in tables:
+206                db.add_column(table, args.column_name, args.type,
 args.default_value)
 Add a new column to the specified tables.
 ⁰
 def do_flush_log(self, arg: str): View Source
-206    def do_flush_log(self, arg: str):
-207        """Clear the log file for this database."""
-208        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
-209        if not log_path.exists():
-210            print(f"No log file at path {log_path}")
-211        else:
-212            print(f"Flushing log...")
-213            log_path.write_text("")
+208    def do_flush_log(self, arg: str):
+209        """Clear the log file for this database."""
+210        log_path = self.dbpath.with_name(self.dbpath.stem + "db.log")
+211        if not log_path.exists():
+212            print(f"No log file at path {log_path}")
+213        else:
+214            print(f"Flushing log...")
+215            log_path.write_text("")
 Clear the log file for this database.
 ⁰
 def do_scan_dbs(self, arg: str): View Source
-215    def do_scan_dbs(self, arg: str):
-216        """Scan the current working directory for `*.db` files and display
+217    def do_scan_dbs(self, arg: str):
+218        """Scan the current working directory for `*.db` files and display
 them.
-217
-218        If the command is entered as `based>scan_dbs r`, the scan will be
+219
+220        If the command is entered as `based>scan_dbs r`, the scan will be
 performed recursively."""
-219        cwd = Pathier.cwd()
-220        if arg.strip() == "r":
-221            dbs = cwd.rglob("*.db")
-222        else:
-223            dbs = cwd.glob("*.db")
-224        for db in dbs:
-225            print(db.separate(cwd.stem))
+221        cwd = Pathier.cwd()
+222        if arg.strip() == "r":
+223            dbs = cwd.rglob("*.db")
+224        else:
+225            dbs = cwd.glob("*.db")
+226        for db in dbs:
+227            print(db.separate(cwd.stem))
 Scan the current working directory for *.db files and display them.
 If the command is entered as based>scan_dbs r, the scan will be performed
 recursively.
 ⁰
 def do_customize(self, arg: str): View Source
-227    def do_customize(self, arg: str):
-228        """Generate a template file in the current working directory for
+229    def do_customize(self, arg: str):
+230        """Generate a template file in the current working directory for
 creating a custom DBShell class.
-229        Expects one argument: the name of the custom dbshell.
-230        This will be used to name the generated file as well as several
+231        Expects one argument: the name of the custom dbshell.
+232        This will be used to name the generated file as well as several
 components in the file content."""
-231        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
+233        custom_file = (Pathier.cwd() / arg.replace(" ", "_")).with_suffix
 (".py")
-232        if custom_file.exists():
-233            print(f"Error: {custom_file.name} already exists in this
+234        if custom_file.exists():
+235            print(f"Error: {custom_file.name} already exists in this
 location.")
-234        else:
-235            variable_name = "_".join(word for word in arg.lower().split())
-236            class_name = "".join(word.capitalize() for word in arg.split())
-237            content = (Pathier(__file__).parent /
+236        else:
+237            variable_name = "_".join(word for word in arg.lower().split())
+238            class_name = "".join(word.capitalize() for word in arg.split())
+239            content = (Pathier(__file__).parent /
 "customshell.py").read_text()
-238            content = content.replace("CustomShell", class_name)
-239            content = content.replace("customshell", variable_name)
-240            custom_file.write_text(content)
+240            content = content.replace("CustomShell", class_name)
+241            content = content.replace("customshell", variable_name)
+242            custom_file.write_text(content)
 Generate a template file in the current working directory for creating a custom
 DBShell class. Expects one argument: the name of the custom dbshell. This will
 be used to name the generated file as well as several components in the file
 content.
 ⁰
 def do_vacuum(self, arg: str): View Source
-242    def do_vacuum(self, arg: str):
-243        """Reduce database disk memory."""
-244        starting_size = self.dbpath.size()
-245        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
-246        print("Vacuuming database...")
-247        with DataBased(self.dbpath) as db:
-248            db.vacuum()
-249        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-250        print(f"Freed up {Pathier.format_size(starting_size -
+244    def do_vacuum(self, arg: str):
+245        """Reduce database disk memory."""
+246        starting_size = self.dbpath.size()
+247        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
+248        print("Vacuuming database...")
+249        with DataBased(self.dbpath) as db:
+250            db.vacuum()
+251        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+252        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
 Reduce database disk memory.
 ⁰
 def preloop(self): View Source
-270    def preloop(self):
-271        """Scan the current directory for a .db file to use.
-272        If not found, prompt the user for one or to try again
+272    def preloop(self):
+273        """Scan the current directory for a .db file to use.
+274        If not found, prompt the user for one or to try again
 recursively."""
-273        if self.dbpath:
-274            self.dbpath = Pathier(self.dbpath)
-275            print(f"Defaulting to database {self.dbpath}")
-276        else:
-277            print("Searching for database...")
-278            cwd = Pathier.cwd()
-279            dbs = list(cwd.glob("*.db"))
-280            if len(dbs) == 1:
-281                self.dbpath = dbs[0]
-282                print(f"Using database {self.dbpath}.")
-283            elif dbs:
-284                self.dbpath = self._choose_db(dbs)
-285            else:
-286                print(f"Could not find a .db file in {cwd}.")
-287                path = input(
-288                    "Enter path to .db file to use or press enter to search
+275        if self.dbpath:
+276            self.dbpath = Pathier(self.dbpath)
+277            print(f"Defaulting to database {self.dbpath}")
+278        else:
+279            print("Searching for database...")
+280            cwd = Pathier.cwd()
+281            dbs = list(cwd.glob("*.db"))
+282            if len(dbs) == 1:
+283                self.dbpath = dbs[0]
+284                print(f"Using database {self.dbpath}.")
+285            elif dbs:
+286                self.dbpath = self._choose_db(dbs)
+287            else:
+288                print(f"Could not find a .db file in {cwd}.")
+289                path = input(
+290                    "Enter path to .db file to use or press enter to search
 again recursively: "
-289                )
-290                if path:
-291                    self.dbpath = Pathier(path)
-292                elif not path:
-293                    print("Searching recursively...")
-294                    dbs = list(cwd.rglob("*.db"))
-295                    if len(dbs) == 1:
-296                        self.dbpath = dbs[0]
-297                        print(f"Using database {self.dbpath}.")
-298                    elif dbs:
-299                        self.dbpath = self._choose_db(dbs)
-300                    else:
-301                        print("Could not find a .db file.")
-302                        self.dbpath = Pathier(input("Enter path to a .db
+291                )
+292                if path:
+293                    self.dbpath = Pathier(path)
+294                elif not path:
+295                    print("Searching recursively...")
+296                    dbs = list(cwd.rglob("*.db"))
+297                    if len(dbs) == 1:
+298                        self.dbpath = dbs[0]
+299                        print(f"Using database {self.dbpath}.")
+300                    elif dbs:
+301                        self.dbpath = self._choose_db(dbs)
+302                    else:
+303                        print("Could not find a .db file.")
+304                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-303        if not self.dbpath.exists():
-304            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-305        if not self.dbpath.is_file():
-306            raise ValueError(f"{self.dbpath} is not a file.")
+305        if not self.dbpath.exists():
+306            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+307        if not self.dbpath.is_file():
+308            raise ValueError(f"{self.dbpath} is not a file.")
 Scan the current directory for a .db file to use. If not found, prompt the user
 for one or to try again recursively.
 ** Inherited Members **
   ⁰
 def main(): View Source
-309def main():
-310    DBShell().cmdloop()
+311def main():
+312    DBShell().cmdloop()
```

### Comparing `databased-2.4.0/src/databased/customshell.py` & `databased-2.4.1/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/src/databased/databased.py` & `databased-2.4.1/src/databased/databased.py`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/src/databased/dbparsers.py` & `databased-2.4.1/src/databased/dbparsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         "--tables",
         type=str,
         nargs="*",
         default=[],
         help=""" Only display info for this table(s). """,
     )
     parser.add_argument(
-        "-rc",
+        "-c",
         "--rowcount",
         action="store_true",
         help=""" Count and display the number of rows for each table. """,
     )
     return parser
```

### Comparing `databased-2.4.0/src/databased/dbshell.py` & `databased-2.4.1/src/databased/dbshell.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,20 +95,22 @@
                     args.match_pairs,
                     columns_to_return=args.columns,
                     order_by=args.order_by,
                     limit=args.limit,
                     exact_match=not args.partial_matching,
                 )
                 db.close()
-                print(f"{len(results)} matching rows in {table} table:")
+                print(f"{len(results)} matching rows in {table} table.")
                 try:
                     print(DataBased.data_to_string(results))  # type: ignore
                 except Exception as e:
                     print("Couldn't fit data into a grid.")
                     print(*results, sep="\n")
+                if results:
+                    print(f"{len(results)} matching rows in {table} table.")
                 print()
 
     @argshell.with_parser(dbparsers.get_search_parser)
     def do_search(self, args: argshell.Namespace):
         """Search and return any rows containg the searched substring in any of its columns.
         Use the -t/--tables flag to limit the search to a specific table(s).
         Use the -c/--columns flag to limit the search to a specific column(s)."""
```

### Comparing `databased-2.4.0/LICENSE.txt` & `databased-2.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/README.md` & `databased-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `databased-2.4.0/pyproject.toml` & `databased-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "2.4.0"
+version = "2.4.1"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier", "griddle"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
```

### Comparing `databased-2.4.0/PKG-INFO` & `databased-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 2.4.0
+Version: 2.4.1
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

