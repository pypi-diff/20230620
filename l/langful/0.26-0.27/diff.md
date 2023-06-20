# Comparing `tmp/langful-0.26-py2.py3-none-any.whl.zip` & `tmp/langful-0.27-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,9 @@
-Zip file size: 7937 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1549 b- defN 23-May-10 08:22 langful/__init__.py
--rw-rw-rw-  2.0 fat      611 b- defN 23-Apr-26 14:01 langful/define.py
--rw-rw-rw-  2.0 fat     2461 b- defN 23-May-23 04:47 langful/function.py
--rw-rw-rw-  2.0 fat    13089 b- defN 23-May-10 08:07 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-May-23 04:50 langful-0.26.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2641 b- defN 23-May-23 04:50 langful-0.26.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-23 04:50 langful-0.26.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-23 04:50 langful-0.26.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-May-23 04:50 langful-0.26.dist-info/RECORD
-9 files, 22212 bytes uncompressed, 6783 bytes compressed:  69.5%
+Zip file size: 4643 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
+-rw-rw-rw-  2.0 fat     6853 b- defN 23-Jun-20 15:46 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2650 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jun-20 15:50 langful-0.27.dist-info/RECORD
+7 files, 11439 bytes uncompressed, 3713 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,28 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
-Filename: langful/define.py
-Comment: 
-
-Filename: langful/function.py
-Comment: 
-
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.26.dist-info/LICENSE
+Filename: langful-0.27.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.26.dist-info/METADATA
+Filename: langful-0.27.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.26.dist-info/WHEEL
+Filename: langful-0.27.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.26.dist-info/top_level.txt
+Filename: langful-0.27.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.26.dist-info/RECORD
+Filename: langful-0.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/__init__.py

```diff
@@ -1,93 +1,15 @@
 """
 # langful
 
 Help to localization
 
-# example
-
-- test.py
-- lang
-    - zh_cn.json
-    - en_us.json
-
-## zh_cn.json
-
-```json
-{
-    "hi" : "你好" ,
-    "welcome" : "欢迎"
-}
-```
-
-## en_us.json
-
-```json
-{
-    "hi" : "Hi" ,
-    "welcome" : "Welcome"
-}
-```
-
-## tset.py
-
-```python
-import langful
-
-Text = langful.lang()
-
-print( Text.language_dict )
-
-print( Text.str_replace( "%hi%" , lang_str = "zh_cn" ) )
-
-print( Text.str_replace( "!hi!" , lang_str = "zh_cn" , change = "!" ) )
-
-print( Text.str_replace( "%welcome%" , lang_str = "zh_cn" ) )
-
-print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
-
-print( Text.str_replace( "%hi%" , lang_str = "en_us" ) )
-
-print( Text.str_replace( "!hi!" , lang_str = "en_us" , change = "!" ) )
-
-print( Text.str_replace( "%welcome%" , lang_str = "en_us" ) )
-
-print( Text.str_replace( "!welcome!" , lang_str = "en_us" , change = "!" ) )
-
-print( )
-
-print( Text.str_replace( "%%" ) )
-print( Text.str_replace( "!!" , change = "!" ) )
-```
-
-## Output
-
-```python
-{'en_us': {'welcome': 'Welcome', 'hi': 'Hi'}, 'zh_cn': {'welcome': '欢迎', 'hi': '你好'}}
-你好
-你好
-欢迎
-欢迎
-Hi
-Hi
-Welcome
-Welcome
-
-%
-!
-```
-
 # About
 
 github: https://github.com/cueavyqwp/langful
 
 pypi: https://pypi.org/project/langful
 
 issues: https://github.com/cueavyqwp/langful/issues
 """
 
-# 'lang' object
-from langful.lang import *
-# Some function for 'langful'
-from langful.function import *
-# define
-from langful.define import *
+from .lang import *
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## langful/lang.py

```diff
@@ -1,403 +1,215 @@
 """
 # lang
 """
