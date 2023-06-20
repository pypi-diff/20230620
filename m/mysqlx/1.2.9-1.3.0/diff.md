# Comparing `tmp/mysqlx-1.2.9.tar.gz` & `tmp/mysqlx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.2.9.tar", last modified: Mon Jun 19 14:27:36 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.0.tar", last modified: Tue Jun 20 08:46:38 2023, max compression
```

## Comparing `mysqlx-1.2.9.tar` & `mysqlx-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:27:36.000000 mysqlx-1.2.9/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.9/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.2.9/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.2.9/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.2.9/mysqlx/db.py
--rw-rw-rw-   0        0        0     9832 2023-06-18 07:05:30.000000 mysqlx-1.2.9/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.2.9/mysqlx/orm.py
--rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.2.9/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.9/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.2.9/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3929 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      487 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 14:27:36.000000 mysqlx-1.2.9/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3929 2023-06-19 14:27:36.000000 mysqlx-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3295 2023-06-12 03:58:38.000000 mysqlx-1.2.9/README.md
--rw-rw-rw-   0        0        0     3396 2023-06-19 14:22:34.000000 mysqlx-1.2.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-19 14:27:36.000000 mysqlx-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-06-19 14:25:41.000000 mysqlx-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:27:36.000000 mysqlx-1.2.9/test/
--rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.2.9/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.2.9/test/coder_test.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.2.9/test/dbx_test.py
--rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.2.9/test/db_test.py
--rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.2.9/test/models.py
--rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.2.9/test/orm_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.2.9/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.2.9/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.9/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.0/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.3.0/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.3.0/mysqlx/db.py
+-rw-rw-rw-   0        0        0    10001 2023-06-20 01:39:01.000000 mysqlx-1.3.0/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.3.0/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.3.0/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.0/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3915 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      487 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3915 2023-06-20 08:46:38.000000 mysqlx-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3291 2023-06-20 08:44:43.000000 mysqlx-1.3.0/README.md
+-rw-rw-rw-   0        0        0     3383 2023-06-20 08:44:43.000000 mysqlx-1.3.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:46:38.000000 mysqlx-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-06-20 08:44:43.000000 mysqlx-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/test/
+-rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.3.0/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.0/test/coder_test.py
+-rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.3.0/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.3.0/test/db_test.py
+-rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.3.0/test/models.py
+-rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.3.0/test/orm_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.0/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.0/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.0/test/__init__.py
```

### Comparing `mysqlx-1.2.9/LICENSE` & `mysqlx-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx/coder.py` & `mysqlx-1.3.0/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx/coder.tpl` & `mysqlx-1.3.0/mysqlx/coder.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx/db.py` & `mysqlx-1.3.0/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx/dbx.py` & `mysqlx-1.3.0/mysqlx/dbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,37 +161,39 @@
 
 
 def get_connection():
     return db.get_connection()
 
 
 # ----------------------------------------------------------Load mapper--------------------------------------------------------------------
-def _get_abs_path(path: str):
-    parent_flg = '../'
-    current_flg = './'
-    if path.startswith(parent_flg):
-        idx = path.rindex(parent_flg) + 3
-        parent_path = path[:idx]
-        os.chdir(parent_path)
-        path = path[idx:]
-    elif path.startswith(current_flg):
-        path = path[2:]
-    return os.path.join(os.getcwd(), path)
+# def _get_abs_path(path: str):
+#     parent_flg = '../'
+#     current_flg = './'
+#     if path.startswith(parent_flg):
+#         idx = path.rindex(parent_flg) + 3
+#         parent_path = path[:idx]
+#         os.chdir(parent_path)
+#         path = path[idx:]
+#     elif path.startswith(current_flg):
+#         path = path[2:]
+#     return os.path.join(os.getcwd(), path)
 
 
 def _load_mapper(path: str):
-    if not os.path.isabs(path):
-        path = _get_abs_path(path)
-
-    for f in os.listdir(path):
-        file = os.path.join(path, f)
-        if os.path.isfile(file) and f.endswith(".xml"):
-            _parse_mapper_file(file)
-        elif os.path.isdir(file):
-            _load_mapper(file)
+    # if not os.path.isabs(path):
+    #     path = _get_abs_path(path)
+    if os.path.isfile(path) and path.endswith(".xml"):
+        _parse_mapper_file(path)
+    elif os.path.isdir(path):
+        for f in os.listdir(path):
+            file = os.path.join(path, f)
+            if os.path.isfile(file) and f.endswith(".xml"):
+                _parse_mapper_file(file)
+            elif os.path.isdir(file):
+                _load_mapper(file)
 
 
 def _parse_mapper_file(file: str):
     tree = ET.parse(file)
     root = tree.getroot()
     namespace = root.attrib.get('namespace', '')
     results = list(map(lambda child: _load_sql(namespace, child, file), root))
```

### Comparing `mysqlx-1.2.9/mysqlx/orm.py` & `mysqlx-1.3.0/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx/support.py` & `mysqlx-1.3.0/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.0/mysqlx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.2.9
+Version: 1.3.0
 Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,iBatis,MyBatis,python
 Platform: UNKNOWN
