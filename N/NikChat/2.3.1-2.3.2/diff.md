# Comparing `tmp/NikChat-2.3.1.tar.gz` & `tmp/NikChat-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikChat-2.3.1.tar", last modified: Wed Jun 14 02:26:38 2023, max compression
+gzip compressed data, was "NikChat-2.3.2.tar", last modified: Mon Jun 19 23:43:19 2023, max compression
```

## Comparing `NikChat-2.3.1.tar` & `NikChat-2.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.213622 NikChat-2.3.1/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.166626 NikChat-2.3.1/NikChat/
--rw-rw-rw-   0        0        0     6650 2023-06-14 02:23:35.000000 NikChat-2.3.1/NikChat/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.1/NikChat/results.py
--rw-rw-rw-   0        0        0     4356 2023-06-11 03:28:01.000000 NikChat-2.3.1/NikChat/training.py
-drwxrwxrwx   0        0        0        0 2023-06-14 02:26:38.208031 NikChat-2.3.1/NikChat.egg-info/
--rw-rw-rw-   0        0        0     1678 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 02:26:38.000000 NikChat-2.3.1/NikChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1678 2023-06-14 02:26:38.214618 NikChat-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-24 05:16:40.000000 NikChat-2.3.1/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      633 2023-06-14 02:26:38.218604 NikChat-2.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.109067 NikChat-2.3.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikChat-2.3.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.084087 NikChat-2.3.2/NikChat/
+-rw-rw-rw-   0        0        0     6738 2023-06-19 23:41:35.000000 NikChat-2.3.2/NikChat/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-06-05 02:13:44.000000 NikChat-2.3.2/NikChat/results.py
+-rw-rw-rw-   0        0        0     4658 2023-06-19 23:24:28.000000 NikChat-2.3.2/NikChat/training.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:43:19.107095 NikChat-2.3.2/NikChat.egg-info/
+-rw-rw-rw-   0        0        0     1658 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 23:43:19.000000 NikChat-2.3.2/NikChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1658 2023-06-19 23:43:19.109067 NikChat-2.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-06-19 23:42:11.000000 NikChat-2.3.2/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikChat-2.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      633 2023-06-19 23:43:19.114782 NikChat-2.3.2/setup.cfg
```

### Comparing `NikChat-2.3.1/LICENSE` & `NikChat-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.1/NikChat/__init__.py` & `NikChat-2.3.2/NikChat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+from os.path import exists
+import json
+import random
+import requests
+import pickle
+import numpy as np
+import nltk
+from nltk.stem import WordNetLemmatizer
+from tensorflow.keras.models import load_model
+from NikChat.results import ctime, weather, internet
+
 def DChat(input):
     try:
         import nltk
         #nltk.download('punkt')
         #nltk.download('wordnet')
         import json
         import random
@@ -44,22 +55,22 @@
             tag = intents_list[0]['intent']
             list_of_intents = intents_json['intents']
             for i in list_of_intents:
                 if i['tag'] == tag:
                     result = random.choice(i['responses'])
                     break
             return result
-        print('THE BOT IS RUNNING')
+        #print('THE BOT IS RUNNING')
         message = input
         ints = predict_class(message)
         res = get_response(ints, intents['record'])
         str1 = ''
         for elm in message.split(' '):
             str1 += elm.lower() + " "
-        print(str1.split(' '))
+        #print(str1.split(' '))
         if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
             res = weather()
         elif "day" in str1.split(' ') or "time" in str1.split(' ') or "date" in str1.split(' '):
             res = ctime()
         elif res == "bob is your dad":
             res = internet(str1)
         else:
@@ -69,44 +80,41 @@
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
             return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
         
 def train(filePath):
-    import NikChat.training as traning
-    traning.init2filePath()
+    from os.path import exists
+    if exists('words.pkl') == False:
+        import NikChat.training as traning
+        traning.init2(filePath)
+        return 'done'
+    else:
+        return 'done'
+
 
 def init():
-    from os.path import exists
     if exists('words.pkl') == False:
         import NikChat.training as traning
         traning.init()
         return 'done'
     else:
         return 'done'
 
-def NChat(filePath):
+def NChat(filePath, input):
     try:
-        import nltk
         #nltk.download('punkt')
         #nltk.download('wordnet')
-        import json
-        import random
-        import requests
-        import pickle
-        import numpy as np
-        from nltk.stem import WordNetLemmatizer
-        from tensorflow.keras.models import load_model
-        from NikChat.results import ctime, weather, internet
         lemmatizer = WordNetLemmatizer()
-        intents = json.loads(filePath)
+        intents = {}
+        with open(filePath, 'r') as f:
+            intents = json.load(f)
         words = pickle.load(open('words.pkl', 'rb'))
         classes = pickle.load(open('classes.pkl', 'rb'))
-        json.dumps(intents, "training.json")
         model = load_model('Speechbot.h5')
         def clean_up_sentence(sentence):
             sentence_words = nltk.word_tokenize(sentence)
             sentence_words = [lemmatizer.lemmatize(word) for word in sentence_words]
             return sentence_words
         def bag_of_words(sentence):
             sentence_words = clean_up_sentence(sentence)
@@ -130,30 +138,30 @@
             tag = intents_list[0]['intent']
             list_of_intents = intents_json['intents']
             for i in list_of_intents:
                 if i['tag'] == tag:
                     result = random.choice(i['responses'])
                     break
             return result
-        print('THE BOT IS RUNNING')
+        #print('THE BOT IS RUNNING')
         message = input
         ints = predict_class(message)
         res = get_response(ints, intents['record'])
         str1 = ''
         for elm in message.split(' '):
             str1 += elm.lower() + " "
