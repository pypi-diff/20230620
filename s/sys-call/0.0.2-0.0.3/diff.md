# Comparing `tmp/sys-call-0.0.2.tar.gz` & `tmp/sys-call-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sys-call-0.0.2.tar", last modified: Mon Jun 19 19:53:35 2023, max compression
+gzip compressed data, was "sys-call-0.0.3.tar", last modified: Mon Jun 19 22:08:22 2023, max compression
```

## Comparing `sys-call-0.0.2.tar` & `sys-call-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 19:53:20.000000 sys-call-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-19 19:53:35.451347 sys-call-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-06-19 19:53:20.000000 sys-call-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:53:35.451347 sys-call-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-19 19:53:20.000000 sys-call-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/sys_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 19:53:35.000000 sys-call-0.0.2/sys_call.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:53:35.451347 sys-call-0.0.2/syscall/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 19:53:20.000000 sys-call-0.0.2/syscall/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6470 2023-06-19 19:53:20.000000 sys-call-0.0.2/syscall/syscall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:08:22.549822 sys-call-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 22:08:03.000000 sys-call-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-06-19 22:08:22.549822 sys-call-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-19 22:08:03.000000 sys-call-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:08:22.549822 sys-call-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 22:08:03.000000 sys-call-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:08:22.549822 sys-call-0.0.3/sys_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 22:08:22.000000 sys-call-0.0.3/sys_call.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:08:22.549822 sys-call-0.0.3/syscall/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 22:08:03.000000 sys-call-0.0.3/syscall/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6315 2023-06-19 22:08:03.000000 sys-call-0.0.3/syscall/syscall.py
```

### Comparing `sys-call-0.0.2/LICENSE` & `sys-call-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sys-call-0.0.2/PKG-INFO` & `sys-call-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,135 @@
 Metadata-Version: 2.1
 Name: sys-call
-Version: 0.0.2
+Version: 0.0.3
 Summary: Linux Syscall implementations, calling conventions, and shellcode examples.
 Home-page: http://github.com/lbirchler/sys-call/
 Author: Lawrence Birchler
 Author-email: bplyr@tutanota.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sys-call
 
-CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
+CLI tool to display Linux syscall implementations, calling conventions, and shellcode examples.
 
