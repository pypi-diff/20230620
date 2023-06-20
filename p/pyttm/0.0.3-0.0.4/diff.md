# Comparing `tmp/pyttm-0.0.3.tar.gz` & `tmp/pyttm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttm-0.0.3.tar", last modified: Tue Jun 20 11:50:33 2023, max compression
+gzip compressed data, was "pyttm-0.0.4.tar", last modified: Tue Jun 20 12:48:16 2023, max compression
```

## Comparing `pyttm-0.0.3.tar` & `pyttm-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.784096 pyttm-0.0.3/
--rw-rw-rw-   0        0        0     1063 2023-06-20 07:08:08.000000 pyttm-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2686 2023-06-20 11:50:33.784096 pyttm-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-06-20 11:06:33.000000 pyttm-0.0.3/README.md
--rw-rw-rw-   0        0        0       68 2023-06-20 11:50:33.789095 pyttm-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-20 11:49:22.000000 pyttm-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.757095 pyttm-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.764095 pyttm-0.0.3/src/pyttm/
--rw-rw-rw-   0        0        0       40 2023-06-20 11:49:22.000000 pyttm-0.0.3/src/pyttm/__init__.py
--rw-rw-rw-   0        0        0      956 2023-06-20 11:33:04.000000 pyttm-0.0.3/src/pyttm/app.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.783095 pyttm-0.0.3/src/pyttm/libs/
--rw-rw-rw-   0        0        0     1092 2023-06-20 08:30:45.000000 pyttm-0.0.3/src/pyttm/libs/crypto.py
--rw-rw-rw-   0        0        0     1689 2023-06-20 11:33:05.000000 pyttm-0.0.3/src/pyttm/libs/db.py
--rw-rw-rw-   0        0        0     5095 2023-06-20 11:49:22.000000 pyttm-0.0.3/src/pyttm/libs/helper.py
--rw-rw-rw-   0        0        0     2960 2023-06-20 06:15:35.000000 pyttm-0.0.3/src/pyttm/libs/totp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.778095 pyttm-0.0.3/src/pyttm.egg-info/
--rw-rw-rw-   0        0        0     2686 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.431038 pyttm-0.0.4/
+-rw-rw-rw-   0        0        0     1063 2023-06-20 07:08:08.000000 pyttm-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2678 2023-06-20 12:48:16.431038 pyttm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1901 2023-06-20 12:13:01.000000 pyttm-0.0.4/README.md
+-rw-rw-rw-   0        0        0       68 2023-06-20 12:48:16.435027 pyttm-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-20 12:47:48.000000 pyttm-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.323247 pyttm-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.329247 pyttm-0.0.4/src/pyttm/
+-rw-rw-rw-   0        0        0       40 2023-06-20 12:47:48.000000 pyttm-0.0.4/src/pyttm/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-06-20 12:13:01.000000 pyttm-0.0.4/src/pyttm/app.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.357247 pyttm-0.0.4/src/pyttm/libs/
+-rw-rw-rw-   0        0        0     1168 2023-06-20 12:26:16.000000 pyttm-0.0.4/src/pyttm/libs/crypto.py
+-rw-rw-rw-   0        0        0     1603 2023-06-20 12:45:38.000000 pyttm-0.0.4/src/pyttm/libs/db.py
+-rw-rw-rw-   0        0        0     5095 2023-06-20 12:47:49.000000 pyttm-0.0.4/src/pyttm/libs/helper.py
+-rw-rw-rw-   0        0        0     2960 2023-06-20 06:15:35.000000 pyttm-0.0.4/src/pyttm/libs/totp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.348247 pyttm-0.0.4/src/pyttm.egg-info/
+-rw-rw-rw-   0        0        0     2678 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 12:48:16.000000 pyttm-0.0.4/src/pyttm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:16.358246 pyttm-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1240 2023-06-20 12:46:36.000000 pyttm-0.0.4/tests/test.py
```

### Comparing `pyttm-0.0.3/LICENSE` & `pyttm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttm-0.0.3/PKG-INFO` & `pyttm-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Terminal based TOTP manager
 Home-page: https://github.com/The-Robin-Hood/ttm
 Author: The Robin Hood
 License: MIT
 Keywords: totp,otp,encryption,decryption,AES256,crypto,security,privacy
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -40,17 +40,17 @@
    pip install pyttm
    ```
 
 ## Usage
 
 To use TOTP Manager, follow these steps:
 
-    1. Open a terminal or command prompt and navigate to the project directory.
+1. Open a terminal or command prompt and navigate to the project directory.
 
-    2. Run the following command:
+2. Run the following command:
 
    ```
    ttm [command]
    ```
 
    Replace `[command]` with one of the following options:
```

### Comparing `pyttm-0.0.3/README.md` & `pyttm-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
    pip install pyttm
    ```
 
 ## Usage
 
 To use TOTP Manager, follow these steps:
 
-    1. Open a terminal or command prompt and navigate to the project directory.
+1. Open a terminal or command prompt and navigate to the project directory.
 
-    2. Run the following command:
+2. Run the following command:
 
    ```
    ttm [command]
    ```
 
    Replace `[command]` with one of the following options:
```

