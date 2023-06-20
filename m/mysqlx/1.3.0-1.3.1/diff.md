# Comparing `tmp/mysqlx-1.3.0.tar.gz` & `tmp/mysqlx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.0.tar", last modified: Tue Jun 20 08:46:38 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.3.1.tar", last modified: Tue Jun 20 09:06:19 2023, max compression
```

## Comparing `mysqlx-1.3.0.tar` & `mysqlx-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx/
--rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.0/mysqlx/coder.py
--rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.3.0/mysqlx/coder.tpl
--rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.3.0/mysqlx/db.py
--rw-rw-rw-   0        0        0    10001 2023-06-20 01:39:01.000000 mysqlx-1.3.0/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.3.0/mysqlx/orm.py
--rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.3.0/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.0/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.0/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3915 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      487 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 08:46:38.000000 mysqlx-1.3.0/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3915 2023-06-20 08:46:38.000000 mysqlx-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3291 2023-06-20 08:44:43.000000 mysqlx-1.3.0/README.md
--rw-rw-rw-   0        0        0     3383 2023-06-20 08:44:43.000000 mysqlx-1.3.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-20 08:46:38.000000 mysqlx-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-06-20 08:44:43.000000 mysqlx-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:46:38.000000 mysqlx-1.3.0/test/
--rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.3.0/test/all_unit_test.py
--rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.0/test/coder_test.py
--rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.3.0/test/dbx_test.py
--rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.3.0/test/db_test.py
--rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.3.0/test/models.py
--rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.3.0/test/orm_test.py
--rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.0/test/unit_test.py
--rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.0/test/user_mapper.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx/
+-rw-rw-rw-   0        0        0     5827 2023-06-19 12:47:48.000000 mysqlx-1.3.1/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1589 2023-06-09 01:09:35.000000 mysqlx-1.3.1/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    17467 2023-06-18 07:05:30.000000 mysqlx-1.3.1/mysqlx/db.py
+-rw-rw-rw-   0        0        0    10001 2023-06-20 01:39:01.000000 mysqlx-1.3.1/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0    30506 2023-06-19 05:19:22.000000 mysqlx-1.3.1/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     6107 2023-06-18 03:07:16.000000 mysqlx-1.3.1/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 14:08:07.000000 mysqlx-1.3.1/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      487 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 09:06:19.000000 mysqlx-1.3.1/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4737 2023-06-20 09:06:19.000000 mysqlx-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4022 2023-06-20 08:57:34.000000 mysqlx-1.3.1/README.md
+-rw-rw-rw-   0        0        0     4185 2023-06-20 09:05:43.000000 mysqlx-1.3.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:06:19.000000 mysqlx-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-06-20 09:01:58.000000 mysqlx-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:06:19.000000 mysqlx-1.3.1/test/
+-rw-rw-rw-   0        0        0      216 2023-06-10 13:13:30.000000 mysqlx-1.3.1/test/all_unit_test.py
+-rw-rw-rw-   0        0        0      312 2023-06-19 03:27:12.000000 mysqlx-1.3.1/test/coder_test.py
+-rw-rw-rw-   0        0        0     2966 2023-06-13 02:46:47.000000 mysqlx-1.3.1/test/dbx_test.py
+-rw-rw-rw-   0        0        0     5025 2023-06-13 09:20:17.000000 mysqlx-1.3.1/test/db_test.py
+-rw-rw-rw-   0        0        0     5090 2023-06-19 12:47:52.000000 mysqlx-1.3.1/test/models.py
+-rw-rw-rw-   0        0        0     6869 2023-06-19 05:16:27.000000 mysqlx-1.3.1/test/orm_test.py
+-rw-rw-rw-   0        0        0      710 2023-06-11 02:56:34.000000 mysqlx-1.3.1/test/unit_test.py
+-rw-rw-rw-   0        0        0      320 2023-06-13 02:39:09.000000 mysqlx-1.3.1/test/user_mapper.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.1/test/__init__.py
```

### Comparing `mysqlx-1.3.0/LICENSE` & `mysqlx-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/coder.py` & `mysqlx-1.3.1/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/coder.tpl` & `mysqlx-1.3.1/mysqlx/coder.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/db.py` & `mysqlx-1.3.1/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/dbx.py` & `mysqlx-1.3.1/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/orm.py` & `mysqlx-1.3.1/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx/support.py` & `mysqlx-1.3.1/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,105 @@
-Metadata-Version: 2.1
-Name: mysqlx
-Version: 1.3.0
-Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
-Home-page: https://gitee.com/summry/mysqlx
-Author: summry
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: sql,MySQL,iBatis,MyBatis,python
-Platform: UNKNOWN
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Install
-'''''''
-
-::
-
-   pip install mysqlx
-
-Sample
-''''''
-
-::
-
-   from mysqlx import db
-
-   db_conf = {
-       'host': HOST,
-       'port': 3306, 
-       'user': 'root', 
-       'password': 'xxx', 
-       'database': 'test',
-       'pool_size': 5,
-       'show_sql': True
-   }
-
-   if __name__ == '__main__':
-       db.init_db(**db_conf)
-       
-       # Return effect rowcount
-       rowcount = db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert rowcount == 1, '1 effect rowcount'
-       assert db.get('select count(1) from user') == 1, 'count is 1'
-
-       # Return primary key
-       id2 = db.save('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       assert db.get('select count(1) from user') == 2, 'count is 2'
-
-       db.execute('update user set name=? where id=?', '鐜嬩簲', id2)
-       assert db.get('select name from user where id=?', id2) == '鐜嬩簲', 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
-
-       db.execute('update user set name=:name where id=:id', name='璧靛叚', id=id2)
-       assert db.query_one('select name from user where id=:id', id=id2)['name'] == '璧靛叚', 'execute'
-
-       args = [
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
-           ('寮犱笁', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
-       ]
-       db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
-       users = db.select('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-       users = db.query('select id, del_flag from user')
-       assert len(users) == 4, 'batch_execute'
-
-       users = db.select('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=?', id2)
-       assert len(users) == 1, 'select'
-
-       users = db.select('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-       users = db.query('select id, del_flag from user where id=:id', id=id2)
-       assert len(users) == 1, 'select'
-
-       db.execute('delete from user where id=? limit 1', id2)
-       assert db.get('select count(1) from user') == 3, 'execute delete'
-
-Transaction
-'''''''''''
-
-::
-
-   @db.with_transaction
-   def test_transaction():
-       db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-       db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-
-   def test_transaction2():
-       with db.transaction():
-           db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-           db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
-
-Note
-''''
-
-::
-
-   get: Return only one object, like count
-   query_one: Return one row with dict
-   select_one: Return one row with tuple
-   find_by_id: Return one row with class instance object
-   query: Return list of dict
-   select: Return list of tuple
-   find: Return list of class instance object
-
-
+##### Install
+```
+pip install mysqlx
+```
+##### Usage Sample
+```
+CREATE TABLE `user` (
+  `id` bigint NOT NULL AUTO_INCREMENT,
+  `name` varchar(45) NOT NULL,
+  `age` int NOT NULL,
+  `birth_date` date DEFAULT NULL,
+  `sex` tinyint DEFAULT NULL,
+  `grade` float DEFAULT NULL,
+  `point` double DEFAULT NULL,
+  `money` decimal(8,4) DEFAULT NULL,
+  `create_by` bigint DEFAULT NULL,
+  `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
+  `update_by` bigint DEFAULT NULL,
+  `update_time` datetime DEFAULT NULL,
+  `del_flag` tinyint NOT NULL DEFAULT '0',
+  PRIMARY KEY (`id`)
+) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+
+
+----------------------------------------------------------------------------------------
+
+from mysqlx import db
+
+db_conf = {
+    'host': '127.0.0.1',
+    'port': 3306, 
+    'user': 'root', 
+    'password': 'xxx', 
+    'database': 'test',
+    'pool_size': 5,
+    'show_sql': True
+}
+
+if __name__ == '__main__':
+    db.init_db(**db_conf)
+    
+    # Return effect rowcount
+    rowcount = db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert rowcount == 1, '1 effect rowcount'
+    assert db.get('select count(1) from user') == 1, 'count is 1'
+
+    # Return primary key
+    id2 = db.save('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    assert db.get('select count(1) from user') == 2, 'count is 2'
+
+    db.execute('update user set name=? where id=?', '王五', id2)
+    assert db.get('select name from user where id=?', id2) == '王五', 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.select_one('select id, name from user where id=:id', id=id2)[0] == id2, 'execute'
+
+    db.execute('update user set name=:name where id=:id', name='赵六', id=id2)
+    assert db.query_one('select name from user where id=:id', id=id2)['name'] == '赵六', 'execute'
+
+    args = [
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56),
+        ('张三', 55, '1968=-10-08', 0, 1.0, 20.5, 854.56)
+    ]
+    db.batch_execute('insert into user(name, age, birth_date, sex, grade, point, money) values(?,?,?,?,?,?,?)', args)
+    users = db.select('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+    users = db.query('select id, del_flag from user')
+    assert len(users) == 4, 'batch_execute'
+
+    users = db.select('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=?', id2)
+    assert len(users) == 1, 'select'
+
+    users = db.select('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+    users = db.query('select id, del_flag from user where id=:id', id=id2)
+    assert len(users) == 1, 'select'
+
+    db.execute('delete from user where id=? limit 1', id2)
+    assert db.get('select count(1) from user') == 3, 'execute delete'
+```
+##### Transaction
+```
+@db.with_transaction
+def test_transaction():
+    db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+    db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+
+
+def test_transaction2():
+    with db.transaction():
+        db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+        db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
+```
+##### Note: the functions return type
+```
+get: Return only one object, like count
+query_one: Return one row with dict
+select_one: Return one row with tuple
+find_by_id: Return one row with class instance object
+query: Return list of dict
+select: Return list of tuple
+find: Return list of class instance object
+```
```

### Comparing `mysqlx-1.3.0/PKG-INFO` & `mysqlx-1.3.1/mysqlx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.0
+Version: 1.3.1
 Summary: MySqlx is a simple python sql executor for MySQL like iBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,iBatis,MyBatis,python
 Platform: UNKNOWN
@@ -15,23 +15,43 @@
 Install
 '''''''
 
 ::
 
    pip install mysqlx
 
-Sample
-''''''
+Usage Sample
+''''''''''''
 
 ::
 
+   CREATE TABLE `user` (
+     `id` bigint NOT NULL AUTO_INCREMENT,
+     `name` varchar(45) NOT NULL,
+     `age` int NOT NULL,
+     `birth_date` date DEFAULT NULL,
+     `sex` tinyint DEFAULT NULL,
+     `grade` float DEFAULT NULL,
+     `point` double DEFAULT NULL,
+     `money` decimal(8,4) DEFAULT NULL,
+     `create_by` bigint DEFAULT NULL,
+     `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
+     `update_by` bigint DEFAULT NULL,
+     `update_time` datetime DEFAULT NULL,
+     `del_flag` tinyint NOT NULL DEFAULT '0',
+     PRIMARY KEY (`id`)
+   ) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+
+
+   ----------------------------------------------------------------------------------------
+
    from mysqlx import db
 
    db_conf = {
-       'host': HOST,
+       'host': '127.0.0.1',
        'port': 3306, 
        'user': 'root', 
        'password': 'xxx', 
        'database': 'test',
        'pool_size': 5,
        'show_sql': True
    }
@@ -92,16 +112,16 @@
 
 
    def test_transaction2():
        with db.transaction():
            db.insert('user', name='寮犱笁', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
            db.insert('user', name='鏉庡洓', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
 
-Note
-''''
+Note: the functions return type
+'''''''''''''''''''''''''''''''
 
 ::
 
    get: Return only one object, like count
    query_one: Return one row with dict
    select_one: Return one row with tuple
    find_by_id: Return one row with class instance object
```

### Comparing `mysqlx-1.3.0/README.rst` & `mysqlx-1.3.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 Install
 '''''''
 
 ::
 
    pip install mysqlx
 
-Sample
-''''''
+Usage Sample
+''''''''''''
 
 ::
 
+   CREATE TABLE `user` (
+     `id` bigint NOT NULL AUTO_INCREMENT,
+     `name` varchar(45) NOT NULL,
+     `age` int NOT NULL,
+     `birth_date` date DEFAULT NULL,
+     `sex` tinyint DEFAULT NULL,
+     `grade` float DEFAULT NULL,
+     `point` double DEFAULT NULL,
+     `money` decimal(8,4) DEFAULT NULL,
+     `create_by` bigint DEFAULT NULL,
+     `create_time` datetime DEFAULT CURRENT_TIMESTAMP,
+     `update_by` bigint DEFAULT NULL,
+     `update_time` datetime DEFAULT NULL,
+     `del_flag` tinyint NOT NULL DEFAULT '0',
+     PRIMARY KEY (`id`)
+   ) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci
+
+
+   ----------------------------------------------------------------------------------------
+
    from mysqlx import db
 
    db_conf = {
-       'host': HOST,
+       'host': '127.0.0.1',
        'port': 3306, 
        'user': 'root', 
        'password': 'xxx', 
        'database': 'test',
        'pool_size': 5,
        'show_sql': True
    }
@@ -78,16 +98,16 @@
 
 
    def test_transaction2():
        with db.transaction():
            db.insert('user', name='张三', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
            db.insert('user', name='李四', age=55, birth_date='1968=-10-08', sex=0, grade=1.0, point=20.5, money=854.56)
 
-Note
-''''
+Note: the functions return type
+'''''''''''''''''''''''''''''''
 
 ::
 
    get: Return only one object, like count
    query_one: Return one row with dict
    select_one: Return one row with tuple
    find_by_id: Return one row with class instance object
```

### Comparing `mysqlx-1.3.0/setup.py` & `mysqlx-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like iBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.3.0',
+    version='1.3.1',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `mysqlx-1.3.0/test/dbx_test.py` & `mysqlx-1.3.1/test/dbx_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/test/db_test.py` & `mysqlx-1.3.1/test/db_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/test/models.py` & `mysqlx-1.3.1/test/models.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/test/orm_test.py` & `mysqlx-1.3.1/test/orm_test.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.0/test/unit_test.py` & `mysqlx-1.3.1/test/unit_test.py`

 * *Files identical despite different names*

