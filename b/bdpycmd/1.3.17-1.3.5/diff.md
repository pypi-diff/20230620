# Comparing `tmp/bdpycmd-1.3.17.tar.gz` & `tmp/bdpycmd-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.17.tar", last modified: Tue Jun 20 07:20:07 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.5.tar", last modified: Tue Jun 13 12:39:16 2023, max compression
```

## Comparing `bdpycmd-1.3.17.tar` & `bdpycmd-1.3.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.689419 bdpycmd-1.3.17/
--rw-r--r--   0 zhicheng   (501) staff       (20)     3278 2023-06-20 07:20:07.689481 bdpycmd-1.3.17/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     2617 2023-06-20 07:19:32.000000 bdpycmd-1.3.17/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.17/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      785 2023-06-20 07:20:07.689746 bdpycmd-1.3.17/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.687306 bdpycmd-1.3.17/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.688095 bdpycmd-1.3.17/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.17/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.688693 bdpycmd-1.3.17/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.688902 bdpycmd-1.3.17/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2895 2023-06-20 07:19:54.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.689327 bdpycmd-1.3.17/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     5815 2023-06-13 17:37:07.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      957 2023-06-14 02:32:50.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/factory/dacmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      903 2023-06-14 16:23:24.000000 bdpycmd-1.3.17/src/bdpycmd/cmd/factory/dafunc.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8133 2023-06-13 17:12:10.000000 bdpycmd-1.3.17/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-20 07:20:07.688549 bdpycmd-1.3.17/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     3278 2023-06-20 07:20:07.000000 bdpycmd-1.3.17/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-06-20 07:20:07.000000 bdpycmd-1.3.17/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-20 07:20:07.000000 bdpycmd-1.3.17/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-20 07:20:07.000000 bdpycmd-1.3.17/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965275 bdpycmd-1.3.5/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.965357 bdpycmd-1.3.5/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.5/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.5/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:39:16.965645 bdpycmd-1.3.5/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.962929 bdpycmd-1.3.5/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.963689 bdpycmd-1.3.5/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.5/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964298 bdpycmd-1.3.5/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964479 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965159 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     4132 2023-06-13 12:39:09.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8331 2023-06-13 12:39:08.000000 bdpycmd-1.3.5/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964191 bdpycmd-1.3.5/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.17/README.md` & `bdpycmd-1.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: bdpycmd
+Version: 1.3.5
+Summary: Run Python`s file as command line
+Home-page: https://github.com/biandoucheng/bd-py-cmd
+Author: biandoucheng
+Author-email: biandoucheng@outlook.com
+Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
+Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
+Classifier: Programming Language :: Python :: 3.5
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
 # Python command tool
 
 ## Require
 + python3.5 +
 
 ## Description
 `
@@ -36,37 +52,8 @@
 ## New features
 `
 2023.06.13
 1. Support command keyword retrieval:
     No content input, press Enter directly to reality the next command
     Enter the command number or any range, and relevant commands will be queried based on the provided content
     Enter the '/' symbol to exit the help prompt
-
-2. Support executable methods for directly querying commands during command queries
-    Enter the '.' symbol to exit the help prompt
-    Enter '/' to query the executable method of the selected command
-
-3. Fix Bugs
-    Fix the issue of execution errors caused by the 'None' parameter in the run dictionary and optimize information output
-
-2023.06.14
-1. Support direct execution of methods when querying command executable methods
-    Enter the '.' symbol to exit the help prompt
-    Enter '/' to executable the selected method of the selected command
-2. Fix Bug
-    Fix 'm' parameter error in command method help
-3. Fix Bug
-    Fix the issue of command generation assistant generating command errors
-4. Perf
-    Optimize the command generation assistant to make the parameters of the command generation method clearer and easier to use
-5. Perf
-    When using the command assistant to generate commands, it supports forcibly overwriting the parameter 'abs' of existing command files
-
-2023.06.15
-1. Fix
-    Fix errors in keyword retrieval methods
-
-
-2023.06.20
-1. Feat assistant
-    Optimizing the Naming of Command File Names. Allow the parameter cmd to be passed in as the name of the command and command file.
-`
+`
```

### Comparing `bdpycmd-1.3.17/setup.cfg` & `bdpycmd-1.3.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.17
+version = 1.3.5
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.17/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file is a command execution file generated by the command assistant. 
-# Do not edit it.
+# Please do not modify it
 
 import os
 from ..factory import base
 
 # Command Description Information
 _BDCMD_DESC_ = {
     "name":"assistant",
@@ -12,73 +12,68 @@
 }
 
 class Command(base.BaseCommand):
     def __init__(self):
         super().__init__(name=__class__.__module__,alias='command assistant',description='Generate execution commands from existing modules')
     
     @base.BaseCommand.as_cmder
