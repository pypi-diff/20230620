# Comparing `tmp/acore_server_metadata-0.4.2.tar.gz` & `tmp/acore_server_metadata-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.4.2.tar", last modified: Mon Jun 19 20:48:53 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.4.3.tar", last modified: Tue Jun 20 01:15:09 2023, max compression
```

## Comparing `acore_server_metadata-0.4.2.tar` & `acore_server_metadata-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.517553 acore_server_metadata-0.4.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 20:48:53.517422 acore_server_metadata-0.4.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.514417 acore_server_metadata-0.4.2/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.2/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 20:47:25.000000 acore_server_metadata-0.4.2/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.2/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.515300 acore_server_metadata-0.4.2/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.2/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    26210 2023-06-19 20:43:44.000000 acore_server_metadata-0.4.2/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.2/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.516022 acore_server_metadata-0.4.2/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.2/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.516769 acore_server_metadata-0.4.2/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.515158 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2852 2023-06-19 20:47:19.000000 acore_server_metadata-0.4.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 20:48:53.517593 acore_server_metadata-0.4.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.517103 acore_server_metadata-0.4.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.2/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.961312 acore_server_metadata-0.4.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 01:15:09.961161 acore_server_metadata-0.4.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.957242 acore_server_metadata-0.4.3/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.3/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-20 01:10:12.000000 acore_server_metadata-0.4.3/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.3/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958226 acore_server_metadata-0.4.3/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.3/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    26467 2023-06-20 01:13:24.000000 acore_server_metadata-0.4.3/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.3/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958984 acore_server_metadata-0.4.3/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.3/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.3/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.960386 acore_server_metadata-0.4.3/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.958111 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-20 01:15:09.000000 acore_server_metadata-0.4.3/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3122 2023-06-20 01:11:36.000000 acore_server_metadata-0.4.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-20 01:15:09.961355 acore_server_metadata-0.4.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-20 01:15:09.960785 acore_server_metadata-0.4.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.3/tests/test_server.py
```

### Comparing `acore_server_metadata-0.4.2/AUTHORS.rst` & `acore_server_metadata-0.4.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/LICENSE.txt` & `acore_server_metadata-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/PKG-INFO` & `acore_server_metadata-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.4.2
+Version: 0.4.3
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.2/README.rst` & `acore_server_metadata-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata/paths.py` & `acore_server_metadata-0.4.3/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata/server.py` & `acore_server_metadata-0.4.3/acore_server_metadata/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,18 +343,19 @@
         instance_type: str,
         key_name: str,
         subnet_id: str,
         security_group_ids: T.List[str],
         iam_instance_profile_arn: str,
         tags: T.Optional[T.Dict[str, str]] = None,
         check_exists: bool = True,
+        **kwargs,
     ):
         """
         Launch a new EC2 instance as the Game server from the AMI.
-        The configurations are already optimized for the Game server.
+        The mandatory arguments match how we launch a new WOW server.
 
         在服务器运维过程中, 我们都是从自己构建的游戏服务器 AMI 启动 EC2 实例. 它的 Tag 必须
         要符合一定的规则 (详情请参考 :class:`Server`). 本方法会自动为新的 EC2 实例打上这些
         必要的 Tag.
 
         Reference:
 
@@ -393,33 +394,34 @@
             IamInstanceProfile=dict(Arn=iam_instance_profile_arn),
             TagSpecifications=[
                 dict(
                     ResourceType="instance",
                     Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
                 ),
             ],
+            **kwargs,
         )
 
     create_ec2 = run_ec2  # alias
 
     def run_rds(
         self,
         rds_client,
         db_snapshot_identifier: str,
         db_instance_class: str,
         db_subnet_group_name: str,
         security_group_ids: T.List[str],
         multi_az: bool = False,
-        allocated_storage: int = 20,
         tags: T.Optional[T.Dict[str, str]] = None,
         check_exists: bool = True,
+        **kwargs,
     ):
         """
         Launch a new RDS DB instance from the backup snapshot.
-        The configurations are already optimized for the Game server.
+        The mandatory arguments match how we launch a new WOW database.
 
         在数据库运维过程中, 我们都是从自己备份的 Snapshot 启动 DB 实例. 它的 Tag 必须
         要符合一定的规则 (详情请参考 :class:`Server`). 本方法会自动为新的 DB 实例打上这些
         必要的 Tag.
 
         Reference:
 
@@ -448,19 +450,19 @@
         tags["tech:machine_creator"] = "acore_server_metadata"
         rds_client.restore_db_instance_from_db_snapshot(
             DBInstanceIdentifier=self.id,
             DBSnapshotIdentifier=db_snapshot_identifier,
             DBInstanceClass=db_instance_class,
             MultiAZ=multi_az,
             DBSubnetGroupName=db_subnet_group_name,
-            AllocatedStorage=allocated_storage,
             PubliclyAccessible=False,  # you should never expose your database to the public
             AutoMinorVersionUpgrade=False,  # don't update MySQL minor version, PLEASE!
             VpcSecurityGroupIds=security_group_ids,
             Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
+            **kwargs,
         )
 
     create_rds = run_rds  # alias
 
     def start_ec2(self, ec2_client):
         """
         Start the EC2 instance of this server.
@@ -528,14 +530,19 @@
         or this one, and each association will incur a small fee. So I would like
         to check before doing this.
 
         当对生产服务器进行运维时, 我们需要维护给每个服务器一个固定 IP. 我们可以通过定义一个
         映射表, 然后用这个方法确保每个服务器的 IP 是正确的 (该方法是幂等的, 如果已经设置好了
         则什么也不会做).
 
+        Reference:
+
+        - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/client/describe_addresses.html
+        - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/client/associate_address.html
+
         :param ec2_client: boto3 ec2 client
         :param allocation_id: the EIP allocation id, not the pulibc ip,
             example "eipalloc-1a2b3c4d"
         :param check_exists: check if the EC2 instance exists before associating.
 
         :return: if we actually send the ``rds_client.associate_address`` API,
             it returns the response of that API. Otherwise, it returns None.
```

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.4.3/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.4.3/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.4.3/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.4.3/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.4.2
+Version: 0.4.3
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.2/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.4.3/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/release-history.rst` & `acore_server_metadata-0.4.3/release-history.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
-0.4.2 (2023-06-19)
+0.4.3 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-**Features and Improvements**
+**Minor Improvements**
+
+- ``acore_server_metadata.api.Server.run_ec2`` and ``acore_server_metadata.api.Server.run_rds`` now receive additional kwargs. The ``allocated_storage`` is no longer mandatory.
 
+
+0.4.2 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - ``acore_server_metadata.api.Server.associate_eip_address`` now returns API response or None
 - ``acore_server_metadata.api.Server.update_db_master_password`` now returns API response or None
 - ``acore_server_metadata.api.Server.cleanup_db_snapshot`` now returns API response or None
 - add ``acore_server_metadata.api.Server.create_ec2``, it is a alias of ``run_ec2``
 - add ``acore_server_metadata.api.Server.create_rds``, it is a alias of ``run_rds``
```

### Comparing `acore_server_metadata-0.4.2/requirements-doc.txt` & `acore_server_metadata-0.4.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/setup.py` & `acore_server_metadata-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/tests/test_api.py` & `acore_server_metadata-0.4.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.2/tests/test_server.py` & `acore_server_metadata-0.4.3/tests/test_server.py`

 * *Files identical despite different names*

