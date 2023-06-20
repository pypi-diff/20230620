# Comparing `tmp/kfp-kubernetes-0.0.1.tar.gz` & `tmp/kfp-kubernetes-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-kubernetes-0.0.1.tar", last modified: Wed Apr 12 21:27:03 2023, max compression
+gzip compressed data, was "kfp-kubernetes-1.0.0.tar", last modified: Tue Jun 20 21:12:56 2023, max compression
```

## Comparing `kfp-kubernetes-0.0.1.tar` & `kfp-kubernetes-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,19 @@
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.171398 kfp-kubernetes-0.0.1/
--rw-r-----   0 chesu    (630462) primarygroup (89939)      304 2023-04-12 21:27:03.171398 kfp-kubernetes-0.0.1/PKG-INFO
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3160 2023-03-13 19:10:15.000000 kfp-kubernetes-0.0.1/README.md
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2130 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/create_release_branch.sh
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.159397 kfp-kubernetes-0.0.1/docs/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1167 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/Makefile
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.163397 kfp-kubernetes-0.0.1/docs/_static/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      213 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/_static/custom.css
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    15406 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/_static/favicon.ico
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5837 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/_static/kubeflow.png
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     6133 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/conf.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      216 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/index.rst
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1364 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/make.bat
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      114 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/requirements.txt
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.163397 kfp-kubernetes-0.0.1/docs/source/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)       86 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/source/api.rst
--rw-r--r--   0 chesu    (630462) primarygroup (89939)       74 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/docs/source/kubernetes.rst
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2406 2023-03-11 00:17:43.000000 kfp-kubernetes-0.0.1/generate_proto.py
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.159397 kfp-kubernetes-0.0.1/kfp/
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.163397 kfp-kubernetes-0.0.1/kfp/kubernetes/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1051 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/__init__.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      987 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/common.py
--rw-r-----   0 chesu    (630462) primarygroup (89939)    27911 2023-04-12 21:01:00.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/kubernetes_executor_config_pb2.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1688 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/node_selector.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2837 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/secret.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5882 2023-03-22 20:59:06.000000 kfp-kubernetes-0.0.1/kfp/kubernetes/volume.py
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.167398 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/
--rw-r-----   0 chesu    (630462) primarygroup (89939)      304 2023-04-12 21:27:02.000000 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/PKG-INFO
--rw-r-----   0 chesu    (630462) primarygroup (89939)     1385 2023-04-12 21:27:03.000000 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/SOURCES.txt
--rw-r-----   0 chesu    (630462) primarygroup (89939)        1 2023-04-12 21:27:02.000000 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/dependency_links.txt
--rw-r-----   0 chesu    (630462) primarygroup (89939)      169 2023-04-12 21:27:02.000000 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/requires.txt
--rw-r-----   0 chesu    (630462) primarygroup (89939)        4 2023-04-12 21:27:02.000000 kfp-kubernetes-0.0.1/kfp_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2072 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/release.sh
--rw-r-----   0 chesu    (630462) primarygroup (89939)       38 2023-04-12 21:27:03.171398 kfp-kubernetes-0.0.1/setup.cfg
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     2081 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/setup.py
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.159397 kfp-kubernetes-0.0.1/test/
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.167398 kfp-kubernetes-0.0.1/test/snapshot/
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.167398 kfp-kubernetes-0.0.1/test/snapshot/data/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1748 2023-04-12 20:07:43.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_dynamic_pvc.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5708 2023-04-12 20:07:43.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_dynamic_pvc.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1244 2023-03-13 19:10:15.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_existing_pvc.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     3647 2023-03-22 20:59:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_existing_pvc.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1335 2023-03-13 19:10:15.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_existing_pvc_from_task_output.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     5124 2023-03-22 20:59:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/create_mount_delete_existing_pvc_from_task_output.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1008 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/test/snapshot/data/node_selector.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1576 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/test/snapshot/data/node_selector.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      996 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/secret_as_env.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1614 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/secret_as_env.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      963 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/secret_as_vol.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     1563 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/snapshot/data/secret_as_vol.yaml
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     7718 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/test/snapshot/read_write_test.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)      960 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/test/snapshot/test_data_config.yaml
-drwxr-x---   0 chesu    (630462) primarygroup (89939)        0 2023-04-12 21:27:03.171398 kfp-kubernetes-0.0.1/test/unit/
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     4318 2023-03-15 21:18:15.000000 kfp-kubernetes-0.0.1/test/unit/test_node_selector.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)    12095 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/unit/test_secret.py
--rw-r--r--   0 chesu    (630462) primarygroup (89939)     6215 2023-03-11 00:18:06.000000 kfp-kubernetes-0.0.1/test/unit/test_volume.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-20 21:12:56.441758 kfp-kubernetes-1.0.0/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4587 2023-06-20 21:12:56.441611 kfp-kubernetes-1.0.0/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3143 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-20 21:12:56.439427 kfp-kubernetes-1.0.0/kfp/
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-20 21:12:56.440670 kfp-kubernetes-1.0.0/kfp/kubernetes/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1051 2023-06-20 21:01:35.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      987 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/common.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7874 2023-06-20 21:05:30.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/kubernetes_executor_config_pb2.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1688 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/node_selector.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2837 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/secret.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5882 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/kfp/kubernetes/volume.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-20 21:12:56.441386 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4587 2023-06-20 21:12:56.000000 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      390 2023-06-20 21:12:56.000000 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-06-20 21:12:56.000000 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      169 2023-06-20 21:12:56.000000 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-06-20 21:12:56.000000 kfp-kubernetes-1.0.0/kfp_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-06-20 21:12:56.441809 kfp-kubernetes-1.0.0/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2622 2023-06-15 22:44:46.000000 kfp-kubernetes-1.0.0/setup.py
```

### Comparing `kfp-kubernetes-0.0.1/README.md` & `kfp-kubernetes-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Kubernetes Platform-specific Features
 
 The `kfp-kubernetes` Python library enables authoring [Kubeflow pipelines](https://www.kubeflow.org/docs/components/pipelines/v2/) with Kubernetes-specific features. These features are supported by the [default KFP open source BE](https://github.com/kubeflow/pipelines/tree/master/backend). Specifically, the `kfp-kubernetes` library supports authoring pipelines that use:
 
 * [Secrets](https://kubernetes.io/docs/concepts/configuration/secret/)
 * [PersistentVolumeClaims](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaims)
 
-<!-- TODO: add reference to kubeflow user docs on support for platform-specific features once they exist -->
+See the [`kfp-kubernetes` reference documentation](https://kfp-kubernetes.readthedocs.io/).
 
 ## Installation
 The `kfp-kubernetes` package can be installed as a `kfp` SDK extra dependency with `kfp==2.x.x`:
 <!-- TODO: remove --pre when kfp v2 goes to GA -->
 ```sh
 pip install kfp[kubernetes] --pre
 ```
@@ -73,15 +73,15 @@
         print(f.read())
 
 @dsl.pipeline
 def my_pipeline():
     pvc1 = kubernetes.CreatePVC(
         # can also use pvc_name instead of pvc_name_suffix to use a pre-existing PVC
         pvc_name_suffix='-my-pvc',
-        access_modes=['ReadWriteMany'],
+        access_modes=['ReadWriteOnce'],
         size='5Gi',
         storage_class_name='standard',
     )
 
     task1 = make_data()
     # normally task sequencing is handled by data exchange via component inputs/outputs
     # but since data is exchanged via volume, we need to call .after explicitly to sequence tasks
```

### Comparing `kfp-kubernetes-0.0.1/kfp/kubernetes/__init__.py` & `kfp-kubernetes-1.0.0/kfp/kubernetes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.0.1'
+__version__ = '1.0.0'
 
 __all__ = [
     'CreatePVC',
     'DeletePVC',
     'mount_pvc',
     'use_secret_as_env',
     'use_secret_as_volume',
```

### Comparing `kfp-kubernetes-0.0.1/kfp/kubernetes/common.py` & `kfp-kubernetes-1.0.0/kfp/kubernetes/common.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-0.0.1/kfp/kubernetes/node_selector.py` & `kfp-kubernetes-1.0.0/kfp/kubernetes/node_selector.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-0.0.1/kfp/kubernetes/secret.py` & `kfp-kubernetes-1.0.0/kfp/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-0.0.1/kfp/kubernetes/volume.py` & `kfp-kubernetes-1.0.0/kfp/kubernetes/volume.py`

 * *Files identical despite different names*

### Comparing `kfp-kubernetes-0.0.1/setup.py` & `kfp-kubernetes-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,21 +49,37 @@
     )
     if version_match:
         return version_match[1]
     else:
         raise ValueError('Could not find version.')
 
 
+def read_readme() -> str:
+    readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
+    with open(readme_path) as f:
+        return f.read()
+
+
 setuptools.setup(
     name=NAME,
     version=find_version('kfp', 'kubernetes', '__init__.py'),
     description='Kubernetes platform configuration library and generated protos.',
+    long_description=read_readme(),
+    long_description_content_type='text/markdown',
     author='google',
     author_email='kubeflow-pipelines@google.com',
     url='https://github.com/kubeflow/pipelines',
+    project_urls={
+        'Documentation':
+            'https://kfp-kubernetes.readthedocs.io/',
+        'Bug Tracker':
+            'https://github.com/kubeflow/pipelines/issues',
+        'Source':
+            'https://github.com/kubeflow/pipelines/tree/master/kubernetes_platform/python',
+    },
     packages=setuptools.find_namespace_packages(include=['kfp.*']),
     python_requires='>=3.7.0',
     install_requires=REQUIREMENTS,
     include_package_data=True,
     extras_require={
         'dev': DEV_REQUIREMENTS,
     },
```

