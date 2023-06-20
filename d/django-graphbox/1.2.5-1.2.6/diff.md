# Comparing `tmp/django_graphbox-1.2.5.tar.gz` & `tmp/django_graphbox-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_graphbox-1.2.5.tar", last modified: Sat Jun 10 02:29:33 2023, max compression
+gzip compressed data, was "django_graphbox-1.2.6.tar", last modified: Tue Jun 20 19:46:44 2023, max compression
```

## Comparing `django_graphbox-1.2.5.tar` & `django_graphbox-1.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.5/LICENSE
--rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/MANIFEST.in
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)    20300 2023-02-23 04:15:18.000000 django_graphbox-1.2.5/README.md
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.800131 django_graphbox-1.2.5/docs/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.804131 django_graphbox-1.2.5/docs/source/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    17832 2023-06-10 02:21:38.000000 django_graphbox-1.2.5/docs/source/quickstart.rst
--rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/pyproject.toml
--rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-06-10 02:29:33.812130 django_graphbox-1.2.5/setup.cfg
--rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2022-07-20 15:01:25.000000 django_graphbox-1.2.5/setup.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.800131 django_graphbox-1.2.5/src/
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.804131 django_graphbox-1.2.5/src/django_graphbox/
--rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    12736 2023-06-10 02:21:38.000000 django_graphbox-1.2.5/src/django_graphbox/builder.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     1821 2023-06-10 02:26:09.000000 django_graphbox-1.2.5/src/django_graphbox/constants.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2022-07-30 04:00:13.000000 django_graphbox-1.2.5/src/django_graphbox/exceptions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/hasher.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/src/django_graphbox/helpers/
--rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/__init__.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    16216 2023-06-10 02:27:05.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/mutations.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     6662 2023-05-07 23:58:24.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/queries.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2022-07-30 04:08:45.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/sessions.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2022-07-20 02:16:01.000000 django_graphbox-1.2.5/src/django_graphbox/helpers/shared.py
--rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-02-23 21:40:53.000000 django_graphbox-1.2.5/src/django_graphbox/session.py
-drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:29:33.808130 django_graphbox-1.2.5/src/django_graphbox.egg-info/
--rw-r--r--   0 yeison    (1000) yeison    (1000)    18375 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-06-10 02:29:33.000000 django_graphbox-1.2.5/src/django_graphbox.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.419966 django_graphbox-1.2.6/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1086 2023-02-22 16:07:59.000000 django_graphbox-1.2.6/LICENSE
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       34 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18661 2023-06-20 19:46:44.419966 django_graphbox-1.2.6/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    20702 2023-06-20 04:05:52.000000 django_graphbox-1.2.6/README.md
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.407966 django_graphbox-1.2.6/docs/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.411966 django_graphbox-1.2.6/docs/source/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18118 2023-06-20 04:04:29.000000 django_graphbox-1.2.6/docs/source/quickstart.rst
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      108 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/pyproject.toml
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      890 2023-06-20 19:46:44.423966 django_graphbox-1.2.6/setup.cfg
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       52 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/setup.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.407966 django_graphbox-1.2.6/src/
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.415966 django_graphbox-1.2.6/src/django_graphbox/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        0 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    13509 2023-06-20 04:01:35.000000 django_graphbox-1.2.6/src/django_graphbox/builder.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     1821 2023-06-10 02:34:40.000000 django_graphbox-1.2.6/src/django_graphbox/constants.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     3417 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/exceptions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      522 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/hasher.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.419966 django_graphbox-1.2.6/src/django_graphbox/helpers/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       60 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/helpers/__init__.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    16216 2023-06-10 02:34:40.000000 django_graphbox-1.2.6/src/django_graphbox/helpers/mutations.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     6662 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/helpers/queries.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2101 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/helpers/sessions.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)     2381 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/helpers/shared.py
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    24289 2023-06-10 02:34:31.000000 django_graphbox-1.2.6/src/django_graphbox/session.py
+drwxr-xr-x   0 yeison    (1000) yeison    (1000)        0 2023-06-20 19:46:44.419966 django_graphbox-1.2.6/src/django_graphbox.egg-info/
+-rw-r--r--   0 yeison    (1000) yeison    (1000)    18661 2023-06-20 19:46:44.000000 django_graphbox-1.2.6/src/django_graphbox.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      693 2023-06-20 19:46:44.000000 django_graphbox-1.2.6/src/django_graphbox.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)        1 2023-06-20 19:46:44.000000 django_graphbox-1.2.6/src/django_graphbox.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)      165 2023-06-20 19:46:44.000000 django_graphbox-1.2.6/src/django_graphbox.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) yeison    (1000)       16 2023-06-20 19:46:44.000000 django_graphbox-1.2.6/src/django_graphbox.egg-info/top_level.txt
```

### Comparing `django_graphbox-1.2.5/LICENSE` & `django_graphbox-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/PKG-INFO` & `django_graphbox-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_graphbox
-Version: 1.2.5
+Version: 1.2.6
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -347,7 +347,9 @@
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
     * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