-Supported architectures: arm, arm64, x64, x86
+Supported Architectures: 
+- arm
+- arm64
+- x86
+- x64
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh) 
 - Shellcode Examples: [shell-storm](http://shell-storm.org/shellcode/index.html)
 
 ## Install
 ```
 pip install sys-call
 ```
 
 ## Usage 
-
-### `syscall-info`
 ```
-usage: syscall-info [-h] [-a {arm,arm64,x64,x86}] [--update] [syscall ...]
+usage: sys-call [-h] [-a {arm,arm64,x64,x86}] {shellcode,info} ...
 
 positional arguments:
-  syscall               syscall name(s)
+  {shellcode,info}      commands
 
 options:
   -h, --help            show this help message and exit
   -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
                                  defaults to x64
-  --update              Update syscall database
+```
+
+### `sys-call info`
+```
+usage: sys-call info [-h] [--update] [syscall ...]
+
+positional arguments:
+  syscall     syscall name(s)
+
+options:
+  -h, --help  show this help message and exit
+  --update    Update syscall database
 ```
 
 **Examples**
 
 For single syscall:
 ```
-$ syscall-info execve
+$ sys-call info execve
                                                                   x64 Syscalls                                                                  
 ┏━━━━┳━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name   ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi             ┃ arg2    rdx             ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 59 │ execve │ 0x3b        │ const char *filename │ const char *const *argv │ const char *const *envp │             │            │            │
 └────┴────────┴─────────────┴──────────────────────┴─────────────────────────┴─────────────────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For multiple syscalls:
 ```
-$ syscall-info open read write
+$ sys-call info open read write
                                                         x64 Syscalls                                                        
 ┏━━━━┳━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name  ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi     ┃ arg2    rdx  ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 2  │ open  │ 0x02        │ const char *filename │ int flags       │ umode_t mode │             │            │            │
 │ 0  │ read  │ 0x00        │ unsigned int fd      │ char *buf       │ size_t count │             │            │            │
 │ 1  │ write │ 0x01        │ unsigned int fd      │ const char *buf │ size_t count │             │            │            │
-│ 60 │ exit  │ 0x3c        │ int error_code       │                 │              │             │            │            │
 └────┴───────┴─────────────┴──────────────────────┴─────────────────┴──────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For all syscalls:
 ```
-$ syscall-info 
+$ sys-call info 
                                                                x64 Syscalls                                                                
 ┏━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┓
 ┃ nr  ┃ name           ┃ return  rax ┃ arg0    rdi    ┃ arg1    rsi    ┃ arg2    rdx    ┃ arg3    r10    ┃ arg4    r8    ┃ arg5    r9     ┃
 ┡━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━┩
 │ 67  │ shmdt          │ 0x43        │ char *shmaddr  │                │                │                │               │                │
 │ 112 │ setsid         │ 0x70        │                │                │                │                │               │                │
 │ 68  │ msgget         │ 0x44        │ key_t key      │ int msgflg     │                │                │               │                │
 │ 0   │ read           │ 0x00        │ unsigned int   │ char *buf      │ size_t count   │                │               │                │
 │     │                │             │ fd             │                │                │                │               │                │
 │ 1   │ write          │ 0x01        │ unsigned int   │ const char     │ size_t count   │                │               │                │
 │     │                │             │ fd             │ *buf           │                │                │               │                │
 ...
 ```
 
-Update syscall database:
+Update sys-call database:
 ```
-$ syscall-info --update
+$ sys-call info --update
 [+] Updated x64 syscalls
 [+] Updated arm64 syscalls
 [+] Updated arm syscalls
 [+] Updated x86 syscalls
 [+] Saved syscall db to: ./syscalldb.json
 ```
 
-### `syscall-shellcode`
+### `sys-call shellcode`
 ```
-usage: syscall-shellcode [-h] [-a {arm,arm64,x64,x86}] [--get GET] [syscall ...]
+usage: sys-call shellcode [-h] [--get GET] [syscall ...]
 
 positional arguments:
-  syscall               syscall name(s)
+  syscall     syscall name(s)
 
 options:
-  -h, --help            show this help message and exit
-  -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
-                                 defaults to x64
-  --get GET             shell-storm shellcode id
+  -h, --help  show this help message and exit
+  --get GET   download shell-storm example; specify id
 ```
 
 **Examples**
 
 Search for execve shellcode examples:
 ```
-$ syscall-shellcode execve
-                                                      x86 Shellcode 
+$ sys-call shellcode execve
+                                                      x64 Shellcode 
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━┓
 ┃ author                        ┃ platform     ┃ desc                                                              ┃ id  ┃
 ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━┩
 │ ZadYree, vaelio and DaShrooms │ Linux/x86-64 │ execveat("/bin//sh") - 29 bytes                                   │ 905 │
 │ 10n1z3d                       │ Linux/x86-64 │ execve(/sbin/iptables, [/sbin/iptables, -F], NULL) - 49 bytes     │ 683 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/ash,NULL,NULL) + XOR - 85 bytes         │ 815 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/csh, [/bin/csh, NULL]) + XOR - 87 bytes │ 816 │
@@ -129,15 +139,15 @@
 │ hophet                        │ Linux/x86-64 │ execve(/bin/sh, [/bin/sh], NULL) - 33 bytes                       │ 76  │
 │ zbt                           │ Linux/x86-64 │ execve(/bin/sh); - 30 bytes                                       │ 603 │
 └───────────────────────────────┴──────────────┴───────────────────────────────────────────────────────────────────┴─────┘
 ```
 
 Download shellcode example: 
 ```
-$ syscall-shellcode --get 76
+$ sys-call shellcode --get 76
 
 # [Linux/X86-64]
 # Dummy for shellcode:
 # execve("/bin/sh", ["/bin/sh"], NULL)
 # hophet [at] gmail.com
 
 .text
```

### Comparing `sys-call-0.0.2/README.md` & `sys-call-0.0.3/sys_call.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,135 @@
+Metadata-Version: 2.1
+Name: sys-call
+Version: 0.0.3
+Summary: Linux Syscall implementations, calling conventions, and shellcode examples.
+Home-page: http://github.com/lbirchler/sys-call/
+Author: Lawrence Birchler
+Author-email: bplyr@tutanota.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sys-call
 
-CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
+CLI tool to display Linux syscall implementations, calling conventions, and shellcode examples.
 
-Supported architectures: arm, arm64, x64, x86
+Supported Architectures: 
+- arm
+- arm64
+- x86
+- x64
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh) 
 - Shellcode Examples: [shell-storm](http://shell-storm.org/shellcode/index.html)
 
 ## Install
 ```
 pip install sys-call
 ```
 
 ## Usage 
-
-### `syscall-info`
 ```
-usage: syscall-info [-h] [-a {arm,arm64,x64,x86}] [--update] [syscall ...]
+usage: sys-call [-h] [-a {arm,arm64,x64,x86}] {shellcode,info} ...
 
 positional arguments:
-  syscall               syscall name(s)
+  {shellcode,info}      commands
 
 options:
   -h, --help            show this help message and exit
   -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
                                  defaults to x64
-  --update              Update syscall database
+```
+
+### `sys-call info`
+```
+usage: sys-call info [-h] [--update] [syscall ...]
+
+positional arguments:
+  syscall     syscall name(s)
+
+options:
+  -h, --help  show this help message and exit
+  --update    Update syscall database
 ```
 
 **Examples**
 
 For single syscall:
 ```
-$ syscall-info execve
+$ sys-call info execve
                                                                   x64 Syscalls                                                                  
 ┏━━━━┳━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name   ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi             ┃ arg2    rdx             ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 59 │ execve │ 0x3b        │ const char *filename │ const char *const *argv │ const char *const *envp │             │            │            │
 └────┴────────┴─────────────┴──────────────────────┴─────────────────────────┴─────────────────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For multiple syscalls:
 ```
-$ syscall-info open read write
+$ sys-call info open read write
                                                         x64 Syscalls                                                        
 ┏━━━━┳━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name  ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi     ┃ arg2    rdx  ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 2  │ open  │ 0x02        │ const char *filename │ int flags       │ umode_t mode │             │            │            │
 │ 0  │ read  │ 0x00        │ unsigned int fd      │ char *buf       │ size_t count │             │            │            │
 │ 1  │ write │ 0x01        │ unsigned int fd      │ const char *buf │ size_t count │             │            │            │
-│ 60 │ exit  │ 0x3c        │ int error_code       │                 │              │             │            │            │
 └────┴───────┴─────────────┴──────────────────────┴─────────────────┴──────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For all syscalls:
 ```
-$ syscall-info 
+$ sys-call info 
                                                                x64 Syscalls                                                                
 ┏━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┓
 ┃ nr  ┃ name           ┃ return  rax ┃ arg0    rdi    ┃ arg1    rsi    ┃ arg2    rdx    ┃ arg3    r10    ┃ arg4    r8    ┃ arg5    r9     ┃
 ┡━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━┩
 │ 67  │ shmdt          │ 0x43        │ char *shmaddr  │                │                │                │               │                │
 │ 112 │ setsid         │ 0x70        │                │                │                │                │               │                │
 │ 68  │ msgget         │ 0x44        │ key_t key      │ int msgflg     │                │                │               │                │
 │ 0   │ read           │ 0x00        │ unsigned int   │ char *buf      │ size_t count   │                │               │                │
 │     │                │             │ fd             │                │                │                │               │                │
 │ 1   │ write          │ 0x01        │ unsigned int   │ const char     │ size_t count   │                │               │                │
 │     │                │             │ fd             │ *buf           │                │                │               │                │
 ...
 ```
 
-Update syscall database:
+Update sys-call database:
 ```
-$ syscall-info --update
+$ sys-call info --update
 [+] Updated x64 syscalls
 [+] Updated arm64 syscalls
 [+] Updated arm syscalls
 [+] Updated x86 syscalls
 [+] Saved syscall db to: ./syscalldb.json
 ```
 
-### `syscall-shellcode`
+### `sys-call shellcode`
 ```
-usage: syscall-shellcode [-h] [-a {arm,arm64,x64,x86}] [--get GET] [syscall ...]
+usage: sys-call shellcode [-h] [--get GET] [syscall ...]
 
 positional arguments:
-  syscall               syscall name(s)
+  syscall     syscall name(s)
 
 options:
-  -h, --help            show this help message and exit
-  -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
-                                 defaults to x64
-  --get GET             shell-storm shellcode id
+  -h, --help  show this help message and exit
+  --get GET   download shell-storm example; specify id
 ```
 
 **Examples**
 
 Search for execve shellcode examples:
 ```
-$ syscall-shellcode execve
-                                                      x86 Shellcode 
+$ sys-call shellcode execve
+                                                      x64 Shellcode 
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━┓
 ┃ author                        ┃ platform     ┃ desc                                                              ┃ id  ┃
 ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━┩
 │ ZadYree, vaelio and DaShrooms │ Linux/x86-64 │ execveat("/bin//sh") - 29 bytes                                   │ 905 │
 │ 10n1z3d                       │ Linux/x86-64 │ execve(/sbin/iptables, [/sbin/iptables, -F], NULL) - 49 bytes     │ 683 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/ash,NULL,NULL) + XOR - 85 bytes         │ 815 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/csh, [/bin/csh, NULL]) + XOR - 87 bytes │ 816 │
@@ -116,15 +139,15 @@
 │ hophet                        │ Linux/x86-64 │ execve(/bin/sh, [/bin/sh], NULL) - 33 bytes                       │ 76  │
 │ zbt                           │ Linux/x86-64 │ execve(/bin/sh); - 30 bytes                                       │ 603 │
 └───────────────────────────────┴──────────────┴───────────────────────────────────────────────────────────────────┴─────┘
 ```
 
 Download shellcode example: 
 ```
-$ syscall-shellcode --get 76
+$ sys-call shellcode --get 76
 
 # [Linux/X86-64]
 # Dummy for shellcode:
 # execve("/bin/sh", ["/bin/sh"], NULL)
 # hophet [at] gmail.com
 
 .text
```

### Comparing `sys-call-0.0.2/setup.py` & `sys-call-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,12 +36,11 @@
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
     ],
     entry_points={
         'console_scripts': [
-            'syscall-info=syscall.syscall:CLI.info',
-            'syscall-shellcode=syscall.syscall:CLI.shellcode'
+            'sys-call=syscall.syscall:main'
         ]
     }
 )
