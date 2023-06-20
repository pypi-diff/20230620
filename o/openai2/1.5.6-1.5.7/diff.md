# Comparing `tmp/openai2-1.5.6.tar.gz` & `tmp/openai2-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.6.tar", last modified: Tue Jun 13 15:51:38 2023, max compression
+gzip compressed data, was "openai2-1.5.7.tar", last modified: Tue Jun 20 13:41:32 2023, max compression
```

## Comparing `openai2-1.5.6.tar` & `openai2-1.5.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.6/LICENSE
--rw-r--r--   0        0        0     2944 2023-06-13 15:29:36.465110 openai2-1.5.6/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.6/openai2/Licenses of dependent packages/openai/LICENSE
--rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.6/openai2/__init__.py
--rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.6/openai2/_core.py
--rw-r--r--   0        0        0      633 2023-06-13 15:51:17.749084 openai2-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 openai2-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.7/LICENSE
+-rw-r--r--   0        0        0     3202 2023-06-20 13:40:21.926193 openai2-1.5.7/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.7/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.7/openai2/__init__.py
+-rw-r--r--   0        0        0     2576 2023-05-28 05:05:03.581780 openai2-1.5.7/openai2/_core.py
+-rw-r--r--   0        0        0      637 2023-06-20 13:40:48.811746 openai2-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3568 1970-01-01 00:00:00.000000 openai2-1.5.7/PKG-INFO
```

### Comparing `openai2-1.5.6/LICENSE` & `openai2-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.6/README.md` & `openai2-1.5.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -30,59 +30,66 @@
 Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Lucy = Chat(api_key=api_key, model="gpt-3.5-turbo")  # 每个实例可使用 相同 或者 不同 的api_key
 ```
 
 #### 对话
 
 ```python
-Tony.request('数字1的后面是几?')  # >>> 2
-Lucy.request('数字101的后面是几?')  # >>> 102
+Tony.request('自然数50的后面是几?')  # >>> 51
+Lucy.request('自然数100的后面是几?')  # >>> 101
 
-Tony.request('再往后是几?')  # >>> 3
-Lucy.request('再往后是几?')  # >>> 103
+Tony.request('再往后是几?')  # >>> 52
+Lucy.request('再往后是几?')  # >>> 102
+
+Tony.request('再往后呢?')  # >>> 53
+Lucy.request('再往后呢?')  # >>> 103
 ```
 
 #### 存档
 
 ```python
-Tony.dump('./talk_record.json')
+Tony.dump('./talk_record.json')  # 可使用相对路径或绝对路径
 ```
 
 #### 载入存档
 
 ```python
 Jenny = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Jenny.load('./talk_record.json')
 
-Jenny.request('再往后呢?')  # >>> 4
+Jenny.request('再往后呢?')  # >>> 54
 ```
 
 #### 对话回滚
 
 ```python
 Anna = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
-Anna.request('数字1的后面是几?')  # >>> 2
+Anna.request('自然数1的后面是几?')  # >>> 2
 Anna.request('再往后是几?')  # >>> 3
 Anna.request('再往后呢?')  # >>> 4
+Anna.request('再往后呢?')  # >>> 5
+Anna.request('再往后呢?')  # >>> 6
+Anna.request('再往后呢?')  # >>> 7
+Anna.request('再往后呢?')  # >>> 8
 
-# 回滚
-Anna.rollback()  # >>> [user]:再往后是几?  [assistant]:3
+# 回滚1轮对话
+Anna.rollback()  # >>> [user]:再往后呢? [assistant]:7
 
-# 再回滚
-Anna.rollback()  # >>> [user]:数字1的后面是几?  [assistant]:2
+# 再回滚3轮对话
+Anna.rollback(n=3)  # >>> [user]:再往后呢? [assistant]:4
 
