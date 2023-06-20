# Comparing `tmp/ilcdlib-0.7.1.tar.gz` & `tmp/ilcdlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.7.1.tar", max compression
+gzip compressed data, was "ilcdlib-0.8.0.tar", max compression
```

## Comparing `ilcdlib-0.7.1.tar` & `ilcdlib-0.8.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    11357 2023-06-16 11:14:34.003952 ilcdlib-0.7.1/LICENSE
--rw-r--r--   0        0        0     4949 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/README.md
--rw-r--r--   0        0        0     3457 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17041 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1773 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4431 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6375 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     2665 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     3638 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     2738 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2023-06-16 11:14:34.007952 ilcdlib-0.7.1/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3774 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2596 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2003 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    31787 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2050 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0     8856 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     1206 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3329 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-06-16 11:14:34.011952 ilcdlib-0.7.1/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 ilcdlib-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 16:09:12.734236 ilcdlib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-06-20 16:09:12.734236 ilcdlib-0.8.0/README.md
+-rw-r--r--   0        0        0     3489 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17413 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1773 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4431 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6375 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     2665 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3638 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2738 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.738236 ilcdlib-0.8.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2596 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2003 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    31853 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2050 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0     9638 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     1206 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-06-20 16:09:12.742236 ilcdlib-0.8.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 ilcdlib-0.8.0/PKG-INFO
```

### Comparing `ilcdlib-0.7.1/LICENSE` & `ilcdlib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/README.md` & `ilcdlib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/pyproject.toml` & `ilcdlib-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.7.1"
+version = "0.8.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -29,14 +29,15 @@
 openepd = { version = ">=0.11.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
+wheel = { version ="~=0.40.0" }
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
 pytest = "~=7.2"
 pytest-subtests = "~=0.4"
 pytest-cov = "~=4.0"
 teamcity-messages = ">=1.31"
 lxml-stubs = { version = ">=0.4.0" }
@@ -59,15 +60,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.7.1"
+version = "0.8.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.7.1/src/ilcdlib/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/__main__.py` & `ilcdlib-0.8.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/__version__.py` & `ilcdlib-0.8.0/src/ilcdlib/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.7.1"
+VERSION = "0.8.0"
```

### Comparing `ilcdlib-0.7.1/src/ilcdlib/cli.py` & `ilcdlib-0.8.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/common.py` & `ilcdlib-0.8.0/src/ilcdlib/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,24 @@
                 process="http://lca.jrc.it/ILCD/Process",
                 source="http://lca.jrc.it/ILCD/Source",
                 ug="http://lca.jrc.it/ILCD/UnitGroup",
                 fp="http://lca.jrc.it/ILCD/FlowProperty",
                 mm="http://www.matml.org/",
                 epd2013="http://www.iai.kit.edu/EPD/2013",
                 epd2019="http://www.iai.kit.edu/EPD/2019",
+                epd2019_indata="http://www.indata.network/EPD/2019",
             )
         )
 
+    def remap_xml_ns(self, doc_ns_map: dict[str, str]) -> None:
+        """Remap XML namespaces."""
+        for n, url in doc_ns_map.items():
+            if url and url.endswith("EPD/2019"):  # Some providers use outdated, non-standard namespace
+                self.xml_parser.xml_ns["epd2019"] = url
+
     def get_xml_tree(
         self, entity_type: str, entity_id: str, entity_version: str | None, *, allow_static_datasets: bool = True
     ) -> T_ET.Element:
         """
         Get the xml tree for the given entity.
 
         :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
```

### Comparing `ilcdlib-0.7.1/src/ilcdlib/const.py` & `ilcdlib-0.8.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.8.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/dto.py` & `ilcdlib-0.8.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/category.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/compliance.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/contact.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/exchage.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/flow.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/material.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/source.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/unit.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/entity/validation.py` & `ilcdlib-0.8.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/cli.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/factory.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/epd/reader.py` & `ilcdlib-0.8.0/src/ilcdlib/epd/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         self.validation_reader_cls = validation_reader_cls
         if epd_process_id is None:
             entities = data_provider.list_entities(IlcdDatasetType.Processes)
             self.__epd_entity_ref = entities[0]
         else:
             self.__epd_entity_ref = IlcdReference(IlcdDatasetType.Processes, epd_process_id, epd_version)
         self.epd_el_tree = self.get_xml_tree(*self.__epd_entity_ref, allow_static_datasets=False)
+        self.remap_xml_ns(self.epd_el_tree.nsmap)  # type: ignore
         self.post_init()
 
     def post_init(self):
         """
         Post-initialization actions, will be executed as a last step in constructor.
 
         It could be overriden by subclasses to perform additional initialization actions.
```

### Comparing `ilcdlib-0.7.1/src/ilcdlib/extension.py` & `ilcdlib-0.8.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/http_common.py` & `ilcdlib-0.8.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/common.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/compliance.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/flows.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/indicators.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/properties.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/mapping/units.py` & `ilcdlib-0.8.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/medium/archive.py` & `ilcdlib-0.8.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.8.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/reference_data.py` & `ilcdlib-0.8.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.8.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.8.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/sanitizing/text.py` & `ilcdlib-0.8.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-0.8.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-0.8.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
+from hashlib import sha1
 from io import BytesIO
 from typing import IO, Iterable, Type
 from urllib.parse import urlencode
 
 from requests import HTTPError
 
 from ilcdlib.dto import Category, IlcdReference, ListResponseMeta, ProcessBasicInfo, ProcessSearchResponse
@@ -212,7 +213,30 @@
             total = response.meta.total_items_count
             processed_items_count = len(response.items)
             if processed_items_count == 0:
                 has_next = False
             else:
                 has_next = offset + processed_items_count <= total
             offset += processed_items_count
+
+    def get_sha1_by_url(self, url: str) -> str:
+        """
+        Get SHA1 hash of the file at the given URL or raise error if it is impossible to fetch the file.
+
+        :param url: URL of the file
+        """
+        response = self._do_request("get", url, stream=True)
+        hasher = sha1()
+        for x in response.iter_content(chunk_size=200):
+            hasher.update(x)
+        return hasher.hexdigest()
+
+    def get_sha1_by_url_or_none(self, url: str) -> str | None:
+        """
+        Get SHA1 hash of the file at the given URL or return none if it is impossible to fetch the file.
+
+        :param url: URL of the file
+        """
+        try:
+            return self.get_sha1_by_url(url)
+        except HTTPError:
+            return None
```

### Comparing `ilcdlib-0.7.1/src/ilcdlib/type.py` & `ilcdlib-0.8.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/utils.py` & `ilcdlib-0.8.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/src/ilcdlib/xml_parser.py` & `ilcdlib-0.8.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.7.1/PKG-INFO` & `ilcdlib-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.7.1
+Version: 0.8.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.7.1 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.8.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

