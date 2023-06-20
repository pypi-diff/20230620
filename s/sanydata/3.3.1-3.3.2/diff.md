# Comparing `tmp/sanydata-3.3.1.tar.gz` & `tmp/sanydata-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanydata-3.3.1.tar", last modified: Fri Jun  2 06:34:38 2023, max compression
+gzip compressed data, was "sanydata-3.3.2.tar", last modified: Tue Jun 20 08:31:04 2023, max compression
```

## Comparing `sanydata-3.3.1.tar` & `sanydata-3.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.868323 sanydata-3.3.1/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-02 06:34:38.868035 sanydata-3.3.1/PKG-INFO
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.864328 sanydata-3.3.1/sanydata/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.1/sanydata/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)   117531 2023-06-02 06:32:38.000000 sanydata-3.3.1/sanydata/datatools.py
--rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.3.1/sanydata/model_data_message_pb2.py
--rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.3.1/sanydata/model_data_message_pb2_grpc.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.865989 sanydata-3.3.1/sanydata.egg-info/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/PKG-INFO
--rw-r--r--   0 thao       (501) staff       (20)      371 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/SOURCES.txt
--rw-r--r--   0 thao       (501) staff       (20)        1 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/dependency_links.txt
--rw-r--r--   0 thao       (501) staff       (20)      130 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/requires.txt
--rw-r--r--   0 thao       (501) staff       (20)       15 2023-06-02 06:34:38.000000 sanydata-3.3.1/sanydata.egg-info/top_level.txt
--rw-r--r--   0 thao       (501) staff       (20)       38 2023-06-02 06:34:38.868407 sanydata-3.3.1/setup.cfg
--rw-r--r--   0 thao       (501) staff       (20)      999 2023-06-02 06:30:09.000000 sanydata-3.3.1/setup.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-02 06:34:38.867409 sanydata-3.3.1/utils/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.1/utils/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.1/utils/cos_handler.py
--rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.1/utils/file_operation.py
--rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.1/utils/local_handler.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.596533 sanydata-3.3.2/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-20 08:31:04.596272 sanydata-3.3.2/PKG-INFO
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.592195 sanydata-3.3.2/sanydata/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.2/sanydata/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)   120883 2023-06-20 08:30:08.000000 sanydata-3.3.2/sanydata/datatools.py
+-rw-r--r--   0 thao       (501) staff       (20)   102791 2023-06-20 08:22:53.000000 sanydata-3.3.2/sanydata/model_data_message_pb2.py
+-rw-r--r--   0 thao       (501) staff       (20)    22020 2023-06-20 08:22:53.000000 sanydata-3.3.2/sanydata/model_data_message_pb2_grpc.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.593492 sanydata-3.3.2/sanydata.egg-info/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-20 08:31:03.000000 sanydata-3.3.2/sanydata.egg-info/PKG-INFO
+-rw-r--r--   0 thao       (501) staff       (20)      371 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/SOURCES.txt
+-rw-r--r--   0 thao       (501) staff       (20)        1 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/dependency_links.txt
+-rw-r--r--   0 thao       (501) staff       (20)      130 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/requires.txt
+-rw-r--r--   0 thao       (501) staff       (20)       15 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/top_level.txt
+-rw-r--r--   0 thao       (501) staff       (20)       38 2023-06-20 08:31:04.596627 sanydata-3.3.2/setup.cfg
+-rw-r--r--   0 thao       (501) staff       (20)      999 2023-06-20 08:26:47.000000 sanydata-3.3.2/setup.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.595485 sanydata-3.3.2/utils/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.2/utils/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.2/utils/cos_handler.py
+-rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.2/utils/file_operation.py
+-rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.2/utils/local_handler.py
```

### Comparing `sanydata-3.3.1/sanydata/datatools.py` & `sanydata-3.3.2/sanydata/datatools.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
     return wrapper
 
 
 class DataTools(object):
     # This programme is to get data.
     PROGRAMME = 'DataTools'
