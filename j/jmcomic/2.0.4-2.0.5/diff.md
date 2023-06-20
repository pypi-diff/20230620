# Comparing `tmp/jmcomic-2.0.4.tar.gz` & `tmp/jmcomic-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-1esw4jd9/jmcomic-2.0.4.tar", last modified: Mon Jun  5 08:06:15 2023, max compression
+gzip compressed data, was "jmcomic-2.0.5.tar", last modified: Tue Jun 20 07:54:42 2023, max compression
```

## Comparing `jmcomic-2.0.4.tar` & `jmcomic-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-05 08:06:06.000000 jmcomic-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-05 08:06:15.000000 jmcomic-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-05 08:06:06.000000 jmcomic-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:06:15.000000 jmcomic-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-05 08:06:06.000000 jmcomic-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-05 08:06:06.000000 jmcomic-2.0.4/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 08:06:15.000000 jmcomic-2.0.4/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 07:54:30.000000 jmcomic-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-20 07:54:42.889842 jmcomic-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-20 07:54:30.000000 jmcomic-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:54:42.889842 jmcomic-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 07:54:30.000000 jmcomic-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jmcomic-2.0.4/LICENSE` & `jmcomic-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.4/PKG-INFO` & `jmcomic-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.4/README.md` & `jmcomic-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.4/setup.py` & `jmcomic-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.4/src/jmcomic/api.py` & `jmcomic-2.0.5/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.5/src/jmcomic/jm_client_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,26 +109,26 @@
 
         # 请求
         resp = self.get_jm_html(f"/album/{album_id}")
 
         # 用 JmcomicText 解析 html，返回实体类
         return JmcomicText.analyse_jm_album_html(resp.text)
 
-    def get_photo_detail(self, photo_id: str, album=True) -> JmPhotoDetail:
+    def get_photo_detail(self, photo_id, fetch_album=True) -> JmPhotoDetail:
         # 参数校验
         photo_id = JmcomicText.parse_to_photo_id(photo_id)
 
         # 请求
         resp = self.get_jm_html(f"/photo/{photo_id}")
 
         # 用 JmcomicText 解析 html，返回实体类
         photo_detail = JmcomicText.analyse_jm_photo_html(resp.text)
 
         # 一并获取该章节的所处本子
-        if album is True:
+        if fetch_album is True:
             photo_detail.from_album = self.get_album_detail(photo_detail.album_id)
 
         return photo_detail
 
     def ensure_photo_can_use(self, photo_detail: JmPhotoDetail):
         # 检查 from_album
         if photo_detail.from_album is None:
```

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.5/src/jmcomic/jm_client_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 
 class JmDetailClient:
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         raise NotImplementedError
 
-    def get_photo_detail(self, photo_id: str, album=True) -> JmPhotoDetail:
+    def get_photo_detail(self, photo_id, fetch_album=True) -> JmPhotoDetail:
         raise NotImplementedError
 
     def ensure_photo_can_use(self, photo_detail: JmPhotoDetail):
         raise NotImplementedError
 
     def search_album(self, search_query, main_tag=0) -> Union[JmSearchPage, JmAlbumDetail]:
         raise NotImplementedError
@@ -206,8 +206,12 @@
 
 class JmcomicClient(
     JmImageClient,
     JmDetailClient,
     JmUserClient,
     Postman,
 ):
-    pass
+    def get_jmcomic_url(self, postman=None):
+        return JmModuleConfig.get_jmcomic_url(postman or self)
+
+    def get_jmcomic_domain_all(self, postman=None):
+        return JmModuleConfig.get_jmcomic_domain_all(postman or self)
```

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_config.py` & `jmcomic-2.0.5/src/jmcomic/jm_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
     DOMAIN = None
     JM_REDIRECT_URL = f'{PROT}jm365.xyz/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
