# Comparing `tmp/cgcomponents-2.0.2.tar.gz` & `tmp/cgcomponents-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcomponents-2.0.2.tar", last modified: Sat May 21 05:31:40 2022, max compression
+gzip compressed data, was "cgcomponents-2.0.3.tar", last modified: Tue Jun 20 16:30:05 2023, max compression
```

## Comparing `cgcomponents-2.0.2.tar` & `cgcomponents-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-21 05:31:40.933536 cgcomponents-2.0.2/
--rw-rw-rw-   0        0        0     1102 2022-05-20 13:48:10.000000 cgcomponents-2.0.2/LICENSE
--rw-rw-rw-   0        0        0      955 2022-05-21 05:31:40.927542 cgcomponents-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      433 2022-05-20 13:48:10.000000 cgcomponents-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-05-21 05:31:40.878530 cgcomponents-2.0.2/cgcomponents/
--rw-rw-rw-   0        0        0     2192 2022-05-20 13:48:10.000000 cgcomponents-2.0.2/cgcomponents/exceptions.py
--rw-rw-rw-   0        0        0     1227 2022-05-20 13:48:10.000000 cgcomponents-2.0.2/cgcomponents/logs.py
--rw-rw-rw-   0        0        0    14313 2022-05-21 05:31:30.000000 cgcomponents-2.0.2/cgcomponents/requests_cg.py
-drwxrwxrwx   0        0        0        0 2022-05-21 05:31:40.924532 cgcomponents-2.0.2/cgcomponents.egg-info/
--rw-rw-rw-   0        0        0      955 2022-05-21 05:31:40.000000 cgcomponents-2.0.2/cgcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2022-05-21 05:31:40.000000 cgcomponents-2.0.2/cgcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-21 05:31:40.000000 cgcomponents-2.0.2/cgcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-05-21 05:31:40.000000 cgcomponents-2.0.2/cgcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-05-21 05:31:40.000000 cgcomponents-2.0.2/cgcomponents.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-21 05:31:40.933536 cgcomponents-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      815 2022-05-21 05:28:28.000000 cgcomponents-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:30:04.628347 cgcomponents-2.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-06-20 12:10:50.000000 cgcomponents-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0      926 2023-06-20 16:30:04.307348 cgcomponents-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-06-20 12:10:50.000000 cgcomponents-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 16:30:04.118673 cgcomponents-2.0.3/cgcomponents/
+-rw-rw-rw-   0        0        0     2112 2023-06-20 12:10:50.000000 cgcomponents-2.0.3/cgcomponents/exceptions.py
+-rw-rw-rw-   0        0        0     1164 2023-06-20 12:10:50.000000 cgcomponents-2.0.3/cgcomponents/logs.py
+-rw-rw-rw-   0        0        0    13697 2023-06-20 12:30:57.000000 cgcomponents-2.0.3/cgcomponents/requests_cg.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:30:04.272169 cgcomponents-2.0.3/cgcomponents.egg-info/
+-rw-rw-rw-   0        0        0      926 2023-06-20 16:30:01.000000 cgcomponents-2.0.3/cgcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-20 16:30:01.000000 cgcomponents-2.0.3/cgcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:30:01.000000 cgcomponents-2.0.3/cgcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 16:30:01.000000 cgcomponents-2.0.3/cgcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 16:30:01.000000 cgcomponents-2.0.3/cgcomponents.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:30:04.629345 cgcomponents-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-20 16:29:34.000000 cgcomponents-2.0.3/setup.py
```

### Comparing `cgcomponents-2.0.2/LICENSE` & `cgcomponents-2.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
-python setup.py sdist
-
-Copyright (c) 2022 portalcomponents
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+python setup.py sdist
+
+Copyright (c) 2022 portalcomponents
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `cgcomponents-2.0.2/PKG-INFO` & `cgcomponents-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: cgcomponents
-Version: 2.0.2
+Version: 2.0.3
 Summary: Components para scrapping da CG.
 Home-page: https://github.com/ramirooliveiracg/cgcomponents
 Author: Gabriel Dalacorte e Rogerio Filho
 Author-email: gnunes.servico@gmail.com, crofilho2@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Portal Components
+# CG Components
 
 ## Getting Started
 #### Dependencies
-You need Python 3.7 or later to use **portalcomponents**.
+You need Python 3.7 or later to use **cgcomponents**.
 ```
 pip install setuptools
 pip install wheel
 pip install twine
 ```
 #### Installation
 Clone this repo to your local machine using:
 ```
 git clone https://github.com/ramirooliveiracg/cgcomponents.git
 ```
 ## Features
 - File structure for PyPI packages
 - Setup with package informations
 - License example
-
```

