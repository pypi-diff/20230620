# Comparing `tmp/edc-form-describer-0.3.8.tar.gz` & `tmp/edc-form-describer-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-form-describer-0.3.8.tar", last modified: Thu Jun 23 20:51:41 2022, max compression
+gzip compressed data, was "edc-form-describer-0.3.9.tar", last modified: Fri Aug 12 13:05:11 2022, max compression
```

## Comparing `edc-form-describer-0.3.8.tar` & `edc-form-describer-0.3.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.670951 edc-form-describer-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2021-05-15 18:59:22.000000 edc-form-describer-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.663859 edc-form-describer-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.667022 edc-form-describer-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-form-describer-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1234 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-07-08 03:39:32.000000 edc-form-describer-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-07-08 03:39:32.000000 edc-form-describer-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1489 2022-06-23 20:51:41.671047 edc-form-describer-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      627 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.668207 edc-form-describer-0.3.8/edc_form_describer/
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-07-08 03:39:32.000000 edc-form-describer-0.3.8/edc_form_describer/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-07-09 05:36:09.000000 edc-form-describer-0.3.8/edc_form_describer/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7696 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/form_describer.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4202 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/forms_reference.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1521 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/markdown_writer.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.669490 edc-form-describer-0.3.8/edc_form_describer/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-07-08 03:39:32.000000 edc-form-describer-0.3.8/edc_form_describer/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      749 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.670528 edc-form-describer-0.3.8/edc_form_describer/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1563 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.670734 edc-form-describer-0.3.8/edc_form_describer/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      811 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/edc_form_describer/tests/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1323 2021-02-09 03:33:41.000000 edc-form-describer-0.3.8/edc_form_describer/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      768 2020-07-08 03:39:32.000000 edc-form-describer-0.3.8/edc_form_describer/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:41.668835 edc-form-describer-0.3.8/edc_form_describer.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1489 2022-06-23 20:51:41.000000 edc-form-describer-0.3.8/edc_form_describer.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1277 2022-06-23 20:51:41.000000 edc-form-describer-0.3.8/edc_form_describer.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-06-23 20:51:41.000000 edc-form-describer-0.3.8/edc_form_describer.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-07-08 03:42:52.000000 edc-form-describer-0.3.8/edc_form_describer.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       19 2022-06-23 20:51:41.000000 edc-form-describer-0.3.8/edc_form_describer.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1597 2022-06-23 20:51:14.000000 edc-form-describer-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2063 2021-09-11 18:23:29.000000 edc-form-describer-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1165 2022-06-23 20:51:41.671331 edc-form-describer-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.586501 edc-form-describer-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2021-05-15 18:59:22.000000 edc-form-describer-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.577925 edc-form-describer-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.580702 edc-form-describer-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1234 2022-06-23 20:51:14.000000 edc-form-describer-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:14.000000 edc-form-describer-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-23 20:51:14.000000 edc-form-describer-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-07-08 03:39:32.000000 edc-form-describer-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       51 2020-07-08 03:39:32.000000 edc-form-describer-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1618 2022-08-12 13:05:11.586616 edc-form-describer-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      627 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.583591 edc-form-describer-0.3.9/edc_form_describer/
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-07-08 03:39:32.000000 edc-form-describer-0.3.9/edc_form_describer/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-07-09 05:36:09.000000 edc-form-describer-0.3.9/edc_form_describer/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7796 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/edc_form_describer/form_describer.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4202 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/forms_reference.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1619 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/edc_form_describer/markdown_writer.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.585153 edc-form-describer-0.3.9/edc_form_describer/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-07-08 03:39:32.000000 edc-form-describer-0.3.9/edc_form_describer/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      749 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.586193 edc-form-describer-0.3.9/edc_form_describer/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1563 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.586410 edc-form-describer-0.3.9/edc_form_describer/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      837 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/edc_form_describer/tests/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      264 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/edc_form_describer/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1323 2021-02-09 03:33:41.000000 edc-form-describer-0.3.9/edc_form_describer/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      768 2020-07-08 03:39:32.000000 edc-form-describer-0.3.9/edc_form_describer/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 13:05:11.584349 edc-form-describer-0.3.9/edc_form_describer.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1618 2022-08-12 13:05:11.000000 edc-form-describer-0.3.9/edc_form_describer.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1344 2022-08-12 13:05:11.000000 edc-form-describer-0.3.9/edc_form_describer.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-12 13:05:11.000000 edc-form-describer-0.3.9/edc_form_describer.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-07-08 03:42:52.000000 edc-form-describer-0.3.9/edc_form_describer.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       19 2022-08-12 13:05:11.000000 edc-form-describer-0.3.9/edc_form_describer.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1738 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2087 2022-08-12 13:05:03.000000 edc-form-describer-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1263 2022-08-12 13:05:11.586926 edc-form-describer-0.3.9/setup.cfg
```

### Comparing `edc-form-describer-0.3.8/.github/workflows/build.yml` & `edc-form-describer-0.3.9/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+---
 name: build
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9']
-        django-version: ['3.2']
+        python-version: ['3.9', '3.10']
+        django-version: ['3.2', '4.0', '4.1', 'dev']
 
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-    - name: Install pycups and words dependency
-      run: |
-        sudo apt-get install libcups2-dev wamerican
-
-    - uses: actions/checkout@v2
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Get pip cache dir
-      id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
-
-    - name: Cache
-      uses: actions/cache@v2
-      with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key:
-          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
-        restore-keys: |
-          ${{ matrix.python-version }}-v1-
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
-
-
-    - name: Tox tests
-      run: |
-        tox -v
-      env:
-        DJANGO: ${{ matrix.django-version }}
-
-    - name: Upload coverage
-      uses: codecov/codecov-action@v1
-      with:
-        name: Python ${{ matrix.python-version }}
+      - name: Install pycups and words dependency
+        run: |
+          sudo sed -i 's/azure\.//' /etc/apt/sources.list
+          sudo apt-get -y update
+          sudo apt-get install libcups2-dev wamerican
+
+      - uses: actions/checkout@v2
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Get pip cache dir
+        id: pip-cache
+        run: |
+          echo "::set-output name=dir::$(pip cache dir)"
+
+      - name: Cache
+        uses: actions/cache@v2
+        with:
+          path: ${{ steps.pip-cache.outputs.dir }}
+          key:
+            ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
+          restore-keys: |
+            ${{ matrix.python-version }}-v1-
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
+
+
+      - name: Tox tests
+        run: |
+          tox -v
+        env:
+          DJANGO: ${{ matrix.django-version }}
+
+      - name: Upload coverage
+        uses: codecov/codecov-action@v1
+        with:
+          name: Python ${{ matrix.python-version }}
```

### Comparing `edc-form-describer-0.3.8/.gitignore` & `edc-form-describer-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/LICENSE` & `edc-form-describer-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/PKG-INFO` & `edc-form-describer-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-form-describer
-Version: 0.3.8
+Version: 0.3.9
 Summary: Describe clinicedc/edc forms in markdown
 Home-page: https://github.com/clinicedc/edc-form-describer
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc,forms,markdown,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
```

### Comparing `edc-form-describer-0.3.8/README.rst` & `edc-form-describer-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/form_describer.py` & `edc-form-describer-0.3.9/edc_form_describer/form_describer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import string
 import sys
 from datetime import datetime
 from math import floor