```

### Comparing `sys-call-0.0.2/sys_call.egg-info/PKG-INFO` & `sys-call-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,122 @@
-Metadata-Version: 2.1
-Name: sys-call
-Version: 0.0.2
-Summary: Linux Syscall implementations, calling conventions, and shellcode examples.
-Home-page: http://github.com/lbirchler/sys-call/
-Author: Lawrence Birchler
-Author-email: bplyr@tutanota.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sys-call
 
-CLI tool to display Linux Syscall implementations, calling conventions, and shellcode examples.
+CLI tool to display Linux syscall implementations, calling conventions, and shellcode examples.
 
-Supported architectures: arm, arm64, x64, x86
+Supported Architectures: 
+- arm
+- arm64
+- x86
+- x64
 
 Data Sources:
 - Syscall implementations and calling conventions: [syscall.sh](https://syscall.sh) 
 - Shellcode Examples: [shell-storm](http://shell-storm.org/shellcode/index.html)
 
 ## Install
 ```
 pip install sys-call
 ```
 
 ## Usage 
-
-### `syscall-info`
 ```
-usage: syscall-info [-h] [-a {arm,arm64,x64,x86}] [--update] [syscall ...]
+usage: sys-call [-h] [-a {arm,arm64,x64,x86}] {shellcode,info} ...
 
 positional arguments:
-  syscall               syscall name(s)
+  {shellcode,info}      commands
 
 options:
   -h, --help            show this help message and exit
   -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
                                  defaults to x64
-  --update              Update syscall database
+```
+
+### `sys-call info`
+```
+usage: sys-call info [-h] [--update] [syscall ...]
+
+positional arguments:
+  syscall     syscall name(s)
+
+options:
+  -h, --help  show this help message and exit
+  --update    Update syscall database
 ```
 
 **Examples**
 
 For single syscall:
 ```
-$ syscall-info execve
+$ sys-call info execve
                                                                   x64 Syscalls                                                                  
 ┏━━━━┳━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name   ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi             ┃ arg2    rdx             ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 59 │ execve │ 0x3b        │ const char *filename │ const char *const *argv │ const char *const *envp │             │            │            │
 └────┴────────┴─────────────┴──────────────────────┴─────────────────────────┴─────────────────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For multiple syscalls:
 ```
-$ syscall-info open read write
+$ sys-call info open read write
                                                         x64 Syscalls                                                        
 ┏━━━━┳━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ nr ┃ name  ┃ return  rax ┃ arg0    rdi          ┃ arg1    rsi     ┃ arg2    rdx  ┃ arg3    r10 ┃ arg4    r8 ┃ arg5    r9 ┃
 ┡━━━━╇━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ 2  │ open  │ 0x02        │ const char *filename │ int flags       │ umode_t mode │             │            │            │
 │ 0  │ read  │ 0x00        │ unsigned int fd      │ char *buf       │ size_t count │             │            │            │
 │ 1  │ write │ 0x01        │ unsigned int fd      │ const char *buf │ size_t count │             │            │            │
-│ 60 │ exit  │ 0x3c        │ int error_code       │                 │              │             │            │            │
 └────┴───────┴─────────────┴──────────────────────┴─────────────────┴──────────────┴─────────────┴────────────┴────────────┘
 ```
 
 For all syscalls:
 ```
-$ syscall-info 
+$ sys-call info 
                                                                x64 Syscalls                                                                
 ┏━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┓
 ┃ nr  ┃ name           ┃ return  rax ┃ arg0    rdi    ┃ arg1    rsi    ┃ arg2    rdx    ┃ arg3    r10    ┃ arg4    r8    ┃ arg5    r9     ┃
 ┡━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━┩
 │ 67  │ shmdt          │ 0x43        │ char *shmaddr  │                │                │                │               │                │
 │ 112 │ setsid         │ 0x70        │                │                │                │                │               │                │
 │ 68  │ msgget         │ 0x44        │ key_t key      │ int msgflg     │                │                │               │                │
 │ 0   │ read           │ 0x00        │ unsigned int   │ char *buf      │ size_t count   │                │               │                │
 │     │                │             │ fd             │                │                │                │               │                │
 │ 1   │ write          │ 0x01        │ unsigned int   │ const char     │ size_t count   │                │               │                │
 │     │                │             │ fd             │ *buf           │                │                │               │                │
 ...
 ```
 
-Update syscall database:
+Update sys-call database:
 ```
-$ syscall-info --update
+$ sys-call info --update
 [+] Updated x64 syscalls
 [+] Updated arm64 syscalls
 [+] Updated arm syscalls
 [+] Updated x86 syscalls
 [+] Saved syscall db to: ./syscalldb.json
 ```
 
-### `syscall-shellcode`
+### `sys-call shellcode`
 ```
-usage: syscall-shellcode [-h] [-a {arm,arm64,x64,x86}] [--get GET] [syscall ...]
+usage: sys-call shellcode [-h] [--get GET] [syscall ...]
 
 positional arguments:
-  syscall               syscall name(s)
+  syscall     syscall name(s)
 
 options:
-  -h, --help            show this help message and exit
-  -a {arm,arm64,x64,x86}, --arch {arm,arm64,x64,x86}
-                                 defaults to x64
-  --get GET             shell-storm shellcode id
+  -h, --help  show this help message and exit
+  --get GET   download shell-storm example; specify id
 ```
 
 **Examples**
 
 Search for execve shellcode examples:
 ```
-$ syscall-shellcode execve
-                                                      x86 Shellcode 
+$ sys-call shellcode execve
+                                                      x64 Shellcode 
 ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━┓
 ┃ author                        ┃ platform     ┃ desc                                                              ┃ id  ┃
 ┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━┩
 │ ZadYree, vaelio and DaShrooms │ Linux/x86-64 │ execveat("/bin//sh") - 29 bytes                                   │ 905 │
 │ 10n1z3d                       │ Linux/x86-64 │ execve(/sbin/iptables, [/sbin/iptables, -F], NULL) - 49 bytes     │ 683 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/ash,NULL,NULL) + XOR - 85 bytes         │ 815 │
 │ egeektronic                   │ Linux/x86-64 │ setreuid(0,0) execve(/bin/csh, [/bin/csh, NULL]) + XOR - 87 bytes │ 816 │
@@ -129,15 +126,15 @@
 │ hophet                        │ Linux/x86-64 │ execve(/bin/sh, [/bin/sh], NULL) - 33 bytes                       │ 76  │
 │ zbt                           │ Linux/x86-64 │ execve(/bin/sh); - 30 bytes                                       │ 603 │
 └───────────────────────────────┴──────────────┴───────────────────────────────────────────────────────────────────┴─────┘
 ```
 
 Download shellcode example: 
 ```
-$ syscall-shellcode --get 76
+$ sys-call shellcode --get 76
 
 # [Linux/X86-64]
 # Dummy for shellcode:
 # execve("/bin/sh", ["/bin/sh"], NULL)
 # hophet [at] gmail.com
 
 .text
```

### Comparing `sys-call-0.0.2/syscall/syscall.py` & `sys-call-0.0.3/syscall/syscall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import html
 import json
 import os
 import pathlib
 import re
 import sys
@@ -73,21 +75,14 @@
   for thread in threads: thread.join()
 
   with open(SYSCALL_DB, 'w') as f:
     json.dump(db, f, indent=4)
     info('Saved syscall db to: %s' % SYSCALL_DB)
 
 
-def get_syscall(arch: str, syscall: str | int) -> None | dict:
-  key = 'nr' if str(syscall).isnumeric() else 'name'
-  with open(SYSCALL_DB) as f:
-    syscalls = json.load(f)
-  return next((item for item in syscalls.get(arch) if item.get(key) == syscall), None)
-
-
 def print_table(title: str, cols: list, rows: list):
   table = Table(title=title)
   for col in cols: table.add_column(col)
   for row in rows: table.add_row(*row)
   console = Console()
   console.print(table, markup=False)
 
@@ -155,46 +150,42 @@
     print_table(
         title=f'{self.arch} Shellcode',
         cols=[col for col in examples[0]._fields],
         rows=[ex._asdict().values() for ex in examples]
     )
 
 
-class CLI:
-
-  # base parser
+def main():
   parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
   parser.add_argument(
       '-a', '--arch',
       choices=sorted(ARCHS),
       help=f'\t defaults to {DEFAULT_ARCH}',
       default=DEFAULT_ARCH,
   )
-  parser.add_argument('syscall', nargs='*', help='syscall name(s)')
 
-  @staticmethod
-  def shellcode():
-    parser = CLI.parser
-    parser.add_argument('--get', type=int, help='shell-storm shellcode id')
-    CLI.check_args(parser)
-    args = parser.parse_args()
+  cmd_parser = parser.add_subparsers(dest='cmd', help='commands')
+
+  info_parser = cmd_parser.add_parser('info')
+  info_parser.add_argument('--update', action='store_true', help='Update syscall database')
+  info_parser.add_argument('syscall', nargs='*', help='syscall name(s)')
+
+  shellcode_parser = cmd_parser.add_parser('shellcode')
+  shellcode_parser.add_argument('--get', type=int, help='download shell-storm example; specify id')
+  shellcode_parser.add_argument('syscall', nargs='*', help='syscall name(s)')
+
+  if len(sys.argv) < 2:
+    parser.print_usage()
+    sys.exit(1)
+
+  args = parser.parse_args()
+
+  if args.cmd == 'info':
+    if args.update:
+      sys.exit(update_syscall_db())
+    Syscalls(args.arch).display([sc for sc in args.syscall])
+  if args.cmd == 'shellcode':
     shellcode = Shellcode(args.arch)
     if args.get:
       shellcode.get(args.get)
     else:
       shellcode.display([sc for sc in args.syscall])
-
-  @staticmethod
-  def info():
-    parser = CLI.parser
-    parser.add_argument('--update', action='store_true', help='Update syscall database')
-    CLI.check_args(parser)
-    args = parser.parse_args()
-    if args.update:
-      sys.exit(update_syscall_db())
-    Syscalls(args.arch).display([sc for sc in args.syscall])
-
-  @staticmethod
-  def check_args(parser):
-    if len(sys.argv) < 2:
-      parser.print_usage()
-      sys.exit(1)
```

