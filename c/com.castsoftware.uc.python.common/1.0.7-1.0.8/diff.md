# Comparing `tmp/com.castsoftware.uc.python.common-1.0.7.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.7.tar", last modified: Wed Jun  7 19:23:10 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.8.tar", last modified: Tue Jun 20 20:52:47 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.7.tar` & `com.castsoftware.uc.python.common-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.661091 com.castsoftware.uc.python.common-1.0.7/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      714 2023-06-07 19:23:10.644834 com.castsoftware.uc.python.common-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.530756 com.castsoftware.uc.python.common-1.0.7/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    13723 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0    10826 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5625 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/logger.py
--rw-rw-rw-   0        0        0     5264 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     7054 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.596930 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      714 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      643 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 19:23:10.661091 com.castsoftware.uc.python.common-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.945505 com.castsoftware.uc.python.common-1.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-06-20 20:52:47.938477 com.castsoftware.uc.python.common-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.857826 com.castsoftware.uc.python.common-1.0.8/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    13723 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     4469 2023-06-19 13:01:19.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/greenIt.py
+-rw-rw-rw-   0        0        0     9980 2023-06-20 20:44:31.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5625 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1778 2023-06-14 17:36:16.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/logger.py
+-rw-rw-rw-   0        0        0    13409 2023-06-19 13:18:16.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/powerpoint.py
+-rw-rw-rw-   0        0        0     5457 2023-06-20 20:37:23.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     7380 2023-06-14 13:23:51.000000 com.castsoftware.uc.python.common-1.0.8/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.915660 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 20:52:47.000000 com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      643 2023-06-12 16:21:04.000000 com.castsoftware.uc.python.common-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 20:52:47.945505 com.castsoftware.uc.python.common-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 20:52:47.925268 com.castsoftware.uc.python.common-1.0.8/test/
+-rw-rw-rw-   0        0        0      494 2023-06-12 17:37:07.000000 com.castsoftware.uc.python.common-1.0.8/test/TestMultiInstance.py
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/LICENSE` & `com.castsoftware.uc.python.common-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.7/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.7
+Version: 1.0.8
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/aipRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/highlight.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,131 @@
 from cast_common.restAPI import RestCall
-from cast_common.logger import INFO
+from cast_common.logger import Logger, INFO,DEBUG
 from cast_common.util import format_table
 
 from requests import codes
 from pandas import ExcelWriter,DataFrame,json_normalize,concat
 from typing import List
-from json import loads
+from json import loads,dumps
 
 class Highlight(RestCall):
 
     _data = {}
-    _apps = []
     _tags = []
     _cloud = []
     _oss = []
     _elegance = []
-    _instance_id = None
+    _apps_full_list = None
+    _instance_id = 0
+
+    log = None
 
     def __init__(self,  hl_user:str, hl_pswd:str, 
                  hl_instance:int,hl_apps:str=[],hl_tags:str=[], 
                  hl_base_url:str='https://rpa.casthighlight.com', 
                  log_level=INFO, timer_on=False):
 
-        super().__init__(f'{hl_base_url}/WS2/', hl_user, hl_pswd, timer_on,log_level)
+        if Highlight.log is None:
+            Highlight.log = Logger('Highlight',log_level)
 
-        self._hl_instance = hl_instance
+        reset_data = False
+        if Highlight._instance_id is not hl_instance:
+            self.log.debug(f'new instance id: {hl_instance}')
+            Highlight._instance_id = hl_instance
+            Highlight._data = {}
+            reset_data = True
+
+        super().__init__(f'{hl_base_url}/WS2/', hl_user, hl_pswd, timer_on,log_level)
 
         # self._business = self._get_top_metric('businessValue')
         # self._cloud = self._get_top_metric('cloudValue')
         # self._oss = self._get_top_metric('openSourceSafty')
         # #self._elegance = self._get_top_metric('softwareElegance')
 