+    * Version 1.2.4 Fix custom attributes on the model Type.
+    * Version 1.2.5 Add support to select the operations to build for the model. You can select between field_by_id, list_field, create_field, update_field and delete_field operations. By default all operations are selected.
```

### Comparing `django_graphbox-1.2.5/README.md` & `django_graphbox-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 -   login (Mutation)
 -   social_login (Mutation)
 -   actual_user (Query)
 
 This package don't limit to use this basic operations. Custom operations can be defined on classic style of Graphene and Graphene-Django and finally can be merged on the main schema as described on the Quickstart section of this documentation at 4. Create a main schema in a new file called schema.py on my_project folder. This file can be used to merge all queries and mutations from all apps builded with django_graphbox or just add your own queries and mutations.
 
-See the full documentation at <https://90horasporsemana.com/graphbox/>
+See the API REFERENCE at <https://90horasporsemana.com/graphbox/>
 
 # Installation
 
 > ``` bash
 > $ pip install django-graphbox
 > ```
 
@@ -443,7 +443,10 @@
 -   Callbacks by operation (callbacks that can be used to execute a
     callable resolver after the mutation is executed)
 -   Automatic integration with [Django Auditor Logs](https://pypi.org/project/django-auditor-logs/) (A package that can be used to log the data changes on the models, maintained by the same author of this package)
 
 # Release Notes
 
 > -   Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
+> -   Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
+> -   Version 1.2.4 Fix custom attributes on the model Type.
+> -   Version 1.2.5 Add support to select the operations to build for the model. You can select between field_by_id, list_field, create_field, update_field and delete_field operations. By default all operations are selected.
```

### Comparing `django_graphbox-1.2.5/docs/source/quickstart.rst` & `django_graphbox-1.2.6/docs/source/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -330,8 +330,10 @@
             
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
-    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
+    * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
+    * Version 1.2.4 Fix custom attributes on the model Type.
+    * Version 1.2.5 Add support to select the operations to build for the model. You can select between field_by_id, list_field, create_field, update_field and delete_field operations. By default all operations are selected.
```

### Comparing `django_graphbox-1.2.5/setup.cfg` & `django_graphbox-1.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_graphbox
-version = 1.2.5
+version = 1.2.6
 description = Package for easy building GraphQL API with Django
 long_description = file:docs/source/quickstart.rst
 url = https://github.com/yefeza/django-graphbox
 author = Yeison Fernandez
 author_email = contacto@90horasporsemana.com
 license = MIT
 classifiers =
```

### Comparing `django_graphbox-1.2.5/src/django_graphbox/builder.py` & `django_graphbox-1.2.6/src/django_graphbox/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Args:
             session_manager (SessionManager): Session manager to use.
         """
         self._models_config = {}
         self._models_by_op_name = {}
         self._session_manager = session_manager
 
-    def add_model(self, model, exclude_fields=(), pagination_length=0, pagination_style='infinite', external_filters=[], internal_filters=[], filters_opeator=Q.AND, access_group=None, access_by_operation={}, validators_by_operation={}, internal_field_resolvers={}, exclude_fields_by_operation={}, save_as_password=[], callbacks_by_operation={}, custom_attrs_for_type=[], ordering_field='id', **kwargs):
+    def add_model(self, model, exclude_fields=(), pagination_length=0, pagination_style='infinite', external_filters=[], internal_filters=[], filters_opeator=Q.AND, access_group=None, access_by_operation={}, validators_by_operation={}, internal_field_resolvers={}, exclude_fields_by_operation={}, save_as_password=[], callbacks_by_operation={}, custom_attrs_for_type=[], ordering_field='id', operations_to_build=['field_by_id', 'list_field', 'create_field', 'update_field', 'delete_field'], **kwargs):
         """Add model for build operations.
 
         Args:
             model (django.models.Model): Model to add to the schema.
             exclude_fields (tuple or list): Fields to exclude from the model type.
             pagination_length (int): Number of items to return in a paginated response. 0 means no pagination.
             pagination_style (str): Pagination style. Possible values are 'infinite' and 'paginated'.
@@ -38,23 +38,24 @@
             access_by_operation (dict): Dictionary with the operations to use for the access. {'operation': 'access_group', ...}
             validators_by_operation (dict): Dictionary with the validators to use for the access. {'operation': callable(info, model_instance, **kwargs), ...}
             internal_field_resolvers (dict): Dictionary with the internal field value resolvers on create_field and update_field operations
             save_as_password (list): List of fields to save as password with make_password function.
             callbacks_by_operation (dict): Dictionary with the callbacks list to use for the access. {'operation': [callable(info, model_instance, **kwargs)], ...}
             custom_attrs_for_type (list): List of custom attributes to add to the model type. [{'name': 'attr_name', 'value': 'attr_value'}, ...]
             ordering_field (str): Field to use for ordering the list_field operation.
+            operations_to_build (list): List of operations to build. Possible values are 'field_by_id', 'list_field', 'create_field', 'update_field' and 'delete_field'.
         """
         #get the model name
         model_name = model.__name__
         #crreate the model type
         model_metaclass = type(f"Meta", (), {'model': model, 'exclude_fields': exclude_fields})
-        model_type = type(f"{model_name}Type", (DjangoObjectType,), {'Meta': model_metaclass})
-        #add custom attributes to the model type
+        type_attrs={'Meta': model_metaclass}
         for attr in custom_attrs_for_type:
-            setattr(model_type, attr['name'], attr['value'])
+            type_attrs[attr['name']]=attr['value']
+        model_type = type(f"{model_name}Type", (DjangoObjectType,), type_attrs)
         #create paginated type
         if pagination_length > 0 and pagination_style == 'paginated':
             paginated_type = type(f"{model_name}PageType", (graphene.ObjectType,), {'items': graphene.List(model_type), 'page': graphene.Int(), 'has_next_page': graphene.Boolean(), 'has_previous_page': graphene.Boolean(), 'total_pages': graphene.Int(), 'total_items': graphene.Int()})
         else:
             paginated_type = None
         #make a new model config
         config = {
@@ -70,75 +71,81 @@
             'access_group': access_group,
             'access_by_operation': access_by_operation,
             'validators_by_operation': validators_by_operation,
             'internal_field_resolvers': internal_field_resolvers,
             'exclude_fields_by_operation': exclude_fields_by_operation,
             'save_as_password': save_as_password,
             'callbacks_by_operation': callbacks_by_operation,
-            'ordering_field': ordering_field
+            'ordering_field': ordering_field,
+            'operations_to_build': operations_to_build
         }
         self._models_config[model_name]=config
 
     def build_schema_query(self):
         """ Build query class for the schema.
 
         Returns:
             graphene.ObjectType: Query class for the schema.
         """
         query_class= type("Query", (graphene.ObjectType,), {})
         for key in self._models_config.keys():
             model_config=self._models_config[key]
             object_name=model_config['name'].lower()
             # build field_by_id query
-            field_by_id_resolver_function=build_field_by_id_resolver(self)
-            self._models_by_op_name[object_name]=model_config
-            setattr(query_class, object_name, graphene.Field(model_config['type'], id=graphene.ID(required=True)))
-            setattr(query_class, f'resolve_{object_name}', field_by_id_resolver_function)
+            if 'field_by_id' in model_config['operations_to_build']:
+                field_by_id_resolver_function=build_field_by_id_resolver(self)
+                self._models_by_op_name[object_name]=model_config
+                setattr(query_class, object_name, graphene.Field(model_config['type'], id=graphene.ID(required=True)))
+                setattr(query_class, f'resolve_{object_name}', field_by_id_resolver_function)
             # build list_field query
-            field_list_resolver_function=build_field_list_resolver(self)
-            self._models_by_op_name['all' + object_name]=model_config
-            return_object=get_return_object(model_config)
-            setattr(query_class, f"all_{object_name}", return_object)
-            setattr(query_class, f'resolve_all_{object_name}',field_list_resolver_function)
+            if 'list_field' in model_config['operations_to_build']:
+                field_list_resolver_function=build_field_list_resolver(self)
+                self._models_by_op_name['all' + object_name]=model_config
+                return_object=get_return_object(model_config)
+                setattr(query_class, f"all_{object_name}", return_object)
+                setattr(query_class, f'resolve_all_{object_name}',field_list_resolver_function)
         return query_class
     
     def build_schema_mutation(self):
         """Build mutations class for the schema. 
         
         Returns:
             graphene.ObjectType: Mutations class for the schema.
         """
         mutation_class= type("Mutation", (), {})
         for key in self._models_config.keys():
             model_config=self._models_config[key]
             # create the create mutation
-            mutate_create_function=build_mutate_for_create(self)
-            # get fields to ignore on arguments
-            fields_to_ignore=get_fields_to_ignore(model_config, 'create_field')
-            # build argumants class
-            arguments_create=create_arguments_class(model_config['model'], fields_to_ignore)
-            create_mutation=type("Create"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(),model_config['name'].lower(): graphene.Field(model_config['type']), "error":graphene.Field(ErrorMsgType), 'Arguments': arguments_create, 'mutate': mutate_create_function})
-            setattr(mutation_class, f"create_{model_config['name'].lower()}", create_mutation.Field())
-            self._models_by_op_name['create' + model_config['name'].lower()]=model_config
+            if 'create_field' in model_config['operations_to_build']:
+                mutate_create_function=build_mutate_for_create(self)
+                # get fields to ignore on arguments
+                fields_to_ignore=get_fields_to_ignore(model_config, 'create_field')
+                # build argumants class
+                arguments_create=create_arguments_class(model_config['model'], fields_to_ignore)
+                create_mutation=type("Create"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(),model_config['name'].lower(): graphene.Field(model_config['type']), "error":graphene.Field(ErrorMsgType), 'Arguments': arguments_create, 'mutate': mutate_create_function})
+                setattr(mutation_class, f"create_{model_config['name'].lower()}", create_mutation.Field())
+                self._models_by_op_name['create' + model_config['name'].lower()]=model_config
             # create the update mutation
-            mutate_update_function=build_mutate_for_update(self)
-            # get fields to omit
-            fields_to_ignore=get_fields_to_ignore(model_config, 'update_field')
-            # build argumants class
-            arguments_update=update_arguments_class(model_config['model'], fields_to_ignore, model_config.get('save_as_password'))
-            update_mutation=type("Update"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(),model_config['name'].lower(): graphene.Field(model_config['type']), "error":graphene.Field(ErrorMsgType), 'Arguments': arguments_update, 'mutate': mutate_update_function})
-            setattr(mutation_class, f"update_{model_config['name'].lower()}", update_mutation.Field())
-            self._models_by_op_name['update' + model_config['name'].lower()]=model_config
+            if 'update_field' in model_config['operations_to_build']:
+                mutate_update_function=build_mutate_for_update(self)
+                # get fields to omit
+                fields_to_ignore=get_fields_to_ignore(model_config, 'update_field')
+                # build argumants class
+                arguments_update=update_arguments_class(model_config['model'], fields_to_ignore, model_config.get('save_as_password'))
+                update_mutation=type("Update"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(),model_config['name'].lower(): graphene.Field(model_config['type']), "error":graphene.Field(ErrorMsgType), 'Arguments': arguments_update, 'mutate': mutate_update_function})
+                setattr(mutation_class, f"update_{model_config['name'].lower()}", update_mutation.Field())
+                self._models_by_op_name['update' + model_config['name'].lower()]=model_config
             # create the delete mutation
-            mutate_delete_function=build_mutate_for_delete(self)
-            # build argumants class
-            delete_arguments=delete_arguments_class()
-            delete_mutation=type("Delete"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(), "error":graphene.Field(ErrorMsgType), 'Arguments': delete_arguments, 'mutate': mutate_delete_function})
-            setattr(mutation_class, f"delete_{model_config['name'].lower()}", delete_mutation.Field())
-            self._models_by_op_name['delete' + model_config['name'].lower()]=model_config
+            if 'delete_field' in model_config['operations_to_build']:
+                mutate_delete_function=build_mutate_for_delete(self)
+                # build argumants class
+                delete_arguments=delete_arguments_class()
+                delete_mutation=type("Delete"+model_config['name'], (graphene.Mutation,), {"estado":graphene.Boolean(), "error":graphene.Field(ErrorMsgType), 'Arguments': delete_arguments, 'mutate': mutate_delete_function})
+                setattr(mutation_class, f"delete_{model_config['name'].lower()}", delete_mutation.Field())
+                self._models_by_op_name['delete' + model_config['name'].lower()]=model_config
         return mutation_class
 
     def build_session_schema(self):
         """ Build the session mutations and queries for the schema.
             The operations are:
                 - login Mutation
                 - social_login Mutation (if the social login is configured)
```

### Comparing `django_graphbox-1.2.5/src/django_graphbox/constants.py` & `django_graphbox-1.2.6/src/django_graphbox/constants.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/exceptions.py` & `django_graphbox-1.2.6/src/django_graphbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/hasher.py` & `django_graphbox-1.2.6/src/django_graphbox/hasher.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/helpers/mutations.py` & `django_graphbox-1.2.6/src/django_graphbox/helpers/mutations.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/helpers/queries.py` & `django_graphbox-1.2.6/src/django_graphbox/helpers/queries.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/helpers/sessions.py` & `django_graphbox-1.2.6/src/django_graphbox/helpers/sessions.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/helpers/shared.py` & `django_graphbox-1.2.6/src/django_graphbox/helpers/shared.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox/session.py` & `django_graphbox-1.2.6/src/django_graphbox/session.py`

 * *Files identical despite different names*

### Comparing `django_graphbox-1.2.5/src/django_graphbox.egg-info/PKG-INFO` & `django_graphbox-1.2.6/src/django_graphbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-graphbox
-Version: 1.2.5
+Version: 1.2.6
 Summary: Package for easy building GraphQL API with Django
 Home-page: https://github.com/yefeza/django-graphbox
 Author: Yeison Fernandez
 Author-email: contacto@90horasporsemana.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -347,7 +347,9 @@
             SessionManager.build_access_level_validator(model_field='role') will return a function that will validate if the user_instance.role exists on the list of MODIFY_PERMISSIONS[actual_user.role].
 
 Release Notes
 ----------------------------
 
     * Version 1.0.0 to 1.1.5 was a package developed for a specific project, and the code was not published on GitHub. The code was refactored and published on GitHub on version 1.2.0.
     * Version 1.2.3 add support to set custom attributes on the model Type and set custom ordering field for the queries.
+    * Version 1.2.4 Fix custom attributes on the model Type.
+    * Version 1.2.5 Add support to select the operations to build for the model. You can select between field_by_id, list_field, create_field, update_field and delete_field operations. By default all operations are selected.
```

### Comparing `django_graphbox-1.2.5/src/django_graphbox.egg-info/SOURCES.txt` & `django_graphbox-1.2.6/src/django_graphbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