+from typing import Optional
 
 from django.core.management.color import color_style
 from edc_fieldsets import Fieldsets
 from edc_model import DEFAULT_BASE_FIELDS
 
 from .markdown_writer import MarkdownWriter
 
@@ -138,16 +139,16 @@
                             number = self.get_next_number(number, fname)
                             self.add_field(fname=fname, number=number)
 
     def to_markdown(self):
         markdown_writer = self.markdown_writer_cls()
         return markdown_writer.to_markdown(markdown=self.markdown)
 
-    def to_file(self, path=None):
-        markdown_writer = self.markdown_writer_cls(path=path)
+    def to_file(self, path: Optional[str] = None, overwrite: Optional[bool] = None):
+        markdown_writer = self.markdown_writer_cls(path=path, overwrite=overwrite)
         markdown_writer.to_file(markdown=self.markdown)
 
     def add_hidden_fields(self):
         self.markdown.append("\n**Hidden fields:**")
         self.add_field(fname="report_datetime")
         base_fields = DEFAULT_BASE_FIELDS
         base_fields.append("revision")
```

### Comparing `edc-form-describer-0.3.8/edc_form_describer/forms_reference.py` & `edc-form-describer-0.3.9/edc_form_describer/forms_reference.py`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/markdown_writer.py` & `edc-form-describer-0.3.9/edc_form_describer/markdown_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from datetime import datetime
+from typing import Optional
 
 
 class MarkdownWriter:
-    def __init__(self, path=None, exists_ok=None):
-        self.path = self.get_path(path=path, exists_ok=exists_ok)
+    def __init__(self, path: Optional[str] = None, overwrite: Optional[bool] = None):
+        self.path = self.get_path(path=path, overwrite=overwrite)
 
     @staticmethod
-    def get_path(path=None, exists_ok=None):
+    def get_path(path: Optional[str] = None, overwrite: Optional[bool] = None):
         if not path:
             timestamp = datetime.today().strftime("%Y%m%d%H%M")
             path = f"forms_{timestamp}.md"
         if os.path.exists(path):
-            if exists_ok:
+            if overwrite:
                 os.remove(path)
             else:
                 raise FileExistsError(f"File exists. Got '{path}'")
         return path
 
     @staticmethod
     def to_markdown(markdown=None):
```

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/admin.py` & `edc-form-describer-0.3.9/edc_form_describer/tests/admin.py`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-local-private.pem` & `edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/etc/user-rsa-restricted-private.pem` & `edc-form-describer-0.3.9/edc_form_describer/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/models.py` & `edc-form-describer-0.3.9/edc_form_describer/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/tests/tests.py` & `edc-form-describer-0.3.9/edc_form_describer/tests/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tempfile import mktemp
+from tempfile import mkstemp
 
 from django.test import TestCase
 
 from ...form_describer import FormDescriber
 from ..admin import MyModelAdmin
 from ..models import MyModel
 
@@ -11,14 +11,14 @@
     def test_ok(self):
         describer = FormDescriber(admin_cls=MyModelAdmin, include_hidden_fields=True)
         txt = " ".join(describer.markdown)
         for f in MyModel._meta.get_fields():
             self.assertIn(f.verbose_name, txt)
 
     def test_to_file(self):
-        tmp = mktemp()
+        tmp, name = mkstemp()
         describer = FormDescriber(admin_cls=MyModelAdmin, include_hidden_fields=True)
-        describer.to_file(path=tmp)
-        with open(tmp, "r") as describer_file:
+        describer.to_file(path=name, overwrite=True)
+        with open(name, "r") as describer_file:
             txt = describer_file.read()
             for f in MyModel._meta.get_fields():
                 self.assertIn(f.verbose_name, txt)
```