-        self._tags = self._get_tags()
-        self._apps = DataFrame(self._get_applications())
-        self.info(f'Found {len(self._apps)} applications')
-        self._apps.dropna(subset=['metrics'],inplace=True)
-        self.info(f'Found {len(self._apps)} analyzed applications')
+        if reset_data:
+            Highlight._tags = self._get_tags()
+            Highlight._apps_full_list = []
+
+            # retrieve all applications from HL REST API
+            Highlight._apps_full_list = DataFrame(self._get_applications())
+#            Highlight._apps_full_list.dropna(subset=['metrics'],inplace=True)
+            self.info(f'Found {len(Highlight._apps_full_list)} analyzed applications: {",".join(Highlight._apps_full_list["name"])}')
+    
+        # if the apps is not already of list type then convert it now
+        if not isinstance(hl_apps,list):
+            hl_apps=list(hl_apps.split(','))
+
+        #if hl_apps is empty, include all applications prevously retrieved
+        #otherwise filter the list down to include only the selected applications
         if len(hl_apps) > 0:
-            self._apps = self._apps[self._apps['name'].isin(hl_apps)]
-        self.info(f'{len(self._apps)} applications selected')
+            self._apps = Highlight._apps_full_list[Highlight._apps_full_list['name'].isin(hl_apps)]
+        else:
+            self._apps = Highlight._apps_full_list
 
-        self._data = {}
-        # for idx,app in self._apps.iterrows():
-        #     try:
-        #         app_name = app['name']
-                
-        #         self.info(f'Loading Highlight data for {app_name}')
-        #         self._data[app_name]= self._get_application_data(app_name)
-
-
-                # domains = app_data[app_name]['domains']
-                # metrics = app_data[app_name]['metrics'][0]
-                # green_detail = json_normalize(metrics['greenDetail'],['greenIndexDetails'],meta=['technology','greenIndexScan'])
-                # cloud_detail = metrics['cloudReadyDetail'][0]
-                # technology_detail = metrics['technologies'][0]
-                # vulnerability_detail = metrics['vulnerabilities'][0]
-                # components_detail = metrics['components'][0]
-
-                # app_data[app]={'domains':domains}
-
-        #         pass
-        #     except KeyError as ke:
-        #         pass
-        #     except Exception as ex:
-        #         self.error(str(ex))
-        # pass
-
-
-        # file_name = r'e:/work/wellsfargo/tags.xlsx'
-        # writer = ExcelWriter(file_name, engine='xlsxwriter')
-        # summary_tab = format_table(writer,DataFrame(self._tags),'Tags')
-        # writer.close()
+        self.info(f'{len(self._apps)} applications selected: {",".join(self._apps["name"])}')
 
         pass
 
-    def _get_all_application_data(self):
-        self.info('Retrieving all HL application specific data')
-        self._data = {}
-        for idx,app in self._apps.iterrows():
-            try:
-                app_name = app['name']
-                self.info(f'Loading Highlight data for {app_name}')
-                self._data[app_name]= self._get_application_data(app_name)
-            except KeyError as ke:
-                self.warning(str(ke))
-                pass
-            except Exception as ex:
-                self.error(str(ex))
+    @property
+    def app_list(self) -> DataFrame:
+        return self._apps
+
+    def _get_application_data(self,app:str=None):
+        self.debug('Retrieving all HL application specific data')
+        
+        if str is None:
+            df = self._apps
+        else:
+            df = self._apps[self._apps['name']==app]
+
+        for idx,app in df.iterrows():
+            app_name = app['name']
+            self.debug(f'Loading Highlight data for {app_name}')
+            if app_name not in Highlight._data:
+                try:
+                    self.debug(f'{app_name} - loading from REST')
+                    Highlight._data[app_name]=self._get_app_from_rest(app_name)
+                except KeyError as ke:
+                    self.warning(str(ke))
+                    pass
+                except Exception as ex:
+                    self.error(str(ex))
         pass
 
     def _get_metrics(self,app_name):
         try:
