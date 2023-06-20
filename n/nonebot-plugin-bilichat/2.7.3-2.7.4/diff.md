# Comparing `tmp/nonebot_plugin_bilichat-2.7.3.tar.gz` & `tmp/nonebot_plugin_bilichat-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.7.3.tar", last modified: Mon Jun 19 10:35:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.7.4.tar", last modified: Tue Jun 20 03:47:19 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.7.3.tar` & `nonebot_plugin_bilichat-2.7.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-06-19 10:35:28.958203 nonebot_plugin_bilichat-2.7.3/LICENSE
--rw-r--r--   0        0        0    13119 2023-06-19 10:35:28.958203 nonebot_plugin_bilichat-2.7.3/README.md
--rw-r--r--   0        0        0     9598 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5512 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16205 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7279 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1363 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-19 10:35:39.650212 nonebot_plugin_bilichat-2.7.3/pyproject.toml
--rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-20 03:47:09.348728 nonebot_plugin_bilichat-2.7.4/LICENSE
+-rw-r--r--   0        0        0    13120 2023-06-20 03:47:09.348728 nonebot_plugin_bilichat-2.7.4/README.md
+-rw-r--r--   0        0        0     9598 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5513 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16205 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-20 03:47:09.376730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7279 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1363 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-20 03:47:09.380730 nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-20 03:47:19.361150 nonebot_plugin_bilichat-2.7.4/pyproject.toml
+-rw-r--r--   0        0        0    14695 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.4/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.7.3/LICENSE` & `nonebot_plugin_bilichat-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/README.md` & `nonebot_plugin_bilichat-2.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_word_cloud  | bool | True | 是否开启词云功能 |
+| bilichat_word_cloud  | bool | False | 是否开启词云功能 |
 
 注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
 
 ### AI视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
```

#### html2text {}

```diff
@@ -67,15 +67,15 @@
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
 æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
 ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
 htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
 bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ |
+bilichat_word_cloud | bool | False | æ¯å¦å¼å¯è¯äºåè½ |
 æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
 åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
 AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
 plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
 -----:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
 newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
 åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
```

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     bilichat_basic_info_url: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
-    bilichat_word_cloud: bool = True
+    bilichat_word_cloud: bool = False
 
     # AI Summary
     bilichat_newbing_cookie: Optional[str]
     bilichat_newbing_token_limit: int = 0
     bilichat_newbing_preprocess: bool = True
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
```

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.7.4/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.3/pyproject.toml` & `nonebot_plugin_bilichat-2.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.7.3"
+version = "2.7.4"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.7.3/PKG-INFO` & `nonebot_plugin_bilichat-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.7.3
+Version: 2.7.4
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -225,15 +225,15 @@
 
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_word_cloud  | bool | True | 是否开启词云功能 |
+| bilichat_word_cloud  | bool | False | 是否开启词云功能 |
 
 注：词云功能在 python3.11 中由于 `wordcloud` 包安装失败暂时无法启用，请不要在 3.11 中开启此功能
 
 ### AI视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[openai,newbing]`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.4 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
@@ -90,15 +90,15 @@
 åç»­æ¶æ¯æ¯å¦åå¤åºç¡ä¿¡æ¯(å³é­ååå¤åéèçä¿¡æ¯) |
 æ³¨ï¼bilichat_basic_info_style é¤é»è®¤ç bbot_default ä½¿ç¨ PIL
 ç»å¾ï¼å¶ä»åä¾èµäº `nonebot-plugin-
 htmlrender`ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º  bbot_default ![](docs/
 bbot_default.png)   style_blue ![](docs/style_blue.png)  ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ |
+bilichat_word_cloud | bool | False | æ¯å¦å¼å¯è¯äºåè½ |
 æ³¨ï¼è¯äºåè½å¨ python3.11 ä¸­ç±äº `wordcloud`
 åå®è£å¤±è´¥ææ¶æ æ³å¯ç¨ï¼è¯·ä¸è¦å¨ 3.11 ä¸­å¼å¯æ­¤åè½ ###
 AIè§é¢æ»ç»éç½®é¡¹ å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-
 plugin-bilichat[openai,newbing]` | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:
 -----:|:----:|:----:|:----:| | bilichat_newbing_cookie | str | None |
 newbingçcookieæä»¶è·¯å¾, å¡«å `no_login`
 åä¸è¿è¡ç»å½ï¼å¯è½ææ¬¡æ°éå¶ï¼, è¥çç©ºåç¦ç¨newbingæ»ç»
```