-import traceback
-import locale
+from locale import getdefaultlocale
 import json
 import os
 
-from langful.define import *
-from langful.function import to_json , to_lang
+def lang_to_json( lang_file : str ) -> dict :
+    """
+    .lang -> .json
+    """
+    ret = {}
+    for i in lang_file.split( "\n" ) :
+        i = i.split("#")[0]
+        i = "".join( i.split( maxsplit = 2 ) )
+        if i :
+            k , v = i.split( "=" , 1 )
+            ret[ k ] = v
+    return ret
+
+def json_to_lang( dict_file : dict ) -> str :
+    """
+    .json -> .lang
+    """
+    ret = ""
+    for k , v in dict_file.items() :
+        if not ( isinstance( v , int ) or isinstance( v , str ) ) :
+            raise TypeError( f"can't use type '{ type( v ) }'" )
+        ret += f"{ k } = { v }\n"
+    return ret
 
 class lang :
+    """
+    # lang
+    """
 
-    def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_type : str = JSON , change : str = "%" ) -> None :
+    def __init__( self , lang_dir : str  |  bool = "lang" , default_locale : str = "en_us" ) -> None :
         """
-        # lang object
-
-        ---
-
-        lang_dir: Translation file storage directory / Translation file dictionary
-
-        default_lang: Default translation
-
-        file_type: 'json' or 'lang'
-
-        change: Specifies what character to use for substitution , default is '%'
-
-        ---
-
-        lang_dir: 翻译文件的存放目录 / 翻译文件字典
-
-        default_lang: 默认使用的翻译
-
-        file_type: 文件后缀 'json' 或 'lang'
-
-        change: 选择用什么符号做替换 默认为'%'
-
+        lang_dir: lang files dir, if use dict to set that False
+        default_locale: default locale
         """
-
-        default_locale = locale.getdefaultlocale()[0].lower() # 默认语言
-        self.type = get_type( lang_dir )
-
-        if self.type == FILE :
-
-            file_suffix = f".{file_type}"
-
-            if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
-                raise KeyError( f"'{lang_dir}' dir not find" )
-            if not len( os.listdir(lang_dir) ) :
-                raise FileNotFoundError( f"'{lang_dir}' has no file!" ) # lang文件夹里没有语言文件
-            if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
-                raise KeyError( f"'{default_lang}' not find" )
-
-            lang_file = os.path.join( lang_dir , default_locale + file_suffix )
-            file_suffix_len = len( file_suffix )
-            lang_file_list = []
-            language_dict = {}
-            use_locale = default_locale
-            if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
-                use_locale = default_lang
-                lang_file = default_lang + file_suffix
-
-            for filename in os.listdir( lang_dir ): # 尝试加载所有能加载的模块
-                if len( filename ) > file_suffix_len and filename[ -file_suffix_len: ] == file_suffix :
-                    try :
-                        with open( os.path.join( lang_dir , filename ) , encoding = UTF8 ) as file :
-                            if file_type == JSON :
-                                loaded_lang_file = json.load( file ) # 直接加载JSON文件
-                            elif file_type == LANG :
-                                loaded_lang_file = to_json( file.read() )
-                            else :
-                                raise TypeError( f"can't use type '{file_type}'" )
-                        language_dict[ filename[ :-file_suffix_len ] ] = loaded_lang_file # 加载文件
-                        lang_file_list.append( filename )
-                    except Exception as error :
-                        print( f"{error}\n" )
-                        traceback.print_exc()
-
-        elif self.type == DICT :
-            use_locale = default_lang
-            if default_lang not in lang_dir :
-                raise KeyError( f"'{default_lang}' not find" )
-            if default_locale in lang_dir :
-                use_locale = default_locale
-            language_dict = lang_dir
-
-        #lang_dir: Translation file storage directory
-        #lang_dir: 翻译文件的存放目录
-        self.lang_dir = lang_dir
-        #default_lang: Default translation
-        #default_lang: 默认使用的翻译
-        self.default_lang = default_lang
-        # language_dict: Load all can read's language file
-        # language_dict: 加载所有可以读取的语言文件
-        self.language_dict = language_dict
-        # default_locale: The default language
-        # default_locale:  默认语言
+        system_locale = self.get_system_locale
         self.default_locale = default_locale