-            if len(self._data)==0:
-                self._get_all_application_data()
-            data = self._data[app_name]
+            if app_name not in self._apps['name'].to_list():
+                raise ValueError(f'{app_name} is not a selected application')
+
+            self._get_application_data(app_name)
+            data = Highlight._data[app_name]
             metrics = data['metrics'][0]
             return metrics
         except KeyError as ke:
             self.error(f'{app_name} has no Metric Data')
             raise ke
 
-    def _get(self,url:str) -> DataFrame:
-        (status, json) = self.get(url)
+    def _get(self,url:str,header=None) -> DataFrame:
+        (status, json) = self.get(url,header)
         if status == codes.ok:
             return DataFrame(json)
         else:
             raise KeyError (f'Server returned a {status} while accessing {url}')
 
     def _get_applications(self):
-        return self._get(f'domains/{self._hl_instance}/applications/')
+        return self._get(f'domains/{Highlight._instance_id}/applications/', {'Accept': 'application/vnd.castsoftware.api.basic+json'} )
         
     def _get_tags(self) -> DataFrame:
-        return DataFrame(self._get(f'domains/{self._hl_instance}/tags/'))
+        return DataFrame(self._get(f'domains/{Highlight._instance_id}/tags/'))
 
     # def _get_top_metric(self,metric:str) -> DataFrame:
-    #     return DataFrame(self.post(f'domains/{self._hl_instance}/metrics/top?metric=cloudReady&order=desc',header={'Content-type':'application/json'}))
+    #     return DataFrame(self.post(f'domains/{Highlight._instance_id}/metrics/top?metric=cloudReady&order=desc',header={'Content-type':'application/json'}))
 
-    def _get_application_data(self,app:str) -> dict:
-        return self._get(f'domains/{self._hl_instance}/applications/{self.get_app_id(app)}')
+    def _get_app_from_rest(self,app:str) -> dict:
+        return self._get(f'domains/{Highlight._instance_id}/applications/{self.get_app_id(app)}')
 
     def get_app_id(self,app_name:str) -> int:
         """get the application id
 
         Args:
             app_name (str): application name 
 
@@ -148,18 +152,18 @@
 
         Raises:
             KeyError: tag not found
 
         Returns:
             int: highlight tag id
         """
-        if len(self._tags)==0:
-            self._tags = self._get_tags()
+        if len(Highlight._tags)==0:
+            Highlight._tags = self._get_tags()
 
-        series = self._tags[self._tags['label']==tag_name]
+        series = Highlight._tags[Highlight._tags['label']==tag_name]
         if series.empty:
             raise KeyError (f'Highlight tag not found: {tag_name}')
         else:
             return int(series.iloc[0]['id'])
             
     def add_tag(self,app_name,tag_name) -> bool:
         """Add tag for application 
@@ -169,27 +173,27 @@
             tag_name (_type_): tag name
         Returns:
             bool: True if tag added
         """
         app_id = self.get_app_id(app_name)
         tag_id = self.get_tag_id(tag_name)
 
-        url = f'domains/{self._hl_instance}/applications/{app_id}/tags/{tag_id}'
+        url = f'domains/{Highlight._instance_id}/applications/{app_id}/tags/{tag_id}'
         (status,json) = self.post(url)
         if status == codes.ok or status == codes.no_content:
             return True
         else:
             return False 
     
     def get_tech_debt_advisor(self,order:List[str],tag:str=None) -> DataFrame:
         #https://rpa.casthighlight.com/WS2/domains/1271/technicalDebt/aggregated?tagIds=685&activePagination=false&pageOffset=0&maxEntryPerPage=9999&maxPage=999&order=healthFactor&order=alert
         tag_part = ""
         if tag is not None:
             tag_part = f'tagIds={self.get_tag_id(tag)}&'
