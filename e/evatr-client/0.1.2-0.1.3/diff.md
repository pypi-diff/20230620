# Comparing `tmp/evatr-client-0.1.2.tar.gz` & `tmp/evatr-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evatr-client-0.1.2.tar", last modified: Sun Jun 18 20:33:36 2023, max compression
+gzip compressed data, was "evatr-client-0.1.3.tar", last modified: Tue Jun 20 13:00:17 2023, max compression
```

## Comparing `evatr-client-0.1.2.tar` & `evatr-client-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.533229 evatr-client-0.1.2/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1068 2023-06-16 08:34:10.000000 evatr-client-0.1.2/LICENSE.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-18 20:33:36.533398 evatr-client-0.1.2/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3366 2023-06-18 20:29:03.000000 evatr-client-0.1.2/README.md
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.530634 evatr-client-0.1.2/evatr_client/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      171 2023-06-16 17:00:00.000000 evatr-client-0.1.2/evatr_client/__init__.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     6120 2023-06-18 20:21:06.000000 evatr-client-0.1.2/evatr_client/client.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-17 16:38:13.000000 evatr-client-0.1.2/evatr_client/status_codes.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     5913 2023-06-18 20:25:16.000000 evatr-client-0.1.2/evatr_client/util.py
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-18 20:33:36.532921 evatr-client-0.1.2/evatr_client.egg-info/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      317 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/SOURCES.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/dependency_links.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/requires.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-18 20:33:36.000000 evatr-client-0.1.2/evatr_client.egg-info/top_level.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-18 20:33:36.534039 evatr-client-0.1.2/setup.cfg
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1221 2023-06-18 20:32:26.000000 evatr-client-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:17.155938 evatr-client-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-06-19 11:15:02.000000 evatr-client-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      881 2023-06-20 13:00:17.156952 evatr-client-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3444 2023-06-19 11:15:02.000000 evatr-client-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:17.147938 evatr-client-0.1.3/evatr_client/
+-rw-rw-rw-   0        0        0      173 2023-06-19 11:15:02.000000 evatr-client-0.1.3/evatr_client/__init__.py
+-rw-rw-rw-   0        0        0     6373 2023-06-20 12:55:48.000000 evatr-client-0.1.3/evatr_client/client.py
+-rw-rw-rw-   0        0        0     4612 2023-06-19 11:15:02.000000 evatr-client-0.1.3/evatr_client/status_codes.py
+-rw-rw-rw-   0        0        0     6074 2023-06-20 12:50:01.000000 evatr-client-0.1.3/evatr_client/util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:17.154951 evatr-client-0.1.3/evatr_client.egg-info/
+-rw-rw-rw-   0        0        0      881 2023-06-20 13:00:17.000000 evatr-client-0.1.3/evatr_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-20 13:00:17.000000 evatr-client-0.1.3/evatr_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:00:17.000000 evatr-client-0.1.3/evatr_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 13:00:17.000000 evatr-client-0.1.3/evatr_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 13:00:17.000000 evatr-client-0.1.3/evatr_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 13:00:17.157938 evatr-client-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-06-20 12:56:47.000000 evatr-client-0.1.3/setup.py
```

### Comparing `evatr-client-0.1.2/LICENSE.txt` & `evatr-client-0.1.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-MIT License
-Copyright (c) 2023 Cedric Altermatt
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+Copyright (c) 2023 Cedric Altermatt
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `evatr-client-0.1.2/PKG-INFO` & `evatr-client-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: evatr-client
-Version: 0.1.2
-Summary: A client for: https://evatr.bff-online.de/eVatR/
-Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.2.tar.gz
-Author: CeeDiii
-License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Metadata-Version: 2.1
+Name: evatr-client
+Version: 0.1.3
+Summary: A client for: https://evatr.bff-online.de/eVatR/
+Home-page: https://github.com/CeeDiii/evatr-client
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/0.1.3.tar.gz
+Author: CeeDiii
+License: MIT
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
```