### Comparing `cgcomponents-2.0.2/cgcomponents/exceptions.py` & `cgcomponents-2.0.3/cgcomponents/exceptions.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-
-
-class CGExceptionsErros(Exception):
-    """Base class for CG exceptions"""
-    pass
-
-
-class CGExceptionsRDS(IOError):
-    """Base class for RDS exceptions"""
-    pass
-
-
-class CGExceptionsRequestsErros(IOError):
-    """Base class for requestsCG exceptions"""
-    pass
-
-
-""" Generic Exceptions """
-
-
-class ErrorJson(CGExceptionsRequestsErros):
-
-    def __init__(self, component, message="JSON Tratase de um DataSet, por gentileza utilize json.dumps(json)"):
-        self.component = component
-        self.message = message
-        super().__init__(self.message)
-
-    def __str__(self):
-        return f'{self.component} -> {self.message}'
-
-
-class ErrorCredentials(CGExceptionsErros):
-
-    def __init__(self, component, message="Credenciais de Login incorretas. Por gentileza verifique-as"):
-        self.component = component
-        self.message = message
-        super().__init__(self.message)
-
-    def __str__(self):
-        return f'{self.component} -> {self.message}'
-
-
-""" BackEnd Exceptions """
-
-
-class BackEndConnectionError(CGExceptionsRequestsErros):
-    def __init__(self, suggestion="Inicie o Serviço do BackEnd", message="Falha ao conectar-se ao servidor Django"):
-        self.message = message
-        self.suggestion = suggestion
-        super().__init__(self.message, suggestion)
-
-    def __str__(self):
-        return f'{self.suggestion} -> {self.message}'
-
-
-""" INTRANET EXCEPTIONS """
-
-
-class IntranetConnectionError(CGExceptionsRequestsErros):
-    def __init__(self, suggestion="Conect-se ao FortClient", message="Falha ao conectar-se com o Intranet"):
-        self.message = message
-        self.suggestion = suggestion
-        super().__init__(self.message, suggestion)
-
-    def __str__(self):
-        return f'{self.suggestion} -> {self.message}'
-
-
-""" RDS EXCEPTIONS """
-
-
-class ErrorConnectionRDS(CGExceptionsRDS):
-
-    def __init__(self, component, message="Erro ao tentar conectar-se ao banco RDS"):
-        self.component = component
-        self.message = message
-        super().__init__(self.message)
-
-    def __str__(self):
-        return f'{self.component} -> {self.message}'
+
+
+class CGExceptionsErros(Exception):
+    """Base class for CG exceptions"""
+    pass
+
+
+class CGExceptionsRDS(IOError):
+    """Base class for RDS exceptions"""
+    pass
+
+
+class CGExceptionsRequestsErros(IOError):
+    """Base class for requestsCG exceptions"""
+    pass
+
+
+""" Generic Exceptions """
+
+
+class ErrorJson(CGExceptionsRequestsErros):
+
+    def __init__(self, component, message="JSON Tratase de um DataSet, por gentileza utilize json.dumps(json)"):
+        self.component = component
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return f'{self.component} -> {self.message}'
+
+
+class ErrorCredentials(CGExceptionsErros):
+
+    def __init__(self, component, message="Credenciais de Login incorretas. Por gentileza verifique-as"):
+        self.component = component
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return f'{self.component} -> {self.message}'
+
+
+""" BackEnd Exceptions """
+
+
+class BackEndConnectionError(CGExceptionsRequestsErros):
+    def __init__(self, suggestion="Inicie o Serviço do BackEnd", message="Falha ao conectar-se ao servidor Django"):
+        self.message = message
+        self.suggestion = suggestion
+        super().__init__(self.message, suggestion)
+
+    def __str__(self):
+        return f'{self.suggestion} -> {self.message}'
+
+
+""" INTRANET EXCEPTIONS """
+
+
+class IntranetConnectionError(CGExceptionsRequestsErros):
+    def __init__(self, suggestion="Conect-se ao FortClient", message="Falha ao conectar-se com o Intranet"):
+        self.message = message
+        self.suggestion = suggestion
+        super().__init__(self.message, suggestion)
+
+    def __str__(self):
+        return f'{self.suggestion} -> {self.message}'
+
+
+""" RDS EXCEPTIONS """
+
+
+class ErrorConnectionRDS(CGExceptionsRDS):
+
+    def __init__(self, component, message="Erro ao tentar conectar-se ao banco RDS"):
+        self.component = component
+        self.message = message
+        super().__init__(self.message)
+
+    def __str__(self):
+        return f'{self.component} -> {self.message}'
```

### Comparing `cgcomponents-2.0.2/cgcomponents/requests_cg.py` & `cgcomponents-2.0.3/cgcomponents/requests_cg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,355 +1,347 @@
-import json
-from typing import AnyStr,  Iterable, List, Optional
-import requests
-from itertools import count
-import logging
-from re import findall
-from calendar import monthrange
-import unidecode
-
-
-class RequestsPortal(object):
-    def __init__(self, url_login: str = None, username: str = None,
-                 password: AnyStr = None):
-
-        self.url_login = url_login
-        self.username = username
-        self.password = password
-
-    def get_cg(self, url, filter: str = None):
-
-        """
-        :param url: url -> Link
-        :return: returns values referring to the endpoint
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-
-        if filter:
-            headers = {'Authorization': 'Token ' + key_headers['key']}
-            return_inform = requests.get(url=f'{url}{filter}', headers=headers, verify=True)
-            return_inform_format = json.loads(return_inform.text)
-            return return_inform_format
-        else:
-            headers = {'Authorization': 'Token ' + key_headers['key']}
-            return_inform = requests.get(url=url, headers=headers, verify=True)
-            return_inform_format = json.loads(return_inform.text)
-
-            return return_inform_format
-
-    def post_cg(self, url, json_request):
-        """
-        :param url: url -> Link
-        :param json_request: json for request
-        :return: return status code
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-        headers = {'Authorization': 'Token ' + key_headers['key'],
-                   'Content-type': 'application/json',
-                   'Accept': 'application/json'}
-        try:
-            x = requests.post(url=url, data=json.dumps(json_request),
-                              headers=headers, verify=True)
-        except:
-            pass
-
-    def patch_cg(self, url, json_request, filter: str = None):
-        """
-        :param url: url -> Link
-        :param json_request: json with request
-        :param filter: filter for request -> Exemple: ID or empresa__cnpj=0003131
-        :return: return status code
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-        headers = {'Authorization': 'Token ' + key_headers['key'],
-                   'Content-type': 'application/json',
-                   'Accept': 'application/json'}
-
-        if filter:
-            requests.patch(url=f'{url}{filter}', data=json.dumps(json_request),
-                           headers=headers, verify=True)
-        else:
-            print('Não é possivel realizar um patch sem passar o Indice')
-
-    def patch_file_cg(self, url, path, filter):
-        """
-        :param url: url -> Link
-        :param path: file path
-        :param filter: filter for request -> Exemple: ID or empresa__cnpj=0003131
-        :return: return status code
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-        headers = {'Authorization': 'Token ' + key_headers['key']}
-
-        file_ob = {'arquivo': open(path, 'rb')}
-
-        if filter:
-            requests.patch(f'{url}{filter}', headers=headers, files=file_ob)
-        else:
-            print('Não é possivel realizar um patch sem passar o Indice')
-
-    def delete_cg_generic(self, url, id, dict_inform, other_url):
-        """
-        :param url: url -> Link
-        :param dict_inform: dict with informs for date iterable
-        :param other_url: url for delete
-        :param json_request: json with request
-        :param id: filter for request -> Exemple: ID
-        :return: return status code
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-
-        headers = {'Authorization': 'Token ' + key_headers['key'],
-                   'Content-type': 'application/json',
-                   'Accept': 'application/json'
-                   }
-
-        return_inform = requests.get(url=f'{url}{id}/', headers=headers, verify=True)
-        return_inform_format = json.loads(return_inform.text)
-
-        n = count(0)
-
-        for i_return_portal in return_inform_format['colaborador']:
-            num = next(n)
-            if str(dict_inform['id']) == str(i_return_portal['id']):
-                return_inform_format['colaborador'].pop(num)
-
-        try:
-            x = requests.patch(url=f'{other_url}{return_inform_format["id"]}/',
-                               data=json.dumps(return_inform_format),
-                               headers=headers, verify=True)
-        except:
-            pass
-
-    """ Generic Gets in projects the Portal """
-
-    def get_generic_holerite(self, url, filter_cnpj, filter_competence, filter_type_competence):
-
-        """
-        :param url: url: url -> Link
-        :param filter_cnpj: cnpj for filter
-        :param filter_competence: date for filter
-        :param filter_type_competence: type_competence for filter, Exemple: Adiantamento or Mensal
-        :return: returns values referring to the endpoint
-        """
-
-        params = {
-            'username': self.username,
-            'password': self.password
-        }
-        key = requests.post(self.url_login, data=params)
-        key_headers = json.loads(key.text)
-
-        headers = {'Authorization': 'Token ' + key_headers['key']}
-        return_inform = requests.get(url=f'{url}?empresa__cnpj={filter_cnpj}&competencia__competencia='
-                                         f'{filter_competence}&tipo_calculo={filter_type_competence}',
-                                     headers=headers, verify=True)
-
-        return_inform_format = json.loads(return_inform.text)
-
-        return return_inform_format
-
-
-class SigHandler:
-    def __init__(self, url_sig_company_events: str = AnyStr, url_sig_company_events_task: str = AnyStr):
-        self.url_sig_company_events = url_sig_company_events
-        self.url_sig_company_events_task = url_sig_company_events_task
-
-    def mark_on_sig(self, id_task: list = List, id_dominio: str = AnyStr, event: str = AnyStr, tag: str = AnyStr,
-             user: str = AnyStr):
-        """
-
-        :param user: user id which will be shown in sig
-        :param id_task: list with the ids that will be marked
-        :param id_dominio: str with the 'id dominio' of the company
-        :param event: str with the event that will be marked, ex.: 'BALANCETE'
-        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
-        :return: bool, True if marked or False if not marked
-        """
-        logging.warning("Starting to mark...")
-        data_dictionary = json.loads(requests.get(self.url_sig_company_events, verify=False).text)["dados"]
-        mark = False
-        for data in data_dictionary:
-            if (data["id_dominio"] == id_dominio) and (unidecode.unidecode(data[tag]) == event or
-                                                       event in unidecode.unidecode(data[tag])):
-                for dice in data["tarefas"]:
-                    for ID in id_task:
-                        if dice["id_tarefa"] == ID:
-                            url2 = self.url_sig_company_events_task.format(dice["id_empresa_evento_tarefa"])
-                            task_completed = {"dados": json.dumps({"status": "CON", "id_usuario": user})}
-                            headers = {'Accept': 'application/json, text/plain, */*',
-                                       'Content-Type': 'application/x-www-form-urlencoded'}
-                            requests.put(url=url2, data=task_completed, headers=headers, verify=False)
-                            mark = True
-        logging.warning("Finished marking")
-        return mark
-
-    def check_sig(self, id_dominio: str = AnyStr, event: str = AnyStr, tag: str = AnyStr):
-        """
-
-        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
-        :param event: str with the event that will be checked, ex.: 'BALANCETE'
-        :param id_dominio: str with the 'id dominio' of the company
-        :return: dict with the tasks ids and status, true if the task has been marked else false
-        """
-        logging.warning("Starting to check...")
-        data_dictionary = json.loads(requests.get(self.url_sig_company_events, verify=False).text)["dados"]
-        task = {}
-        for data in data_dictionary:
-            if (data["id_dominio"] == id_dominio) and (unidecode.unidecode(data[tag]) == event or
-                                                       event in unidecode.unidecode(data[tag])):
-                for dice in data["tarefas"]:
-                    task.update({dice["id_tarefa"]: False if dice["status"] == "NCON" else True})
-        logging.warning("Finished checking")
-        return task
-
-
-class IntranetRequests:
-    def __init__(self, id_dominio: str = Optional, id_company: str = Optional):
-        self.id_dominio = id_dominio
-        self.id_company = id_company
-
-    def tax_amount(self, url_tax_amount: str = AnyStr, code: int = Iterable, date: str = AnyStr):
-        """
-
-        :param url_tax_amount:
-        :param date: str containing the competence of the file being worked on
-        :param code: int with the tax code for identification on the intranet
-        :return: float with the tax value
-        """
-        logging.warning("Extracting value...")
-
-        date = date.split('.')
-        last_day = monthrange(int(date[1]), int(date[0]))
-        first_date = f"{str(date[1])}-{str(date[0])}-01"
-        last_date = f"{str(date[1])}-{str(date[0])}-{str(last_day[1])}"
-        url = url_tax_amount.format(self.id_dominio, first_date, last_date, str(code))
-        req = requests.get(url, verify=False)
-        text = req.text
-        text = (text.replace('Array', '')).replace('  ', '')
-        lines = text.splitlines()
-        data_list = []
-
-        for line in lines:
-            if findall('[a-z]', line):
-                data_list.append(line)
-        value = float((data_list[-1]).split(' ')[-1])
-        logging.warning(f"The value that was extracted: {value}")
-        return value
-
-    def get_intranet(self, url, filter: str = None):
-
-        """
-        :param url: Url do GET - Deve ser informada no .env
-        :return: Informacoes do Intranet
-        """
-
-        headers = {'Content-type': 'application/json',
-                   'Accept': 'application/json'}
-        if filter:
-            return_inform = requests.get(url=f'{url}{filter}', headers=headers, verify=True)
-            return_inform_format = json.loads(return_inform.text)
-
-            return return_inform_format
-        else:
-            return_inform = requests.get(url=url, headers=headers, verify=True)
-            return_inform_format = json.loads(return_inform.text)
-
-            return return_inform_format
-
-    def get_company_email(self, url_client_email: str = AnyStr, company: str = AnyStr, sector: str = AnyStr,
-                          tag_number: str = AnyStr):
-        """
-
-        :param url_client_email:
-        :param company: str with the company name
-        :param sector: str with the sector number and name, ex.: '2-Fiscal'
-        :param tag_number: str with the tag number in the db
-        :return: dict with data and status of the request
-        """
-        logging.warning("Extracting company email...")
-
-        req = requests.get(url_client_email + self.id_company, verify=False)
-        text = req.text
-
-        text_json = json.loads(text)
-        data = text_json["dados"]
-        group = [company, self.id_dominio]
-        email = []
-
-        if not data:
-            if group not in email:
-                logging.warning("Email not found")
-                return {"data": '', "status": False}
-        else:
-            for dat in data:
-                try:
-                    if sector in dat["setores"] and tag_number in dat["tags"]:
-                        email.append(dat['email'])
-                except TypeError:
-                    continue
-            if not email:
-                logging.warning("Email not found")
-                return {"data": '', "status": False}
-        for item in email:
-            try:
-                if '@' in item:
-                    logging.warning("Extracted email")
-                    return {"data": email, "status": True}
-            except TypeError:
-                continue
-        logging.warning("Email not found")
-        return {"data": '', "status": False}
-
-    def get_deadline(self, url_deadline: str = AnyStr, event: str = AnyStr, tag: str = AnyStr):
-        """
-
-        :param url_deadline:
-        :param event: str with the event that will be marked, ex.: 'BALANCETE'
-        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
-        :return: str with the deadline
-        """
-        logging.warning("Extracting deadline...")
-        data_dictionary = json.loads(requests.get(url_deadline, verify=False).text)["dados"]
-        deadline = AnyStr
-        for dic in data_dictionary:
-            try:
-                if dic['id_dominio'] == self.id_dominio:
-                    if dic[tag] == event or event in dic[tag]:
-                        date = str(dic['prazo_final']).split('-')
-                        deadline = f"{date[2]}/{date[1]}/{date[0]}"
-            except:
-                continue
-        logging.warning("Extracted deadline")
-        return deadline
-
-
+import json
+from typing import AnyStr,  Iterable, List, Optional
+import requests
+from itertools import count
+import logging
+from re import findall
+from calendar import monthrange
+import unidecode
+
+
+class RequestsPortal(object):
+    def __init__(self, url_login: str = None, username: str = None,
+                 password: AnyStr = None, json_request: AnyStr = None, id_request: int = None):
+
+        self.url_login = url_login
+        self.username = username
+        self.password = password
+        self.json_request = json_request
+        self.id_request = id_request
+
+    def get_cg(self, url):
+
+        """
+        :param url: Url do GET - Deve ser informada no .env
+        :return: Informacoes solicitadas
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+
+        if self.id_request is not None:
+            headers = {'Authorization': 'Token ' + key_headers['token']}
+            return_inform = requests.get(url=f'{url}{self.id_request}', headers=headers, verify=True)
+            return_inform_format = json.loads(return_inform.text)
+
+            return return_inform_format
+        else:
+            headers = {'Authorization': 'Token ' + key_headers['token']}
+            return_inform = requests.get(url=url, headers=headers, verify=True)
+            return_inform_format = json.loads(return_inform.text)
+
+            return return_inform_format
+
+    def post_cg(self, url):
+        """
+        :param url: Url do Post - Deve ser informada no .env
+        :return: Registra informacoes no Portal
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+        headers = {'Authorization': 'Token ' + key_headers['token'],
+                   'Content-type': 'application/json',
+                   'Accept': 'application/json'}
+        try:
+            x = requests.post(url=url, data=json.dumps(self.json_request),
+                              headers=headers, verify=True)
+        except:
+            pass
+
+    def patch_cg(self, url):
+        """
+        :param url: Url do Post - Deve ser informada no .env
+        :return: Registra informacoes no Portal
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+        headers = {'Authorization': 'Token ' + key_headers['token'],
+                   'Content-type': 'application/json',
+                   'Accept': 'application/json'}
+
+        if self.id_request is not None:
+            requests.patch(url=f'{url}{self.id_request}', data=json.dumps(self.json_request),
+                           headers=headers, verify=True)
+        else:
+            print('Não é possivel realizar um patch sem passar o Indice')
+
+    def patch_file_cg(self, url, path):
+        """
+        :param url: Url do Post - Deve ser informada no .env
+        :return: Registra informacoes no Portal
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+        headers = {'Authorization': 'Token ' + key_headers['token']}
+
+        file_ob = {'arquivo': open(path, 'rb')}
+
+        if self.id_request is not None:
+            requests.patch(f'{url}{self.id_request}', headers=headers, files=file_ob)
+        else:
+            print('Não é possivel realizar um patch sem passar o Indice')
+
+    def delete_cg_generic(self, url, id, dict_inform, other_url):
+        """
+        :param url: Url do Delet - Deve ser informada no .env
+        :return: Status code
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+
+        headers = {'Authorization': 'Token ' + key_headers['token'],
+                   'Content-type': 'application/json',
+                   'Accept': 'application/json'
+                   }
+
+        return_inform = requests.get(url=f'{url}{id}/', headers=headers, verify=True)
+        return_inform_format = json.loads(return_inform.text)
+
+        n = count(0)
+
+        for i_return_portal in return_inform_format['colaborador']:
+            num = next(n)
+            if str(dict_inform['id']) == str(i_return_portal['id']):
+                return_inform_format['colaborador'].pop(num)
+
+        try:
+            x = requests.patch(url=f'{other_url}{return_inform_format["id"]}/',
+                               data=json.dumps(return_inform_format),
+                               headers=headers, verify=True)
+        except:
+            pass
+
+    """ Generic Gets in projects the Portal """
+
+    def get_generic_holerite(self, url, filter_cnpj, filter_competence, filter_type_competence):
+
+        """
+        :param url: Url do GET - Deve ser informada no .env, CNPJ da empresa, competencia, tipo competencia( Mensal,
+        Adiantamento ).
+        :return: Informacoes solicitadas
+        """
+
+        params = {
+            'username': self.username,
+            'password': self.password
+        }
+        key = requests.post(self.url_login, data=params)
+        key_headers = json.loads(key.text)
+
+        headers = {'Authorization': 'Token ' + key_headers['token']}
+        return_inform = requests.get(url=f'{url}?empresa__cnpj={filter_cnpj}&competencia__competencia='
+                                         f'{filter_competence}&tipo_calculo={filter_type_competence}', 
+                                     headers=headers, verify=True)
+
+        return_inform_format = json.loads(return_inform.text)
+
+        return return_inform_format
+
+
+class SigHandler:
+    def __init__(self, url_sig_company_events: str = AnyStr, url_sig_company_events_task: str = AnyStr):
+        self.url_sig_company_events = url_sig_company_events
+        self.url_sig_company_events_task = url_sig_company_events_task
+
+    def mark_on_sig(self, id_task: list = List, id_dominio: str = AnyStr, event: str = AnyStr, tag: str = AnyStr,
+             user: str = AnyStr):
+        """
+
+        :param user: user id which will be shown in sig
+        :param id_task: list with the ids that will be marked
+        :param id_dominio: str with the 'id dominio' of the company
+        :param event: str with the event that will be marked, ex.: 'BALANCETE'
+        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
+        :return: bool, True if marked or False if not marked
+        """
+        logging.warning("Starting to mark...")
+        data_dictionary = json.loads(requests.get(self.url_sig_company_events, verify=False).text)["dados"]
+        mark = False
+        for data in data_dictionary:
+            if (data["id_dominio"] == id_dominio) and (unidecode.unidecode(data[tag]) == event or
+                                                       event in unidecode.unidecode(data[tag])):
+                for dice in data["tarefas"]:
+                    for ID in id_task:
+                        if dice["id_tarefa"] == ID:
+                            url2 = self.url_sig_company_events_task.format(dice["id_empresa_evento_tarefa"])
+                            task_completed = {"dados": json.dumps({"status": "CON", "id_usuario": user})}
+                            headers = {'Accept': 'application/json, text/plain, */*',
+                                       'Content-Type': 'application/x-www-form-urlencoded'}
+                            requests.put(url=url2, data=task_completed, headers=headers, verify=False)
+                            mark = True
+        logging.warning("Finished marking")
+        return mark
+
+    def check_sig(self, id_dominio: str = AnyStr, event: str = AnyStr, tag: str = AnyStr):
+        """
+
+        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
+        :param event: str with the event that will be checked, ex.: 'BALANCETE'
+        :param id_dominio: str with the 'id dominio' of the company
+        :return: dict with the tasks ids and status, true if the task has been marked else false
+        """
+        logging.warning("Starting to check...")
+        data_dictionary = json.loads(requests.get(self.url_sig_company_events, verify=False).text)["dados"]
+        task = {}
+        for data in data_dictionary:
+            if (data["id_dominio"] == id_dominio) and (unidecode.unidecode(data[tag]) == event or
+                                                       event in unidecode.unidecode(data[tag])):
+                for dice in data["tarefas"]:
+                    task.update({dice["id_tarefa"]: False if dice["status"] == "NCON" else True})
+        logging.warning("Finished checking")
+        return task
+
+
+class IntranetRequests:
+    def __init__(self, id_dominio: str = Optional, id_company: str = Optional):
+        self.id_dominio = id_dominio
+        self.id_company = id_company
+
+    def tax_amount(self, url_tax_amount: str = AnyStr, code: int = Iterable, date: str = AnyStr):
+        """
+
+        :param url_tax_amount:
+        :param date: str containing the competence of the file being worked on
+        :param code: int with the tax code for identification on the intranet
+        :return: float with the tax value
+        """
+        logging.warning("Extracting value...")
+
+        date = date.split('.')
+        last_day = monthrange(int(date[1]), int(date[0]))
+        first_date = f"{str(date[1])}-{str(date[0])}-01"
+        last_date = f"{str(date[1])}-{str(date[0])}-{str(last_day[1])}"
+        url = url_tax_amount.format(self.id_dominio, first_date, last_date, str(code))
+        req = requests.get(url, verify=False)
+        text = req.text
+        text = (text.replace('Array', '')).replace('  ', '')
+        lines = text.splitlines()
+        data_list = []
+
+        for line in lines:
+            if findall('[a-z]', line):
+                data_list.append(line)
+        value = float((data_list[-1]).split(' ')[-1])
+        logging.warning(f"The value that was extracted: {value}")
+        return value
+
+    def get_intranet(self, url):
+
+        """
+        :param url: Url do GET - Deve ser informada no .env
+        :return: Informacoes do Intranet
+        """
+
+        headers = {'Content-type': 'application/json',
+                   'Accept': 'application/json'}
+        if self.id_request is not None:
+            return_inform = requests.get(url=f'{url}{self.id_request}', headers=headers, verify=True)
+            return_inform_format = json.loads(return_inform.text)
+
+            return return_inform_format
+        else:
+            return_inform = requests.get(url=url, headers=headers, verify=True)
+            return_inform_format = json.loads(return_inform.text)
+
+            return return_inform_format
+
+    def get_company_email(self, url_client_email: str = AnyStr, company: str = AnyStr, sector: str = AnyStr,
+                          tag_number: str = AnyStr):
+        """
+
+        :param url_client_email:
+        :param company: str with the company name
+        :param sector: str with the sector number and name, ex.: '2-Fiscal'
+        :param tag_number: str with the tag number in the db
+        :return: dict with data and status of the request
+        """
+        logging.warning("Extracting company email...")
+
+        req = requests.get(url_client_email + self.id_company, verify=False)
+        text = req.text
+
+        text_json = json.loads(text)
+        data = text_json["dados"]
+        group = [company, self.id_dominio]
+        email = []
+
+        if not data:
+            if group not in email:
+                logging.warning("Email not found")
+                return {"data": '', "status": False}
+        else:
+            for dat in data:
+                try:
+                    if sector in dat["setores"] and tag_number in dat["tags"]:
+                        email.append(dat['email'])
+                except TypeError:
+                    continue
+            if not email:
+                logging.warning("Email not found")
+                return {"data": '', "status": False}
+        for item in email:
+            try:
+                if '@' in item:
+                    logging.warning("Extracted email")
+                    return {"data": email, "status": True}
+            except TypeError:
+                continue
+        logging.warning("Email not found")
+        return {"data": '', "status": False}
+
+    def get_deadline(self, url_deadline: str = AnyStr, event: str = AnyStr, tag: str = AnyStr):
+        """
+
+        :param url_deadline:
+        :param event: str with the event that will be marked, ex.: 'BALANCETE'
+        :param tag: str with the key, ex.: 'nome_evento', 'nome_evento_tarefa'...
+        :return: str with the deadline
+        """
+        logging.warning("Extracting deadline...")
+        data_dictionary = json.loads(requests.get(url_deadline, verify=False).text)["dados"]
+        deadline = AnyStr
+        for dic in data_dictionary:
+            try:
+                if dic['id_dominio'] == self.id_dominio:
+                    if dic[tag] == event or event in dic[tag]:
+                        date = str(dic['prazo_final']).split('-')
+                        deadline = f"{date[2]}/{date[1]}/{date[0]}"
+            except:
+                continue
+        logging.warning("Extracted deadline")
+        return deadline
+
+
```

### Comparing `cgcomponents-2.0.2/cgcomponents.egg-info/PKG-INFO` & `cgcomponents-2.0.3/cgcomponents.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: cgcomponents
-Version: 2.0.2
+Version: 2.0.3
 Summary: Components para scrapping da CG.
 Home-page: https://github.com/ramirooliveiracg/cgcomponents
 Author: Gabriel Dalacorte e Rogerio Filho
 Author-email: gnunes.servico@gmail.com, crofilho2@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Portal Components