-    VERSION = '3.3.1'
+    VERSION = '3.3.2'
 
     def __init__(self, stub=None, es_hosts='http://es.sanywind.net:9200/'):
         self.es = Elasticsearch(hosts=es_hosts)
 
         if stub:
             with grpc.insecure_channel(stub, options=options) as channel:
                 stub = model_data_message_pb2_grpc.ModelDataMessageStub(channel)
@@ -841,15 +841,15 @@
         :param src_file: 原始文件地址/str/"emi/data/HNFC/plc-sync/20220816/history/csv/HNFC_002_20220816_history.csv"
         :param dst_file: 处理后地址/str/"model_result/cos_single_file/speed_overcurrent/fm=HNFC/tb=002/2022-08-16.parquet"
         :return:
         """
         assert all([pinyin_code, turbine_num, file_date, func_name, func_version, dst_file]), "未传入有效参数"
         from datetime import datetime
         docs = pd.DataFrame(data=[[file_date, "model_file", func_name, "success", func_version, src_file, pinyin_code,
-                            datetime.now().strftime("%Y-%m-%d %H:%M:%S"), turbine_num, dst_file]],
+                                   datetime.now().strftime("%Y-%m-%d %H:%M:%S"), turbine_num, dst_file]],
                             columns=["date", "file_type", "func_name", "func_status", "func_version", "path",
                                      "pinyin_code", "record_time", "turbine_num", "upload_path"])
         bulk_data = []
         for _, line in docs.iterrows():
             doc = line.to_dict()
             bulk_data.append({
                 '_index': "model_maped_file",
@@ -1245,15 +1245,15 @@
             request = model_data_message_pb2.GetFirstFaultRequest(windfarm=farm,
                                                                   turbines=turbine,
                                                                   fault_code=fault_code,
                                                                   fault_tags=fault_tags,
                                                                   fault_start_time_s=fault_start_time_s,
                                                                   fault_start_time_e=fault_start_time_e,
                                                                   fault_end_time_s=fault_end_time_s,
-                                                                  fault_end_time_e=fault_end_time_e,)
+                                                                  fault_end_time_e=fault_end_time_e, )
 
             res = stub.GetFirstFault(request, timeout=20000)
 
             result_dataframe = res.output
 
             if result_dataframe != '':
                 return pd.read_json(result_dataframe)
@@ -1261,14 +1261,72 @@
                 return None
 
         except Exception as e:
             print(str(e))
             print('云平台首发故障获取错误')
             return None
 
+    @stub_channel
+    def get_first_faultV2(self, stub, farm=None, turbine=None, fault_code=None,
+                          fault_tags=None, fault_start_time_list=[None, None],
+                          fault_end_time_list=[None, None], fault_create_time_list=[None, None]):
+        """
+        获取云端首发故障信息
+        :param farm：风场中文拼音名（例如：DBCFCB），如果为多个，则传入list，如果是一个，可直接传入字符串
+        :param turbine：机组号,str或list（例如：'001'，必须为三位数,或['001', '002']），可省略
+        :param fault_code：故障码,str或list（例如：706，或[706, 707]），可省略
+        :param fault_tags：云端首发故障标签,str或list（例如：'受累'，或['受累', '人为']），可以省略
+        :param fault_start_time_list：故障开始时间（包含）范围, 例如：['2021-03-03', '2021-03-04']，可省略
+        :param fault_end_time_list：故障结束时间（包含）范围, 例如：['2021-03-03', '2021-03-04']，可省略
+        :param fault_create_time_list：故障记录时间（包含）范围, 例如：['2021-03-03', '2021-03-04']，可省略
+        :return: 匹配到的所有数据pandas.DataFrame
+        """
+        turbine = self.change_turbine(turbine)
+        farm = self.change_v(farm)
+
+        fault_code = self.change_v(fault_code)
+        fault_tags = self.change_v(fault_tags)
+
+        # 时间格式检查
+        for str_time_list in [fault_start_time_list, fault_end_time_list, fault_create_time_list]:
+            self.check_time_list(str_time_list)
+            for str_time in str_time_list:
+                self.check_time(str_time)
+
+        fault_start_time_s, fault_start_time_e = self.get_time_str(fault_start_time_list)
+        fault_end_time_s, fault_end_time_e = self.get_time_str(fault_end_time_list)
+        fault_create_time_s, fault_create_time_e = self.get_time_str(fault_create_time_list)
+
+        try:
+
+            request = model_data_message_pb2.GetFirstFaultRequestV2(windfarm=farm,
+                                                                  turbines=turbine,
+                                                                  fault_code=fault_code,
+                                                                  fault_tags=fault_tags,
+                                                                  fault_start_time_s=fault_start_time_s,
+                                                                  fault_start_time_e=fault_start_time_e,
+                                                                  fault_end_time_s=fault_end_time_s,
+                                                                  fault_end_time_e=fault_end_time_e,
+                                                                  fault_create_time_s=fault_create_time_s,
+                                                                  fault_create_time_e=fault_create_time_e, )
+
+            res = stub.GetFirstFaultV2(request, timeout=20000)
+
+            result_dataframe = res.output
+
+            if result_dataframe != '':
+                return pd.read_json(result_dataframe)
+            else:
+                return None
+
+        except Exception as e:
+            print(str(e))
+            print('云平台首发故障获取错误')
+            return None
+
 
 class WindFarmInf(object):
     # This programme is to get wind farm information.
     PROGRAMME = 'WindFarmInf'
     VERSION = '1.1.5'
 
     def __init__(self, sql_file='/tmp/1597716056484sqlite.sqlite',
@@ -1903,15 +1961,15 @@
                     return
             else:
                 print('请检查时间格式，例如：2021-03-03')
                 return
 
         start_time = start_time[:10] + ' 00:00:00'
         end_time = end_time[:10] + ' 23:59:59'
-        results=[]
+        results = []
         if isinstance(turbine, list):
             for tb in turbine:
                 docs = self.get_single_turbine(farm, tb, start_time, end_time, data_type)
                 results.extend(docs)
         if not turbine:
             docs = self.get_all_turbines(farm, start_time, end_time, data_type)
             results.extend(docs)
@@ -2056,24 +2114,24 @@
         else:
             c = columns
 
         for file in files:
             if file.endswith(".csv.gz"):
                 try:
                     with self.hdfs_client.read(file) as f:
-                       df = pd.read_csv(f, compression='gzip', engine='c', usecols=c)
-                       df = df.rename(columns=point_map)
+                        df = pd.read_csv(f, compression='gzip', engine='c', usecols=c)
+                        df = df.rename(columns=point_map)
                 except Exception as e:
-                       df = pd.DataFrame()
+                    df = pd.DataFrame()
 
             elif file.endswith(".csv"):
                 try:
                     with self.hdfs_client.read(file) as f:
-                       df = pd.read_csv(f, compression='infer', engine='c', usecols=c)
-                       df = df.rename(columns=point_map)
+                        df = pd.read_csv(f, compression='infer', engine='c', usecols=c)
+                        df = df.rename(columns=point_map)
                 except Exception as e:
                     df = pd.DataFrame()
             elif file.endswith(".parquet"):
                 try:
                     with self.pyarrow_client.open(file, "rb") as f:
                         df = pd.read_parquet(f, columns=c)
                         df = df.rename(columns=point_map)
@@ -2098,16 +2156,16 @@
         if isinstance(data_docs, dict):
             data_docs = [data_docs]
 
         bulk_data = list()
 
         for data_doc in data_docs:
             up_dict = {'_index': model_tag_index, '_op_type': 'update', "doc_as_upsert": True,
-                       '_id':'@'.join(['first_fault', data_doc['pinyin_code'],
-                                       data_doc['turbine_name'], data_doc['fault_start_time']])}
+                       '_id': '@'.join(['first_fault', data_doc['pinyin_code'],
+                                        data_doc['turbine_name'], data_doc['fault_start_time']])}
             data_doc = json.dumps(data_doc)
             data_doc = data_doc.replace('NaN', 'null')
             data_doc = json.loads(data_doc)
             up_dict['doc'] = data_doc
             bulk_data.append(up_dict)
 
         status = helpers.bulk(es, bulk_data)  # 正确插入后返回插入(更新)条数
@@ -2320,15 +2378,14 @@
             except Exception as e:
                 pass
         # es.clear_scroll(scroll_id=scroll_id)  # 清理游标
         return df_result
 
 
 class SanyLog(object):
-
     # This programme is print log to es or sentry.
     PROGRAMME = 'SanyLog'
     VERSION = '1.0.1'
 
     def __init__(self, project_name, project_version, author, set_level='work',
                  logstash_ip='logstash.sanywind.net', logstash_port=5651,
                  sentry_url='https://0bddde96d09f4a46aa67bd8977b9708f@platform.dc.sanywind.net:31119/6',
```

### Comparing `sanydata-3.3.1/sanydata/model_data_message_pb2_grpc.py` & `sanydata-3.3.2/sanydata/model_data_message_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
                 response_deserializer=model__data__message__pb2.GetModelResultResponse.FromString,
                 )
         self.GetFirstFault = channel.unary_unary(
                 '/ModelDataMessage/GetFirstFault',
                 request_serializer=model__data__message__pb2.GetFirstFaultRequest.SerializeToString,
                 response_deserializer=model__data__message__pb2.GetFirstFaultResponse.FromString,
                 )
+        self.GetFirstFaultV2 = channel.unary_unary(
+                '/ModelDataMessage/GetFirstFaultV2',
+                request_serializer=model__data__message__pb2.GetFirstFaultRequestV2.SerializeToString,
+                response_deserializer=model__data__message__pb2.GetFirstFaultResponse.FromString,
+                )
         self.GetDeployment = channel.unary_unary(
                 '/ModelDataMessage/GetDeployment',
                 request_serializer=model__data__message__pb2.GetDeploymentRequest.SerializeToString,
                 response_deserializer=model__data__message__pb2.GetDeploymentResponse.FromString,
                 )
 
 
@@ -147,14 +152,20 @@
 
     def GetFirstFault(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetFirstFaultV2(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetDeployment(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -211,14 +222,19 @@
                     response_serializer=model__data__message__pb2.GetModelResultResponse.SerializeToString,
             ),
             'GetFirstFault': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFirstFault,
                     request_deserializer=model__data__message__pb2.GetFirstFaultRequest.FromString,
                     response_serializer=model__data__message__pb2.GetFirstFaultResponse.SerializeToString,
             ),
+            'GetFirstFaultV2': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetFirstFaultV2,
+                    request_deserializer=model__data__message__pb2.GetFirstFaultRequestV2.FromString,
+                    response_serializer=model__data__message__pb2.GetFirstFaultResponse.SerializeToString,
+            ),
             'GetDeployment': grpc.unary_unary_rpc_method_handler(
                     servicer.GetDeployment,
                     request_deserializer=model__data__message__pb2.GetDeploymentRequest.FromString,
                     response_serializer=model__data__message__pb2.GetDeploymentResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -414,14 +430,31 @@
         return grpc.experimental.unary_unary(request, target, '/ModelDataMessage/GetFirstFault',
             model__data__message__pb2.GetFirstFaultRequest.SerializeToString,
             model__data__message__pb2.GetFirstFaultResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetFirstFaultV2(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ModelDataMessage/GetFirstFaultV2',
+            model__data__message__pb2.GetFirstFaultRequestV2.SerializeToString,
+            model__data__message__pb2.GetFirstFaultResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetDeployment(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `sanydata-3.3.1/setup.py` & `sanydata-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import importlib
 
 importlib.reload(sys)
 
 setup(
     name="sanydata",
-    version="3.3.1",
+    version="3.3.2",
     keywords=["pip", "sanydata", "thao"],
     description="get data and get wind farm information",
     long_description="get data and get wind farm information",
     license="MIT Licence",
 
     url="http://gitlab.sanywind.net/sanydata/sanydata",
     author="thao",
```

### Comparing `sanydata-3.3.1/utils/cos_handler.py` & `sanydata-3.3.2/utils/cos_handler.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.1/utils/file_operation.py` & `sanydata-3.3.2/utils/file_operation.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.1/utils/local_handler.py` & `sanydata-3.3.2/utils/local_handler.py`

 * *Files identical despite different names*

