# Comparing `tmp/mse_cli_core-0.1a4.tar.gz` & `tmp/mse_cli_core-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a4.tar", last modified: Tue May 30 14:34:50 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a5.tar", last modified: Tue Jun 20 16:40:42 2023, max compression
```

## Comparing `mse_cli_core-0.1a4.tar` & `mse_cli_core-0.1a5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.831401 mse_cli_core-0.1a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.255714 mse_cli_core-0.1a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a4/PKG-INFO` & `mse_cli_core-0.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a4
+Version: 0.1a5
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a4/setup.cfg` & `mse_cli_core-0.1a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/setup.py` & `mse_cli_core-0.1a5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     long_description_content_type="text/markdown",
     python_requires=">=3.8.0",
     description="Utils for MicroService Encryption Python CLIs",
     packages=find_packages("src"),
     package_dir={"": "src"},
     zip_safe=True,
     install_requires=[
-        "cryptography>=40.0.2,<41.0",
+        "cryptography>=41.0.1,<42.0.0",
         "docker>=6.0.1,<7.0.0",
-        "intel-sgx-ra==2.0a7",
+        "intel-sgx-ra==2.0a11",
         "pydantic>=1.10.2,<2.0.0",
-        "requests>=2.28.1,<2.29.0",
+        "requests>=2.31.0,<3.0.0",
         "toml>=0.10.2,<0.11.0",
     ],
     setup_requires=["wheel"],
     tests_require=["pytest>=7.2.0,<7.3.0"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a5/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a5/src/mse_cli_core/bootstrap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """mse_cli_core.bootstrap module."""
 
-from typing import Any, Dict, Optional, Union
+from typing import Any, Callable, Dict, Iterable, Optional, Union
 from uuid import UUID
 
 import requests
 from pydantic import BaseModel
 
 from mse_cli_core.base64 import base64url_encode
 from mse_cli_core.clock_tick import ClockTick
@@ -53,17 +53,26 @@
     if not r.ok:
         raise Exception(
             "Fail to send data to the configuration server "
             f"(Response {r.status_code} {r.text})"
         )
 
 
-def wait_for_conf_server(clock: ClockTick, url: str, verify: Union[bool, str] = True):
+def wait_for_conf_server(
+    clock: ClockTick,
+    url: str,
+    verify: Union[bool, str] = True,
+    extra_check: Optional[Callable] = None,
+    extra_check_args: Iterable = (),
+):
     """Hold on until the configuration server is up and listing."""
     while clock.tick():
+        if extra_check:
+            extra_check(*extra_check_args)
+
         if is_waiting_for_secrets(url, verify):
             break
 
 
 def is_waiting_for_secrets(url: str, verify: Union[bool, str] = True) -> bool:
     """Check whether the configuration server is up."""
     try:
@@ -80,17 +89,22 @@
 
 
 def wait_for_app_server(
     clock: ClockTick,
     url: str,
     healthcheck_endpoint: str,
     verify: Union[bool, str] = True,
+    extra_check: Optional[Callable] = None,
+    extra_check_args: Iterable = (),
 ):
     """Hold on until the configuration server is stopped and the app starts."""
     while clock.tick():
+        if extra_check:
+            extra_check(*extra_check_args)
+
         if is_ready(url, healthcheck_endpoint, verify):
             break
 
 
 def is_ready(
     url: str, healthcheck_endpoint: str, verify: Union[bool, str] = True
 ) -> bool:
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a5/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a5/src/mse_cli_core/enclave.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,21 @@
 
 
 def verify_enclave(
     signer_pk: Union[RSAPublicKey, Path, bytes],
     ratls_certificate: Union[str, bytes, Path, Certificate],
     fingerprint: Optional[str],
     collaterals: Optional[
-        Tuple[bytes, Certificate, CertificateRevocationList, CertificateRevocationList]
+        Tuple[
+            bytes,
+            bytes,
+            Certificate,
+            CertificateRevocationList,
+            CertificateRevocationList,
+        ]
     ] = None,
     pccs_url: Optional[str] = None,
 ):
     """Verify an enclave trustworthiness."""
     # Compute MRSIGNER value from public key
     mrsigner = mr_signer_from_pk(signer_pk)
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a5/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a5/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a5/src/mse_cli_core/no_sgx_docker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """mse_cli_core.no_sgx_docker module."""
 
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import ClassVar, Dict, List, Optional
 from uuid import UUID
 
-import toml
 from pydantic import BaseModel
 
 from mse_cli_core.sgx_docker import SgxDockerConfig
 
 
 class NoSgxDockerConfig(BaseModel):
     """Definition of an mse docker running on a non-sgx hardware."""
@@ -63,38 +62,16 @@
                 "bind": NoSgxDockerConfig.app_cert_mountpoint,
                 "mode": "rw",
             }
 
         return v
 
     @staticmethod
