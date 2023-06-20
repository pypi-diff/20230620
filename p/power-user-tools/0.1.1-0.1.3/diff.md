# Comparing `tmp/power-user-tools-0.1.1.tar.gz` & `tmp/power-user-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-user-tools-0.1.1.tar", last modified: Wed Feb 22 12:36:45 2023, max compression
+gzip compressed data, was "power-user-tools-0.1.3.tar", last modified: Tue Jun 20 11:07:22 2023, max compression
```

## Comparing `power-user-tools-0.1.1.tar` & `power-user-tools-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-02-22 12:36:45.976817 power-user-tools-0.1.1/
--rw-r--r--   0 davmeyer   (503) staff       (20)     1095 2022-11-24 13:41:28.000000 power-user-tools-0.1.1/LICENSE
--rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-02-22 12:36:45.976418 power-user-tools-0.1.1/PKG-INFO
--rw-r--r--   0 davmeyer   (503) staff       (20)      382 2022-11-25 14:55:50.000000 power-user-tools-0.1.1/README.md
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-02-22 12:36:45.968347 power-user-tools-0.1.1/commands/
--rw-r--r--   0 davmeyer   (503) staff       (20)        0 2022-11-24 15:12:46.000000 power-user-tools-0.1.1/commands/__init__.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     1220 2023-02-22 12:28:12.000000 power-user-tools-0.1.1/commands/devutils.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     6076 2023-02-14 08:13:30.000000 power-user-tools-0.1.1/commands/dockertools.py
--rw-r--r--   0 davmeyer   (503) staff       (20)     4147 2023-02-06 12:50:35.000000 power-user-tools-0.1.1/commands/helpers.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     1740 2022-11-25 16:02:15.000000 power-user-tools-0.1.1/commands/sshutils.py
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-02-22 12:36:45.970781 power-user-tools-0.1.1/power_user_tools.egg-info/
--rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/PKG-INFO
--rw-r--r--   0 davmeyer   (503) staff       (20)      562 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/SOURCES.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/dependency_links.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)      320 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/entry_points.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/not-zip-safe
--rw-r--r--   0 davmeyer   (503) staff       (20)       93 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/requires.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        9 2023-02-22 12:36:45.000000 power-user-tools-0.1.1/power_user_tools.egg-info/top_level.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)       38 2023-02-22 12:36:45.976979 power-user-tools-0.1.1/setup.cfg
--rw-r--r--   0 davmeyer   (503) staff       (20)     1799 2023-02-22 12:28:27.000000 power-user-tools-0.1.1/setup.py
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-02-22 12:36:45.975833 power-user-tools-0.1.1/shell/
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      521 2020-12-23 09:23:36.000000 power-user-tools-0.1.1/shell/dtimg
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      645 2020-02-11 08:02:45.000000 power-user-tools-0.1.1/shell/dtip
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      426 2020-02-11 08:02:45.000000 power-user-tools-0.1.1/shell/dtnet
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      200 2020-10-13 14:08:48.000000 power-user-tools-0.1.1/shell/dtports
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      239 2020-11-17 08:09:21.000000 power-user-tools-0.1.1/shell/dtrestart
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      492 2021-01-15 06:06:32.000000 power-user-tools-0.1.1/shell/dtrm
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      235 2020-02-11 08:02:45.000000 power-user-tools-0.1.1/shell/dtstart
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      233 2020-02-11 08:02:45.000000 power-user-tools-0.1.1/shell/dtstop
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      416 2022-11-25 14:27:10.000000 power-user-tools-0.1.1/shell/xpgrmhistory
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      502 2022-11-25 14:27:10.000000 power-user-tools-0.1.1/shell/xppr
--rwxr-xr-x   0 davmeyer   (503) staff       (20)       55 2022-11-25 14:27:10.000000 power-user-tools-0.1.1/shell/xprandpw
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.821775 power-user-tools-0.1.3/
+-rw-r--r--   0 davmeyer   (503) staff       (20)     1095 2022-11-24 13:41:28.000000 power-user-tools-0.1.3/LICENSE
+-rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-20 11:07:22.821965 power-user-tools-0.1.3/PKG-INFO
+-rw-r--r--   0 davmeyer   (503) staff       (20)      546 2023-06-06 07:35:46.000000 power-user-tools-0.1.3/README.md
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.810014 power-user-tools-0.1.3/commands/
+-rw-r--r--   0 davmeyer   (503) staff       (20)        0 2022-11-24 15:12:46.000000 power-user-tools-0.1.3/commands/__init__.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     1291 2023-06-05 13:36:27.000000 power-user-tools-0.1.3/commands/devutils.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     6468 2023-06-20 11:05:53.000000 power-user-tools-0.1.3/commands/dockertools.py
+-rw-r--r--   0 davmeyer   (503) staff       (20)     4158 2023-06-05 13:37:33.000000 power-user-tools-0.1.3/commands/helpers.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     2101 2023-06-05 13:42:55.000000 power-user-tools-0.1.3/commands/sshutils.py
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.812578 power-user-tools-0.1.3/power_user_tools.egg-info/
+-rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/PKG-INFO
+-rw-r--r--   0 davmeyer   (503) staff       (20)      572 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)      356 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/entry_points.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/not-zip-safe
+-rw-r--r--   0 davmeyer   (503) staff       (20)       93 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/requires.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        9 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/top_level.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)      152 2023-06-20 11:07:22.822638 power-user-tools-0.1.3/setup.cfg
+-rw-r--r--   0 davmeyer   (503) staff       (20)     1807 2023-06-20 11:06:54.000000 power-user-tools-0.1.3/setup.py
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.821150 power-user-tools-0.1.3/shell/
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      521 2020-12-23 09:23:36.000000 power-user-tools-0.1.3/shell/dtimg
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      645 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtip
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      426 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtnet
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      200 2020-10-13 14:08:48.000000 power-user-tools-0.1.3/shell/dtports
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      239 2020-11-17 08:09:21.000000 power-user-tools-0.1.3/shell/dtrestart
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      492 2021-01-15 06:06:32.000000 power-user-tools-0.1.3/shell/dtrm
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      235 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtstart
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      233 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtstop
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      416 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xpgrmhistory
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      502 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xppr
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)       55 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xprandpw
```

### Comparing `power-user-tools-0.1.1/LICENSE` & `power-user-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.1/PKG-INFO` & `power-user-tools-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-user-tools
-Version: 0.1.1
+Version: 0.1.3
 Summary: Power User Tools make your life so much easier
 Home-page: https://github.com/dameyerdave/power-user-tools
 Author: dameyerdave
 Author-email: dameyerdave@gmail.com
 License: MIT
 Keywords: power user tools ssh sshd reverse tunnel docker easy development
 Classifier: Programming Language :: Python :: 3
