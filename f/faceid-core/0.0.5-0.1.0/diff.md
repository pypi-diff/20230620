# Comparing `tmp/faceid_core-0.0.5.tar.gz` & `tmp/faceid_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid_core-0.0.5.tar", last modified: Tue Jun 20 13:00:11 2023, max compression
+gzip compressed data, was "faceid_core-0.1.0.tar", last modified: Tue Jun 20 13:21:59 2023, max compression
```

## Comparing `faceid_core-0.0.5.tar` & `faceid_core-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.642921 faceid_core-0.0.5/
--rw-rw-rw-   0        0        0      358 2023-06-20 13:00:11.642921 faceid_core-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.622716 faceid_core-0.0.5/faceid_core/
--rw-rw-rw-   0        0        0      137 2023-06-20 12:16:38.000000 faceid_core-0.0.5/faceid_core/__init__.py
--rw-rw-rw-   0        0        0      589 2023-06-20 12:11:39.000000 faceid_core-0.0.5/faceid_core/deploy_configuration.py
--rw-rw-rw-   0        0        0     3716 2023-06-20 12:54:07.000000 faceid_core-0.0.5/faceid_core/face_recognition.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.642921 faceid_core-0.0.5/faceid_core.egg-info/
--rw-rw-rw-   0        0        0      358 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 13:00:11.642921 faceid_core-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-06-20 13:00:00.000000 faceid_core-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:21:59.847089 faceid_core-0.1.0/
+-rw-rw-rw-   0        0        0      358 2023-06-20 13:21:59.847089 faceid_core-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 13:21:59.831423 faceid_core-0.1.0/faceid_core/
+-rw-rw-rw-   0        0        0      137 2023-06-20 12:16:38.000000 faceid_core-0.1.0/faceid_core/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-06-20 12:11:39.000000 faceid_core-0.1.0/faceid_core/deploy_configuration.py
+-rw-rw-rw-   0        0        0     3379 2023-06-20 13:20:16.000000 faceid_core-0.1.0/faceid_core/face_recognition.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:21:59.847089 faceid_core-0.1.0/faceid_core.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-06-20 13:21:59.000000 faceid_core-0.1.0/faceid_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-20 13:21:59.000000 faceid_core-0.1.0/faceid_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:21:59.000000 faceid_core-0.1.0/faceid_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-20 13:21:59.000000 faceid_core-0.1.0/faceid_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 13:21:59.000000 faceid_core-0.1.0/faceid_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:21:59.847089 faceid_core-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-06-20 13:21:17.000000 faceid_core-0.1.0/setup.py
```

### Comparing `faceid_core-0.0.5/faceid_core/deploy_configuration.py` & `faceid_core-0.1.0/faceid_core/deploy_configuration.py`

 * *Files identical despite different names*

### Comparing `faceid_core-0.0.5/faceid_core/face_recognition.py` & `faceid_core-0.1.0/faceid_core/face_recognition.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,25 @@
         self.config = DeployConfig(conf_file)
         self.model = insightface.app.FaceAnalysis()
         self.model.prepare(ctx_id=self.config.gpu_id, det_size=(640, 640))
         self.faces_embedding = list()
         #
         self.load_faces(self.config.face_db)
 
-    #
+
     def load_faces(self, face_db_path):
         if not Path(face_db_path).exists():
-            Path.mkdir(face_db_path)
+            Path(face_db_path).mkdir()
 
-        face_db_path = Path(face_db_path)  # преобразуем строку в объект Path
-        for path in face_db_path.rglob("*"):  # используем .rglob() для рекурсивного обхода всех файлов
-            if path.is_file():  # проверяем, что path является файлом
+        face_db_path = Path(face_db_path)
+        for path in face_db_path.rglob("*"):
+            if path.is_file():
                 input_image = cv2.imdecode(np.fromfile(path, dtype=np.uint8),
                                            1)
                 user_id = path.stem
-                print("Loader face: % s" % user_id)
                 face = self.model.get(input_image)[0]
                 embedding = np.array(face.embedding).reshape((1, -1))
                 embedding = preprocessing.normalize(embedding)
                 self.faces_embedding.append({
                     "user_id": user_id,
                     "feature": embedding
                 })
@@ -54,15 +53,16 @@
         users_id = [d["user_id"] for d in self.faces_embedding]
 
         if len(users_id) == 0:
             user_id = 0
         else:
             user_id = int(users_id[-1]) + 1
 
-        cv2.imencode('.jpg', image)[1].tofile(Path.joinpath(self.config.face_db, '%s.jpg' % user_id))
+        cv2.imencode('.jpg', image)[1].tofile(Path(self.config.face_db).joinpath('%s.jpg' % user_id))
+
         self.faces_embedding.append({
             "user_id": user_id,
             "feature": embedding
         })
         return user_id
 
     def recognition(self, image):
@@ -82,12 +82,11 @@
             results.append(result)
         return is_similar
 
     @staticmethod
     def feature_compare(feature1, feature2, threshold):
         diff = np.subtract(feature1, feature2)
         dist = np.sum(np.square(diff), 1)
-        print("Human Face European Distance:% F" % dist)
         if dist < threshold:
             return True
         else:
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `faceid_core-0.0.5/setup.py` & `faceid_core-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = dict(
     name='faceid_core',
-    version='0.0.5',
+    version='0.1.0',
     description='Face Recognition',
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
     author='Orhan Salahetdinov',
     author_email='salahetdinovorxan@gmail.com',
     keywords=['FaceId', 'Face Recognition', 'Python 3'],
@@ -16,12 +16,12 @@
 
 install_requires = [
     'opencv-python',
     'insightface',
     'numpy',
     'pathlib',
     'sklearn',
-
+    'pyyaml',
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