-        print(str1.split(' '))
+        #print(str1.split(' '))
         if "weather" in str1.split(' ') or "temperature" in str1.split(' ') or "forecast" in str1.split(' '):
             res = weather()
         elif "day" in str1.split(' ') or "time" in str1.split(' ') or "date" in str1.split(' '):
             res = ctime()
         elif res == "bob is your dad":
             res = internet(str1)
         else:
             res = res
         return res
     except Exception as e:
         from os.path import exists
         if exists('words.pkl') == False:
             return 'Remember to use nikchat.init() before you use nikchat.NChat()'
         else:
-            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
+            return e, " If your OS doesn't support automated downloads, please install the following libraries: nltk, numpy, tensorflow, wikipedia, bs4, geopy, geocoder"
```

### Comparing `NikChat-2.3.1/NikChat/results.py` & `NikChat-2.3.2/NikChat/results.py`

 * *Files identical despite different names*

### Comparing `NikChat-2.3.1/NikChat/training.py` & `NikChat-2.3.2/NikChat/training.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.layers import Dense, Activation, Dropout
 from tensorflow.keras.optimizers.legacy import SGD
 
 def init():
     lemmatizer = WordNetLemmatizer()
     x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
-    intents = json.loads(x.text)
+    intents = json.load(x.text)
     words = []
     classes = []
     documents = []
     ignore_letters = ["?", "!", ".", ","]
     for intent in intents['record']['intents']:
         for pattern in intent['patterns']: 
             word_list = nltk.word_tokenize(pattern)
@@ -56,16 +56,25 @@
     sgd = SGD(lr=0.01, decay=1e-6, momentum=0.9, nesterov=True)
     model.compile(loss="categorical_crossentropy", optimizer="sgd", metrics=['accuracy'])
     hist = model.fit(np.array(train_x), np.array(train_y), epochs=200, batch_size=5, verbose=1)
     model.save("Speechbot.h5", hist)
     return
 
 def init2(filePath):
+    import os
     lemmatizer = WordNetLemmatizer()
-    intents = json.loads(str(filePath))
+    if os.path.exists(filePath) == False:
+        x = requests.get('https://api.jsonbin.io/v3/b/64698dac8e4aa6225ea0fcce')
+        y = json.load(x.text)
+        print(y)
+        with open(filePath, 'w') as f:
+            json.dump(y, f)
+    intents = {}
+    with open(filePath, 'r') as f:
+        intents = json.load(f)
     words = []
     classes = []
     documents = []
     ignore_letters = ["?", "!", ".", ","]
     for intent in intents['record']['intents']:
         for pattern in intent['patterns']: 
             word_list = nltk.word_tokenize(pattern)
```

### Comparing `NikChat-2.3.1/NikChat.egg-info/PKG-INFO` & `NikChat-2.3.2/NikChat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.1
+Version: 2.3.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,13 +29,12 @@
 
 First use the `init()` method which initializes the library
 
 Then use the `NChat()` method. This is how you communicate with the bot. This method takes one argument: the prompt.
 Example: ```print(NChat("who is joe biden"))```
 
 ## Upcoming Features
-- Faster speeeeeds
 - Story generation
 - song lyric fetcher
 - basic personality
 - basic personality recognition
 - inappropriate content recognition
```

### Comparing `NikChat-2.3.1/PKG-INFO` & `NikChat-2.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikChat
-Version: 2.3.1
+Version: 2.3.2
 Summary: A full-fledged chatbot designed to be incorperated into other projects. (Speeds of 0.1 seconds)
 Home-page: https://github.com/Nikhilodeon1/NikChat
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,13 +29,12 @@
 
 First use the `init()` method which initializes the library
 
 Then use the `NChat()` method. This is how you communicate with the bot. This method takes one argument: the prompt.
 Example: ```print(NChat("who is joe biden"))```
 
 ## Upcoming Features
-- Faster speeeeeds
 - Story generation
 - song lyric fetcher
 - basic personality
 - basic personality recognition
 - inappropriate content recognition
```

### Comparing `NikChat-2.3.1/README.md` & `NikChat-2.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,13 +15,12 @@
 
 First use the `init()` method which initializes the library
 
 Then use the `NChat()` method. This is how you communicate with the bot. This method takes one argument: the prompt.
 Example: ```print(NChat("who is joe biden"))```
 
 ## Upcoming Features
-- Faster speeeeeds
 - Story generation
 - song lyric fetcher
 - basic personality
 - basic personality recognition
 - inappropriate content recognition
```

### Comparing `NikChat-2.3.1/setup.cfg` & `NikChat-2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 4368 6174 0d0a 7665 7273   = NikChat..vers
-00000020: 696f 6e20 3d20 322e 332e 310d 0a61 7574  ion = 2.3.1..aut
+00000020: 696f 6e20 3d20 322e 332e 320d 0a61 7574  ion = 2.3.2..aut
 00000030: 686f 7220 3d20 4e69 6b68 696c 2054 616d  hor = Nikhil Tam
 00000040: 7661 6461 2028 4e69 6b68 696c 6f64 656f  vada (Nikhilodeo
 00000050: 6e31 290d 0a61 7574 686f 725f 656d 6169  n1)..author_emai
 00000060: 6c20 3d20 6e69 6b68 696c 7461 6d76 6164  l = nikhiltamvad
 00000070: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
 00000080: 6372 6970 7469 6f6e 203d 2041 2066 756c  cription = A ful
 00000090: 6c2d 666c 6564 6765 6420 6368 6174 626f  l-fledged chatbo
```

