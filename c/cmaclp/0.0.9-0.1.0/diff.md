# Comparing `tmp/cmaclp-0.0.9-py3-none-any.whl.zip` & `tmp/cmaclp-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11913 bytes, number of entries: 8
--rw-r--r--  2.0 unx    21604 b- defN 23-Jun-14 16:22 cmaclp/SVM_prediction.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 16:22 cmaclp/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      755 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx      164 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      629 b- defN 23-Jun-14 16:25 cmaclp-0.0.9.dist-info/RECORD
-8 files, 34608 bytes uncompressed, 10813 bytes compressed:  68.8%
+Zip file size: 12231 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    22149 b- defN 23-Jun-20 14:01 cmaclp/SVM_prediction.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 14:01 cmaclp/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1178 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      630 b- defN 23-Jun-20 14:03 cmaclp-0.1.0.dist-info/RECORD
+8 files, 35577 bytes uncompressed, 11131 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: cmaclp/SVM_prediction.py
 Comment: 
 
 Filename: cmaclp/__init__.py
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/LICENSE
+Filename: cmaclp-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/METADATA
+Filename: cmaclp-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/WHEEL
+Filename: cmaclp-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/entry_points.txt
+Filename: cmaclp-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/top_level.txt
+Filename: cmaclp-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmaclp-0.0.9.dist-info/RECORD
+Filename: cmaclp-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmaclp/SVM_prediction.py