```

### Comparing `power-user-tools-0.1.1/commands/dockertools.py` & `power-user-tools-0.1.3/commands/dockertools.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,174 +10,209 @@
 import sh
 from commands.helpers import Executor as E, Message as M, TableOutput as T
 from os.path import isfile, isdir
 from dotenv import load_dotenv
 import traceback
 
 # declare the commands globally
-bash = sh.Command('bash')
-docker = sh.Command('docker')
+bash = sh.Command("bash")
+docker = sh.Command("docker")
 
 
 @click.command(context_settings={"ignore_unknown_options": True})
-@click.option('--shell', '-s', is_flag=True, default=False, help='open a shell to the container, basically exec')
-@click.option('--logs', '-l', is_flag=True, default=False, help='follows the logs, basically logs -f')
-@click.option('--ignore-override', '-i', is_flag=True, default=False, help='ignores the docker-compose.override.yml')
-@click.argument('docker_arguments', nargs=-1)
-def dcc(docker_arguments, shell=False, logs=False, ignore_override=False):
+@click.option(
+    "--shell",
+    "-s",
+    is_flag=True,
+    default=False,
+    help="open a shell to the container, basically exec",
+)
+@click.option(
+    "--logs",
+    "-l",
+    is_flag=True,
+    default=False,
+    help="follows the logs, basically logs -f",
+)
+@click.option(
+    "--build-plain",
+    "-b",
+    is_flag=True,
+    default=False,
+    help="build the containers in with --progress=plain",
+)
+@click.option(
+    "--ignore-override",
+    "-i",
+    is_flag=True,
+    default=False,
+    help="ignores the docker-compose.override.yml",
+)
+@click.argument("docker_arguments", nargs=-1)
+def dcc(
+    docker_arguments, shell=False, logs=False, build_plain=False, ignore_override=False
+):
     """
     DCC is a wrapper around docker-compose. If you are executing it inside a git
     repository it will set the following environment variables:
     - GIT_VERSION
     - GIT_BRANCH
     - GIT_LASTCOMMITDATE
     - GIT_COMMITHASH
-    You can use those in the build process to pass the git version information to the application. 
+    You can use those in the build process to pass the git version information to the application.
 
     Additionally it handles the docker-compose files. You can set the environment variable DCC_ENV to
     whatever string is in between docker-compose.<????>.yml. DCC will then take docker-compose.yml as
     the base file, the next is the docker-compose.<????>.yml and if a docker-compose.override.yml exists
     it will take this as the last compose file in the -f ordering.
     """
