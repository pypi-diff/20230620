# Comparing `tmp/libzac-0.0.7-py3-none-any.whl.zip` & `tmp/libzac-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13423 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      134 b- defN 23-May-30 07:53 libzac/__init__.py
--rw-rw-rw-  2.0 fat     4799 b- defN 23-Jun-06 01:57 libzac/bitfield.py
+Zip file size: 14647 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-19 08:09 libzac/__init__.py
+-rw-rw-rw-  2.0 fat     5564 b- defN 23-Jun-19 09:14 libzac/bitfield.py
 -rw-rw-rw-  2.0 fat     1960 b- defN 23-May-17 07:50 libzac/dsp.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-May-17 07:56 libzac/e.py
+-rw-rw-rw-  2.0 fat     4978 b- defN 23-Jun-19 08:10 libzac/e.py
 -rw-rw-rw-  2.0 fat     3007 b- defN 23-May-17 07:56 libzac/io.py
 -rw-rw-rw-  2.0 fat     1510 b- defN 23-May-23 02:36 libzac/math.py
 -rw-rw-rw-  2.0 fat     3074 b- defN 23-May-17 08:19 libzac/plt.py
--rw-rw-rw-  2.0 fat     8791 b- defN 23-Jun-05 08:39 libzac/reg.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      947 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/RECORD
-13 files, 29492 bytes uncompressed, 11881 bytes compressed:  59.7%
+-rw-rw-rw-  2.0 fat     9564 b- defN 23-Jun-20 02:04 libzac/reg.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1734 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      947 b- defN 23-Jun-20 02:14 libzac-0.0.8.dist-info/RECORD
+13 files, 33658 bytes uncompressed, 13105 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: libzac/plt.py
 Comment: 
 
 Filename: libzac/reg.py
 Comment: 
 
-Filename: libzac-0.0.7.dist-info/LICENSE
+Filename: libzac-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: libzac-0.0.7.dist-info/METADATA
+Filename: libzac-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: libzac-0.0.7.dist-info/WHEEL
+Filename: libzac-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: libzac-0.0.7.dist-info/top_level.txt
+Filename: libzac-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: libzac-0.0.7.dist-info/RECORD
+Filename: libzac-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libzac/__init__.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
+from . import e
 from . import bitfield
 from . import dsp
-from . import e
 from . import io
 from . import math
 from . import plt
 from . import reg
```

## libzac/bitfield.py

```diff
@@ -1,13 +1,14 @@
+from typing import Any
 import numpy as np
 from .e import eread, ewrite
 
 ########## used for debug without actually read/wrtie memory #############
-eread = lambda addr,length: np.random.randint(0,255,length,dtype="u1")
-ewrite = lambda addr,value: None
+# eread = lambda addr,length: np.random.randint(0,255,length,dtype="u1")
+# ewrite = lambda addr,value: None
 ##########################################################################
 
 class bitfield():
     _fields_ = {}
     addr = ""
     __ENDIANESS = 'little'
     def __init__(self, data:int=0):
@@ -19,22 +20,28 @@
                 return (self.data & mask) >> shift
             def setter(self, value, mask=mask, shift=shift):
                 self._data = ((value << shift) & mask) | (self.data & ~mask)
             setattr(type(self),field,property(getter, setter))
             shift += bit
 
     def __str__(self): # print(bitfield) will print all info about it
-        s = f"{self.__class__.__name__} @ {self.addr} = {self.hex}\n"
+        s = f"{self.__class__.__name__} @ {self.addr} = 0x{self.data:0{self.size*2}x}\n"
         start = 0
         for field,bit in self._fields_.items():
-            width = f"[{start+bit-1:2d}:{start:2d}]" if bit > 1 else f"[{start}]"
+            width = f"[{start+bit-1:d}:{start:d}]" if bit > 1 else f"[{start}]"
             s += f"  {field}{width} = {hex(getattr(self,field))}\n"
             start += bit
         return s
     
+    def __setattr__(self, __name: str, __value: Any) -> None: # prevent add new attribute other than _fields_
+        if __name in list(self._fields_.keys())+["_data"]:
+            super().__setattr__(__name, __value)
+        else:
+            raise AttributeError(f"Bitfield '{self.__class__.__name__}' has no field '{__name}'")
+    
     @property
     def data(self):
         return self._data
     @property
     def hex(self):
         return hex(self.data)[2:]
     @property