-        # use_locale: The selected language
-        # use_locale: 选定的语言
-        self.use_locale = use_locale
-        # change: Specifies what character to use for substitution , default is '%'
-        # change: 选择用什么符号做替换 默认为'%'
-        self.change = change
-
-        if self.type == FILE :
-            #file_type: 'json' or 'lang'
-            #file_type: 'json' 或 'lang'
-            self.file_type = file_type
-            # lang_file: Choose to use's language file
-            # lang_file: 选择使用的语言文件
-            self.lang_file = lang_file
-            # lang_file_list: All can find's language file
-            # lang_file_list: 所有能找到的语言文件
-            self.lang_file_list = lang_file_list
-
-        self._reload()
-
-    def _lang_str_list_reload( self ) -> None :
-        # lang_str_list: All can find's language file's name
-        # lang_str_list: 所有能找到的语言文件的名字
-        self.lang_str_list = list( self.language_dict.keys() )
-    def _language_reload( self ) -> None :
-        # language: Load need's language file
-        # language: 加载需要的语言文件
-        self.language = self.language_dict[ self.use_locale ]
-    def _file_suffix_reload( self ) -> None :
-        #file_suffix: Such as '.json' '.lang'
-        #file_suffix: 文件后缀 例如 '.json' '.lang'
-        if self.type == FILE :
-            self.file_suffix = "." + self.file_type
-    def _reload( self ) -> None :
-        self._lang_str_list_reload()
-        self._language_reload()
-        self._file_suffix_reload()
-
-    def _lang_str_to_language( self , lang_str ) -> dict :
-        if not lang_str :
-            lang_str = self.use_locale
-        if lang_str in self.lang_str_list :
-            return self.language_dict[ lang_str ]
-        else :
-            raise KeyError( f"lang '{lang_str}' has not find!" )
+        self.system_locale = system_locale
+        self.replace_letter = "%"
+        self.lang_dir = lang_dir
+        self.is_file = False
+        self.languages = {}
+        self.locales = []
+        self.types = {}
+        self.init()
+
+    def init( self ) -> None :
+        """
+        # init
+        """
+        path = self.lang_dir
+        if not isinstance( path , str ) :
+            return
+        if not os.path.exists( path ) :
+            raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
+        self.is_file = True
+        files = []
+        for i in os.listdir( path ) :
+            name , suffix = os.path.splitext( i )
+            if ( suffix == ".json" ) or ( name + ".json" not in files ) :
+                files.append( i )
+                with open( os.path.join( path , i ) , encoding = "utf-8" ) as file :
+                    if suffix == ".json" :
+                        data = json.load( file )
+                    else :
+                        data = lang_to_json( file.read() )
+                self.locales.append( name )
+                self.languages[ name ] = data
+                self.types[ name ] = suffix
 
-    def save( self ) -> None :
+    def init_dict( self , language : dict ) -> None :
         """
-        # save
-        to save all lang file
-
-        ---
-
-        保存所有lang文件
+        init by a dictionary, but cant't to save
         """