-    if not isfile('docker-compose.yml'):
-        M.error('There is no docker-compose.yml file in this directory!')
+    if not isfile("docker-compose.yml"):
+        M.error("There is no docker-compose.yml file in this directory!")
         sys.exit(1)
     dcc_env = None
     env = {
-        'GIT_VERSION': '?.?.?',
-        'GIT_BRANCH': 'N/A',
-        'GIT_LASTCOMMITDATE': 'N/A',
-        'GIT_COMMITHASH': 'N/A',
-        'UID': 0,
-        'GID': 0,
-        'UNAME': 'root'
+        "GIT_VERSION": "?.?.?",
+        "GIT_BRANCH": "N/A",
+        "GIT_LASTCOMMITDATE": "N/A",
+        "GIT_COMMITHASH": "N/A",
+        "UID": 0,
+        "GID": 0,
+        "UNAME": "root",
     }
-    if isfile('.env'):
-        load_dotenv('.env')
-        dcc_env = os.environ.get('DCC_ENV')
+    if isfile(".env"):
+        load_dotenv(".env")
+        dcc_env = os.environ.get("DCC_ENV")
         M.debug(f"Running DCC environment {dcc_env}.")
     else:
         M.warn(f"No .env file found in current directory: {os.getcwd()}")
-    if isdir('.git'):
-        if E.success('git rev-parse --is-inside-work-tree'):
-            env['GIT_VERSION'] = E.run('git describe --always')
-            env['GIT_BRANCH'] = E.run('git rev-parse --abbrev-ref HEAD')
-            env['GIT_LASTCOMMITDATE'] = E.run('git log -1 --format=%cI')
-            env['GIT_COMMITHASH'] = E.run('git rev-parse HEAD')
-        M.debug('Git repository detected.')
+    if isdir(".git"):
+        if E.success("git rev-parse --is-inside-work-tree"):
+            env["GIT_VERSION"] = E.run("git describe --always")
+            env["GIT_BRANCH"] = E.run("git rev-parse --abbrev-ref HEAD")
+            env["GIT_LASTCOMMITDATE"] = E.run("git log -1 --format=%cI")
+            env["GIT_COMMITHASH"] = E.run("git rev-parse HEAD")
+        M.debug("Git repository detected.")
     else:
         M.warn("Not a git repository.")
 
-    env['UID'] = E.run('id -u')
-    env['GID'] = E.run('id -g')
-    env['UNAME'] = E.run('whoami')
-
-    docker_files = [
-        'docker-compose.yml'
-    ]
+    env["UID"] = E.run("id -u")
+    env["GID"] = E.run("id -g")
+    env["UNAME"] = E.run("whoami")
+
+    docker_files = ["docker-compose.yml"]
     if dcc_env:
         docker_files.append(f"docker-compose.{dcc_env}.yml")