-Anna.request('再往后是几?')  # >>> 3
+Anna.request('再往后呢?')  # >>> 5
 ```
 
 注：
 
-执行1次 `Anna.rollback(n=x)` 等效于执行x次 `Anna.rollback()`  ，例如：
+1、执行 `Anna.rollback(n=x)` 可回滚 x 轮对话。
 
-执行1次 `Anna.rollback(n=5)` 等效于执行5次 `Anna.rollback()`  。
+2、`Anna.rollback()` 相当于 `Anna.rollback(n=1)` 。
 
 #### 修改api_key
 
 ```python
 Anna.api_key = 'new api_key'
 ```
```

### Comparing `openai2-1.5.6/openai2/Licenses of dependent packages/openai/LICENSE` & `openai2-1.5.7/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.6/openai2/_core.py` & `openai2-1.5.7/openai2/_core.py`

 * *Files identical despite different names*

### Comparing `openai2-1.5.6/PKG-INFO` & `openai2-1.5.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.6
-Summary: 根据 openai 官方接口‘openai’改造的‘openai2’，比官方接口更好用一点
+Version: 1.5.7
+Summary: 根据 openai 官方接口 ‘openai’ 改造的 ‘openai2’ ，比官方接口更好用一点
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/openai2#readme
@@ -42,59 +42,66 @@
 Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Lucy = Chat(api_key=api_key, model="gpt-3.5-turbo")  # 每个实例可使用 相同 或者 不同 的api_key
 ```
 
 #### 对话
 
 ```python
-Tony.request('数字1的后面是几?')  # >>> 2
-Lucy.request('数字101的后面是几?')  # >>> 102
+Tony.request('自然数50的后面是几?')  # >>> 51
+Lucy.request('自然数100的后面是几?')  # >>> 101
 
-Tony.request('再往后是几?')  # >>> 3
-Lucy.request('再往后是几?')  # >>> 103
+Tony.request('再往后是几?')  # >>> 52
+Lucy.request('再往后是几?')  # >>> 102
+
+Tony.request('再往后呢?')  # >>> 53
+Lucy.request('再往后呢?')  # >>> 103
 ```
 
 #### 存档
 
 ```python
-Tony.dump('./talk_record.json')
+Tony.dump('./talk_record.json')  # 可使用相对路径或绝对路径
 ```
 
 #### 载入存档
 
 ```python
 Jenny = Chat(api_key=api_key, model="gpt-3.5-turbo")
 Jenny.load('./talk_record.json')
 
-Jenny.request('再往后呢?')  # >>> 4
+Jenny.request('再往后呢?')  # >>> 54
 ```
 
 #### 对话回滚
 
 ```python
 Anna = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
-Anna.request('数字1的后面是几?')  # >>> 2
+Anna.request('自然数1的后面是几?')  # >>> 2
 Anna.request('再往后是几?')  # >>> 3
 Anna.request('再往后呢?')  # >>> 4
+Anna.request('再往后呢?')  # >>> 5
+Anna.request('再往后呢?')  # >>> 6
+Anna.request('再往后呢?')  # >>> 7
+Anna.request('再往后呢?')  # >>> 8
 
-# 回滚
-Anna.rollback()  # >>> [user]:再往后是几?  [assistant]:3
+# 回滚1轮对话
+Anna.rollback()  # >>> [user]:再往后呢? [assistant]:7
 
-# 再回滚
-Anna.rollback()  # >>> [user]:数字1的后面是几?  [assistant]:2
+# 再回滚3轮对话
+Anna.rollback(n=3)  # >>> [user]:再往后呢? [assistant]:4
 
-Anna.request('再往后是几?')  # >>> 3
+Anna.request('再往后呢?')  # >>> 5
 ```
 
 注：
 
-执行1次 `Anna.rollback(n=x)` 等效于执行x次 `Anna.rollback()`  ，例如：
+1、执行 `Anna.rollback(n=x)` 可回滚 x 轮对话。
 
-执行1次 `Anna.rollback(n=5)` 等效于执行5次 `Anna.rollback()`  。
+2、`Anna.rollback()` 相当于 `Anna.rollback(n=1)` 。
 
 #### 修改api_key
 
 ```python
 Anna.api_key = 'new api_key'
 ```
```

