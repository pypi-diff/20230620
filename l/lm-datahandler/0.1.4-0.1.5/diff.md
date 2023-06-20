# Comparing `tmp/lm_datahandler-0.1.4.tar.gz` & `tmp/lm_datahandler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.4.tar", last modified: Mon Jun 19 08:11:56 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.5.tar", last modified: Mon Jun 19 09:31:12 2023, max compression
```

## Comparing `lm_datahandler-0.1.4.tar` & `lm_datahandler-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.552041 lm_datahandler-0.1.4/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      325 2023-06-19 08:11:56.551551 lm_datahandler-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.471544 lm_datahandler-0.1.4/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.4/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.488884 lm_datahandler-0.1.4/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-06-15 10:20:25.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.4/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24102 2023-06-19 08:08:17.000000 lm_datahandler-0.1.4/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.541721 lm_datahandler-0.1.4/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.4/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.4/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.4/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.4/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.4/lm_datahandler/functions/posture_analyse.py
--rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.4/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3240 2023-06-14 03:25:28.000000 lm_datahandler-0.1.4/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.4/lm_datahandler/functions/spindle_detect.py
--rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.4/lm_datahandler/functions/wear_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.542749 lm_datahandler-0.1.4/lm_datahandler/models/
--rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.4/lm_datahandler/models/wear_detection_1s.txt
--rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.4/lm_datahandler/models/wholenight_sleep_staging.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.548032 lm_datahandler-0.1.4/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.4/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.4/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     6390 2023-06-16 05:16:37.000000 lm_datahandler-0.1.4/lm_datahandler/plots/sleep_staging_plot.py
--rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.4/lm_datahandler/plots/stim_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.548231 lm_datahandler-0.1.4/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.4/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.4/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.550400 lm_datahandler-0.1.4/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.4/lm_datahandler/preprocess/tailor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.550935 lm_datahandler-0.1.4/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.4/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.4/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:11:56.487010 lm_datahandler-0.1.4/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 08:11:56.000000 lm_datahandler-0.1.4/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 08:11:56.552041 lm_datahandler-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-19 08:09:38.000000 lm_datahandler-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.220058 lm_datahandler-0.1.5/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-19 09:31:12.220058 lm_datahandler-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.191967 lm_datahandler-0.1.5/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.5/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.209140 lm_datahandler-0.1.5/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.5/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     2024 2023-06-15 10:20:25.000000 lm_datahandler-0.1.5/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.5/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24236 2023-06-19 09:16:14.000000 lm_datahandler-0.1.5/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.213737 lm_datahandler-0.1.5/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.5/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    31179 2023-06-14 03:24:58.000000 lm_datahandler-0.1.5/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.5/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.5/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.5/lm_datahandler/functions/posture_analyse.py
+-rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.5/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.5/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.5/lm_datahandler/functions/spindle_detect.py
+-rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.5/lm_datahandler/functions/wear_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.214508 lm_datahandler-0.1.5/lm_datahandler/models/
+-rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.5/lm_datahandler/models/wear_detection_1s.txt
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.5/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.216375 lm_datahandler-0.1.5/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.5/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.5/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.5/lm_datahandler/plots/sleep_staging_plot.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.5/lm_datahandler/plots/stim_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.216994 lm_datahandler-0.1.5/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.5/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.5/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.218111 lm_datahandler-0.1.5/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.5/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.5/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.5/lm_datahandler/preprocess/tailor.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.219637 lm_datahandler-0.1.5/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.5/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.5/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:31:12.207496 lm_datahandler-0.1.5/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-19 09:31:12.000000 lm_datahandler-0.1.5/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-06-19 09:31:12.000000 lm_datahandler-0.1.5/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:31:12.000000 lm_datahandler-0.1.5/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-19 09:31:12.000000 lm_datahandler-0.1.5/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 09:31:12.000000 lm_datahandler-0.1.5/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:31:12.220918 lm_datahandler-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-19 09:31:09.000000 lm_datahandler-0.1.5/setup.py
```

### Comparing `lm_datahandler-0.1.4/LICENSE` & `lm_datahandler-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.5/lm_datahandler/data_load/data_loader.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.5/lm_datahandler/data_load/loaders.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.5/lm_datahandler/datahandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,21 +275,24 @@
         sl = sl_compute(self.sleep_staging_result, self.epoch_len)
         if sl == -1:
             self.logger.info("No continuous sleep epochs are detected!")
             se = 0.0
             arousal_time = np.asarray([])
             arousal_count = 0
             waso = 0