### Comparing `evatr-client-0.1.2/README.md` & `evatr-client-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# Python eVatR Client
-A Python client for simple and qualified VAT-number validations. 
-
-This is a Python port of the Typescript client that can be found here: [eVatR Typescript Client](https://github.com/qqilihq/evatr/tree/master)
-
-You can find detailed information on the underlying API here (German): https://evatr.bff-online.de/eVatR/xmlrpc/
-
-Users need to provide a registered German VAT-number (Umsatzsteuer-Identifikationsnummern) to use this client.
-
-This tool is not endorsed by the "Bundeszentralamt für Steuern".
-
-## Usage
-```python
-from evatr_client import EvatrClient, ISimpleParams, IQualifiedParams
-
-client = EvatrClient()
-
-simpleParams: ISimpleParams = ISimpleParams(include_raw_xml=False,
-                                                own_vat_number='<your own VAT number>', 
-                                                validate_vat_number='<the VAT number to validate>')
-
-client.check_simple(simpleParams)
-
-qualifiedParams: IQualifiedParams = IQualifiedParams(include_raw_xml=False,
-                                                own_vat_number='<your own VAT number>', 
-                                                validate_vat_number='<the VAT number to validate>', 
-                                                company_name='<SomeCompany Srl>', 
-                                                city='Milano', 
-                                                zip='20123', 
-                                                street='Via Italia 22')
-
-client.check_qualified(qualifiedParams)
-```
-
-## Installation
-The source code is currently hosted on GitHub at: https://github.com/CeeDiii/evatr-client
-
-The Python package is available at Python Package Index (PyPI)
-
-```
-$ pip install evatr-client
-```
-## Development
-
-Install dependencies from the `requirements.txt` file:
-
-```shell
-$ pip install -r requirements.txt
-```
-
-You can scrape the error codes with the script `scripts/scrape_status_codes.py`. The script has to be executed from the project root directory:
-
-```shell
-$ python scripts/scrape_status_codes.py
-```
-
-## Testing 
-To get the actual test results, execute the following command from the root project directory:
-
-```shell
-$ python -m unittest tests/test_client.py
-```
-
-## Contributing 
-Feel free to open issues and pull requests in this repo.
-
-## License MIT
-Copyright © 2023 CeeDiii
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-
-
+# Python eVatR Client
+A Python client for simple and qualified VAT-number validations. 
+
+This is a Python port of the Typescript client that can be found here: [eVatR Typescript Client](https://github.com/qqilihq/evatr/tree/master)
+
+You can find detailed information on the underlying API here (German): https://evatr.bff-online.de/eVatR/xmlrpc/
+
+Users need to provide a registered German VAT-number (Umsatzsteuer-Identifikationsnummern) to use this client.
+
+This tool is not endorsed by the "Bundeszentralamt für Steuern".
+
+## Usage
+```python
+from evatr_client import EvatrClient, ISimpleParams, IQualifiedParams
+
+client = EvatrClient()
+
+simpleParams: ISimpleParams = ISimpleParams(include_raw_xml=False,
+                                                own_vat_number='<your own VAT number>', 
+                                                validate_vat_number='<the VAT number to validate>')
+
+client.check_simple(simpleParams)
+
+qualifiedParams: IQualifiedParams = IQualifiedParams(include_raw_xml=False,
+                                                own_vat_number='<your own VAT number>', 
+                                                validate_vat_number='<the VAT number to validate>', 
+                                                company_name='<SomeCompany Srl>', 
+                                                city='Milano', 
+                                                zip='20123', 
+                                                street='Via Italia 22')
+
+client.check_qualified(qualifiedParams)
+```
+
+## Installation
+The source code is currently hosted on GitHub at: https://github.com/CeeDiii/evatr-client
+
+The Python package is available at Python Package Index (PyPI)
+
+```
+$ pip install evatr-client
+```
+## Development
+
+Install dependencies from the `requirements.txt` file:
+
+```shell
+$ pip install -r requirements.txt
+```
+
+You can scrape the error codes with the script `scripts/scrape_status_codes.py`. The script has to be executed from the project root directory:
+
+```shell
+$ python scripts/scrape_status_codes.py
+```
+
+## Testing 
+To get the actual test results, execute the following command from the root project directory:
+
+```shell
+$ python -m unittest tests/test_client.py
+```
+
+## Contributing 
+Feel free to open issues and pull requests in this repo.
+
+## License MIT
+Copyright © 2023 CeeDiii
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+
+
```

### Comparing `evatr-client-0.1.2/evatr_client/client.py` & `evatr-client-0.1.3/evatr_client/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,167 +1,169 @@
-import requests
-
-from dataclasses import asdict
-from typing import Dict
-from urllib.parse import urlencode
-from xml.etree.ElementTree import fromstring
-
-from .util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, get_error_description, get_result_description
-
-class EvatrClient:
-    '''
-    A client for making requests to the eVatR service and parsing the XML responses.
-
-    This client provides methods to retrieve XML data from the eVatR RPC-API and parse the responses into simple or qualified result objects.
-    
-    A detailed definition of this API can be found here (link in German):
-    https://evatr.bff-online.de/eVatR/xmlrpc/
-    
-    '''
-    def _retrieve_xml(self, params: ISimpleParams | IQualifiedParams, qualified: bool = False) -> str:
-        '''
-        Retrieves XML data from the eVatR service based on the provided parameters.
-
-        Args:
-            params (ISimpleParams | IQualifiedParams): The parameters to be included in the request.
-            qualified (bool, optional): Indicates whether the request should include qualified parameters. Defaults to False.
-
-        Returns:
-            str: The XML data retrieved from the eVatR service.
-
-        Raises:
-            AttributeError: If the `params` argument is None.
-        
-        '''
-        if params is None:
-            raise AttributeError()
-
-        query = {
-            'UstId_1': params.own_vat_number,
-            'UstId_2': params.validate_vat_number
-        }
-
-        if qualified:
-            query['Firmenname'] = params.company_name
-            query['Ort'] = params.city
-            query['PLZ'] = params.zip
-            query['Strasse'] = params.street
-
-        requestUrl = f'https://evatr.bff-online.de/evatrRPC?{urlencode(query)}'
-        res = requests.get(requestUrl)
-
-        if res.ok:
-            return res.text
-        else:
-            raise Exception()
-        
-    def _map_xml_response_data(self, raw_xml: str) -> Dict:
-        '''
-        Maps the XML response data to a dictionary.
-
-        Args:
-            raw_xml (str): The raw XML response data.
-
-        Returns:
-            dict: A dictionary containing the mapped response data.
-
-        '''
-        root = fromstring(raw_xml)
-        params = root.findall('.//param')
-        label = []
-        values = []
-        for param in params:
-            val_tag = param.findall('.//string')
-            if len(val_tag) >= 2:
-                label.append(val_tag[0].text)
-                values.append(val_tag[1].text)
-        response = dict(zip(label, values))
-        return response
-
-    def _parse_xml_response(self, raw_xml: str, qualified: bool = False, include_raw_xml: bool = False) -> ISimpleResult | IQualifiedResult:   
-        '''
-        Parses the XML response into a simple or qualified result object.
-
-        Args:
-            raw_xml (str): The raw XML response data.
-            qualified (bool, optional): Indicates whether the response should be parsed as a qualified result. Defaults to False.
-            include_raw_xml (bool, optional): Indicates whether to include the raw XML in the result object. Defaults to False.
-
-        Returns:
-            ISimpleResult | IQualifiedResult: The parsed result object.
-        
-        '''
-        response = self._map_xml_response_data(raw_xml)
-
-        error_code = int(response['ErrorCode'])
-        result_name = response['Erg_Name']
-        result_city = response['Erg_Ort']
-        result_zip = response['Erg_PLZ']
-        result_street = response['Erg_Str']
-
-        result = ISimpleResult(
-            valid=error_code == 200,
-            date=response['Datum'],
-            time=response['Uhrzeit'],
-            error_code=response['ErrorCode'],
-            error_description=get_error_description(error_code),
-            own_vat_number=response['UstId_1'],
-            validated_vat_number=response['UstId_2'],
-            valid_from=response['Gueltig_ab'],
-            valid_until=response['Gueltig_bis'],
-            raw_xml=raw_xml if include_raw_xml else None
-        )
-
-        if qualified:
-            result = IQualifiedResult(
-                *asdict(result).values(),
-                company_name=response['Firmenname'],
-                city=response['Ort'],
-                zip=response['PLZ'],
-                street=response['Strasse'],
-                result_name=result_name,
-                result_city=result_city,
-                result_zip=result_zip,
-                result_street=result_street,
-                result_name_description=get_result_description(result_name),
-                result_city_description=get_result_description(result_city),
-                result_zip_description=get_result_description(result_zip),
-                result_street_description=get_result_description(result_street)
-            )
-
-        return result
-
-
-    def check_simple(self, params: ISimpleParams):
-        '''
-        Performs a simple VAT number check using the provided parameters.
-
-        Args:
-            params (ISimpleParams): The parameters for the simple VAT number check.
-
-        Returns:
-            ISimpleResult: The result of the simple VAT number check.
-        
-        For more information, see (link in German):
-        https://evatr.bff-online.de/eVatR/xmlrpc/schnittstelle
-        
-        '''
-        xml = self._retrieve_xml(params, qualified=False)
-        return self._parse_xml_response(xml, qualified=False, include_raw_xml=params.include_raw_xml)
-
-
-    def check_qualified(self, params: IQualifiedParams):
-        '''
-        Performs a qualified VAT number check using the provided parameters.
-
-        Args:
-            params (IQualifiedParams): The parameters for the qualified VAT number check.
-
-        Returns:
-            IQualifiedResult: The result of the qualified VAT number check.
-        
-        For more information, see (link in German):
-        https://evatr.bff-online.de/eVatR/xmlrpc/schnittstelle
-        
-        '''
-        xml = self._retrieve_xml(params, qualified=True)
+import requests
+
+from dataclasses import asdict
+from typing import Dict, Union
+from urllib.parse import urlencode
+from xml.etree.ElementTree import fromstring
+
+from .util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, get_error_description, get_result_description
+
+class EvatrClient:
+    '''
+    A client for making requests to the eVatR service and parsing the XML responses.
+
+    This client provides methods to retrieve XML data from the eVatR RPC-API and parse the responses into simple or qualified result objects.
+    
+    A detailed definition of this API can be found here (link in German):
+    https://evatr.bff-online.de/eVatR/xmlrpc/
+    
+    '''
+    def _retrieve_xml(self, params: Union[ISimpleParams, IQualifiedParams], qualified: bool = False) -> str:
+        '''
+        Retrieves XML data from the eVatR service based on the provided parameters.
+
+        Args:
+            params (ISimpleParams | IQualifiedParams): The parameters to be included in the request.
+            qualified (bool, optional): Indicates whether the request should include qualified parameters. Defaults to False.
+
+        Returns:
+            str: The XML data retrieved from the eVatR service.
+
+        Raises:
+            AttributeError: If the `params` argument is None.
+        
+        '''
+        if params is None:
+            raise AttributeError()
+
+        query = {
+            'UstId_1': params.own_vat_number,
+            'UstId_2': params.validate_vat_number
+        }
+
+        if qualified:
+            query['Firmenname'] = params.company_name
+            query['Ort'] = params.city
+            query['PLZ'] = params.zip
+            query['Strasse'] = params.street
+
+        requestUrl = f'https://evatr.bff-online.de/evatrRPC?{urlencode(query)}'
+
+        # explicitly throw exception if it times out
+        res = requests.get(requestUrl, timeout=15)
+
+        if res.ok:
+            return res.text
+        else:
+            raise Exception()
+        
+    def _map_xml_response_data(self, raw_xml: str) -> Dict:
+        '''
+        Maps the XML response data to a dictionary.
+
+        Args:
+            raw_xml (str): The raw XML response data.
+
+        Returns:
+            dict: A dictionary containing the mapped response data.
+
+        '''
+        root = fromstring(raw_xml)
+        params = root.findall('.//param')
+        label = []
+        values = []
+        for param in params:
+            val_tag = param.findall('.//string')
+            if len(val_tag) >= 2:
+                label.append(val_tag[0].text)
+                values.append(val_tag[1].text)
+        response = dict(zip(label, values))
+        return response
+
+    def _parse_xml_response(self, raw_xml: str, qualified: bool = False, include_raw_xml: bool = False) -> Union[ISimpleResult, IQualifiedResult]:   
+        '''
+        Parses the XML response into a simple or qualified result object.
+
+        Args:
+            raw_xml (str): The raw XML response data.
+            qualified (bool, optional): Indicates whether the response should be parsed as a qualified result. Defaults to False.
+            include_raw_xml (bool, optional): Indicates whether to include the raw XML in the result object. Defaults to False.
+
+        Returns:
+            ISimpleResult | IQualifiedResult: The parsed result object.
+        
+        '''
+        response = self._map_xml_response_data(raw_xml)
+
+        error_code = int(response['ErrorCode'])
+        result_name = response['Erg_Name']
+        result_city = response['Erg_Ort']
+        result_zip = response['Erg_PLZ']
+        result_street = response['Erg_Str']
+
+        result = ISimpleResult(
+            valid=error_code == 200,
+            date=response['Datum'],
+            time=response['Uhrzeit'],
+            error_code=response['ErrorCode'],
+            error_description=get_error_description(error_code),
+            own_vat_number=response['UstId_1'],
+            validated_vat_number=response['UstId_2'],
+            valid_from=response['Gueltig_ab'],
+            valid_until=response['Gueltig_bis'],
+            raw_xml=raw_xml if include_raw_xml else None
+        )
+
+        if qualified:
+            result = IQualifiedResult(
+                *asdict(result).values(),
+                company_name=response['Firmenname'],
+                city=response['Ort'],
+                zip=response['PLZ'],
+                street=response['Strasse'],
+                result_name=result_name,
+                result_city=result_city,
+                result_zip=result_zip,
+                result_street=result_street,
+                result_name_description=get_result_description(result_name),
+                result_city_description=get_result_description(result_city),
+                result_zip_description=get_result_description(result_zip),
+                result_street_description=get_result_description(result_street)
+            )
+
+        return result
+
+
+    def check_simple(self, params: ISimpleParams):
+        '''
+        Performs a simple VAT number check using the provided parameters.
+
+        Args:
+            params (ISimpleParams): The parameters for the simple VAT number check.
+
+        Returns:
+            ISimpleResult: The result of the simple VAT number check.
+        
+        For more information, see (link in German):
+        https://evatr.bff-online.de/eVatR/xmlrpc/schnittstelle
+        
+        '''
+        xml = self._retrieve_xml(params, qualified=False)
+        return self._parse_xml_response(xml, qualified=False, include_raw_xml=params.include_raw_xml)
+
+
+    def check_qualified(self, params: IQualifiedParams):
+        '''
+        Performs a qualified VAT number check using the provided parameters.
+
+        Args:
+            params (IQualifiedParams): The parameters for the qualified VAT number check.
+
+        Returns:
+            IQualifiedResult: The result of the qualified VAT number check.
+        
+        For more information, see (link in German):
+        https://evatr.bff-online.de/eVatR/xmlrpc/schnittstelle
+        
+        '''
+        xml = self._retrieve_xml(params, qualified=True)
         return self._parse_xml_response(xml, qualified=True, include_raw_xml=params.include_raw_xml)
```

### Comparing `evatr-client-0.1.2/evatr_client/util.py` & `evatr-client-0.1.3/evatr_client/util.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from dataclasses import dataclass
-from enum import Enum
-from typing import Optional
-
-from .status_codes import status_codes
-
-class ResultType(Enum):
-    MATCH = 'A',
-    NO_MATCH = 'B',
-    NOT_QUERIED = 'C',
-    NOT_RETURNED = 'D',
-
-@dataclass
-class ISimpleParams:
-    '''
-    Parameters for a simple VAT number check.
-
-    Args:
-        include_raw_xml (bool): Whether to include the raw XML response in the result.
-        own_vat_number (str): The VAT number used for validation.
-        validate_vat_number (str): The VAT number to validate.
-
-    '''
-    include_raw_xml: bool
-    own_vat_number: str
-    validate_vat_number: str
-
-
-@dataclass
-class IQualifiedParams(ISimpleParams):
-    '''
-    Parameters for a qualified VAT number check.
-
-    Args:
-        include_raw_xml (bool): Whether to include the raw XML response in the result.
-        own_vat_number (str): The VAT number used for validation.
-        validate_vat_number (str): The VAT number to validate.
-        company_name (str): The name of the company to validate.
-        city (str): The city of the company to validate.
-        zip (Optional[str]): The zip code of the company to validate (optional).
-        street (Optional[str]): The street of the company to validate (optional).
-    
-    '''
-    company_name: str
-    city: str
-    zip: Optional[str] = None
-    street: Optional[str] = None
-
-
-@dataclass
-class ISimpleResult:
-    '''
-    Result of a simple VAT number check.
-
-    Args:
-        valid (bool): Indicates whether the VAT number is valid.
-        date (str): The date of the check.
-        time (str): The time of the check.
-        error_code (int): The error code of the check.
-        error_description (str): The description of the error.
-        own_vat_number (str): The VAT number that was used for validation.
-        validated_vat_number (str): The VAT number that was validated.
-        valid_from (Optional[str]): The start date of the VAT number validity (optional).
-        valid_until (Optional[str]): The end date of the VAT number validity (optional).
-        raw_xml (Optional[str]): The raw XML response (optional).
-
-    '''
-    valid: bool
-    date: str
-    time: str
-    error_code: int
-    error_description: str
-    own_vat_number: str
-    validated_vat_number: str
-    valid_from: Optional[str] = None
-    valid_until: Optional[str] = None
-    raw_xml: Optional[str] = None
-
-
-@dataclass
-class IQualifiedResult(ISimpleResult):
-    '''
-    Result of a qualified VAT number check.
-
-    Args:
-    Result of a simple VAT number check.
-
-    Args:
-        valid (bool): Indicates whether the VAT number is valid.
-        date (str): The date of the check.
-        time (str): The time of the check.
-        error_code (int): The error code of the check.
-        error_description (str): The description of the error.
-        own_vat_number (str): The VAT number that was used for validation.
-        validated_vat_number (str): The VAT number that was validated.
-        valid_from (Optional[str]): The start date of the VAT number validity (optional).
-        valid_until (Optional[str]): The end date of the VAT number validity (optional).
-        raw_xml (Optional[str]): The raw XML response (optional).
-        company_name (Optional[str]): The name of the company (optional).
-        city (Optional[str]): The city where the company is located (optional).
-        zip (Optional[str]): The postal code of the company (optional).
-        street (Optional[str]): The street address of the company (optional).
-        result_name (Optional[ResultType]): The result of the name validation (optional).
-        result_city (Optional[ResultType]): The result of the city validation (optional).
-        result_zip (Optional[ResultType]): The result of the postal code validation (optional).
-        result_street (Optional[ResultType]): The result of the street address validation (optional).
-        result_name_description (Optional[str]): The description of the name validation result (optional).
-        result_city_description (Optional[str]): The description of the city validation result (optional).
-        result_zip_description (Optional[str]): The description of the zip code validation result (optional).
-        result_street_description (Optional[str]): The description of the street address validation result (optional).
-
-    '''
-    company_name: Optional[str] = None
-    city: Optional[str] = None
-    zip: Optional[str] = None
-    street: Optional[str] = None
-    result_name: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_city: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_zip: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_street: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_name_description: Optional[str] = None
-    result_city_description: Optional[str] = None
-    result_zip_description: Optional[str] = None
-    result_street_description: Optional[str] = None
-
-def get_result_description(result_type):
-    '''
-    Get the description for a specific result type.
-
-    Args:
-        result_type (ResultType): The result type.
-
-    Returns:
-        str: The description of the result type.
-
-    '''
-    if result_type == ResultType.MATCH:
-        return 'stimmt überein'
-    elif result_type == ResultType.NO_MATCH:
-        return 'stimmt nicht überein'
-    elif result_type == ResultType.NOT_QUERIED:
-        return 'nicht angefragt'
-    elif result_type == ResultType.NOT_RETURNED:
-        return 'vom EU-Mitgliedsstaat nicht mitgeteilt'
-    else:
-        return None
-    
-def get_error_description(error_code: int):
-    '''
-    Get the description for a specific error code.
-
-    Args:
-        error_code (int): The error code.
-
-    Returns:
-        str: The description of the error code.
-
-    '''
-    if str(error_code) in status_codes:
-       return status_codes[str(error_code)]
-    return 'Description not found for the given code.'
+from dataclasses import dataclass
+from enum import Enum
+from typing import Optional
+
+from .status_codes import status_codes
+
+class ResultType(Enum):
+    MATCH = 'A',
+    NO_MATCH = 'B',
+    NOT_QUERIED = 'C',
+    NOT_RETURNED = 'D',
+
+@dataclass
+class ISimpleParams:
+    '''
+    Parameters for a simple VAT number check.
+
+    Args:
+        include_raw_xml (bool): Whether to include the raw XML response in the result.
+        own_vat_number (str): The VAT number used for validation.
+        validate_vat_number (str): The VAT number to validate.
+
+    '''
+    include_raw_xml: bool
+    own_vat_number: str
+    validate_vat_number: str
+
+
+@dataclass
+class IQualifiedParams(ISimpleParams):
+    '''
+    Parameters for a qualified VAT number check.
+
+    Args:
+        include_raw_xml (bool): Whether to include the raw XML response in the result.
+        own_vat_number (str): The VAT number used for validation.
+        validate_vat_number (str): The VAT number to validate.
+        company_name (str): The name of the company to validate.
+        city (str): The city of the company to validate.
+        zip (Optional[str]): The zip code of the company to validate (optional).
+        street (Optional[str]): The street of the company to validate (optional).
+    
+    '''
+    company_name: str
+    city: str
+    zip: Optional[str] = None
+    street: Optional[str] = None
+
+
+@dataclass
+class ISimpleResult:
+    '''
+    Result of a simple VAT number check.
+
+    Args:
+        valid (bool): Indicates whether the VAT number is valid.
+        date (str): The date of the check.
+        time (str): The time of the check.
+        error_code (int): The error code of the check.
+        error_description (str): The description of the error.
+        own_vat_number (str): The VAT number that was used for validation.
+        validated_vat_number (str): The VAT number that was validated.
+        valid_from (Optional[str]): The start date of the VAT number validity (optional).
+        valid_until (Optional[str]): The end date of the VAT number validity (optional).
+        raw_xml (Optional[str]): The raw XML response (optional).
+
+    '''
+    valid: bool
+    date: str
+    time: str
+    error_code: int
+    error_description: str
+    own_vat_number: str
+    validated_vat_number: str
+    valid_from: Optional[str] = None
+    valid_until: Optional[str] = None
+    raw_xml: Optional[str] = None
+
+
+@dataclass
+class IQualifiedResult(ISimpleResult):
+    '''
+    Result of a qualified VAT number check.
+
+    Args:
+    Result of a simple VAT number check.
+
+    Args:
+        valid (bool): Indicates whether the VAT number is valid.
+        date (str): The date of the check.
+        time (str): The time of the check.
+        error_code (int): The error code of the check.
+        error_description (str): The description of the error.
+        own_vat_number (str): The VAT number that was used for validation.
+        validated_vat_number (str): The VAT number that was validated.
+        valid_from (Optional[str]): The start date of the VAT number validity (optional).
+        valid_until (Optional[str]): The end date of the VAT number validity (optional).
+        raw_xml (Optional[str]): The raw XML response (optional).
+        company_name (Optional[str]): The name of the company (optional).
+        city (Optional[str]): The city where the company is located (optional).
+        zip (Optional[str]): The postal code of the company (optional).
+        street (Optional[str]): The street address of the company (optional).
+        result_name (Optional[ResultType]): The result of the name validation (optional).
+        result_city (Optional[ResultType]): The result of the city validation (optional).
+        result_zip (Optional[ResultType]): The result of the postal code validation (optional).
+        result_street (Optional[ResultType]): The result of the street address validation (optional).
+        result_name_description (Optional[str]): The description of the name validation result (optional).
+        result_city_description (Optional[str]): The description of the city validation result (optional).
+        result_zip_description (Optional[str]): The description of the zip code validation result (optional).
+        result_street_description (Optional[str]): The description of the street address validation result (optional).
+
+    '''
+    company_name: Optional[str] = None
+    city: Optional[str] = None
+    zip: Optional[str] = None
+    street: Optional[str] = None
+    result_name: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_city: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_zip: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_street: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_name_description: Optional[str] = None
+    result_city_description: Optional[str] = None
+    result_zip_description: Optional[str] = None
+    result_street_description: Optional[str] = None
+
+def get_result_description(result_type):
+    '''
+    Get the description for a specific result type.
+
+    Args:
+        result_type (ResultType): The result type.
+
+    Returns:
+        str: The description of the result type.
+
+    '''
+    if result_type == ResultType.MATCH:
+        return 'stimmt überein'
+    elif result_type == ResultType.NO_MATCH:
+        return 'stimmt nicht überein'
+    elif result_type == ResultType.NOT_QUERIED:
+        return 'nicht angefragt'
+    elif result_type == ResultType.NOT_RETURNED:
+        return 'vom EU-Mitgliedsstaat nicht mitgeteilt'
+    else:
+        return None
+    
+def get_error_description(error_code: int):
+    '''
+    Get the description for a specific error code.
+
+    Args:
+        error_code (int): The error code.
+
+    Returns:
+        str: The description of the error code.
+
+    '''
+    if str(error_code) in status_codes:
+       return status_codes[str(error_code)]
+    return 'Description not found for the given code.'
```

### Comparing `evatr-client-0.1.2/evatr_client.egg-info/PKG-INFO` & `evatr-client-0.1.3/evatr_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
-Name: evatr-client
-Version: 0.1.2
-Summary: A client for: https://evatr.bff-online.de/eVatR/
-Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.2.tar.gz
-Author: CeeDiii
-License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Metadata-Version: 2.1
+Name: evatr-client
+Version: 0.1.3
+Summary: A client for: https://evatr.bff-online.de/eVatR/
+Home-page: https://github.com/CeeDiii/evatr-client
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/0.1.3.tar.gz
+Author: CeeDiii
+License: MIT
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
```

