# Comparing `tmp/openAIInsight-0.0.8-py3-none-any.whl.zip` & `tmp/openAIInsight-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6033 bytes, number of entries: 8
--rw-rw-r--  2.0 unx    12218 b- defN 23-May-25 19:47 openAIInsight/OpenAI_PineConeVector.py
--rw-rw-r--  2.0 unx       84 b- defN 23-May-25 19:30 openAIInsight/__init__.py
--rw-rw-r--  2.0 unx     3604 b- defN 23-May-25 19:30 openAIInsight/openAI.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      609 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      675 b- defN 23-May-25 19:48 openAIInsight-0.0.8.dist-info/RECORD
-8 files, 18369 bytes uncompressed, 4845 bytes compressed:  73.6%
+Zip file size: 6029 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx    12169 b- defN 23-May-31 08:52 openAIInsight/OpenAI_PineConeVector.py
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-31 08:38 openAIInsight/__init__.py
+-rw-rw-r--  2.0 unx     3604 b- defN 23-May-31 08:38 openAIInsight/openAI.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-May-31 08:54 openAIInsight-0.0.9.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-May-31 08:54 openAIInsight-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-31 08:54 openAIInsight-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-31 08:54 openAIInsight-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      675 b- defN 23-May-31 08:54 openAIInsight-0.0.9.dist-info/RECORD
+8 files, 18320 bytes uncompressed, 4841 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: openAIInsight/__init__.py
 Comment: 
 
 Filename: openAIInsight/openAI.py
 Comment: 
 
-Filename: openAIInsight-0.0.8.dist-info/LICENCE.txt
+Filename: openAIInsight-0.0.9.dist-info/LICENCE.txt
 Comment: 
 
-Filename: openAIInsight-0.0.8.dist-info/METADATA
+Filename: openAIInsight-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: openAIInsight-0.0.8.dist-info/WHEEL
+Filename: openAIInsight-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: openAIInsight-0.0.8.dist-info/top_level.txt
+Filename: openAIInsight-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: openAIInsight-0.0.8.dist-info/RECORD
+Filename: openAIInsight-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openAIInsight/OpenAI_PineConeVector.py