+# CG Components
 
 ## Getting Started
 #### Dependencies
-You need Python 3.7 or later to use **portalcomponents**.
+You need Python 3.7 or later to use **cgcomponents**.
 ```
 pip install setuptools
 pip install wheel
 pip install twine
 ```
 #### Installation
 Clone this repo to your local machine using:
 ```
 git clone https://github.com/ramirooliveiracg/cgcomponents.git
 ```
 ## Features
 - File structure for PyPI packages
 - Setup with package informations
 - License example
-
```

### Comparing `cgcomponents-2.0.2/setup.py` & `cgcomponents-2.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from setuptools import setup
-
-
-def readme():
-    with open('README.md') as f:
-        README = f.read()
-    return README
-
-
-setup(
-    name="cgcomponents",
-    version="2.0.2",
-    description="Components para scrapping da CG.",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/ramirooliveiracg/cgcomponents",
-    author="Gabriel Dalacorte e Rogerio Filho",
-    author_email="gnunes.servico@gmail.com, crofilho2@gmail.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-    ],
-    packages=["cgcomponents"],
-    include_package_data=True,
-    install_requires=["requests", "Unidecode"],
-)
+from setuptools import setup
+
+
+def readme():
+    with open('README.md') as f:
+        README = f.read()
+    return README
+
+
+setup(
+    name="cgcomponents",
+    version="2.0.3",
+    description="Components para scrapping da CG.",
+    long_description=readme(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/ramirooliveiracg/cgcomponents",
+    author="Gabriel Dalacorte e Rogerio Filho",
+    author_email="gnunes.servico@gmail.com, crofilho2@gmail.com",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+    ],
+    packages=["cgcomponents"],
+    include_package_data=True,
+    install_requires=["requests", "Unidecode"],
+)
```