-    def make_cmd(self,mpth:str,cls:str,cdir:str,cmd:str,alias:str,desc:str,abs:str="yes",inner:str='false'):
+    def make_cmd(self,pkg:str,name:str,pdir:str,alias:str,desc:str,inner:str='false'):
         """
         Create a command from a module
         
-        :param mpth:  str #Module relative path, such as: ./a/b/c
-        :param cls:   str #Class name
-        :param cdir:  str #Relative Directory, such as: ./cmder
-        :param cmd:   str #Command name
+        :param pkg:   str #Module package path such as: a.b.c
+        :param name:  str #Module name, without the .py suffix
+        :param pdir:  str #Script storage relative directory
         :param alias: str #command alias
         :param desc:  str #command description
-        :param abs:   str #Do you want to forcibly replace existing command files. yes/no
         """
-        if cdir == "./cmd" or cdir == "cmd":
-            raise Exception("The current command storage directory conflicts with the internal command storage directory")
-
-        # Extract Command Name
-        mpth = mpth.replace("\\","/").rstrip("/")
-        mdu = mpth.replace("/",".")
-
-        # Determine if it has the same cmd as a built-in command
-        if not cmd:
-            cmd  = mpth.split("/")[-1]
-        if cmd in self.INNER_CMD:
+        # Determine if it has the same name as a built-in command
+        if name in self.INNER_CMD:
             self.format_print("Command name conflicts with built-in commands")
             return
         
-        c_fn = "%s.py" % cmd
-        c_fn = cdir.replace("\\","/").rstrip("/") + "/" + c_fn
-
-        if abs != "yes" and os.path.exists(c_fn):
+        fn = "%s.py" % name
+        f_fn = pdir.replace("\\","/").rstrip("/") + "/" + fn
+        
+        if os.path.exists(f_fn):
             self.format_print("command already exists")
             return
 
         if inner == 'true':
             bscmd = '..factory'
         else:
             bscmd = 'bdpycmd.cmd.factory'
         
         tmp = \
-        f"""
+        """
 # This file is a command execution file generated by the command assistant. 
-# Do not edit it.
+# Please do not modify it
 
-from {bscmd}.base import BaseCommand 
-from {mdu} import {cls}
+from {bscmd} import base
+from {pkg} import {name}
 
 # Command Description Information
-_BDCMD_DESC_ = {{
-    "name":'{cmd}',
+_BDCMD_DESC_ = {
+    "name":'{name}',
     "alias":'{alias}',
     "desc":'{desc}'
-}}
+}
 
-class Command(BaseCommand,{cls}):
+class Command(base.BaseCommand,{name}.{name}):
     def __init__(self):
         super().__init__(name=__class__.__module__,alias='{alias}',description='{desc}')
-        super(BaseCommand,self).__init__()
-        """
-        with open(file=c_fn,mode='w',encoding='utf8') as f:
+        super(base.BaseCommand,self).__init__()
+        """ .format(
+            bscmd=bscmd,
+            pkg=pkg,
+            name=name,
+            alias=alias,
+            desc=desc
+        )
+        with open(file=f_fn,mode='w',encoding='utf8') as f:
             f.write(tmp.lstrip())
         
         self.format_print("Command created successfully")
     
     @base.BaseCommand.as_cmder
     def test(self,a=1,b=2):
         """
```

### Comparing `bdpycmd-1.3.17/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from functools import wraps
 from types import FunctionType
-from .dacmd import CmdMeta
-from .dafunc import MethodMeta
+from ..factory.cmd import CmdMeta
 
 # Command Description Information
 _BDCMD_DESC_ = {
     "name":"base",
     "alias":"command base class",
     "desc":"All commands need to inherit from this base class"
 }
@@ -31,23 +30,25 @@
             alias=alias,
             desc=description
         )
         #Methods not shown in the help information
         self.protected_methods = {'__init__','as_cmder'}
 
 
-    def help(self,**kwargs):
+    def help(self,m=''):
         """
         help    Help method, output help information
         """
         tab = """
         """
+        if not isinstance(m,str):
+            m = ''
 
-        #method to run
-        mtds = []
+        #help output command
+        hps = []
 
         #Handling inheritance of command classes
         class_objects = [self.__class__]
         self.deep_clss(self.__class__,class_objects)
 
         #Traverse the object members of the command class and the parent class
         # inherited by the command class to find the command method
@@ -55,99 +56,32 @@
             class_name = class_object.__name__
             for k, v in vars(class_object).items():
                 k = k.replace(class_name + '_', '')
                 if k in self.protected_methods:
                     continue
                 
                 if not k.startswith('_') and isinstance(v,FunctionType) and v.__name__.endswith('___bdcmder'):
-                    mtds.append(MethodMeta(
-                        number=0,
-                        cname=class_name,
-                        name=k,
-                        desc=str(v.__doc__).lstrip(tab)
-                    ))
+                    hps.append(tab + k + '  ' + str(v.__doc__).lstrip(tab))
 
         print(self.info.info())
-        _mtd,info = self.search(mtds=mtds)
-
-        if not _mtd:
-            msg = """
-        Target method not found
-            """
-            print(msg)
-        else:
-            print(info)
-            self.__getattribute__(_mtd)()
-    
-
-    @classmethod
-    def search(self,mtds:list):
-        """
-        Retrieve command list based on keywords
-
-        :param mtds: list[MethodMeta] Method Meta Information List
-        :return: str Target Command
-        """
-        keyword = ""
-        tag_func = ""
-        checked = "/"
-        exited = "."
-        info = ""
-        
-        while True:
-            if keyword == exited:
-                tag_func = ""
-                info = ""
-                break
-            
-            if keyword == checked:
-                break
-            
-            if not keyword:
-                for _cmd in mtds:
-                    tag_func = _cmd.name
-                    info = _cmd.info()
-                    keyword = input(_cmd.say()).strip()
-                    if not keyword:
-                        continue
-                    else:
-                        break
-                else:
-                    break
-            else:
-                _word = keyword
-                for _cmd in mtds:
-                    if _cmd.search(_word):
-                        tag_func = _cmd.name
-                        info = _cmd.info()
-                        keyword = input(_cmd.say()).strip()
-                        if not keyword or keyword == _word:
-                            continue
-                        else:
-                            break
-                else:
-                    break
-        
-        return tag_func,info
-
+        self.format_print(infos=hps)
 
     def deep_clss(self,obj:object,clss:list):
         """
         Recursively complete inherited class query
         
         :param obj: object #initial class
         :param clss: list #target class list
         """
         for it in obj.__bases__:
             if it.__name__ == 'BaseCommand' or it == object:
                 continue
             else:
                 clss.append(it)
                 self.deep_clss(it,clss=clss)
-    
 
     def format_print(self,*args,infos:list=[],ft:bool=True):
         """
         formatted print
         
         :param infos: list #List of information to be printed
         :param ft: bool #Lines beyond the first line are indented