@@ -45,39 +52,51 @@
     def size(cls):
         return (sum(cls._fields_.values())-1)//8 + 1
     @classmethod
     def get(cls, field): 
         """get a signle bit field"""
         bf = cls()
         bf.read()
-        return getattr(bf, field)
+        attr = getattr(bf, field, None)
+        if attr is None:
+            raise AttributeError(f"Bitfield '{cls.__name__}' has no field '{field}'")
+        return attr
     @classmethod
     def set(cls, field, value):
         """set a single bit field while keep others untouched"""
         bf = cls()
         bf.read()
         setattr(bf, field, value)
         bf.write()
     @classmethod
     def from_bytes(cls, byte:bytes):
         return cls(int.from_bytes(byte, cls.__ENDIANESS))
     @classmethod
     def from_np(cls, np_array:np.ndarray):
         return cls.from_bytes(np_array.tobytes())
+    @classmethod
+    def show(cls, verbose=True):
+        bf = cls()
+        bf.read()
+        if verbose:
+            print(bf)
+        return bf.data
 
     def to_np(self, dtype:np.dtype="u1"):
         return np.frombuffer(self.bytes, dtype=dtype)
 
-    def read(self):
+    def read(self, verbose=False):
         r = eread(self.addr, self.size) # read `self.size` bytes from memory at address `self.addr`
-        print(f"read {r} @ {self.addr}")
+        if verbose:
+            print(f"read {r} @ {self.addr}")
         self._data = int.from_bytes(r.tobytes(), self.__ENDIANESS)
 
-    def write(self):
-        print(f"write {self.hex} @ {self.addr}")
+    def write(self, verbose=False):
+        if verbose:
+            print(f"write {self.hex} @ {self.addr}")
         ewrite(self.addr, self.hex) # write `self.size` bytes to memory at address `self.addr`
 
 if __name__ == "__main__":
     # following C bitfield struct `Example` has total 24 bits, which is 3 bytes
     # GCC's `__attribute__((packed))` minimize memory usage, no padding between members
     # ```c
     # typedef struct
```

## libzac/e.py

```diff
@@ -1,22 +1,52 @@
+from __future__ import annotations
 import os
 import re
 import numpy as np
 import matplotlib.pyplot as plt
-from .math import byte2int
-import subprocess
+from .math import byte2int,i3u1_to_i4
+from subprocess import STDOUT, check_output, CalledProcessError
 
-def eread(addr, length=1, dtype="u1", ch=0):
-    raw = subprocess.run(f"e {addr}l{length}", capture_output=True, env={"ch":f"{ch}"}).stdout.decode("utf8")
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:  # Only imports the below statements during type checking
+    from .bitfield import bitfield
+
+def einput(num, output_int=False):
+    """convert all kind of input to hex string(default) or integer"""
+    if isinstance(num, str):
+        return int(num,16) if output_int else num 
+    elif isinstance(num, (int, np.integer)):
+        return num if output_int else f"{num:x}"
+    elif isinstance(num, (float, np.float_)):
+        num = int(np.around(num))
+        return num if output_int else f"{num:x}"
+    else:
+        raise TypeError(f"Input type [{type(num)}] of [{num}] not supported")
+
+def eread(addr, length=1, dtype="u1", ch=0, timeout=3):
+    addr = einput(addr)
+    length = einput(length)
+    try:
+        raw = check_output(f"e {addr}l{length}", stderr=STDOUT, timeout=timeout,  env={"ch":f"{ch}"}).decode("utf8")
+    except CalledProcessError as e:
+        print(e.output.decode("utf8"))
+        raise e
     return e2int(raw, dtype=dtype)[0]
 
-def ewrite(addr, value, ch=0):
-    subprocess.run(f"e {addr} {value}", env={"ch":f"{ch}"})
+def ewrite(addr, value, ch=0, timeout=3):
+    addr = einput(addr)
+    value = einput(value)
+    try:
+        check_output(f"e {addr} {value}", stderr=STDOUT, timeout=timeout,  env={"ch":f"{ch}"})
+    except CalledProcessError as e:
+        print(e.output.decode("utf8"))
+        raise e
 
 def ewrite_block(addr, u1_data):