### Comparing `edc-form-describer-0.3.8/edc_form_describer/tests/visit_schedule.py` & `edc-form-describer-0.3.9/edc_form_describer/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer/urls.py` & `edc-form-describer-0.3.9/edc_form_describer/urls.py`

 * *Files identical despite different names*

### Comparing `edc-form-describer-0.3.8/edc_form_describer.egg-info/PKG-INFO` & `edc-form-describer-0.3.9/edc_form_describer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-form-describer
-Version: 0.3.8
+Version: 0.3.9
 Summary: Describe clinicedc/edc forms in markdown
 Home-page: https://github.com/clinicedc/edc-form-describer
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc,forms,markdown,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
```

### Comparing `edc-form-describer-0.3.8/edc_form_describer.egg-info/SOURCES.txt` & `edc-form-describer-0.3.9/edc_form_describer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
+.yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 codecov.yml
@@ -23,14 +25,15 @@
 edc_form_describer.egg-info/dependency_links.txt
 edc_form_describer.egg-info/not-zip-safe
 edc_form_describer.egg-info/top_level.txt
 edc_form_describer/tests/__init__.py
 edc_form_describer/tests/admin.py
 edc_form_describer/tests/forms.py
 edc_form_describer/tests/models.py
+edc_form_describer/tests/urls.py
 edc_form_describer/tests/visit_schedule.py
 edc_form_describer/tests/etc/user-aes-local.key
 edc_form_describer/tests/etc/user-aes-restricted.key
 edc_form_describer/tests/etc/user-rsa-local-private.pem
 edc_form_describer/tests/etc/user-rsa-local-public.pem
 edc_form_describer/tests/etc/user-rsa-restricted-private.pem
 edc_form_describer/tests/etc/user-rsa-restricted-public.pem
```

### Comparing `edc-form-describer-0.3.8/pyproject.toml` & `edc-form-describer-0.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,39 +28,47 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
+    py{38,39,310}-dj{32,40,41,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
+    3.8: py38
     3.9: py39, lint
+    3.10: py310
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32, lint
+    4.0: dj40
+    4.1: dj41
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
+    dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
+    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `edc-form-describer-0.3.8/runtests.py` & `edc-form-describer-0.3.9/runtests.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         "edc_visit_tracking.apps.AppConfig",
         "edc_visit_schedule.apps.AppConfig",
         "edc_action_item.apps.AppConfig",
         "edc_fieldsets.apps.AppConfig",
         "edc_form_describer.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
+    use_test_urls=True,
 ).settings
 
 
 def main():
     if not settings.configured:
         settings.configure(**DEFAULT_SETTINGS)
     django.setup()
```

### Comparing `edc-form-describer-0.3.8/setup.cfg` & `edc-form-describer-0.3.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc, forms, markdown, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
@@ -34,14 +37,14 @@
 	bin*
 	edc_form_describer.tests*
 
 [flake8]
 ignore = E226,W503,E203
 max-line-length = 95
 max-complexity = 10
-exclude = */migrations,.tox,.git,__pycache__,build,dist,.eggs
+exclude = */migrations/*,.tox,.git,__pycache__,build,dist,.eggs
 per-file-ignores = __init__.py: F401
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