+            gu = -1
         else:
+            gu = get_up_time_compute(self.sleep_staging_result, self.epoch_len)
             se = se_compute(self.sleep_staging_result)
-            arousal_count, arousal_time = arousal_time_compute(self.sleep_staging_result, self.epoch_len)
+            arousal_count, arousal_time = arousal_time_compute(self.sleep_staging_result, self.epoch_len, sleep_range=[sl, gu])
             waso = arousal_time.shape[0] * self.epoch_len
         self.sleep_variables = {
             "TST": tst,
             "SOL": sl,
+            "GU": gu,
             "WASO": waso,
             "SE": se,
             "AR": arousal_count,
             "ART": arousal_time
         }
         print("TST:\t{} s\nSOL:\t{} s\nSE:\t\t{}%\nWASO:\t{} s\nAR:\t\t{}".format(tst, sl, se * 100, waso, arousal_count))
 
@@ -486,14 +489,14 @@
 
     def show_plots(self):
         plt.show()
 
 
 if __name__ == '__main__':
     data_handler = DataHandler()
-    data_handler.load_data(data_name="20230614_15927226341", data_path=r"E:\dataset\dev_test_data\20230614_15927226341")
+    data_handler.load_data(data_name="20230401_ZX", data_path=r"E:\dataset\x7_new\matlab_data\20230401_ZX")
 
     data_handler.plot_sw_stim_sham()
     data_handler.preprocess().sleep_staging().compute_sleep_variables().plot_sleep_data()
 
     data_handler.show_plots()
```

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/biomarker.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/feature_extract.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/posture_analyse.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/posture_analyse.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/sleep_staging.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,46 +25,63 @@
     :param epoch_length: seconds per epoch
     :return sl: sleep latency
     """
     index = -1
     copy = hypno.copy()
     copy[hypno >= 3] = 1
     copy[hypno < 3] = 0
+
     for i in range(hypno.shape[0] - 30 * 4):
         score = np.sum(copy[i:i + 30 * 4])
         if score < 3 * 4:
             index = i
             break
 
     while index < hypno.shape[0] - 5 * 4 and np.sum(copy[index:index + 5 * 4]) > 0:
         index += 1
 
     return -1 if index < 0 else index * epoch_length
 
 
-def waso_compute(hypno, epoch_length):
+def get_up_time_compute(hypno, epoch_length):
+    copy = hypno.copy()
+    copy = np.asarray(copy).tolist()
+    copy.reverse()
+
+    index = sl_compute(np.asarray(copy), epoch_length)
+
+
+    return -1 if index < 0 else index
+
+
+def waso_compute(hypno, epoch_length, sleep_range=None):
     """
     :param hypno: sleep stage
     :param epoch_length: seconds per epoch
     :return: waso: awake time during sleep
     """
-    copy = hypno.copy()
-    hypno_smooth = pp_label_smooth(copy, window=10)
-    sleep_time = np.where(hypno_smooth < 3)[0]
-    first_sleep_time = sl_compute(hypno, epoch_length)
-    if first_sleep_time == -1:
-        return -1
-    first_sleep_time = int(first_sleep_time / epoch_length)
-    last_sleep_time = sleep_time[-1]
+
+    if sleep_range is None:
+        first_sleep_time = sl_compute(hypno, epoch_length)
+        if first_sleep_time == -1:
+            return -1
+        last_sleep_time = get_up_time_compute(hypno, epoch_length)
+    else:
+        first_sleep_time = sleep_range[0]
+        first_sleep_time = int(first_sleep_time / epoch_length)
+        last_sleep_time = sleep_range[1]
+        last_sleep_time = int(last_sleep_time / epoch_length)
+
     sleep_hypno = hypno[first_sleep_time:last_sleep_time]
     sleep_hypno = sleep_hypno.copy()
     sleep_hypno = pp_label_smooth(sleep_hypno, window=5)
     sleep_hypno[sleep_hypno < 3] = 0
     sleep_hypno[sleep_hypno == 3] = 1
     arousal_time = np.sum(sleep_hypno)
+
     return arousal_time * epoch_length
 
 
 def se_compute(hypno):
     """
     :param hypno: sleep stage
     :return: se: sleep efficiency
@@ -73,27 +90,35 @@
     is_sleep = np.zeros(hypno.shape)
     is_sleep[copy < 3] = 1
     sleep_epoch_count = np.sum(is_sleep)
 
     return sleep_epoch_count / hypno.shape[0]
 
 
-def arousal_time_compute(hypno, epoch_length):
+def arousal_time_compute(hypno, epoch_length, sleep_range=None):
     """
     :param hypno: sleep stage
     :return: arousal_time: awake time during sleep
     """
-    copy = hypno.copy()
+    copy = np.copy(hypno)
     hypno_smooth = pp_label_smooth(copy, window=5)
-    sleep_time = np.where(hypno_smooth < 3)[0]
-    first_sleep_time = sl_compute(hypno, epoch_length)
-    if first_sleep_time == -1:
-        return -1
+
+
+    if sleep_range is None:
+        first_sleep_time = sl_compute(hypno, epoch_length)
+        if first_sleep_time == -1:
+            return -1
+        last_sleep_time = get_up_time_compute(hypno, epoch_length)
+    else:
+        first_sleep_time = sleep_range[0]
+        last_sleep_time = sleep_range[1]
     first_sleep_time = int(first_sleep_time / epoch_length)
-    last_sleep_time = sleep_time[-1]
+
+    last_sleep_time = len(hypno) - int(last_sleep_time / epoch_length)
+
     sleep_hypno = hypno_smooth[first_sleep_time:last_sleep_time]
     sleep_hypno = sleep_hypno.copy()
     sleep_hypno[sleep_hypno < 3] = 0
     sleep_hypno[sleep_hypno == 3] = 1
     arousal_count = sleep_hypno[1:] - sleep_hypno[0:-1]
     arousal_count = np.where(arousal_count == 1)[0]
     arousal_time = np.where(sleep_hypno == 1)[0]
```