```diff
@@ -3,35 +3,34 @@
 import pinecone
 import datetime
 import traceback
 import pandas as pd
 from flask import request
 import loggerutility as logger
 import commonutility as common
-from openai.embeddings_utils import get_embedding, get_embeddings, cosine_similarity
+from openai.embeddings_utils import get_embedding, get_embeddings
 
 
 class OpenAI_PineConeVector:
     
-    index_name      =   "" 
-    openAI_apiKey   =   "" 
-    pineCone_apiKey =   "" 
+    index_name      =   ""
+    openAI_apiKey   =   ""
+    pineCone_apiKey =   ""
     queryList       =   "" 
     dfJson          =   ""
     engineName      =   "text-embedding-ada-002" # Model that we want to use 
     dimensions      =   1536
     my_index        =   ""
     enterpriseName  =   ""
 
     def trainData(self, pineCone_json):
         # When calling from process definition, we need to pass hard-coded openAI_apiKey & pineCone_apiKey.
         try:
             
             logger.log("inside PineConeVector class trainData()","0")
-            
             if "openAI_apiKey" in pineCone_json and pineCone_json["openAI_apiKey"] != None:
                 self.openAI_apiKey = pineCone_json["openAI_apiKey"]           
                 logger.log(f"\ntrain_PineConeVector openAI_apiKey:::\t{self.openAI_apiKey} \t{type(self.openAI_apiKey)}","0")
             
             if "pineCone_apiKey" in pineCone_json and pineCone_json["pineCone_apiKey"] != None:
                 self.pineCone_apiKey = pineCone_json["pineCone_apiKey"]           
                 logger.log(f"\ntrain_PineConeVector pineCone_apiKey:::\t{self.pineCone_apiKey} \t{type(self.pineCone_apiKey)}","0")
@@ -40,39 +39,39 @@
                 self.index_name = pineCone_json["index_name"]
                 logger.log(f"\ntrain_PineConeVector index_name:::\t{self.index_name} \t{type(self.index_name)}","0")
             
             if "dfJson" in pineCone_json and pineCone_json["dfJson"] != None:
                 self.dfJson = pineCone_json["dfJson"]
                 logger.log(f"\ntrain_PineConeVector dfJson:::\t{self.dfJson} \t{type(self.dfJson)}","0")
             
-            if "trainData" in pineCone_json and pineCone_json["trainData"] != None:
-                self.dfJson = pineCone_json["trainData"]
-                logger.log(f"\ntrain_PineConeVector trainData:::\t{self.trainData} \t{type(self.trainData)}","0")
-
             if "enterprise" in pineCone_json and pineCone_json["enterprise"] != None:
                 self.enterpriseName = pineCone_json["enterprise"]
                 logger.log(f"\nPineConeVector class LookUpData() enterprise:::\t{self.enterpriseName} \t{type(self.enterpriseName)}","0")
 
             logger.log(f"\nPineConeVector class trainData() all Parameters:::  \n{locals()}\n","0")
             
-            parsed_json = (json.loads( self.dfJson))
-            df = pd.DataFrame(parsed_json[1:])
-            
+            if type(self.dfJson) == str :
+                parsed_json = json.loads(self.dfJson)
+                df = pd.DataFrame(parsed_json)
+            else:
+                df = pd.DataFrame(self.dfJson)
+                
+            logger.log(f"Pinecone Available indexes List df :: \t {df}", "0")    
             pinecone.init(api_key=self.pineCone_apiKey, environment='us-west4-gcp')
             openai.api_key = self.openAI_apiKey                 
 
             logger.log(f"Pinecone Available indexes List  :: \t {pinecone.list_indexes()}", "0")    
             # Creating index
             if self.index_name not in pinecone.list_indexes():
-                logger.log(f" '{self.index_name}' index not present. Creating New!!!", "0")
+                logger.log(f" \n'{self.index_name}' index not present. Creating New!!!\n", "0")
                 pinecone.create_index(name = self.index_name, dimension=self.dimensions, metric='cosine')
+                self.my_index = pinecone.Index(index_name=self.index_name)
             else:
-                logger.log(f" '{self.index_name}' index is present. Loading now!!!", "0")
+                logger.log(f" \n'{self.index_name}' index is present. Loading now!!!\n", "0")
                 self.my_index = pinecone.Index(index_name=self.index_name)
-                
             logger.log(f"Pinecone Available indexes List  :: \t {pinecone.list_indexes()}", "0")    
 
             df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
             df.fillna("N/A",inplace=True)
             #Changing column names to lowercase and replacing nan values with a string placeholder
             df.columns = ['_'.join(column.lower().split(' ')) for column in df.columns]
             df.fillna("N/A",inplace=True)
@@ -89,34 +88,33 @@
             elif self.index_name == "document":
                 df['embedding'] = get_embeddings(df['description'].to_list(), engine=self.engineName)
                 metadata = df[['description','enterprise']].to_dict(orient='records')
 
             else:
                 logger.log(f"\n\n INVALID INDEX NAME ::: \t{self.index_name}\n", "0")    
             
-            logger.log(f"\ntrain_PineConeVector df.head() line 96 :: {df.head()},\n {df.head()}", "0")    
             upsert = list(zip(df['id'], df['embedding'], metadata))
             _ = self.my_index.upsert(vectors=upsert)
-            logger.log(f"{self.my_index.describe_index_stats()}","0")
+            logger.log(f"line 99:::{self.my_index.describe_index_stats()}","0")
 
             logger.log(f"\nOpenAI_PineConeVector class trainData:::\t{self.my_index}","0")
 
             if self.my_index != "":
-                return f" '{self.index_name}' Index Creation successful. "
+                return f" '{self.index_name}' Index Creation SUCCESSFUL for Enterprise: {self.enterpriseName}. "
             else:
-                return f" '{self.index_name}' Index Creation failed. "
+                return f" '{self.index_name}' Index Creation FAILED for Enterprise: {self.enterpriseName}. "
             
             
         except Exception as e:
             logger.log(f"OpenAI_PineConeVector class trainData() Issue::: \n{e}","0")
             trace = traceback.format_exc()
             descr = str(e)
             errorXml = common.getErrorXml(descr, trace)
             logger.log(f'\n OpenAI_PineConeVector class trainData() errorXml::: \n{errorXml}', "0")
-            raise str(errorXml)
+            return str(errorXml)
 
     def getLookupData(self):               
         try:
             
             logger.log("inside PineConeVector class LookUpData()","0")
             logger.log(f"\nPineConeVector class LookUpData() all Parameters:::  \n{locals()}\n","0")
             result      = []
@@ -196,8 +194,9 @@
             
         except Exception as e:
             logger.log(f"OpenAI_PineConeVector class getLookUP() Issue::: \n{e}","0")
             trace = traceback.format_exc()
             descr = str(e)
             errorXml = common.getErrorXml(descr, trace)
             logger.log(f'\n OpenAI_PineConeVector class getLookUP() errorXml::: \n{errorXml}', "0")
-            raise str(errorXml)
+            return str(errorXml)
+
```

## Comparing `openAIInsight-0.0.8.dist-info/LICENCE.txt` & `openAIInsight-0.0.9.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `openAIInsight-0.0.8.dist-info/METADATA` & `openAIInsight-0.0.9.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openAIInsight
-Version: 0.0.8
+Version: 0.0.9
 Summary: Proteus openAI File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

## Comparing `openAIInsight-0.0.8.dist-info/RECORD` & `openAIInsight-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-openAIInsight/OpenAI_PineConeVector.py,sha256=HVfh_sDvFDWie_TgZ7zaQczeTSLszcNod3Jpa0FHawc,12218
+openAIInsight/OpenAI_PineConeVector.py,sha256=PyYRvGoxO4QipVB2EpzF28g2_wINHcMHjKxhePT4Gl4,12169
 openAIInsight/__init__.py,sha256=xXImeaMgVuR6qaRZ8E4zbB4_kbGg4h2wOUfe9O4vrMI,84
 openAIInsight/openAI.py,sha256=PW6yUTyYZodcqibHiqEQu3IYZwD4h6u__IPSecF531g,3604
-openAIInsight-0.0.8.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
-openAIInsight-0.0.8.dist-info/METADATA,sha256=vSmATxBDWjnZy7bESs-ckk0QILh4e_zWAG6NiJczkQ0,609
-openAIInsight-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-openAIInsight-0.0.8.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
-openAIInsight-0.0.8.dist-info/RECORD,,
+openAIInsight-0.0.9.dist-info/LICENCE.txt,sha256=2qX9IkEUBx0VJp1Vh9O2dsRwE-IpYId0lXDyn7OVsJ8,1073
+openAIInsight-0.0.9.dist-info/METADATA,sha256=QxQ_Se7tXSmFOKwQ2nPwUQSdeZgSiuxdvUCkIaCtREE,609
+openAIInsight-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+openAIInsight-0.0.9.dist-info/top_level.txt,sha256=YzsKehORjpmF7-8r3ivEG7yh7VoqXMt2TfYbfHovmfg,14
+openAIInsight-0.0.9.dist-info/RECORD,,
```

