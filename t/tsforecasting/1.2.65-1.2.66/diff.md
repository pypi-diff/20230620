# Comparing `tmp/tsforecasting-1.2.65-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.66-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18593 bytes, number of entries: 12
+Zip file size: 18592 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      393 b- defN 23-Feb-21 11:35 tsforecasting/__init__.py
 -rw-rw-rw-  2.0 fat    10033 b- defN 23-Apr-17 15:36 tsforecasting/tsf_data_eng.py
--rw-rw-rw-  2.0 fat    10134 b- defN 23-Apr-17 16:08 tsforecasting/tsf_expanding_window.py
+-rw-rw-rw-  2.0 fat    10138 b- defN 23-Jun-20 17:28 tsforecasting/tsf_expanding_window.py
 -rw-rw-rw-  2.0 fat     1684 b- defN 23-Mar-02 11:05 tsforecasting/tsf_model_configs.py
 -rw-rw-rw-  2.0 fat     4009 b- defN 23-Apr-17 15:43 tsforecasting/tsf_model_selection.py
 -rw-rw-rw-  2.0 fat     7891 b- defN 23-Apr-17 15:44 tsforecasting/tsf_performance.py
 -rw-rw-rw-  2.0 fat     8385 b- defN 23-May-27 21:19 tsforecasting/tsf_predictions.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11121 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1047 b- defN 23-May-27 21:24 tsforecasting-1.2.65.dist-info/RECORD
-12 files, 55881 bytes uncompressed, 16821 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1078 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11121 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-20 17:32 tsforecasting-1.2.66.dist-info/RECORD
+12 files, 55885 bytes uncompressed, 16820 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tsforecasting/tsf_performance.py
 Comment: 
 
 Filename: tsforecasting/tsf_predictions.py
 Comment: 
 
-Filename: tsforecasting-1.2.65.dist-info/LICENSE
+Filename: tsforecasting-1.2.66.dist-info/LICENSE
 Comment: 
 
-Filename: tsforecasting-1.2.65.dist-info/METADATA
+Filename: tsforecasting-1.2.66.dist-info/METADATA
 Comment: 
 
-Filename: tsforecasting-1.2.65.dist-info/WHEEL
+Filename: tsforecasting-1.2.66.dist-info/WHEEL
 Comment: 
 
-Filename: tsforecasting-1.2.65.dist-info/top_level.txt
+Filename: tsforecasting-1.2.66.dist-info/top_level.txt
 Comment: 
 
-Filename: tsforecasting-1.2.65.dist-info/RECORD
+Filename: tsforecasting-1.2.66.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsforecasting/tsf_expanding_window.py

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import sys
 import datetime
-from sklearn.preprocessing import MinMaxScaler
+from sklearn.preprocessing import StandardScaler
 from prophet import Prophet
 from pmdarima.arima import auto_arima
 from .tsf_model_selection import model_prediction
 from .tsf_data_eng import slice_timestamp, engin_date, multivariable_lag
 from .tsf_model_configs import model_configurations
 
 h_parameters=model_configurations()
@@ -211,15 +211,15 @@
             print('Rows Test:', len(test))
             
             train[[target]]=train[[target]].astype('int32')
             
             input_cols=list(train.columns)
             input_cols.remove(target)
 
-            scaler = MinMaxScaler() 
+            scaler = StandardScaler() 
 
             scaler = scaler.fit(train[input_cols])
             train[input_cols] = scaler.transform(train[input_cols])
             test[input_cols] = scaler.transform(test[input_cols])            
 
             y_pred=model_prediction(train, test,target,model_configs=model_configs,algo=algo)
             y_pred=y_pred[0:forecast_length]
```

## Comparing `tsforecasting-1.2.65.dist-info/LICENSE` & `tsforecasting-1.2.66.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.65.dist-info/METADATA` & `tsforecasting-1.2.66.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.65
+Version: 1.2.66
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
```