-    if not ignore_override and isfile('docker-compose.override.yml'):
-        docker_files.append('docker-compose.override.yml')
+    if not ignore_override and isfile("docker-compose.override.yml"):
+        docker_files.append("docker-compose.override.yml")
     if shell:
-        docker_arguments = ['exec', *docker_arguments, '/bin/bash']
+        docker_arguments = ["exec", *docker_arguments, "/bin/bash"]
     elif logs:
-        docker_arguments = ['logs', '-f', *docker_arguments]
-    command = f"docker-compose -f {' -f '.join(docker_files)} {' '.join(docker_arguments)}"
+        docker_arguments = ["logs", "-f", *docker_arguments]
+    elif build_plain:
+        docker_arguments = ["build", "--progress=plain", *docker_arguments]
+    command = (
+        f"docker-compose -f {' -f '.join(docker_files)} {' '.join(docker_arguments)}"
+    )
     M.debug(f"Command: {command}")
     os.environ.update(env)
     try:
-        bash('-c', command, _fg=True)
+        bash("-c", command, _fg=True)
     except Exception as ex:
         M.error(f"Error executing command {command}: {ex}")
         traceback.print_exc()
 
 
 @click.command()
-@click.argument('filter', required=False)
+@click.argument("filter", required=False)
 def dtls(filter: str = None):
-    _filter = ''
+    _filter = ""
     if filter:
         _filter = f"--filter name={filter}"
     command = "docker ps %s -a --format '{{.Names}}#{{.Status}}#{{.Image}}'" % _filter
     output = E.run(command)
-    T.out(output, headers=('Name', 'Status', 'Image'))
+    T.out(output, headers=("Name", "Status", "Image"))
 
 
 @click.command()
-@click.argument('filter', required=False)
+@click.argument("filter", required=False)
 def dtins(filter: str = None):
     rows = []
-    args = ['ps', '-a', '--format', '{{.Names}}']
+    args = ["ps", "-a", "--format", "{{.Names}}"]
     if filter:
-        args.append('--filter ')
+        args.append("--filter ")
         args.append(f"name={filter}")
     for container in docker(*args, _iter=True):
-        container = container.rstrip('\n')
-        insp = docker('inspect', '-f',
-                      '{{ .State.Status }}#{{ .HostConfig.RestartPolicy.Name }}', container)
+        container = container.rstrip("\n")
+        insp = docker(
+            "inspect",
+            "-f",
+            "{{ .State.Status }}#{{ .HostConfig.RestartPolicy.Name }}",
+            container,
+        )
         rows.append(f"{container}#{insp}")
-    T.out(rows, headers=('Name', 'Status', 'Restart'))
+    T.out(rows, headers=("Name", "Status", "Restart"))
 
 
 def __get_container_name(pattern):
-    containers = E.run('docker ps -a --format "{{.Names}}"').split('\n')
+    containers = E.run('docker ps -a --format "{{.Names}}"').split("\n")
     found_containers = []
     for container in containers:
         if pattern in container:
             found_containers.append(container)
     if len(found_containers) == 1:
         return found_containers[0]
     elif len(found_containers) == 0:
         M.error(f"No container found with name {pattern}.")
         raise
     else:
         M.error(
-            f"More than one containers found with name {pattern}: {', '.join(found_containers)}")
+            f"More than one containers found with name {pattern}: {', '.join(found_containers)}"
+        )
         raise
 
 
 @click.command()
-@click.argument('pattern')
+@click.argument("pattern")
 def dtail(pattern):
     try:
-        docker('logs', '-f', __get_container_name(pattern), _fg=True)
-    except:
+        docker("logs", "-f", __get_container_name(pattern), _fg=True)
+    except Exception:
         pass
 
 
 @click.command()
-@click.argument('pattern')
+@click.argument("pattern")
 def dtsh(pattern):
     try:
-        docker('exec', '-it', __get_container_name(pattern),
-               '/bin/bash', _fg=True)
-    except sh.ErrorReturnCode as ex:
+        docker("exec", "-it", __get_container_name(pattern), "/bin/bash", _fg=True)
+    except sh.ErrorReturnCode:
         try:
