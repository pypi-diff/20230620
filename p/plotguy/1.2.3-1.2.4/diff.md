# Comparing `tmp/plotguy-1.2.3.tar.gz` & `tmp/plotguy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.2.3.tar", last modified: Fri Jun  9 03:04:52 2023, max compression
+gzip compressed data, was "plotguy-1.2.4.tar", last modified: Tue Jun 20 03:49:06 2023, max compression
```

## Comparing `plotguy-1.2.3.tar` & `plotguy-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.730259 plotguy-1.2.3/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-09 03:04:52.730090 plotguy-1.2.3/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.3/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.729066 plotguy-1.2.3/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25651 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.3/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    65962 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    38129 2023-06-09 02:59:05.000000 plotguy-1.2.3/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.3/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-09 03:04:52.729898 plotguy-1.2.3/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-09 03:04:52.000000 plotguy-1.2.3/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-09 03:04:52.730313 plotguy-1.2.3/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-09 03:04:10.000000 plotguy-1.2.3/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.858642 plotguy-1.2.4/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-20 03:49:06.858485 plotguy-1.2.4/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.2.4/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.857545 plotguy-1.2.4/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    26203 2023-06-20 03:47:28.000000 plotguy-1.2.4/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 plotguy-1.2.4/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    65962 2023-06-09 02:59:05.000000 plotguy-1.2.4/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    38129 2023-06-13 02:24:31.000000 plotguy-1.2.4/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.2.4/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-20 03:49:06.858286 plotguy-1.2.4/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-20 03:49:06.000000 plotguy-1.2.4/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-20 03:49:06.858694 plotguy-1.2.4/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-20 03:48:00.000000 plotguy-1.2.4/setup.py
```

### Comparing `plotguy-1.2.3/plotguy/__init__.py` & `plotguy-1.2.4/plotguy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,18 @@
         para_combination['risk_free_rate'] = risk_free_rate
         cal_performance_list.append((para_combination, manager_list))
 
     pool = mp.Pool(processes=number_of_core)
     pool.map(mp_cal_performance, cal_performance_list)
     pool.close()
 
-    pd.DataFrame(list(manager_list)).to_csv('backtest_result.csv')
+    df_backtest_result = pd.DataFrame(list(manager_list))
+    df_backtest_result = df_backtest_result.sort_values(by='reference_index')
+    df_backtest_result.reset_index(drop=True)
+    df_backtest_result.to_csv('backtest_result.csv')
 
 
 def plot_signal_analysis(py_filename, output_folder, start_date, end_date, para_dict, signal_settings):
     app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath,
                           signal_settings)
 
     return app
@@ -308,14 +311,15 @@
 
     return num_of_trade, num_of_loss, num_of_win, win_rate, loss_rate
 
 
 def calculate_win_rate(df_csv):
     df = df_csv[['date', 'realized_pnl', 'action']].copy()
     df = df[df['action'].notnull()].reset_index(drop=True)
+    df = df.loc[df['action'] != '']  # for parquet
     df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
     df['pnl'] = df['realized_pnl'].shift(-1)
     df['year'] = pd.DatetimeIndex(df['date']).year
     year_list = list(set(df['year']))
     year_list.sort()
 
     win_rate_dict = {}
@@ -596,15 +600,23 @@
                 # print(e)
                 result_dict[str(year)] = 0
                 result_dict[f'{year}_win_rate'] = '--'
 
             year_count.append(result_dict[str(year)])
 
 
-        result_dict['cov_count'] = round(np.std(year_count) / np.mean(year_count), 3)
+        # result_dict['cov_count'] = round(np.std(year_count) / np.mean(year_count), 3)
+
+        std_dev = np.std(year_count)
+        mean = np.mean(year_count)
+
+        if std_dev != 0 and not np.isnan(std_dev) and mean != 0 and not np.isnan(mean):
+            result_dict['cov_count'] = round(std_dev / mean, 3)
+        else:
+            result_dict['cov_count'] = 0  # Assign a value indicating an invalid result
 
 
         # Performance by year
         first_equity_value = 0
         last_equity_value = 0
         year_return_list = []
         for year in year_list:
@@ -633,14 +645,17 @@
             cov_return = 0
         else:
             cov_return = round(return_year_std / return_year_mean, 3)
         result_dict['cov_return'] = cov_return
 
     result_dict['risk_free_rate'] = risk_free_rate
 
+
+
+
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
     bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharpe_ratio(df, 'close',
                                                                                          risk_free_rate)
     initial_capital = df.loc[df.index[0], 'equity_value']
     df['bah_equity_curve'] = df['close'] * initial_capital // df.loc[df.index[0], 'close']
     bah_mdd_pct, bah_mdd_dollar = calculate_mdd(df, 'bah_equity_curve')
```

### Comparing `plotguy-1.2.3/plotguy/aggregate.py` & `plotguy-1.2.4/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.3/plotguy/components.py` & `plotguy-1.2.4/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.3/plotguy/equity_curves.py` & `plotguy-1.2.4/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.3/plotguy/signals.py` & `plotguy-1.2.4/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.2.3/setup.py` & `plotguy-1.2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.2.3",
+    version="1.2.4",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
-        'pandas>=1.5.2',  
+        'pandas==1.5.3',  
         'numpy>=1.24.1',  
         'hkfdb>=2.2', 
         'pyarrow',
         'polars',
         'lxml',        
         'dash',
         'dash_bootstrap_components',
```

