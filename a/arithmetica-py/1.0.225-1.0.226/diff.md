# Comparing `tmp/arithmetica-py-1.0.225.tar.gz` & `tmp/arithmetica-py-1.0.226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.225.tar", last modified: Mon Jun 19 12:58:15 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.226.tar", last modified: Tue Jun 20 14:01:16 2023, max compression
```

## Comparing `arithmetica-py-1.0.225.tar` & `arithmetica-py-1.0.226.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.309144 arithmetica-py-1.0.225/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:58:15.309144 arithmetica-py-1.0.225/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   187678 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75560 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:01:16.639042 arithmetica-py-1.0.226/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-20 14:01:00.000000 arithmetica-py-1.0.226/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-20 14:01:16.639042 arithmetica-py-1.0.226/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-20 14:01:00.000000 arithmetica-py-1.0.226/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:01:16.635041 arithmetica-py-1.0.226/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:01:16.639042 arithmetica-py-1.0.226/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-20 14:01:00.000000 arithmetica-py-1.0.226/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:01:16.635041 arithmetica-py-1.0.226/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:01:16.639042 arithmetica-py-1.0.226/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   187862 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75560 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-20 14:01:00.000000 arithmetica-py-1.0.226/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:01:16.000000 arithmetica-py-1.0.226/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.225/LICENSE` & `arithmetica-py-1.0.226/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.225/README.md` & `arithmetica-py-1.0.226/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.225/setup.py` & `arithmetica-py-1.0.226/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.225/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.226/src/python-module/libarithmetica.a`

 * *Files 1% similar despite different names*

#### file list

```diff
@@ -10,15 +10,15 @@
 ?rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 exponential.c.o
 ?rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 factorial.c.o
 ?rw-r--r--   0        0        0    13176 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
 ?rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 fraction_to_continued_fraction.c.o
 ?rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 igcd.c.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 ilcm.c.o
 ?rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 natural_logarithm.c.o
-?rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 power.c.o
+?rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 power.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18336 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
 ?rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 tangent.c.o
 ?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
```

#### power.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          2208 (bytes into file)
+  Start of section headers:          2392 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         14
   Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,23 +1,23 @@
-There are 14 section headers, starting at offset 0x8a0:
+There are 14 section headers, starting at offset 0x958:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 000234 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000568 0002a0 18   I 11   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000274 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000274 000000 00  WA  0   0  1
-  [ 5] .rodata.cst8      PROGBITS        0000000000000000 000278 000018 08  AM  0   0  8
-  [ 6] .comment          PROGBITS        0000000000000000 000290 00002e 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0002be 000000 00      0   0  1
-  [ 8] .note.gnu.property NOTE            0000000000000000 0002c0 000020 00   A  0   0  8
-  [ 9] .eh_frame         PROGBITS        0000000000000000 0002e0 000068 00   A  0   0  8
-  [10] .rela.eh_frame    RELA            0000000000000000 000808 000018 18   I 11   9  8
-  [11] .symtab           SYMTAB          0000000000000000 000348 000198 18     12   6  8
-  [12] .strtab           STRTAB          0000000000000000 0004e0 000082 00      0   0  1
-  [13] .shstrtab         STRTAB          0000000000000000 000820 000079 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 0002a4 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 0005d8 0002e8 18   I 11   1  8
+  [ 3] .data             PROGBITS        0000000000000000 0002e4 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 0002e4 000000 00  WA  0   0  1
+  [ 5] .rodata.cst8      PROGBITS        0000000000000000 0002e8 000018 08  AM  0   0  8
+  [ 6] .comment          PROGBITS        0000000000000000 000300 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00032e 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 000330 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 000350 000068 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 0008c0 000018 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 0003b8 000198 18     12   6  8
+  [12] .strtab           STRTAB          0000000000000000 000550 000082 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 0008d8 000079 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -3,18 +3,18 @@
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS power.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000010     0 NOTYPE  LOCAL  DEFAULT    5 .LC2
      4: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC0
      5: 0000000000000008     0 NOTYPE  LOCAL  DEFAULT    5 .LC1
-     6: 0000000000000000   564 FUNC    GLOBAL DEFAULT    1 power
+     6: 0000000000000000   676 FUNC    GLOBAL DEFAULT    1 power
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
     10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND remove_zeroes
-    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
-    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND natural_logarithm
-    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply
-    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exponential
-    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
+    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND natural_logarithm
+    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply
+    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exponential
     16: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND power_integer
```

