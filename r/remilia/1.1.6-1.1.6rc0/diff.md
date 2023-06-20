# Comparing `tmp/remilia-1.1.6.tar.gz` & `tmp/remilia-1.1.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remilia-1.1.6.tar", last modified: Mon Jun 19 04:18:20 2023, max compression
+gzip compressed data, was "remilia-1.1.6rc0.tar", last modified: Sat Jun 17 05:29:55 2023, max compression
```

## Comparing `remilia-1.1.6.tar` & `remilia-1.1.6rc0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-06-19 04:17:48.223574 remilia-1.1.6/LICENSE
--rw-r--r--   0        0        0     1063 2023-06-19 04:17:48.223574 remilia-1.1.6/LICENSE
--rw-r--r--   0        0        0      785 2023-06-19 04:17:48.223574 remilia-1.1.6/README.md
--rw-r--r--   0        0        0      785 2023-06-19 04:17:48.223574 remilia-1.1.6/README.md
--rw-r--r--   0        0        0     1282 2023-06-19 04:18:20.341846 remilia-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      190 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/__init__.py
--rw-r--r--   0        0        0      128 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/base/__init__.py
--rw-r--r--   0        0        0       33 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/base/exceptions.py
--rw-r--r--   0        0        0      694 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/base/models.py
--rw-r--r--   0        0        0     1881 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/base/rtypes.py
--rw-r--r--   0        0        0     5117 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/log.py
--rw-r--r--   0        0        0     3111 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/mixin.py
--rw-r--r--   0        0        0     5085 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/mixin_decorations/__init__.py
--rw-r--r--   0        0        0     3255 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/mixin_decorations/omixin.py
--rw-r--r--   0        0        0     3930 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/res.py
--rw-r--r--   0        0        0      997 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/DecoratorUtils.py
--rw-r--r--   0        0        0     1851 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/SignParas.py
--rw-r--r--   0        0        0      158 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/__init__.py
--rw-r--r--   0        0        0      764 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/cli/prompts_extension/__init__.py
--rw-r--r--   0        0        0       71 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/net/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/net/pixiv.py
--rw-r--r--   0        0        0       41 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/os/__init__.py
--rw-r--r--   0        0        0       51 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/os/win/__init__.py
--rw-r--r--   0        0        0      360 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/os/win/exeutils.py
--rw-r--r--   0        0        0     4163 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/thread/Timeout.py
--rw-r--r--   0        0        0      241 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/thread/__init__.py
--rw-r--r--   0        0        0     1149 2023-06-19 04:17:48.223574 remilia-1.1.6/src/Remilia/utils/thread/terminable_thread.py
--rw-r--r--   0        0        0     2995 1970-01-01 00:00:00.000000 remilia-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/LICENSE
+-rw-r--r--   0        0        0     1063 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/LICENSE
+-rw-r--r--   0        0        0      785 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/README.md
+-rw-r--r--   0        0        0      785 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/README.md
+-rw-r--r--   0        0        0     1441 2023-06-17 05:29:55.846594 remilia-1.1.6rc0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/base/__init__.py
+-rw-r--r--   0        0        0     1697 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/base/rtypes.py
+-rw-r--r--   0        0        0     4464 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/log.py
+-rw-r--r--   0        0        0     3104 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin.py
+-rw-r--r--   0        0        0     5120 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin_decorations/__init__.py
+-rw-r--r--   0        0        0     3255 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin_decorations/omixin.py
+-rw-r--r--   0        0        0      997 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/DecoratorUtils.py
+-rw-r--r--   0        0        0     1851 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/SignParas.py
+-rw-r--r--   0        0        0      158 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/__init__.py
+-rw-r--r--   0        0        0      764 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/cli/prompts_extension/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/net/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/net/pixiv.py
+-rw-r--r--   0        0        0       41 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/win/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/win/exeutils.py
+-rw-r--r--   0        0        0     4163 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0        0        0      241 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/__init__.py
+-rw-r--r--   0        0        0     1149 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/terminable_thread.py
+-rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 remilia-1.1.6rc0/PKG-INFO
```

### Comparing `remilia-1.1.6/LICENSE` & `remilia-1.1.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/README.md` & `remilia-1.1.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/pyproject.toml` & `remilia-1.1.6rc0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,28 @@
     { name = "H2Sxxa", email = "H2Sxxa0w0@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = []
 classifiers = [
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "colorama",
     "pyyaml",
     "pydantic",
     "typing_extensions",
 ]
-version = "1.1.6"
+version = "1.1.6rc0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://pypi.org/project/Remilia/"
 Repository = "https://github.com/H2Sxxa/Remilia"
@@ -41,14 +43,19 @@
 tui = [
     "noneprompt",
 ]
 all = [
     "noneprompt",
     "pixivpy_async",
 ]
+publish = [
+    "noneprompt",
+    "pixivpy_async",
+    "twine",
+]
 
 [tool.pdm.version]
 source = "scm"
 write_to = "Remilia/__version__.py"
 write_template = "__version__ = '{}'"
 
 [tool.pdm.build]
```

### Comparing `remilia-1.1.6/src/Remilia/log.py` & `remilia-1.1.6rc0/src/Remilia/log.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from functools import partial
-from pathlib import Path
 from colorama import Fore, Back, Style, Cursor
 from colorama import init as initcolor
-from typing import Callable, Dict, List, Optional,TYPE_CHECKING, Union
+from typing import Dict, Optional,TYPE_CHECKING
 from typing_extensions import Self
+from pydantic import BaseModel
 from time import strftime,localtime
-
-from .res import rFile, rPath
-from .base.models import Ruler
-from .base.rtypes import Pair
-
+from .base.rtypes import RT,T
 from platform import system
 import inspect
- 
+
 if TYPE_CHECKING:
     class _CallMethod:
         def __call__(self, *args: str) -> None:
             ...
 
 
 try:
     if system() == "Windows":
         initcolor(wrap=True)
     else:
         initcolor(wrap=False)
 except:
     pass
 
+class Ruler(BaseModel):
+    '''
+    self -> Type(Log)
+    '''
+    level:int=5
+    excolor:str="fore.LIGHTGREEN_EX+'[ '+name+' '+time+' '+location+'] '+style.RESET_ALL+text"
+    explain:str="'[ '+name+' '+time+' '+location+'] '+text"
+    timeformat:str="%H:%M:%S"
+    def exgenerate(self,model:str,*color:str) -> Self:
+        self.explain=model % tuple(["" for _ in color])
+        self.excolor=model % color
+        return self
+
 class Log:
     def __init__(self,name:str,location:str,logs:tuple=(),ruler:Ruler=Ruler()) -> None:
         super().__init__()
         self.ruler=ruler
         self.location=location
         self.logs=map(str,logs)
         self.name=name.upper()
@@ -63,97 +72,73 @@
         time=strftime(
             self.ruler.timeformat,
             localtime()
             )
         __all__=[ruler,location,name,text,time]
         return eval(self.ruler.explain)
 
-
+#TODO WRITE IT
 class LogCat:
-    all_logs:List[Log]
-    all_subs:List[Pair[Callable[[Log],bool],rFile]]
     def __init__(self) -> None:
-        self.all_logs=[]
-        self.all_subs=[]
-          
-    def get_logs(self,filter:Callable[[Log],bool]) -> List[Log]:
-        return [log for log in self.all_log if filter(log)]
-    
-    def record(self,*logs:Log) -> Self:
-        self.all_logs.extend(logs)
-        self._subwrite(*logs)
-        return self
-    
-    def export(self,path:Union[rFile,rPath,Path,str],filter:Callable[[Log],bool],mode:str="w") -> Self:
-        rflog=rFile(path) if not isinstance(path,rFile) else path
-        rflog.write(data='\n'.join([log.plain for log in self.get_logs(filter)]),mode=mode)
-        return self
-    
-    def subscribe(self,*pairs:Pair[Callable[[Log],bool],Union[rFile,rPath,Path,str]]) -> Self:
-        subs=map(lambda pair:Pair(pair.name,rFile(pair.value) if not isinstance(pair.value,rFile) else pair.value),pairs)
-        self.all_subs.extend(subs)
-        return self
-    
-    def _subwrite(self,*logs:Log) -> None:
-        for sub in self.all_subs:
-            mode ="a" if sub.value.exists() else "w"
-            for log in logs:
-                if sub.name(log):
-                    sub.value.write(data=log.plain,mode=mode)
-            
-    
+        pass
+    def record(self,*log:Log):pass
 class Logger:
     def __init__(self,logcat:LogCat=LogCat(),ruler_map:Optional[Dict[str,Ruler]]={},model:str="'%s[ '+name+' '+time+' '+location+'] %s'+text") -> None:
         self.ruler_map={
             "DEBUG":Ruler(level=3).exgenerate(model,Fore.CYAN,Style.RESET_ALL),
             "INFO":Ruler(level=5).exgenerate(model,Fore.LIGHTGREEN_EX,Style.RESET_ALL),
             "WARN":Ruler(level=6).exgenerate(model,Fore.LIGHTYELLOW_EX,Style.RESET_ALL),
             "ERROR":Ruler(level=7).exgenerate(model,Fore.LIGHTRED_EX,Style.RESET_ALL),
         }
         self.ruler_map.update(ruler_map)
         self.logcat=logcat
         self.handle_out=print
         self.vlevel=5
+        self.wlevel=0
         global instance
         instance=self
     
     def set_vlevel(self,vlevel:int) -> Self:
         self.vlevel=vlevel
         return self
     
+    def set_wlevel(self,wlevel:int) -> Self:
+        self.wlevel=wlevel
+        return self
     
     def ex_ruler(self,model:str,**colors:Dict[str,tuple]) -> Self:
         for n,c in colors.items():
             self.to_ruler(n,self.get_ruler(n).exgenerate(model,*c))
         return self
     
-    def to_ruler(self,name:str,ruler:Ruler) -> Self:
-        self.ruler_map.update({name.upper():ruler})
+    def to_ruler(self,name:str,level:int) -> Self:
+        self.ruler_map.update({name.upper():level})
         return self
     
     def get_ruler(self,name:str) -> Ruler:
         try:
             return self.ruler_map[name.upper()]
         except:
             return Ruler()
         
     def print(self,name:str,*log:Log) -> None:
         clog=Log(name,inspect.getmodule(inspect.stack()[1][0]).__name__,log,self.get_ruler(name))
         if self.vlevel >= clog.ruler.level:
             self.handle_out(clog.color)
-        self.logcat.record(clog)
+        if self.wlevel >= clog.ruler.level:
+            self.logcat.record(clog.plain)
     
     def __getattr__(self,name) -> "_CallMethod":
         if name.startswith("__") and name.endswith("__"):
             raise AttributeError(
                 f"'{self.__class__.__name__}' object has no attribute '{name}'"
             )
         return partial(self.print,name)
-    
-instance:Logger
+
+instance:Logger = None
 def get_logger(*args,**kwargs) -> Logger:
     '''
     args & kwargs only work under (instance == None)
     '''
     global instance
     if instance != None:
         return instance
```

### Comparing `remilia-1.1.6/src/Remilia/mixin.py` & `remilia-1.1.6rc0/src/Remilia/mixin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import gc
 from types import ModuleType
 from typing import Any
-from enum import Enum
 
 from .base.rtypes import Pair
 from .mixin_decorations.omixin import collect_attr
 from .mixin_decorations import DecorationBase
 from . import mixin_decorations
 
 __all__=["mixin_decorations"]
 
-class EnumShadow(Enum):
-    FOLLOW="FOLLOW"
-    
-
+class EnumShadow:
+    class FOLLOW:pass
+class MixinError:pass
 
 class Shadow:
     def __init__(self,default=EnumShadow.FOLLOW) -> None:
         '''
         use to replace target attr (empty default to follow the father)
         
         ---
@@ -91,16 +89,16 @@
         else:
             gc_dict={}
         for liter in mixin_map:
             for k,v in liter.items():
                 while isinstance(v,DecorationBase):
                     pair=v.warp(Pair(k,v))
                     
-                    k=pair.name
-                    v=pair.value
+                    k=pair.attr_A
+                    v=pair.attr_B
                     
                 if isinstance(v,Shadow):
                     if self.gc_mixin:
                         v.gc_fill(k,gc_dict)
                     else:
                         v.fill(k,self.targetClass)
                 else:
```

### Comparing `remilia-1.1.6/src/Remilia/mixin_decorations/__init__.py` & `remilia-1.1.6rc0/src/Remilia/mixin_decorations/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Callable, List
+from types import MethodType
+from typing import List
 from ..base.rtypes import Pair
 from ..utils.SignParas import ParaFilter
 from .omixin import gc_Mixin
 from . import omixin
 from abc import abstractmethod
 
 __all__=["omixin"]
@@ -13,15 +14,15 @@
         return self
     def withObj(self,obj):
         self.obj=obj
         return self
     
     @abstractmethod
     def warp(self,pair:Pair) -> Pair:
-        return Pair(Pair.name,Pair.value)
+        return Pair(Pair.attr_A,Pair.attr_B)
 
 class ParaHandleBase:
     @abstractmethod
     def warp_para(self,arg):pass
 
 class ParaReplacer(ParaHandleBase):
     def __init__(self,paragen=lambda para:para,condition=lambda para:True) -> None:
@@ -35,31 +36,31 @@
     def warp_para(self, arg):
         if self.condition(arg):
             return self.paragen(arg)
         else:
             return arg
 
 class ParaMixin(ParaHandleBase):
-    def __init__(self,mixins:Pair[str,Callable]=[],condition=lambda para:True,gc=False) -> None:
+    def __init__(self,mixins:Pair(str,MethodType)=[],condition=lambda para:True,gc=False) -> None:
         '''
         mixins: Pair(method_name,Method)
         condition: wont work until it return True
         '''
         self.mixins=mixins
         self.cd=condition
         self.gc=gc
     def warp_para(self, arg):
         if not self.cd(arg):
             return arg
         new_arg=arg
         for mixin in self.mixins:
             if self.gc:
-                gc_Mixin(new_arg,mixin.value,mixin.name)
+                gc_Mixin(new_arg,mixin.attr_B,mixin.attr_A)
             else:
-                setattr(new_arg,mixin.name,mixin.value)
+                setattr(new_arg,mixin.attr_A,mixin.attr_B)
         return new_arg
     
 class ParaHooker(ParaHandleBase):
     def __init__(self,hookname="__getattribute__",bfhooker=lambda *_,**__:None,afhooker=lambda result,*_,**__:result,condition=lambda para:True,gc=False) -> None:
         '''
         ### via mixin inject target , wont work for some buildin method
         hookname: hook target(default is all(maybe) )
@@ -94,23 +95,23 @@
         bfhooker: hook before call it
         afhooker: hook after call it
         '''
         self.bf=bfhooker
         self.af=afhooker
         self.ph=parahandle
     def warp(self,pair) -> Pair:
-        return Pair(pair.name,self.warpper)
+        return Pair(pair.attr_A,self.warpper)
     
     @property
     def warpper(self):
         filter=ParaFilter(self.obj)
         filter.load_default()
         filter.fill_none()
         for pair in self.ph:
-            filter.index_put(pair.name,pair.value)
+            filter.index_put(pair.attr_A,pair.attr_B)
         def tmp(*args,**kwargs):
             self.bf(self.obj,*args,**kwargs)
             for arg,index in zip(args,range(0,len(args))):
                 default=filter.kwargs[filter.get_index(index).name]
                 if isinstance(default,ParaHandleBase):
                     filter.index_put(index,default.warp_para(arg))
                 else:
```

### Comparing `remilia-1.1.6/src/Remilia/mixin_decorations/omixin.py` & `remilia-1.1.6rc0/src/Remilia/mixin_decorations/omixin.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/DecoratorUtils.py` & `remilia-1.1.6rc0/src/Remilia/utils/DecoratorUtils.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/SignParas.py` & `remilia-1.1.6rc0/src/Remilia/utils/SignParas.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/cli/__init__.py` & `remilia-1.1.6rc0/src/Remilia/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/net/pixiv.py` & `remilia-1.1.6rc0/src/Remilia/utils/net/pixiv.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/thread/Timeout.py` & `remilia-1.1.6rc0/src/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/src/Remilia/utils/thread/terminable_thread.py` & `remilia-1.1.6rc0/src/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

### Comparing `remilia-1.1.6/PKG-INFO` & `remilia-1.1.6rc0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remilia
-Version: 1.1.6
+Version: 1.1.6rc0
 Summary: Use python with next generation api
 Author-Email: H2Sxxa <H2Sxxa0w0@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 H2Sxxa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,16 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://pypi.org/project/Remilia/
 Project-URL: Repository, https://github.com/H2Sxxa/Remilia
 Project-URL: Issues, https://github.com/H2Sxxa/Remilia/issues
@@ -37,16 +39,20 @@
 Requires-Dist: colorama
 Requires-Dist: pyyaml
 Requires-Dist: pydantic
 Requires-Dist: typing_extensions
 Requires-Dist: noneprompt; extra == "tui"
 Requires-Dist: noneprompt; extra == "all"
 Requires-Dist: pixivpy_async; extra == "all"
+Requires-Dist: noneprompt; extra == "publish"
+Requires-Dist: pixivpy_async; extra == "publish"
+Requires-Dist: twine; extra == "publish"
 Provides-Extra: tui
 Provides-Extra: all
+Provides-Extra: publish
 Description-Content-Type: text/markdown
 
 <div align=center>
   <img src="https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png"  alt="[BG](https://raw.githubusercontent.com/H2Sxxa/Remilia/main/background.png)"/>
   <h1 align="center">Remilia</h1> 
 </div>
 <div align=center>
```