### Comparing `pyttm-0.0.3/setup.py` & `pyttm-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def docs_read(fname):
     f = open(os.path.join(os.path.dirname(__file__), fname)).read()
     return f.replace('â™¥', '♥')
 
 setup(
     name='pyttm',
-    version='0.0.3',
+    version='0.0.4',
     description='A simple Terminal based TOTP manager',
     long_description=(docs_read('README.md')),
     long_description_content_type='text/markdown',
     url='https://github.com/The-Robin-Hood/ttm',
     author='The Robin Hood',
     license='MIT',
     platforms=['any'],
```

### Comparing `pyttm-0.0.3/src/pyttm/app.py` & `pyttm-0.0.4/src/pyttm/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyttm.libs.crypto import *
 
 def main():
     try:
         clear()  
         command_line_args = sys.argv[1:]
         if len(command_line_args) == 0 or command_line_args[0] not in ["add","list","delete"]:
-            print("Usage: python3 app.py add|list|delete\n")
+            print("Usage: ttm add|list|delete\n")
             exit()
 
         password = get_password()        
         command = command_line_args[0]
 
         if command == "add":
             add_creds(password)
@@ -30,8 +30,8 @@
         exit()
     except Exception as e:
         print("Error! Facing Issue, Please Report!")
         print(e)
         exit()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `pyttm-0.0.3/src/pyttm/libs/crypto.py` & `pyttm-0.0.4/src/pyttm/libs/crypto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from Crypto.Cipher import AES
 from Crypto.Random import get_random_bytes
 import hashlib
 
 def encrypt_text(text:str, secret_key:str):
+    secret_key= secret_key.zfill(16)
     nonce = get_random_bytes(8) 
     secret_key_to_bytes = secret_key.encode('utf-8')
     cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
     encrypted_text = cipher.encrypt(text.encode('utf-8'))
     return nonce.hex() + encrypted_text.hex()
 
 def decrypt_text(encrypted_text, secret_key):
     nonce = bytes.fromhex(encrypted_text[:16])
+    secret_key= secret_key.zfill(16)
     encrypted_bytes = bytes.fromhex(encrypted_text[16:])
     secret_key_to_bytes = secret_key.encode('utf-8')
     cipher = AES.new(secret_key_to_bytes, AES.MODE_CTR, nonce=nonce)
     decrypted_text = cipher.decrypt(encrypted_bytes)
     return decrypted_text.decode('utf-8')
 
 def hash_password(password):
```

### Comparing `pyttm-0.0.3/src/pyttm/libs/db.py` & `pyttm-0.0.4/src/pyttm/libs/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,24 +32,22 @@
         return self.data["password"]
     
     def set_password(self, password):
         self.data["password"] = password
         self.write_data()
     
     def add_creds(self, creds,password):
-        secret_key = password.zfill(16)
-        creds['seed'] = encrypt_text(creds['seed'], secret_key)
+        creds['seed'] = encrypt_text(creds['seed'], password)
         self.data["credentials"].append(creds)
         self.write_data()
     
     def get_creds(self,password):
-        secret_key = password.zfill(16)
         creds = copy.deepcopy(self.data["credentials"])
         for cred in creds:
-            cred['seed'] = decrypt_text(cred['seed'], secret_key)
+            cred['seed'] = decrypt_text(cred['seed'], password)
         return creds
     
     def delete_creds(self, cred):
         del self.data["credentials"][cred]
         self.write_data()
 
 json_db = JsonDB("../db.json")
```

### Comparing `pyttm-0.0.3/src/pyttm/libs/helper.py` & `pyttm-0.0.4/src/pyttm/libs/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 |  _____   _____   __  __  |
 | |_   _| |_   _| |  \/  | |
 |   | |     | |   | |\/| | |
 |   | |     | |   | |  | | |
 |   |_|     |_|   |_|  |_| |
 |                          |  
 |   Terminal TOTP Manager  |
-|      version : 0.0.3     |
+|      version : 0.0.4     |
  --------------------------
 """)    
 
 def extract_info_from_otpauth_uri(uri):
     parsed_uri = urllib.parse.urlparse(uri)
 
     if parsed_uri.scheme != "otpauth" or parsed_uri.netloc != "totp":
```

### Comparing `pyttm-0.0.3/src/pyttm/libs/totp.py` & `pyttm-0.0.4/src/pyttm/libs/totp.py`

 * *Files identical despite different names*

### Comparing `pyttm-0.0.3/src/pyttm.egg-info/PKG-INFO` & `pyttm-0.0.4/src/pyttm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Terminal based TOTP manager
 Home-page: https://github.com/The-Robin-Hood/ttm
 Author: The Robin Hood
 License: MIT
 Keywords: totp,otp,encryption,decryption,AES256,crypto,security,privacy
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -40,17 +40,17 @@
    pip install pyttm
    ```
 
 ## Usage
 
 To use TOTP Manager, follow these steps:
 
-    1. Open a terminal or command prompt and navigate to the project directory.
+1. Open a terminal or command prompt and navigate to the project directory.
 
-    2. Run the following command:
+2. Run the following command:
 
    ```
    ttm [command]
    ```
 
    Replace `[command]` with one of the following options:
```