+    addr = einput(addr)
     data_length = len(u1_data)
     addr = addr if isinstance(addr, int) else int(addr,16)
     
     for i in range(0,data_length,8):
         block = u1_data[i:min(i+8,data_length)]
         data = "".join([f"{b:02x}" if isinstance(b,(int,np.integer)) else b for b in block][::-1])
         start_address = f"{addr + i:x}"
@@ -60,11 +90,35 @@
     ax.plot(addr,data)
     if x_hex:
         ax.get_xaxis().set_major_formatter(lambda x, pos: hex(int(x)))
     if y_int:
         ax.get_yaxis().set_major_formatter(lambda x, pos: int(x))
     fig.show()
 
-def ewrite_block(input, skip_row=1):
+def e2write(input, skip_row=1):
     u1_data, addr = e2int(input, "u1", skip_row=skip_row)
     ewrite_block(addr[0], u1_data)
 
+HREAD = HREAD2 = HREAD3 = HREAD_INLINE =        lambda reg: eread(reg)[0]
+HREADW =                                        lambda reg: eread(reg, length=2, dtype="u2")[0]
+HREAD24BIT = HREADADDR3 =                       lambda reg: i3u1_to_i4(eread(reg, length=3))[0]
+HREAD4 = HREADL = HREADRV =                     lambda reg: eread(reg, length=4, dtype="i4")[0]
+
+HWRITE = HWRITE2 = HWRITE3 = HWRITE_INLINE =    lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xff)
+HWRITEW = HWRITEW_INLINE =                      lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffff)
+HWRITE24BIT =                                   lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffffff) 
+HWRITEL = HWRITERV = HWRITE4 =                  lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffffffff)
+
+def HREAD_STRUCT(reg, stc:bitfield):
+    if einput(reg) == einput(stc.addr):
+        stc.read()
+    else:
+        raise ValueError(f"reg '{reg}' is different from bitfield '{stc.__class__.__name__} @ {stc.addr}'")
+
+def HWRITE_STRUCT(reg, stc:bitfield):
+    if einput(reg) == einput(stc.addr):
+        stc.write()
+    else:
+        raise ValueError(f"reg '{reg}' is different from bitfield '{stc.__class__.__name__} @ {stc.addr}'")
+    
+HREADW_STRUCT = HREAD24BIT_STRUCT = HREADL_STRUCT = HREAD_STRUCT
+HWRITEW_STRUCT = HWRITE24BIT_STRUCT = HWRITEL_STRUCT = HWRITE_STRUCT
```

## libzac/reg.py

```diff
@@ -1,14 +1,16 @@
 import os
 import re
+import importlib
+import sys
 import numpy as np
 import pandas as pd
 import xlrd
 import openpyxl
-from .e import e2int
+from .e import e2int,eread,einput
 from typing import Union
 
 if xlrd.__version__ < "2.0.0":
     xlrd.xlsx.ensure_elementtree_imported(False, None)
     xlrd.xlsx.Element_has_iter = True
 
 
@@ -77,15 +79,15 @@
 reg_name = "name"
 width_name = "width"
 domain_name = "domain"
 access_name = "access"
 init_name = "init"
 description_name = "description"
 
-__workbook_type = Union[xlrd.book.Book,openpyxl.workbook.workbook.Workbook]
+__workbook_type = Union[xlrd.book.Book, openpyxl.workbook.workbook.Workbook]
 
 def read_excel(wb:__workbook_type, sheet_name:str) -> pd.DataFrame:
     """read excel from workbook(xlrd/openpyxl), and fill merged cells"""
     if isinstance(wb, xlrd.book.Book):
         table = pd.read_excel(wb,sheet_name=sheet_name,dtype="string")
         for rl, rh, cl, ch in wb.sheet_by_name(sheet_name).merged_cells:
             table.iloc[rl-1:rh-1, cl:ch] = table.iloc[rl-1,cl]
@@ -152,14 +154,22 @@
 def read_yc_reg(wb:__workbook_type, sheet_name:str) -> pd.DataFrame:
     """read table from workbook then format it"""
     table = read_excel(wb,sheet_name)
     keep_rename_columns(table)
     format_table(table)
     return table
 