### Comparing `lm_datahandler-0.1.4/lm_datahandler/functions/wear_detect.py` & `lm_datahandler-0.1.5/lm_datahandler/functions/wear_detect.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/models/wear_detection_1s.txt` & `lm_datahandler-0.1.5/lm_datahandler/models/wear_detection_1s.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/models/wholenight_sleep_staging.txt` & `lm_datahandler-0.1.5/lm_datahandler/models/wholenight_sleep_staging.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.5/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.5/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,21 +63,21 @@
     ax.set_ylabel("Avg Diff ACC", fontdict={"fontsize": 16})
     ax.set_xlabel("Time [hrs]", fontdict={"fontsize": 16})
     return fig, ax
 
 
 def plot_sleep_posture(fig, ax, grade, sf=50):
     # assert grade.shape[0] == 1, "The grade of head bias should be a 1-D ndarray"
-    t = np.arange(grade.shape[0])/sf/3600
+    t = np.arange(grade.shape[0]) / sf / 3600
     ax.plot(t, grade, lw=1.5, color='b')
     ax.set_xlim(0, t.max())
     ax.set_ylim(-3.5, 3.5)
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
-    ax.set_yticks([-np.pi, -np.pi/2, 0, np.pi/2, np.pi])
+    ax.set_yticks([-np.pi, -np.pi / 2, 0, np.pi / 2, np.pi])
     ax.set_yticklabels(['Sleep Face Down', 'Lie on the Left', 'Lie Flat', 'Lie on the Right', 'Sleep Face Down'], )
     ax.set_ylabel("Sleep Postures", fontdict={"fontsize": 16})
     ax.set_xlabel("Time [hrs]", fontdict={"fontsize": 16})
     ax.grid(visible=True, axis='y', linewidth=0.5)
     return fig, ax
 
 
@@ -88,34 +88,43 @@
     deep_sleep = np.ma.masked_not_equal(hypno, 0)
     light_sleep = np.ma.masked_not_equal(hypno, 1)
     rem_sleep = np.ma.masked_not_equal(hypno, 2)
     wake = np.ma.masked_not_equal(hypno, 3)
     abnormal = np.ma.masked_not_equal(hypno, 4)
     if sleep_variables is not None:
         sl = sleep_variables["SOL"]