-        if self.type == FILE :
-            for key , value in self.language_dict.items() :
-                try :
-                    with open( os.path.join( self.lang_dir , key + self.file_suffix ) , "w+" , encoding = UTF8 ) as file :
-                        if self.file_type == JSON :
-                            file.write( json.dumps( value , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
-                        elif self.file_type == LANG :
-                            file.write( to_lang( value ) )
-                except Exception as error :
-                    print( f"{error}\n" )
-                    traceback.print_exc()
-        else :
-            raise TypeError( f"{self.type} can't to save" )
+        if self.is_file :
+            raise TypeError( "can't init by a dictionary, because it's init by a dir" )
+        for k in language.keys() :
+            self.types[ k ] = ".json"
+            self.locales.append( k )
+        self.languages = language
 
-    def get( self , key : str , lang_str : str = None ) -> str : # 输入键 获取对应的值
+    @property
+    def get_system_locale( self ) -> str :
         """
-
-        # get
-
-        Get one value in some one dictionary
-
-        在某个字典中获取一个值
-
-        ---
-
-        key: The dictionary's key
-
-        lang_str: Such as 'zh_cn' or 'en_us' and more
-
-        ---
-
-        key: 键值
-
-        lang_str: 例如 'zh_cn' 或 'en_us' 等等
-
+        get system locale
         """
-        if not lang_str :
-            lang_str = self.use_locale
+        return getdefaultlocale()[0].lower() # 系统语言
 
-        if lang_str in self.lang_str_list :
-            if key in self.language_dict[ lang_str ] :
-                return self.language_dict[ lang_str ] [ key ]
-            else :
-                raise KeyError( f"key '{key}' has not in dictionary!" )
+    @property
+    def locale( self ) -> str :
+        """
+        choose locale
+        """
+        if self.system_locale in self.locales :
+            return self.system_locale
+        elif self.default_locale in self.locales :
+            return self.default_locale
         else :
-            raise KeyError( f"lang '{lang_str}' has not find!" )
+            raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
 
-    def set( self , key : str , value : str , lang_str : str = None ) -> None : # 设置某个键值
+    @property
+    def language( self ) -> dict :
         """
-
-        Set one value with one key in some one dictionary
-
-        在某个字典中用一个值来设置一个键
-
-        # set
-
-        ---
-
-        key: The dictionary's key
-
-        value: Need to change's value
-
-        lang_str: Such as 'zh_cn' or 'en_us' and more
-
-        ---
-
-        key: 键值
-
-        value: 需要更改的值
-
-        lang_str: 例如 'zh_cn' 或 'en_us' 等等
-
+        get now language
         """
-        if not lang_str :
-            lang_str = self.use_locale
+        return self.languages[ self.locale ]
 
-        if lang_str in self.lang_str_list :
-            self.language_dict[ lang_str ] [ key ] = value
+    @property
+    def type( self ) -> str :
+        """
+        get type, '.json' or '.lang'
+        """
+        return self.types[ self.locale ]
 
+    def set_locale( self , locale : str = None  ) -> None :
+        """
+        set/reset locale
+        """
+        if locale != None :
+            self.system_locale = locale
         else :
-            raise KeyError( f"lang '{lang_str}' has not find!" )
+            self.system_locale = self.get_system_locale
 
-    def add( self , lang_str : str , set : dict = {} , change_file : bool = False ) -> None :
+    def get( self , key : str | int , locale : str = None ) -> str :
         """
-
-        # add a new language
-
-        lang_str: the language's name
-
-        set: the language dictionary
-
-        change_file: modify the file
-
-        ---
-
-        # 添加新语言
-
-        lang_str: 语言名称
-
-        set: 语言字典
-
-        change_file: 是否修改文件
-
+        get
         """
-        self.language_dict[ lang_str ] = set
-        if lang_str == self.default_locale :
-            self.use_locale = lang_str
-        if self.type == FILE and change_file :
-            self.save()
-        self._reload()
+        if not locale :
+            locale = self.locale
+        return self.languages[ locale ][ key ]
 
-    def remove( self , lang_str : str , change_file : bool = False ) -> None :
+    def set( self , key : str | int , value : str , locale : str = None ) -> None :
         """
-
-        # remove a language
-
-        lang_str: the language's name
-
-        change_file: modify the file
-
-        ---
-
-        # 移除语言
-
-        lang_str: 语言名称
-
-        change_file: 是否修改文件
-
+        set
         """
-        if lang_str == self.use_locale or lang_str == self.default_lang or lang_str == self.default_locale :
-            raise RuntimeError( f"can't remove '{lang_str}' " )
-        del self.language_dict[ lang_str ]
-        del self.lang_str_list[ self.lang_str_list.index( lang_str ) ]
-        if self.type == FILE and change_file :
-            self.save()
-        self._reload()
+        if not locale :
+            locale = self.locale
+        self.languages[ locale ][ key ] = value
 
-    def replace( self , key : str = None , args = None , lang_str : str = None , change : str = None ) -> str :
+    def remove( self , key : str | int , locale : str = None ) -> None :
         """
-        # replace
-
-        Replace language dictionary one key with list/string
-
-        用 列表/字符串 替换语言字典中的某个键
-
-        ---
-
-        key: dictionary's key
-
-        args: list
-
-        lang_str: Such as 'zh_cn' or 'en_us' and more
-
-        change: Specifies what character to use for substitution , default is '%'
-
-        ---
-
-        key: 键值
-
-        args: 列表
-
-        lang_str: 例如 'zh_cn' 或 'en_us' 等等
-
-        change: 选择用什么符号做替换 默认为'%'
+        remove
         """
-        if not change :
-            change = self.change
-
-        language = self._lang_str_to_language( lang_str )
+        if not locale :
+            locale = self.locale
+        del self.languages[ locale ][ key ]
 
-        if ( not key ) or ( key not in language ) :
-            raise KeyError( f"can't use key '{key}'" )
-
-        if not ( isinstance( args , str ) or isinstance( args , list ) ) :
-            raise TypeError( f"args can't use '{ type( args ) }' type" )
+    def save( self ) -> None :
+        """
+        save file, when is_file is true
+        """
+        if self.is_file :
+            for key , value in self.languages.items() :
+                suffix = self.types[ key ]
+                print(suffix,value)
+                with open( os.path.join( self.lang_dir , key + suffix ) , "w+" , encoding = "utf-8" ) as file :
+                    if suffix == ".json" :
+                        file.write( json.dumps( value , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
+                    elif suffix == ".lang" :
+                        file.write( json_to_lang( value ) )
+        else :
+            raise TypeError( f"can't to save, because it's not a file" )
 
-        text = self.get( key , lang_str ).split( change )
+    def replace( self , key : str = None , args : list = None , locale : str = None , replace_letter : str = None ) -> str :
+        """
+        replace
+        """
+        if not replace_letter :
+            replace_letter = self.replace_letter
+        if not locale :
+            locale = self.locale
+        text = self.get( key , locale ).split( replace_letter )
         if len( text ) == 1 :
             text = text[0]
         ret = ""
-
-        for i in range_len( text ) :
-            if isinstance( text , str ) :
-                ret += text[i]
+        for i in range( len( text ) ) :
+            if ( len( text ) - 1 ) > i :
+                if len( args ) > i :
+                    ret += text[i] + args[i]
+                else :
+                    ret += text[i] + args[-1]
             else :
-                if isinstance( args , list ) :
-                    if ( len( text ) - 1 ) > i :
-                        if len( args ) > i :
-                            ret += text[i] + args[i]
-                        else :
-                            ret += text[i] + args[-1]
-                    else :
-                        ret += text[i]
-                elif isinstance( args , str ) :
-                    if ( len( text ) - 1 ) > i :
-                        ret += text[i] + args
-                    else :
-                        ret += text[i]
-
+                ret += text[i]
         return ret
 
-    def str_replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
+    def replace_str( self , text : str , locale : str = None , replace_letter : str = None ) -> str :
         """
-        # str_replace
-
-        Replace string with some one language dictionary
-
-        用某个语言字典替换字符串
-
-        ---
-
-        key: The dictionary's key
-
-        args: Strings
-
-        lang_str: Such as 'zh_cn' or 'en_us' and more
-
-        change: Specifies what character to use for substitution , default is '%'
-
-        ---
-
-        key: 键值
-
-        args: Strings
-
-        lang_str: 例如 'zh_cn' 或 'en_us' 等等
-
-        change: 选择用什么符号做替换 默认为'%'
+        replace_str
         """
-        if not change :
-            change = self.change
-
+        if not replace_letter :
+            replace_letter = self.replace_letter
+        if not locale :
+            locale = self.locale
         i = 0
         ret = ""
-        text = join( args ).split( change )
-        language = self._lang_str_to_language( lang_str )
-
+        text = text.split( replace_letter )
+        language = self.languages[ locale ]
         for split_text in text :
             if i % 2 :
                 if split_text in language :
                     ret += language[split_text]
                 elif not split_text :
-                    ret += change
+                    ret += replace_letter
                 else :
                     raise KeyError( f"key '{split_text}' has not find!" )
             else :
                 ret += split_text
             i += 1
-
         return ret
```

## Comparing `langful-0.26.dist-info/LICENSE` & `langful-0.27.dist-info/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 langful
+Copyright (c) 2023 cueavyqwp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `langful-0.26.dist-info/METADATA` & `langful-0.27.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.26
+Version: 0.27
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
@@ -31,15 +31,15 @@
     </a>
 </p>
 
 # install
 
 Use `pip` to install `pip install langful` or `pip3 install langful`
 
-# example
+# example(too old)
 
 - test.py
 - lang
     - zh_cn.json
     - en_us.json
 
 ## zh_cn.json
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: langful Version: 0.26 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.27 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
-# example - test.py - lang - zh_cn.json - en_us.json ## zh_cn.json ```json
-{ "hi" : "ä½ å¥½" , "welcome" : "æ¬¢è¿" } ``` ## en_us.json ```json { "hi" :
-"Hi" , "welcome" : "Welcome" } ``` ## tset.py ```python import langful Text =
-langful.lang() print( Text.language_dict ) print( Text.str_replace( "%hi%" ,
-lang_str = "zh_cn" ) ) print( Text.str_replace( "!hi!" , lang_str = "zh_cn" ,
-change = "!" ) ) print( Text.str_replace( "%welcome%" , lang_str = "zh_cn" ) )
-print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change = "!" ) )
-print( Text.str_replace( "%hi%" , lang_str = "en_us" ) ) print
+# example(too old) - test.py - lang - zh_cn.json - en_us.json ## zh_cn.json
+```json { "hi" : "ä½ å¥½" , "welcome" : "æ¬¢è¿" } ``` ## en_us.json ```json
+{ "hi" : "Hi" , "welcome" : "Welcome" } ``` ## tset.py ```python import langful
+Text = langful.lang() print( Text.language_dict ) print( Text.str_replace
+( "%hi%" , lang_str = "zh_cn" ) ) print( Text.str_replace( "!hi!" , lang_str =
+"zh_cn" , change = "!" ) ) print( Text.str_replace( "%welcome%" , lang_str =
+"zh_cn" ) ) print( Text.str_replace( "!welcome!" , lang_str = "zh_cn" , change
+= "!" ) ) print( Text.str_replace( "%hi%" , lang_str = "en_us" ) ) print
 ( Text.str_replace( "!hi!" , lang_str = "en_us" , change = "!" ) ) print
 ( Text.str_replace( "%welcome%" , lang_str = "en_us" ) ) print
 ( Text.str_replace( "!welcome!" , lang_str = "en_us" , change = "!" ) ) print
 ( ) print( Text.str_replace( "%%" ) ) print( Text.str_replace( "!!" , change =
 "!" ) ) ``` ## Output ```python {'en_us': {'welcome': 'Welcome', 'hi': 'Hi'},
 'zh_cn': {'welcome': 'æ¬¢è¿', 'hi': 'ä½ å¥½'}} ä½ å¥½ ä½ å¥½ æ¬¢è¿ æ¬¢è¿ Hi
 Hi Welcome Welcome % ! ``` # About github: https://github.com/cueavyqwp/langful
```