+def read_yc_reg_from_file(filename:str):
+    wb = openpyxl.load_workbook(filename)
+    tables = {sheet_name:read_yc_reg(wb, sheet_name) for sheet_name in wb.sheetnames if sheet_name != 'lpm'}
+    return tables
+
+def keep_only_rows(table:pd.DataFrame, keep_list:list, col:str = addr_name):
+    return table.loc[table[col].isin(keep_list)]
+
 def efile_to_hashmap(filename:str) -> dict:
     """convert an `e [addr]l[size]` output file to dict where key is addr and value is data"""
     return {f"{a:x}":d for d,a in zip(e2int(filename,"u1"))}
 
 def parse_width(width:Union[str,int]) -> tuple[int,int]:
     """parse_width('[x]/x') = (x,x);  parse_width('[x:y]/x:y') = (x,y)"""
     if isinstance(width, (np.integer, int)):
@@ -193,31 +203,31 @@
             if start >= 0 and not pd.isna(table.loc[i,addr_name]):            
                 addr = re.search(r"[\da-f]{4,}",table.loc[i,addr_name])
                 if addr is not None:     
                     table.loc[i,new_column] = parse_reg(addr.group(), reg_map, start, stop)
         except:
             print(f"Unable to parse table line{i}: \n{table.loc[i]}")
 
-def read_yc_reg_map(table:pd.DataFrame, reg_map_file:str, new_column=None) -> pd.DataFrame:
-    """apply `parse_table` to a copy of `table` with reg_map read from `reg_map_file`"""
+def read_yc_reg_map(table:pd.DataFrame, reg_map:dict, new_column=None) -> pd.DataFrame:
+    """apply `parse_table` to a copy of `table` with `reg_map`"""
     table = table.copy()
-    reg_map = efile_to_hashmap(reg_map_file)
-    new_column = reg_map_file if new_column is None else new_column    
+    new_column = "new" if new_column is None else new_column    
     parse_table(table, reg_map, new_column)
     return table
 
 def read_yc_reg_map_in_folder(table:pd.DataFrame, top_folder:str, sheet_name:str, suffix:str=""):
     """apply `read_yc_reg_map` to every files start with `sheet_name` in a folder"""
     table = table[table[access_name]=="RW"]
     count = 0
     for dir,_,files in os.walk(top_folder):
         for f in files:
             if f.startswith(sheet_name):
                 new_column = suffix + str(count) if suffix else f
-                table = read_yc_reg_map(table, dir + "\\" + f, new_column=new_column)
+                reg_map = efile_to_hashmap(dir + "\\" + f)
+                table = read_yc_reg_map(table, reg_map, new_column=new_column)
                 count += 1
     return table
 
 def table2tree(table:pd.DataFrame, key:str) -> dict:
     """convert pandas Dataframe to tree like dict, use either `addr_name` or `reg_name` as `key`"""
     tree = {}
     old_key = ""
@@ -227,7 +237,14 @@
                 raise ValueError(f"multiple '{i[key]}'")
             tree[i[key]].append(i)
         else:
             tree[i[key]] = [i]
         old_key = i[key]
     return tree
 
+def load_reg_1121M(MODULE_PATH = "E:\\Work\\Yichip\\1121M\\Soft_Doc\\xlsxtoStructTool\\reg"):    
+    spec = importlib.util.spec_from_file_location(os.path.split(MODULE_PATH)[1], MODULE_PATH+"/__init__.py")
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[spec.name] = module 
+    spec.loader.exec_module(module)
+    setattr(sys.modules[__name__],"reg_1121M",module)
+    return module
```

## Comparing `libzac-0.0.7.dist-info/LICENSE` & `libzac-0.0.8.dist-info/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2022 YiChip Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `libzac-0.0.7.dist-info/METADATA` & `libzac-0.0.8.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: libzac
-Version: 0.0.7
+Version: 0.0.8
 Summary: A private use library
 Author-email: ZinGer_KyoN <zinger.kyon@gmail.com>
 License: MIT License        
-        Copyright (c) [year] [fullname]        
+        Copyright (c) 2022 YiChip Inc.        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:        
         The above copyright notice and this permission notice shall be included in all
@@ -26,8 +26,10 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: packaging
+Requires-Dist: xlrd
+Requires-Dist: openpyxl
```