@@ -178,14 +112,19 @@
         @wraps(fun)
         def wrapper(self,**kwargs):
             args_regex = re.compile(r':param\s([\w]+):',re.DOTALL)
             dc = fun.__doc__
             if not dc:
                 dc = ''
             
+            fn = f"""
+        {fun.__name__}
+            """
+            print(fn + dc)
+            
             all_arg_names = args_regex.findall(dc)
             target = {}
             for k in all_arg_names:
                 if k in kwargs:
                     target[k] = kwargs[k]
                 else:
                     vl = input(k + " = ")
```

### Comparing `bdpycmd-1.3.17/src/bdpycmd/cmd/factory/dafunc.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from dataclasses import dataclass
 
 @dataclass
-class MethodMeta:
+class CmdMeta:
     number:int
-    cname:str
     name:str
+    alias:str
     desc:str
 
     def search(self,vl:str="") -> bool:
         """
         Determine if the search matches
 
         :param vl: str search word
         """
         if not vl:
             return False
 
         if vl.isdigit():
             return vl == str(self.number)
         
-        return vl in self.name or vl in self.desc
+        return vl in self.name or vl in self.alias or vl in self.desc
     
 
     def say(self,) -> str:
         """
         Describe information
         """
         return f"""
-        *** method check **************
-        {self.cname} . {self.name}
-                Number: {self.number}
-                {self.desc}  
+        {self.name} ----------------------
+                    {self.alias}
+                    {self.desc}
+                    Number: {self.number}
         """
 
-
     def info(self,) -> str:
         """
         Describe information
         """
         return f"""
-        *** method run ******************
-        {self.cname} . {self.name}
-        {self.desc}
+        {self.name} ++++++++++++++++++++++
+                    {self.alias}
+                    {self.desc}
         """
```

### Comparing `bdpycmd-1.3.17/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.5/src/bdpycmd/pycmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys,traceback,os
 from types import FunctionType
 from importlib import import_module
-from .cmd.factory.dacmd import CmdMeta
+from .cmd.factory.cmd import CmdMeta
 
 class CmdBaseConf:
     # project root directory
     __PROJECT_ROOT_DIR = os.path.abspath('.')
     # command script saver relative path
     __CMD_DIR = "cmd"
     # command folder, which can only be a child of the root directory
@@ -209,14 +209,18 @@
             modpth = cls.__INNER_CMD_MODEL_PATH if is_inner and __name__ != "__main__" else cls.__CMD_MODULE_PATH
             
             #import command module
             cmd = __import__(modpth + '.' + kwargs['cmd'], fromlist=['None'])
 
             #Get command execution method
             cmder = cls.find_real_cmder(cmd=cmd.Command,son=kwargs['son'])
+            if kwargs['son'] == 'help':
+                kwargs = {
+                    'm':kwargs['m']
+                }
 
             #run command
             if not cmder:
                 print('{cmd}`s subcommands `{son}` does not exist'.format(cmd=kwargs['cmd'], son=kwargs['son']))
             else:
                 cmder(cmd.Command(),**kwargs)
         except ImportError:
@@ -253,14 +257,16 @@
                 dic_args['cmd'] = 'help'
 
         if dic_args['cmd'] in help_list:
             cls.help()
         else:
             if 'son' not in dic_args or dic_args['son'] in help_list or not dic_args['son']:
                 dic_args['son'] = 'help'
+                if 'm' not in dic_args:
+                    dic_args['m'] = ''
 
             cls.run_command(**dic_args)
 
 
 # execution entry
 if __name__ == '__main__':
     # initialization
```