-            docker('exec', '-it', __get_container_name(pattern),
-                   '/bin/sh', _fg=True)
-        except:
+            docker("exec", "-it", __get_container_name(pattern), "/bin/sh", _fg=True)
+        except Exception:
             pass
-    except:
+    except Exception:
         pass
 
 
 @click.command()
-@click.option('--force', '-f', is_flag=True, default=False, help='force removal, do not ask')
+@click.option(
+    "--force", "-f", is_flag=True, default=False, help="force removal, do not ask"
+)
 def dtclean(force):
     try:
         argss = [
-            ['image', 'prune'],
-            ['image', 'prune', '-a'],
-            ['container', 'prune'],
-            ['system', 'prune'],
-            ['builder', 'prune', '-a']
+            ["image", "prune"],
+            ["image", "prune", "-a"],
+            ["container", "prune"],
+            ["system", "prune"],
+            ["builder", "prune", "-a"],
         ]
         for args in argss:
             if force:
-                args.append('-f')
+                args.append("-f")
             docker(*args, _fg=True)
-    except:
+    except Exception:
         pass
 
-if __name__ == '__main__':
-    globals()[sys.argv[1]]()
+
+if __name__ == "__main__":
+    globals()[sys.argv[1]]()
```

### Comparing `power-user-tools-0.1.1/commands/helpers.py` & `power-user-tools-0.1.3/commands/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Helpers
 ====================================
 Helper classes and functions
 """
 
 import os
 import shlex
-from subprocess import Popen, run
+from subprocess import run
 from enum import Enum
 from yachalk import chalk
 from rich.console import Console
 from rich.table import Table
 
 
 class ReturnCode(Enum):
     OK = 0
 
 
-class Executor():
+class Executor:
     """
     Class to execute shell commands
     """
+
     @classmethod
     def success(cls, command: str, env: dict = None) -> bool:
         ret, _ = cls.__run(command, env=env)
         return ret == ReturnCode.OK.value
 
     @classmethod
     def run(cls, command: str, env: dict = None) -> str:
@@ -42,21 +43,22 @@
             _env.update(env)
         p = run(shlex.split(command), capture_output=True, env=_env)
         return p.returncode, cls.__handle_output(p.stdout.decode())
 
     @classmethod
     def __handle_output(cls, output: str) -> str:
         # We remove the last \n
-        return output.rstrip('\n')
+        return output.rstrip("\n")
 
 
-class Message():
+class Message:
     """
     Class to output colored messages to the console
     """
+
     @classmethod
     def info(cls, message):
         print(chalk.green_bright.bold(message))
 
     @classmethod
     def warn(cls, message):
         print(chalk.yellow_bright.bold(message))
@@ -66,33 +68,38 @@
         print(chalk.red_bright.bold(message))
 
     @classmethod
     def debug(cls, message):
         print(chalk.blue_bright.bold(message))
 
 
-class TableOutput():
+class TableOutput:
     """
     Class to output text in table format
     """
+
     console = Console()
 
     @classmethod
-    def out(cls, data: str | list, sep: str = '#', headers: tuple[str] = None, show_lines = False):
+    def out(
+        cls,
+        data: str | list,
+        sep: str = "#",
+        headers: tuple[str] = None,
+        show_lines=False,
+    ):
         table = Table(
-            show_header=(headers is not None),
-            show_lines=show_lines,
-            show_edge=False
+            show_header=(headers is not None), show_lines=show_lines, show_edge=False
         )
         if headers:
             for header in headers:
                 table.add_column(header)
 
         if isinstance(data, str):
-            data = data.split('\n')
+            data = data.split("\n")
 
         for line in data:
             if isinstance(line, str):
                 table.add_row(*line.split(sep))
             elif isinstance(line, list):
                 table.add_row(*line)
```

### Comparing `power-user-tools-0.1.1/power_user_tools.egg-info/PKG-INFO` & `power-user-tools-0.1.3/power_user_tools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-user-tools
-Version: 0.1.1
+Version: 0.1.3
 Summary: Power User Tools make your life so much easier
 Home-page: https://github.com/dameyerdave/power-user-tools
 Author: dameyerdave
 Author-email: dameyerdave@gmail.com
 License: MIT
 Keywords: power user tools ssh sshd reverse tunnel docker easy development
 Classifier: Programming Language :: Python :: 3
```

### Comparing `power-user-tools-0.1.1/power_user_tools.egg-info/SOURCES.txt` & `power-user-tools-0.1.3/power_user_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 commands/__init__.py
 commands/devutils.py
 commands/dockertools.py
 commands/helpers.py
 commands/sshutils.py
 power_user_tools.egg-info/PKG-INFO
```

### Comparing `power-user-tools-0.1.1/setup.py` & `power-user-tools-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from setuptools import setup, find_packages
 
-long_description = 'Power User Tools make your life so much easier.'
+long_description = "Power User Tools make your life so much easier."
 
 setup(
-    name='power-user-tools',
-    version='0.1.1',
-    author='dameyerdave',
-    author_email='dameyerdave@gmail.com',
-    url='https://github.com/dameyerdave/power-user-tools',
-    description='Power User Tools make your life so much easier',
+    name="power-user-tools",
+    version="0.1.3",
+    author="dameyerdave",
+    author_email="dameyerdave@gmail.com",
+    url="https://github.com/dameyerdave/power-user-tools",
+    description="Power User Tools make your life so much easier",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
     entry_points={
-            'console_scripts': [
-                'sussh = commands.sshutils:sussh',
-                'surtun = commands.sshutils:surtun',
-                'dcc = commands.dockertools:dcc',
-                'dtls = commands.dockertools:dtls',
-                'dtail = commands.dockertools:dtail',
-                'dtsh = commands.dockertools:dtsh',
-                'dtclean = commands.dockertools:dtclean',
-                'dtins = commands.dockertools:dtins',
-                'xpgl = commands.devutils:xpgl',
-            ]
+        "console_scripts": [
+            "sussh = commands.sshutils:sussh",
+            "surtun = commands.sshutils:surtun",
+            "sumount = commands.sshutils:sumount",
+            "dcc = commands.dockertools:dcc",
+            "dtls = commands.dockertools:dtls",
+            "dtail = commands.dockertools:dtail",
+            "dtsh = commands.dockertools:dtsh",
+            "dtclean = commands.dockertools:dtclean",
+            "dtins = commands.dockertools:dtins",
+            "xpgl = commands.devutils:xpgl",
+        ]
     },
     scripts=[
-        'shell/dtip',
-        'shell/dtports',
-        'shell/dtnet',
-        'shell/dtimg',
-        'shell/dtstart',
-        'shell/dtstop',
-        'shell/dtrestart',
-        'shell/dtrm',
-        'shell/xppr',
-        'shell/xprandpw',
-        'shell/xpgrmhistory',
+        "shell/dtip",
+        "shell/dtports",
+        "shell/dtnet",
+        "shell/dtimg",
+        "shell/dtstart",
+        "shell/dtstop",
+        "shell/dtrestart",
+        "shell/dtrm",
+        "shell/xppr",
+        "shell/xprandpw",
+        "shell/xpgrmhistory",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    keywords='power user tools ssh sshd reverse tunnel docker easy development',
+    keywords="power user tools ssh sshd reverse tunnel docker easy development",
     install_requires=[
-        'click==8.1.3',
-        'python-dotenv==0.21.0',
-        'friendlylog==1.0.2',
-        'yachalk==0.1.5',
-        'rich==12.6.0',
-        'sh==1.14.3',
+        "click==8.1.3",
+        "python-dotenv==0.21.0",
+        "friendlylog==1.0.2",
+        "yachalk==0.1.5",
+        "rich==12.6.0",
+        "sh==1.14.3",
     ],
-    zip_safe=False
+    zip_safe=False,
 )
```

### Comparing `power-user-tools-0.1.1/shell/dtimg` & `power-user-tools-0.1.3/shell/dtimg`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.1/shell/dtip` & `power-user-tools-0.1.3/shell/dtip`

 * *Files identical despite different names*