@@ -29,29 +29,28 @@
    db_conf = {
        'host': HOST,
        'port': 3306, 
        'user': 'root', 
        'password': 'xxx', 
        'database': 'test',
        'pool_size': 5,
-       'show_sql': True,
-       'mapper_path': 'mapper'
+       'show_sql': True
    }
 
    if __name__ == '__main__':
        db.init_db(**db_conf)
        
        # Return effect rowcount
        rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, 'insert'
-       assert db.get('select count(1) from user') == 1, 'insert'
+       assert rowcount == 1, '1 effect rowcount'
+       assert db.get('select count(1) from user') == 1, 'count is 1'
 
+       # Return primary key
        id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert id2 > 0, 'save'
-       assert db.get('select count(1) from user') == 2, 'save'
+       assert db.get('select count(1) from user') == 2, 'count is 2'
 
        db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
        assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
 
        db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
        assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
```

### Comparing `mysqlx-1.2.9/PKG-INFO` & `mysqlx-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.2.9
+Version: 1.3.0
 Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,iBatis,MyBatis,python
 Platform: UNKNOWN
@@ -29,29 +29,28 @@
    db_conf = {
        'host': HOST,
        'port': 3306, 
        'user': 'root', 
        'password': 'xxx', 
        'database': 'test',
        'pool_size': 5,
-       'show_sql': True,
-       'mapper_path': 'mapper'
+       'show_sql': True
    }
 
    if __name__ == '__main__':
        db.init_db(**db_conf)
        
        # Return effect rowcount
        rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, 'insert'
-       assert db.get('select count(1) from user') == 1, 'insert'
+       assert rowcount == 1, '1 effect rowcount'
+       assert db.get('select count(1) from user') == 1, 'count is 1'
 
+       # Return primary key
        id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert id2 > 0, 'save'
-       assert db.get('select count(1) from user') == 2, 'save'
+       assert db.get('select count(1) from user') == 2, 'count is 2'
 
        db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
        assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
 
        db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
        assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
```

### Comparing `mysqlx-1.2.9/README.md` & `mysqlx-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 pip install mysqlx
 ```
 ##### Sample
 ```
 from mysqlx import db
 
 db_conf = {
-    'host': HOST,
+    'host': '127.0.0.1',
     'port': 3306, 
     'user': 'root', 
     'password': 'xxx', 
     'database': 'test',
     'pool_size': 5,
-    'show_sql': True,
-    'mapper_path': 'mapper'
+    'show_sql': True
 }
 
 if __name__ == '__main__':
     db.init_db(**db_conf)
     
     # Return effect rowcount
     rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    assert rowcount == 1, 'insert'
-    assert db.get('select count(1) from user') == 1, 'insert'
+    assert rowcount == 1, '1 effect rowcount'
+    assert db.get('select count(1) from user') == 1, 'count is 1'
 
+    # Return primary key
     id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-    assert id2 > 0, 'save'
-    assert db.get('select count(1) from user') == 2, 'save'
+    assert db.get('select count(1) from user') == 2, 'count is 2'
 
     db.execute('update user set name=? where id=?', '王五', id2)
     assert db.get('select name from user where id=?', id2) == '王五', 'execute'
 
     db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
     assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
```

### Comparing `mysqlx-1.2.9/README.rst` & `mysqlx-1.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,28 @@
    db_conf = {
        'host': HOST,
        'port': 3306, 
        'user': 'root', 
        'password': 'xxx', 
        'database': 'test',
        'pool_size': 5,
-       'show_sql': True,
-       'mapper_path': 'mapper'
+       'show_sql': True
    }
 
    if __name__ == '__main__':
        db.init_db(**db_conf)
        
        # Return effect rowcount
        rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, 'insert'
-       assert db.get('select count(1) from user') == 1, 'insert'
+       assert rowcount == 1, '1 effect rowcount'
+       assert db.get('select count(1) from user') == 1, 'count is 1'
 
+       # Return primary key
        id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert id2 > 0, 'save'
-       assert db.get('select count(1) from user') == 2, 'save'
+       assert db.get('select count(1) from user') == 2, 'count is 2'
 
        db.execute('update user set name=? where id=?', '王五', id2)
        assert db.get('select name from user where id=?', id2) == '王五', 'execute'
 
        db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
        assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
```

### Comparing `mysqlx-1.2.9/setup.py` & `mysqlx-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like iBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.2.9',
+    version='1.3.0',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `mysqlx-1.2.9/test/dbx_test.py` & `mysqlx-1.3.0/test/dbx_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/test/db_test.py` & `mysqlx-1.3.0/test/db_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/test/models.py` & `mysqlx-1.3.0/test/models.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/test/orm_test.py` & `mysqlx-1.3.0/test/orm_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.9/test/unit_test.py` & `mysqlx-1.3.0/test/unit_test.py`

 * *Files identical despite different names*