+        gu = max(t) * 3600 - sleep_variables["GU"]
         arousal_time = sleep_variables["ART"]
         if sl > 0:
-            ax.axvline(x=sl/3600, color="r", lw=1, linestyle='--')
-            ax.text(sl/3600, 4.2, 'SL', fontsize=16, color='r', ha='left', va='bottom')
-            ax.axvspan(0, sl/3600, color='gray', alpha=0.5)
+            ax.axvline(x=sl / 3600, color="r", lw=1, linestyle='--')
+            ax.text(sl / 3600, 4.2, 'SL', fontsize=16, color='r', ha='left', va='bottom')
+            ax.axvspan(0, sl / 3600, color='gray', alpha=0.5)
+
+        if gu > 0:
+            ax.axvline(x=gu / 3600, color="r", lw=1, linestyle='--')
+            # ax.text(sl / 3600, 4.2, 'SL', fontsize=16, color='r', ha='left', va='bottom')
+            ax.axvspan(gu / 3600, max(t), color='gray', alpha=0.5)
+
         if arousal_time.shape[0] > 0:
             arousal_time = np.asarray(arousal_time)
             b = np.insert(arousal_time, 0, 0)
             diff = b[1:] - b[:-1]
             c = arousal_time[np.where(diff != 1)[0]]
             d = np.append(arousal_time, 0)
             diff = d[1:] - d[:-1]
             e = arousal_time[np.where(diff != 1)[0]]
             boundaries = np.transpose(np.vstack([c, e]))
             for i in range(boundaries.shape[0]):
                 # ax.axvline(x=boundaries[i][0]*win/3600, color="r", lw=1, linestyle='--')
                 # ax.axvline(x=boundaries[i][1]*win/3600, color="r", lw=1, linestyle='--')
                 # ax.text(boundaries[i][1]*win/3600, 4.2, 'Arousal {}'.format(i), fontsize=12, color='r', ha='center', va='bottom')
-                ax.axvspan(boundaries[i][0]*win/3600, boundaries[i][1]*win/3600, color='gray', alpha=0.5)
-            ax.text(t.max()*0.98, 4.2, "Arousals: {}s in {} times".format(arousal_time.shape[0]*win, boundaries.shape[0]), fontsize=12, color='r', ha='right', va='bottom')
+                ax.axvspan(boundaries[i][0] * win / 3600, boundaries[i][1] * win / 3600, color='gray', alpha=0.5)
+            ax.text(t.max() * 0.98, 4.2,
+                    "Arousals: {}s in {} times".format(arousal_time.shape[0] * win, boundaries.shape[0]), fontsize=12,
+                    color='r', ha='right', va='bottom')
     ax.step(t, hypno, lw=2, color='k')
     ax.step(t, abnormal, lw=2, color='k')
     ax.step(t, wake, lw=2, color='orange')
     ax.step(t, rem_sleep, lw=2, color='lime')
     ax.step(t, light_sleep, lw=2, color='deepskyblue', )
     ax.step(t, deep_sleep, lw=2, color='royalblue')
 
@@ -124,9 +133,8 @@
     ax.set_yticks([0, 1, 2, 3, 4])
     ax.set_yticklabels(['Deep Sleep', 'Light Sleep', 'REM Sleep', 'Wake', 'Abnormal'], )
     ax.tick_params(axis='y', labelsize=12)
     ax.tick_params(axis='x', labelsize=12)
     ax.set_ylabel("Sleep Staging Result", fontdict={"fontsize": 16})
     ax.set_xlabel("Time [hrs]", fontdict={"fontsize": 16})
 
-
     return fig, ax
```

### Comparing `lm_datahandler-0.1.4/lm_datahandler/plots/stim_plot.py` & `lm_datahandler-0.1.5/lm_datahandler/plots/stim_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.5/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/preprocess/filter.py` & `lm_datahandler-0.1.5/lm_datahandler/preprocess/filter.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.5/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.5/lm_datahandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.4/setup.py` & `lm_datahandler-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.4',
+    version = '0.1.5',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