-    JM_PUB_URL = f'{PROT}jmcomic1.bet'
+    JM_PUB_URL = f'{PROT}jmcomic2.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
     JM_IMAGE_SUFFIX = ['.jpg', '.webp', '.png', '.gif']
 
     # 访问JM可能会遇到的异常网页
     JM_ERROR_RESPONSE_TEXT = {
         "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
         "Restricted Access!": "禁漫拒绝你所在ip地区的访问，你可以选择: 换域名/换代理",
@@ -88,15 +88,15 @@
     def get_jmcomic_url(cls, postman=None):
         """
         访问禁漫的永久网域，从而得到一个可用的禁漫网址
         @return: https://jm-comic2.cc
         """
         if postman is None:
             from common import Postmans
-            postman = Postmans.get_impl_clazz('cffi_Session').create()
+            postman = Postmans.new_session()
 
         resp = postman.get(cls.JM_REDIRECT_URL)
         url = resp.url
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
         return url
 
     @classmethod
```

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_entity.py` & `jmcomic-2.0.5/src/jmcomic/jm_entity.py`

 * *Files 9% similar despite different names*

```diff
@@ -200,14 +200,17 @@
     @property
     def id(self):
         return self.photo_id
 
     def __len__(self):
         return len(self.page_arr)
 
+    def __iter__(self) -> Generator[JmImageDetail, Any, None]:
+        return super().__iter__()
+
 
 class JmAlbumDetail(WorkEntity):
 
     def __init__(self,
                  album_id,
                  scramble_id,
                  title,
@@ -293,14 +296,17 @@
 
         for episode in episode_list:
             if not_exist(episode):
                 ret.append(episode)
 
         return ret
 
+    def __iter__(self) -> Generator[JmPhotoDetail, Any, None]:
+        return super().__iter__()
+
 
 class JmSearchPage(IterableEntity):
 
     def __init__(self, album_info_list):
         # (album_id, title, category_none, label_sub_none, tag_list)
         self.album_info_list: List[Tuple[str, str, StrNone, StrNone, List[str]]] = album_info_list
```

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_option.py` & `jmcomic-2.0.5/src/jmcomic/jm_option.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,10 @@
 from .jm_client_impl import *
 
 
-class JmOptionAdvice:
-
-    def decide_image_save_dir(self,
-                              option: 'JmOption',
-                              photo_detail: JmPhotoDetail,
-                              ) -> StrNone:
-        """
-        决定一个本子图片的下载文件夹
-        @param option: JmOption对象
-        @param photo_detail: 本子章节实体类
-        @return: 下载文件夹，为空表示不处理
-        """
-        pass
-
-    def decide_image_filepath(self,
-                              option: 'JmOption',
-                              photo_detail: JmPhotoDetail,
-                              index: int,
-                              ) -> StrNone:
-        """
-        决定一个本子图片的绝对路径
-        @param option: JmOption对象
-        @param photo_detail: 本子章节实体类
-        @param index: 本子章节里的第几章图片
-        @return: 下载绝对路径，为空表示不处理
-        """
-        pass
-
-    def decide_image_suffix(self,
-                            option: 'JmOption',
-                            img_detail: JmImageDetail,
-                            ) -> StrNone:
-        """
-        决定一个图片的保存后缀名
-        @param option: JmOption对象
-        @param img_detail: 禁漫图片实体类
-        @return: 保存后缀名，为空表示不处理
-        """
-        pass
-
-
-class JmAdviceRegistry:
-    advice_registration: Dict[Any, List[JmOptionAdvice]] = {}
-
-    @classmethod
-    def register_advice(cls, base, *advice):
-        advice_ls = cls.advice_registration.get(base, None)
-
-        if advice_ls is None:
-            advice_ls = list(advice)
-            cls.advice_registration[base] = advice_ls
-        else:
-            for e in advice:
-                advice_ls.append(e)
-
-        return advice
-
-    @classmethod
-    def get_advice(cls, base) -> List[JmOptionAdvice]:
-        return cls.advice_registration.setdefault(base, [])
-
-
 class DirRule:
     rule_sample = [
         # 根目录 / Album-id / Photo-序号 /
         'Bd_Aid_Pindex',  # 禁漫网站的默认下载方式
         # 根目录 / Album-作者 / Album-标题 / Photo-序号 /
         'Bd_Aauthor_Atitle_Pindex',
         # 根目录 / Photo-序号&标题 /
@@ -201,65 +139,40 @@
         return self.download.image.suffix
 
     """
     下面是决定图片保存路径的方法
     """
 
     def decide_image_save_dir(self, photo_detail) -> str:
-        # 先检查advice的回调，如果回调支持，则优先使用回调
-        for advice in JmAdviceRegistry.get_advice(self):
-            save_dir = advice.decide_image_save_dir(self, photo_detail)
-            if save_dir is not None:
-                return save_dir
-
         # 使用 self.dir_rule 决定 save_dir
         save_dir = self.dir_rule.deside_image_save_dir(
             photo_detail.from_album,
             photo_detail
         )
 
         mkdir_if_not_exists(save_dir)
         return save_dir
 
     def decide_image_suffix(self, img_detail: JmImageDetail):
-        # 先检查advice的回调，如果回调支持，则优先使用回调
-        for advice in JmAdviceRegistry.get_advice(self):
-            suffix = advice.decide_image_suffix(self, img_detail)
-            if suffix is not None:
-                return suffix
-
         # 动图则使用原后缀
         suffix = img_detail.img_file_suffix
         if suffix.endswith("gif"):
             return suffix
 
         # 非动图，以配置为先
         return self.download_image_suffix or suffix
 
     def decide_image_filepath(self, photo_detail: JmPhotoDetail, index: int) -> str:
-        # 先检查advice的回调，如果回调支持，则优先使用回调
-        for advice in JmAdviceRegistry.get_advice(self):
-            filepath = advice.decide_image_filepath(self, photo_detail, index)
-            if filepath is not None:
-                return filepath
-
         # 通过拼接生成绝对路径
         save_dir = self.decide_image_save_dir(photo_detail)
         image: JmImageDetail = photo_detail[index]
         suffix = self.decide_image_suffix(image)
         return save_dir + image.img_file_name + suffix
 
     """
-    下面是对Advice的支持
-    """
-
-    def register_advice(self, *advice):
-        JmAdviceRegistry.register_advice(self, *advice)
-
-    """
     下面是创建对象相关方法
     """
 
     @classmethod
     def construct(cls, dic: Dict, cover_default=True) -> 'JmOption':
         if cover_default:
             dic = cls.merge_default_dict(dic)
```

### Comparing `jmcomic-2.0.4/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.5/src/jmcomic/jm_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from PIL import Image
-
 from .jm_entity import *
 
 
 class JmcomicText:
     pattern_jm_domain = compile('https://([\w.-]+)')
     pattern_jm_pa_id = compile('/(photos?|album)/(\d+)')
     pattern_html_jm_pub_domain = compile('[\w-]+\.\w+/?\w+')
```

### Comparing `jmcomic-2.0.4/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.5/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