-        url = f'domains/{self._hl_instance}/technicalDebt/aggregated?{tag_part}&activePagination=false&pageOffset=0&maxEntryPerPage=9999&maxPage=999'
+        url = f'domains/{Highlight._instance_id}/technicalDebt/aggregated?{tag_part}&activePagination=false&pageOffset=0&maxEntryPerPage=9999&maxPage=999'
         for o in order:
             url=f'{url}&order={o}'
         
         (status, json) = self.get(url)
         if status == codes.ok:
             d1 = json_normalize(json,['subLevel'], max_level=1)
             d1.rename(columns={'id':'Health Factor'},inplace=True)
@@ -217,76 +221,52 @@
         Args:
             app_name (str): name of the application
 
         Returns:
             DataFrame: flattened version of the Highlight cloud ready data
         """
         try:
-            return json_normalize(self._get_metrics(app_name)['greenDetail'],['cloudReadyDetails'],meta=['technology','cloudReadyScan'])
+            return json_normalize(self._get_metrics(app_name)['cloudDetail'],['cloudReadyDetails'],meta=['technology','cloudReadyScan'])
         except KeyError as ke:
             self.warning(f'{app_name} has no Cloud Ready Data')
             return None
 
-    def get_green_detail(self,app_name:str)->DataFrame:
-        """Highlight green it data
-
-        Args:
-            app_name (str): name of the application
-
-        Returns:
-            DataFrame: flattened version of the Highlight green it data
-        """
-        try:
-            return json_normalize(self._get_metrics(app_name)['greenDetail'],['greenIndexDetails'],meta=['technology','greenIndexScan'])
-        except KeyError as ke:
-            self.warning(f'{app_name} has no Green IT Data')
-            return None
-
     def get_tech_detail(self,app_name:str)->DataFrame:
         """Highlight technology data
 
         Args:
             app_name (str): name of the application
 
         Returns:
             DataFrame: flattened version of the Highlight technology data
         """
         try:
             return json_normalize(self._get_metrics(app_name)['technologies'],['greenIndexDetails'],meta=['technology','greenIndexScan'])
         except KeyError as ke:
             self.warning(f'{app_name} has no Green IT Data')
             return None
+        
 
-
-#https://rpa.casthighlight.com/WS2/domains/1271/applications/188146/tags/679
+#hl = Highlight('n.kaplan+MerckMSD@castsoftware.com','vadKpBFAZ8KIKb2f2y',4711,hl_base_url='https://cloud.casthighlight.com',log_level=DEBUG)
 
 
+# class A (Highlight):
+#         pass
 
-# hl = Highlight('n.kaplan+MerckMSD@castsoftware.com','vadKpBFAZ8KIKb2f2y',4711,hl_base_url='https://cloud.casthighlight.com/')
-# green_data = hl.get_green_details('TPS-2')
-# pass
+# class B (Highlight):
+#         pass
 
+# print ('class A')
+# hl = A('n.kaplan+MerckMSD@castsoftware.com','vadKpBFAZ8KIKb2f2y',4711,hl_base_url='https://cloud.casthighlight.com',log_level=DEBUG)
+# df = hl.get_green_detail('TPS')
+
+# try:
+#     print ('class B')
+#     hl2 = B('n.kaplan+MerckMSD@castsoftware.com','vadKpBFAZ8KIKb2f2y',4711,'Demo',hl_base_url='https://cloud.casthighlight.com',log_level=DEBUG)
+#     df = hl2.get_green_detail('Demo')
+#     df2 = hl2.get_green_detail('TPS')
+# except ValueError as ve:
+#     print (ve)
 
-# hl = Highlight('n.kaplan+WellsFargo@castsoftware.com','mdSi20ty@02',1271,hl_base_url='https://rpa.casthighlight.com/')
+# pass
 
-# df = hl.get_tech_debt_advisor(['healthFactor','alert'],tag='Hamilton, Cliona')
-# df['Effort']=df['Effort']/60/8
-# df=df.rename(columns={'application_name':'Component'})
-# #df['Technology']=''
-# df['Technology']=df['Alert'].str.split('__').str[0]
-# df['Rule']=df['Alert'].str.split('__').str[1]
-# df['Rule']=df['Rule'].str.replace('_','').str.replace(r"(\w)([A-Z])", r"\1 \2",regex=True)
-
-# df['Application']=df['Component'].str.split(':').str[0]
-# df['Component']=df['Component'].str.split(':').str[-1]
-
-# df.drop(columns=['Alert'],inplace=True)
-# df = df[['Health Factor','Application','Component','Effort','Technology','Rule']]
-
-# from os.path import abspath
-
-# apps_df = df['Application'].drop_duplicates().to_frame()
-# file_name = abspath(f'E:/work/WellsFargo/tech-debt-HamiltonCliona.xlsx')
-# writer = ExcelWriter(file_name, engine='xlsxwriter')
-# app_tab = format_table(writer,apps_df,'applications')
-# writer.close
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,18 @@
             self.loggers.add(name)
             self.logger.setLevel(self.level)
             self.logger.addHandler(self.console_logger)
             if not file_name is None:
                 fileHandler = logging.FileHandler(file_name,file_mode)
                 fileHandler.setFormatter(self.console_formatter)
                 self.logger.addHandler(fileHandler)
-        
 
+    @property    
+    def is_debug(self):
+        return self.logger.isEnabledFor(logging.DEBUG)
 
     def set_level(self,level):
         self.logger.setLevel(level)
 
     def debug(self, msg, *args, **kwargs):
         self.logger.debug(msg, *args, **kwargs)
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/restAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,28 +48,32 @@
 
         self._auth = HTTPBasicAuth(user, password)
         self._session.headers.update({'Accept': 'application/json'})
         #self._session.headers.update({'Authorization': self._auth})
 
 
 #    def get(self, url = "", headers = {'Accept': 'application/json'}):
-    def get(self, url = ""):
+    def get(self, url = "",header=None):
         start_dttm = ctime()
         start_tm = perf_counter()
 
         try:
             if len(url) > 0 and url[0] != '/':
                 url=f'/{url}'
             u = urllib.parse.quote(f'{self._base_url}{url}',safe='/:&?=')
             # if self._auth == None:
             #     resp = get(url= u, headers={'Accept': 'application/json'})
             # else:
             #     resp = get(url= u, auth = self._auth, headers={'Accept': 'application/json'})
 
-            resp = self._session.get(u, timeout = (5, 15),auth=self._auth,headers={'Accept': 'application/json'})
+            if header is None:
+                header={'Accept': 'application/json'}
+
+#            resp = self._session.get(u, timeout = (5, 15),auth=self._auth,headers={'Accept': 'application/json'})
+            resp = self._session.get(u, timeout = (5, 15),auth=self._auth,headers=header)
             resp.raise_for_status()
 
             # Save the duration, if enabled.
             if (self._track_time):
                 end_tm = perf_counter()
                 end_dttm = ctime()
                 duration = end_tm - start_tm
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.8/cast_common/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,22 +205,31 @@
     table_options={
                 'total_row':total_line,
                 'columns':columns,
                 'header_row':True,
                 'autofilter':True,
                 'banded_rows':True
                 }
+
     worksheet.add_table(0, 0, rows, cols,table_options)
+    
+    header_format = workbook.add_format({'text_wrap':True,
+                                        'align': 'center'})
 
     col_width = 10
     if width == None:
         width = []
         for i in range(1,len(data.columns)+1):
            width.append(col_width)
 
+    for col_num, value in enumerate(data.columns.values):
+        worksheet.write(0, col_num, value, header_format)
+        w=width[col_num]
+        worksheet.set_column(col_num, col_num, w)
+
     return worksheet
 
 
 def convert_LOC(total:int):
     unit = ''
     if 1000 <= total <= 1000000:
         unit = 'KLoc'
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.8/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.7
+Version: 1.0.8
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.7/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.7' #prod version
+version='1.0.8' #prod version
 
 dependencies = ['pandas','requests','XlsxWriter']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