##### readelf --wide --relocs {}

```diff
@@ -1,35 +1,38 @@
 
-Relocation section '.rela.text' at offset 0x568 contains 28 entries:
+Relocation section '.rela.text' at offset 0x5d8 contains 31 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000031  0000000300000002 R_X86_64_PC32          0000000000000010 .LC2 - 4
 0000000000000039  0000000400000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
 0000000000000041  0000000500000002 R_X86_64_PC32          0000000000000008 .LC1 - 4
 000000000000005d  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 0000000000000072  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000007d  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000008e  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000a2  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 00000000000000b0  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 00000000000000b8  0000000a00000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 00000000000000c0  0000000a00000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
-00000000000000cd  0000000b00000004 R_X86_64_PLT32         0000000000000000 strchr - 4
-00000000000000e1  0000000c00000004 R_X86_64_PLT32         0000000000000000 natural_logarithm - 4
-00000000000000ec  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000000f7  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000106  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000117  0000000d00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
-0000000000000122  0000000e00000004 R_X86_64_PLT32         0000000000000000 exponential - 4
-000000000000012d  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000135  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000013d  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000145  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000152  0000000b00000004 R_X86_64_PLT32         0000000000000000 strchr - 4
-0000000000000162  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001d2  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000213  0000001000000004 R_X86_64_PLT32         0000000000000000 power_integer - 4
-000000000000021e  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000226  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000de  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000107  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000010f  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000131  0000000c00000004 R_X86_64_PLT32         0000000000000000 strchr - 4
+0000000000000145  0000000d00000004 R_X86_64_PLT32         0000000000000000 natural_logarithm - 4
+0000000000000150  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000015b  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000016a  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000017b  0000000e00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
+0000000000000186  0000000f00000004 R_X86_64_PLT32         0000000000000000 exponential - 4
+0000000000000191  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000199  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000001a1  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000001a9  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000001b6  0000000c00000004 R_X86_64_PLT32         0000000000000000 strchr - 4
+00000000000001c6  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000232  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000273  0000001000000004 R_X86_64_PLT32         0000000000000000 power_integer - 4
+000000000000027e  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000286  0000000b00000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x808 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x8c0 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,15 +9,15 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000234
+00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..00000000000002a4
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 5 to 000000000000000b
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 2 to 000000000000000d
@@ -30,29 +30,30 @@
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 4 to 0000000000000014
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_advance_loc: 7 to 000000000000001b
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc2: 345 to 0000000000000174
+  DW_CFA_advance_loc1: 252 to 0000000000000117
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000000178
+  DW_CFA_advance_loc: 4 to 000000000000011b
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000179
+  DW_CFA_advance_loc: 1 to 000000000000011c
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 000000000000017b
+  DW_CFA_advance_loc: 2 to 000000000000011e
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000017d
+  DW_CFA_advance_loc: 2 to 0000000000000120
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000017f
+  DW_CFA_advance_loc: 2 to 0000000000000122
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000181
+  DW_CFA_advance_loc: 2 to 0000000000000124
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 7 to 0000000000000188
+  DW_CFA_advance_loc: 4 to 0000000000000128
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+  DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -8,179 +8,206 @@
 	endbr64
 	push   %r15
 	mov    %rdi,%r8
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
-	mov    %rsi,%rbp
+	mov    %rdx,%rbp
 	push   %rbx
-	mov    %rdx,%rbx
+	mov    %rsi,%rbx
 	sub    $0x18,%rsp
 	test   %rdx,%rdx
-	js     1a0 <power+0x1a0>
+	js     1f8 <power+0x1f8>
 	pxor   %xmm0,%xmm0
 	cvtsi2sd %rdx,%xmm0
 	movsd  0x0(%rip),%xmm1        
  R_X86_64_PC32	.LC2-0x4
 	mulsd  0x0(%rip),%xmm0        
  R_X86_64_PC32	.LC0-0x4
 	divsd  0x0(%rip),%xmm0        
  R_X86_64_PC32	.LC1-0x4
 	comisd %xmm1,%xmm0
-	jae    188 <power+0x188>
+	jae    1e0 <power+0x1e0>
 	cvttsd2si %xmm0,%r14
 	mov    %r8,%rdi
 	mov    %r8,0x8(%rsp)
 	call   61 <power+0x61>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax),%rdx
 	mov    %rdx,%rdi
 	mov    %rdx,(%rsp)
 	call   76 <power+0x76>
  R_X86_64_PLT32	calloc-0x4
-	mov    %rbp,%rdi
-	mov    %rax,%r13
+	mov    %rbx,%rdi
+	mov    %rax,%r12
 	call   81 <power+0x81>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x1(%rax),%r15
 	mov    %r15,%rdi
 	call   92 <power+0x92>
  R_X86_64_PLT32	calloc-0x4
 	mov    (%rsp),%rdx
 	mov    0x8(%rsp),%rsi
-	mov    %r13,%rdi
-	mov    %rax,%r12
+	mov    %r12,%rdi
+	mov    %rax,%r13
 	call   a6 <power+0xa6>
  R_X86_64_PLT32	memcpy-0x4
-	mov    %rbp,%rsi
 	mov    %r15,%rdx
-	mov    %r12,%rdi
+	mov    %rbx,%rsi
+	mov    %r13,%rdi
 	call   b4 <power+0xb4>
  R_X86_64_PLT32	memcpy-0x4
-	mov    %r13,%rdi
+	mov    %r12,%rdi
 	call   bc <power+0xbc>
  R_X86_64_PLT32	remove_zeroes-0x4
-	mov    %r12,%rdi
+	mov    %r13,%rdi
 	call   c4 <power+0xc4>
  R_X86_64_PLT32	remove_zeroes-0x4
-	mov    $0x2e,%esi
+	cmpb   $0x30,(%r12)
+	jne    128 <power+0x128>
+	cmpb   $0x0,0x1(%r12)
+	jne    128 <power+0x128>
+	mov    $0x1,%esi
+	mov    $0x2,%edi
+	call   e2 <power+0xe2>
+ R_X86_64_PLT32	calloc-0x4
+	cmpb   $0x30,0x0(%r13)
+	mov    %rax,%r14
+	jne    290 <power+0x290>
+	cmpb   $0x0,0x1(%r13)
+	jne    290 <power+0x290>
+	mov    $0x31,%edx
 	mov    %r12,%rdi
-	call   d1 <power+0xd1>
+	mov    %dx,(%rax)
+	call   10b <power+0x10b>
+ R_X86_64_PLT32	free-0x4
+	mov    %r13,%rdi
+	call   113 <power+0x113>
+ R_X86_64_PLT32	free-0x4
+	add    $0x18,%rsp
+	mov    %r14,%rax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+	nopl   (%rax)
+	mov    $0x2e,%esi
+	mov    %r13,%rdi
+	call   135 <power+0x135>
  R_X86_64_PLT32	strchr-0x4
 	test   %rax,%rax
-	je     1c0 <power+0x1c0>
+	je     220 <power+0x220>
 	mov    %r14,%rsi
-	mov    %r13,%rdi
-	call   e5 <power+0xe5>
- R_X86_64_PLT32	natural_logarithm-0x4
 	mov    %r12,%rdi
-	mov    %rax,%r15
-	call   f0 <power+0xf0>
+	call   149 <power+0x149>
+ R_X86_64_PLT32	natural_logarithm-0x4
+	mov    %r13,%rdi
+	mov    %rax,%rbx
+	call   154 <power+0x154>
  R_X86_64_PLT32	strlen-0x4
-	mov    %r15,%rdi
-	mov    %rax,%rbp
-	call   fb <power+0xfb>
+	mov    %rbx,%rdi
+	mov    %rax,%r15
+	call   15f <power+0x15f>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
-	lea    0x3(%rbp,%rax,1),%rdi
-	call   10a <power+0x10a>
+	lea    0x3(%r15,%rax,1),%rdi
+	call   16e <power+0x16e>
  R_X86_64_PLT32	calloc-0x4
-	mov    %r15,%rsi
-	mov    %r12,%rdi
+	mov    %rbx,%rsi
+	mov    %r13,%rdi
 	mov    %rax,%rdx
-	mov    %rax,%rbp
-	call   11b <power+0x11b>
+	mov    %rax,%r15
+	call   17f <power+0x17f>
  R_X86_64_PLT32	multiply-0x4
 	mov    %r14,%rsi
-	mov    %rbp,%rdi
-	call   126 <power+0x126>
+	mov    %r15,%rdi
+	call   18a <power+0x18a>
  R_X86_64_PLT32	exponential-0x4
-	mov    %r13,%rdi
+	mov    %r12,%rdi
 	mov    %rax,%r14
-	call   131 <power+0x131>
+	call   195 <power+0x195>
  R_X86_64_PLT32	free-0x4
-	mov    %r12,%rdi
-	call   139 <power+0x139>
+	mov    %r13,%rdi
+	call   19d <power+0x19d>
  R_X86_64_PLT32	free-0x4
-	mov    %r15,%rdi
-	call   141 <power+0x141>
+	mov    %rbx,%rdi
+	call   1a5 <power+0x1a5>
  R_X86_64_PLT32	free-0x4
-	mov    %rbp,%rdi
-	call   149 <power+0x149>
+	mov    %r15,%rdi
+	call   1ad <power+0x1ad>
  R_X86_64_PLT32	free-0x4
 	mov    %r14,%rdi
 	mov    $0x2e,%esi
-	call   156 <power+0x156>
+	call   1ba <power+0x1ba>
  R_X86_64_PLT32	strchr-0x4
 	mov    %r14,%rdi
 	sub    %r14,%rax
-	lea    0x1(%rbx,%rax,1),%rbx
-	call   166 <power+0x166>
+	lea    0x1(%rbp,%rax,1),%rbx
+	call   1ca <power+0x1ca>
  R_X86_64_PLT32	strlen-0x4
 	cmp    %rax,%rbx
-	jae    170 <power+0x170>
+	jae    113 <power+0x113>
 	movb   $0x0,(%r14,%rbx,1)
-	add    $0x18,%rsp
-	mov    %r14,%rax
-	pop    %rbx
-	pop    %rbp
-	pop    %r12
-	pop    %r13
-	pop    %r14
-	pop    %r15
-	ret
-	nopw   0x0(%rax,%rax,1)
+	jmp    113 <power+0x113>
+	nopl   (%rax)
 	subsd  %xmm1,%xmm0
 	cvttsd2si %xmm0,%r14
 	btc    $0x3f,%r14
 	jmp    54 <power+0x54>
 	nopl   0x0(%rax,%rax,1)
 	mov    %rdx,%rax
 	and    $0x1,%edx
 	pxor   %xmm0,%xmm0
 	shr    %rax
 	or     %rdx,%rax
 	cvtsi2sd %rax,%xmm0
 	addsd  %xmm0,%xmm0
 	jmp    2d <power+0x2d>
-	xchg   %ax,%ax
-	movzbl 0x0(%rbp),%r15d
-	xor    %ebx,%ebx
-	mov    %rbp,%rdi
+	cs nopw 0x0(%rax,%rax,1)
+	movzbl (%rbx),%r15d
+	xor    %ebp,%ebp
+	mov    %rbx,%rdi
 	cmp    $0x2d,%r15b
-	sete   %bl
-	call   1d6 <power+0x1d6>
+	sete   %bpl
+	call   236 <power+0x236>
  R_X86_64_PLT32	strlen-0x4
-	cmp    %rbx,%rax
-	jbe    230 <power+0x230>
-	lea    0x0(%rbp,%rbx,1),%rdx
+	cmp    %rbp,%rax
+	jbe    2a0 <power+0x2a0>
+	lea    (%rbx,%rbp,1),%rdx
 	xor    %esi,%esi
-	add    %rax,%rbp
-	nopl   (%rax)
+	add    %rax,%rbx
+	nopl   0x0(%rax)
 	movsbq (%rdx),%rax
 	lea    (%rsi,%rsi,4),%rcx
 	add    $0x1,%rdx
 	lea    -0x30(%rax,%rcx,2),%rsi
-	cmp    %rbp,%rdx
-	jne    1e8 <power+0x1e8>
+	cmp    %rdx,%rbx
+	jne    248 <power+0x248>
 	mov    %rsi,%rax
 	mov    %r14,%rdx
-	mov    %r13,%rdi
+	mov    %r12,%rdi
 	neg    %rax
 	cmp    $0x2d,%r15b
 	cmove  %rax,%rsi
-	call   217 <power+0x217>
+	call   277 <power+0x277>
  R_X86_64_PLT32	power_integer-0x4
-	mov    %r13,%rdi
 	mov    %rax,%r14
-	call   222 <power+0x222>
- R_X86_64_PLT32	free-0x4
 	mov    %r12,%rdi
-	call   22a <power+0x22a>
+	call   282 <power+0x282>
+ R_X86_64_PLT32	free-0x4
+	mov    %r13,%rdi
+	call   28a <power+0x28a>
  R_X86_64_PLT32	free-0x4
-	jmp    170 <power+0x170>
+	jmp    113 <power+0x113>
 	nop
+	mov    $0x30,%eax
+	mov    %ax,(%r14)
+	jmp    27a <power+0x27a>
+	nopl   0x0(%rax,%rax,1)
 	xor    %esi,%esi
-	jmp    1fe <power+0x1fe>
+	jmp    25e <power+0x25e>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
-  0x00000020 00000000 34020000 00460e10 8f02450e ....4....F....E.
+  0x00000020 00000000 a4020000 00460e10 8f02450e .........F....E.
   0x00000030 188e0342 0e208d04 420e288c 05410e30 ...B. ..B.(..A.0
-  0x00000040 8606440e 38830747 0e500359 010a0e38 ..D.8..G.P.Y...8
-  0x00000050 440e3041 0e28420e 20420e18 420e1042 D.0A.(B. B..B..B
-  0x00000060 0e08470b 00000000                   ..G.....
+  0x00000040 8606440e 38830747 0e5002fc 0a0e3844 ..D.8..G.P....8D
+  0x00000050 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
+  0x00000060 08440b00 00000000                   .D......
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,12 +1,12 @@
 
 Hex dump of section '.strtab':
   0x00000000 00706f77 65722e63 002e4c43 32002e4c .power.c..LC2..L
   0x00000010 4330002e 4c433100 706f7765 72007374 C0..LC1.power.st
   0x00000020 726c656e 0063616c 6c6f6300 6d656d63 rlen.calloc.memc
   0x00000030 70790072 656d6f76 655f7a65 726f6573 py.remove_zeroes
-  0x00000040 00737472 63687200 6e617475 72616c5f .strchr.natural_
-  0x00000050 6c6f6761 72697468 6d006d75 6c746970 logarithm.multip
-  0x00000060 6c790065 78706f6e 656e7469 616c0066 ly.exponential.f
-  0x00000070 72656500 706f7765 725f696e 74656765 ree.power_intege
+  0x00000040 00667265 65007374 72636872 006e6174 .free.strchr.nat
+  0x00000050 7572616c 5f6c6f67 61726974 686d006d ural_logarithm.m
+  0x00000060 756c7469 706c7900 6578706f 6e656e74 ultiply.exponent
+  0x00000070 69616c00 706f7765 725f696e 74656765 ial.power_intege
   0x00000080 7200                                r.
```

### Comparing `arithmetica-py-1.0.225/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.226/src/python-module/libbasic_math_operations.a`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.225/src/python-module/module.c` & `arithmetica-py-1.0.226/src/python-module/module.c`

 * *Files identical despite different names*

