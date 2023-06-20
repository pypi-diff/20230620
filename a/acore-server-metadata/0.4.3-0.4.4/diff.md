# Comparing `tmp/acore_server_metadata-0.4.3.tar.gz` & `tmp/acore_server_metadata-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.4.3.tar", last modified: Tue Jun 20 01:15:09 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.4.4.tar", last modified: Tue Jun 20 04:28:33 2023, max compression
```

## Comparing `acore_server_metadata-0.4.3.tar` & `acore_server_metadata-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.961312 acore_server_metadata-0.4.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 01:15:09.961161 acore_server_metadata-0.4.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.957242 acore_server_metadata-0.4.3/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.3/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-20 01:10:12.000000 acore_server_metadata-0.4.3/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.3/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958226 acore_server_metadata-0.4.3/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.3/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    26467 2023-06-20 01:13:24.000000 acore_server_metadata-0.4.3/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.3/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958984 acore_server_metadata-0.4.3/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.3/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.960386 acore_server_metadata-0.4.3/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958111 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     3122 2023-06-20 01:11:36.000000 acore_server_metadata-0.4.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-20 01:15:09.961355 acore_server_metadata-0.4.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.960785 acore_server_metadata-0.4.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.3/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.3/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.098382 acore_server_metadata-0.4.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 04:28:33.098248 acore_server_metadata-0.4.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.095475 acore_server_metadata-0.4.4/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.4/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-20 04:26:54.000000 acore_server_metadata-0.4.4/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.4/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096289 acore_server_metadata-0.4.4/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.4/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    27068 2023-06-20 02:44:53.000000 acore_server_metadata-0.4.4/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.4/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096899 acore_server_metadata-0.4.4/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.4/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.4/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.097609 acore_server_metadata-0.4.4/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.096175 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-20 04:28:33.000000 acore_server_metadata-0.4.4/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3374 2023-06-20 04:26:30.000000 acore_server_metadata-0.4.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-20 04:28:33.098427 acore_server_metadata-0.4.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 04:28:33.097942 acore_server_metadata-0.4.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.4/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.4/tests/test_server.py
```

### Comparing `acore_server_metadata-0.4.3/AUTHORS.rst` & `acore_server_metadata-0.4.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/LICENSE.txt` & `acore_server_metadata-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/PKG-INFO` & `acore_server_metadata-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.4.3
+Version: 0.4.4
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.3/README.rst` & `acore_server_metadata-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata/paths.py` & `acore_server_metadata-0.4.4/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata/server.py` & `acore_server_metadata-0.4.4/acore_server_metadata/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,23 +444,38 @@
                 raise ServerAlreadyExistsError(
                     f"RDS DB instance {self.id!r} already exists"
                 )
         if tags is None:
             tags = dict()
         tags[settings.ID_TAG_KEY] = self.id
         tags["tech:machine_creator"] = "acore_server_metadata"
+
+        res = rds_client.describe_db_snapshots(
+            DBSnapshotIdentifier=db_snapshot_identifier,
+        )
+        db_snapshot_list = res.get("DBSnapshots", [])
+        if len(db_snapshot_list):
+            db_snapshot_tags = {
+                dct["Key"]: dct["Value"]
+                for dct in db_snapshot_list[0].get("TagList", [])
+            }
+            master_password_digest = db_snapshot_tags.get("tech:master_password_digest")
+            if master_password_digest:
+                tags["tech:master_password_digest"] = master_password_digest
+
         rds_client.restore_db_instance_from_db_snapshot(
             DBInstanceIdentifier=self.id,
             DBSnapshotIdentifier=db_snapshot_identifier,
             DBInstanceClass=db_instance_class,
             MultiAZ=multi_az,
             DBSubnetGroupName=db_subnet_group_name,
             PubliclyAccessible=False,  # you should never expose your database to the public
             AutoMinorVersionUpgrade=False,  # don't update MySQL minor version, PLEASE!
             VpcSecurityGroupIds=security_group_ids,
+            CopyTagsToSnapshot=True,
             Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
             **kwargs,
         )
 
     create_rds = run_rds  # alias
 
     def start_ec2(self, ec2_client):
```

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.4.4/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.4.4/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.4.4/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.4.4/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.4.3
+Version: 0.4.4
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.3/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.4.4/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/release-history.rst` & `acore_server_metadata-0.4.4/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.4 (2023-06-20)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- ``acore_server_metadata.api.Server.run_rds`` now also copy ``tech:master_password_digest`` tag from snapshot to RDS instance.
+
+
 0.4.3 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - ``acore_server_metadata.api.Server.run_ec2`` and ``acore_server_metadata.api.Server.run_rds`` now receive additional kwargs. The ``allocated_storage`` is no longer mandatory.
```

### Comparing `acore_server_metadata-0.4.3/requirements-doc.txt` & `acore_server_metadata-0.4.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/setup.py` & `acore_server_metadata-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/tests/test_api.py` & `acore_server_metadata-0.4.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.3/tests/test_server.py` & `acore_server_metadata-0.4.4/tests/test_server.py`

 * *Files identical despite different names*