```diff
@@ -1,23 +1,24 @@
 import argparse
 import os
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import time as tm
 import seaborn as sns
-import rpy2.robjects as robjects
 import matplotlib
 import matplotlib.pyplot as plt
 from sklearn.svm import LinearSVC
 from sklearn.calibration import CalibratedClassifierCV
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from sklearn.metrics import f1_score
+from sklearn.metrics import accuracy_score
+from sklearn.metrics import precision_score
 from scanpy import read_h5ad
 from importlib.resources import files
 
 def SVM_prediction(reference_H5AD, query_H5AD, LabelsPathTrain, OutputDir, rejected=False, Threshold_rej=0.7,meta_atlas=False):
     '''
     run baseline classifier: SVM
     Wrapper script to run an SVM classifier with a linear kernel on a benchmark dataset with 5-fold cross validation,
@@ -332,36 +333,29 @@
     OutputDir : Output directory defining the path of the exported SVM_predictions.
     SVM_type: Type of SVM prediction, SVM or SVMrej (default).
     '''
 
     print("Reading in the data")
     Data=read_h5ad(reference_H5AD)
 
-    Data = pd.DataFrame.sparse.from_spmatrix(Data.X, index=list(Data.obs.index.values), columns=list(Data.var.index.values))
+    data = pd.DataFrame.sparse.from_spmatrix(Data.X, index=list(Data.obs.index.values), columns=list(Data.var.index.values))
 
     labels = pd.read_csv(LabelsPath, header=0,index_col=None, sep=',') #, usecols = col
 
-    # read the data
-    data = Data
-
     # Convert the ordered dataframes back to nparrays
     print("Normalising the data")
-    data = data.to_numpy()
-    data = np.log1p(data)
+    data = data.to_numpy(dtype="float16")
+    np.log1p(data,out=data)
 
     X = data
-    y = labels["x"].to_list()
+    del data
 
     label_encoder = LabelEncoder()
-
-    # Fit the LabelEncoder to the categorical list
-    label_encoder.fit(y)
-
-    # Convert the categorical list to numerical categories
-    y = label_encoder.transform(y)
+    
+    y = label_encoder.fit_transform(labels["x"].tolist())
 
     # Generate a dictionary to map values to strings
     res = dict(zip(label_encoder.inverse_transform(y),y))
     res['Unlabeled'] = 999999
     res = {v: k for k, v in res.items()}
     res
 
@@ -374,33 +368,38 @@
     # Iterate over each fold and split the data
     print("Generate indices for train and test")
     for train_index, test_index in kfold.split(X):
         #X_train, X_test = X[train_index], X[test_index]
         y_train, y_test = y[train_index], y[test_index]
 
         # Store the indices of the training and test sets for each fold
-        train_indices.append(train_index)
-        test_indices.append(test_index)
+        train_indices.append(list(train_index))
+        test_indices.append(list(test_index))
+        
+    #train_indices = list(train_indices)
+    #test_indices = list(test_indices)
 
     # Run the SVM model
     test_ind=test_indices
     train_ind=train_indices
     Classifier = LinearSVC()
+
     if SVM_type == "SVMrej":
         clf = CalibratedClassifierCV(Classifier, cv=3)
 
     tr_time=[]
     ts_time=[]
     truelab = []
     pred = []
+    prob_full = []
 
     for i in range(fold_splits):
         print(f"Running cross-val {i}")
-        train=data[train_ind[i]]
-        test=data[test_ind[i]]
+        train=X[train_ind[i]] # was data
+        test=X[test_ind[i]] # was data
         y_train=y[train_ind[i]]
         y_test=y[test_ind[i]]
 
         if SVM_type == "SVMrej":
             start=tm.time()
             clf.fit(train, y_train.ravel()) #.values
             tr_time.append(tm.time()-start)
@@ -410,14 +409,15 @@
             prob = np.max(clf.predict_proba(test), axis = 1)
 
             unlabeled = np.where(prob < float(Threshold))
             unlabeled=list(unlabeled[0])
             predicted[unlabeled] = 999999 # set arbitrary value to convert it back to a string in the end
             ts_time.append(tm.time()-start)
             pred.extend(predicted)
+            prob_full.extend(prob)
 
         if SVM_type == "SVM":
             start=tm.time()
             Classifier.fit(train, y_train.ravel())
             tr_time.append(tm.time()-start)
 
             start=tm.time()
@@ -431,22 +431,30 @@
 
     truelab = pd.DataFrame(truelab)
     pred = pd.DataFrame(pred)
 
     tr_time = pd.DataFrame(tr_time)
     ts_time = pd.DataFrame(ts_time)
 
+    # Calculating the weighted F1 score:
+    F1score= f1_score(truelab[0].to_list(), pred[0].to_list(), average='weighted')
+    print(f"The {SVM_type} model ran with the weighted F1 score of: {F1score}")
+
+    # Calculating the weighted accuracy score:
+    acc_score = accuracy_score(truelab[0].to_list(), pred[0].to_list())
+    print(f"The {SVM_type} model ran with the weighted accuracy score of: {acc_score}")
+
+    # Calculating the weighted precision score:
+    prec_score = precision_score(truelab[0].to_list(),  pred[0].to_list(),average="weighted")
+    print(f"The {SVM_type} model ran with the weighted precision score of: {prec_score}")
+
     # Relabel truelab and predicted values by names
     truelab[0]=truelab[0].replace(res)
     pred[0]=pred[0].replace(res)
 
-    # Calculating the median F1 score:
-    F1score= f1_score(truelab[0].to_list(), pred[0].to_list(), average='weighted')
-    print(f"The {SVM_type} model ran with the median weighted F1 score of: {F1score}")
-
     print("Saving labels to specified output directory")
     truelab.to_csv(f"{OutputDir}{SVM_type}_True_Labels.csv", index = False)
     pred.to_csv(f"{OutputDir}{SVM_type}_Pred_Labels.csv", index = False)
     tr_time.to_csv(f"{OutputDir}{SVM_type}_Training_Time.csv", index = False)
     ts_time.to_csv(f"{OutputDir}{SVM_type}_Testing_Time.csv", index = False)
 
     ## Plot the SVM figures
@@ -468,15 +476,15 @@
     cnf_matrix = cnf_matrix.sort_index(axis=1)
     cnf_matrix = cnf_matrix.sort_index()
 
     # Plot png
     sns.set(font_scale=0.8)
     cm = sns.clustermap(cnf_matrix.T, cmap="Blues", annot=True,fmt='.2%', row_cluster=False,col_cluster=False)
     cm.savefig(f"figures/{SVM_type}_cnf_matrix.png")
-    return
+    return F1score,acc_score,prec_score
 
 
 def predpars():
     # Create the parser
     parser = argparse.ArgumentParser(description='Run SVM prediction')
 
     # Add arguments
```

## Comparing `cmaclp-0.0.9.dist-info/LICENSE` & `cmaclp-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