-    def load(path: Path):
-        """Load the args from a toml file."""
-        with open(path, encoding="utf8") as f:
-            dataMap = toml.load(f)
-
-            return NoSgxDockerConfig(**dataMap)
-
-    @staticmethod
     def from_sgx(docker_config: SgxDockerConfig):
         """Load from a SgxDockerConfig object."""
         return NoSgxDockerConfig(
             host=docker_config.host,
             expiration_date=docker_config.expiration_date,
             size=docker_config.size,
             app_id=docker_config.app_id,
             application=docker_config.application,
         )
-
-    def save(self, path: Path) -> None:
-        """Save the args into a toml file."""
-        with open(path, "w", encoding="utf8") as f:
-            dataMap: Dict[str, Any] = {
-                "host": self.host,
-                "expiration_date": self.expiration_date,
-                "app_cert": str(self.app_cert) if self.app_cert else None,
-                "size": self.size,
-                "app_id": str(self.app_id),
-                "application": self.application,
-            }
-
-            toml.dump(dataMap, f)
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a5/src/mse_cli_core/sgx_docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             "/dev/sgx_provision:/dev/sgx_provision:rw",
             "/dev/sgx/enclave:/dev/sgx/enclave:rw",
             "/dev/sgx/provision:/dev/sgx/provision:rw",
         ]
 
     @staticmethod
     def load(docker_attrs: Dict[str, Any], docker_labels: Any):
-        """Load the the docker configuration from the container."""
+        """Load the docker configuration from the container."""
         dataMap: Dict[str, Any] = {}
 
         cmd = docker_attrs["Config"]["Cmd"]
         port = docker_attrs["HostConfig"]["PortBindings"]
         signer_key = next(
             filter(
                 lambda mount: mount["Destination"]
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a5/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a5/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a4
+Version: 0.1a5
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a4/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a5/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/mse_cli_core/bootstrap.py
 src/mse_cli_core/clock_tick.py
 src/mse_cli_core/enclave.py
 src/mse_cli_core/fs.py
 src/mse_cli_core/ignore_file.py
 src/mse_cli_core/no_sgx_docker.py
 src/mse_cli_core/sgx_docker.py
+src/mse_cli_core/spinner.py
 src/mse_cli_core/test_docker.py
 src/mse_cli_core.egg-info/PKG-INFO
 src/mse_cli_core.egg-info/SOURCES.txt
 src/mse_cli_core.egg-info/dependency_links.txt
 src/mse_cli_core.egg-info/requires.txt
 src/mse_cli_core.egg-info/top_level.txt
 src/mse_cli_core.egg-info/zip-safe
```

### Comparing `mse_cli_core-0.1a4/tests/test_base64.py` & `mse_cli_core-0.1a5/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/tests/test_boostrap.py` & `mse_cli_core-0.1a5/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/tests/test_ignore_file.py` & `mse_cli_core-0.1a5/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/tests/test_sgx_docker.py` & `mse_cli_core-0.1a5/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a4/tests/test_test_docker.py` & `mse_cli_core-0.1a5/tests/test_test_docker.py`

 * *Files identical despite different names*

