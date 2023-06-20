# Comparing `tmp/reliableGPT-0.1.6.tar.gz` & `tmp/reliableGPT-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reliableGPT-0.1.6.tar", last modified: Tue Jun 20 06:46:47 2023, max compression
+gzip compressed data, was "reliableGPT-0.1.9.tar", last modified: Tue Jun 20 21:53:08 2023, max compression
```

## Comparing `reliableGPT-0.1.6.tar` & `reliableGPT-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.705878 reliableGPT-0.1.6/
--rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.6/LICENSE
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:46:47.705685 reliableGPT-0.1.6/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.6/README.md
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.704638 reliableGPT-0.1.6/reliableGPT.egg-info/
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)      265 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       24 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.705344 reliableGPT-0.1.6/reliablegpt/
--rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.6/reliablegpt/__init__.py
--rw-r--r--   0 daddyish   (501) staff       (20)     4095 2023-06-20 06:40:45.000000 reliableGPT-0.1.6/reliablegpt/main.py
--rw-r--r--   0 daddyish   (501) staff       (20)     2111 2023-06-20 06:41:07.000000 reliableGPT-0.1.6/reliablegpt/tests.py
--rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 06:46:47.705922 reliableGPT-0.1.6/setup.cfg
--rw-r--r--   0 daddyish   (501) staff       (20)      293 2023-06-20 06:46:42.000000 reliableGPT-0.1.6/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.139170 reliableGPT-0.1.9/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-20 21:53:08.139076 reliableGPT-0.1.9/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2083 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.138551 reliableGPT-0.1.9/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      265 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       24 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-20 21:53:08.000000 reliableGPT-0.1.9/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-20 21:53:08.138949 reliableGPT-0.1.9/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.1.9/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4229 2023-06-20 21:44:53.000000 reliableGPT-0.1.9/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1830 2023-06-20 21:45:33.000000 reliableGPT-0.1.9/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-20 21:53:08.139200 reliableGPT-0.1.9/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      293 2023-06-20 21:52:40.000000 reliableGPT-0.1.9/setup.py
```

### Comparing `reliableGPT-0.1.6/LICENSE` & `reliableGPT-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.1.6/reliablegpt/main.py` & `reliableGPT-0.1.9/reliablegpt/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,78 +16,76 @@
             new_kwargs.pop('messages', None) # remove messages for completion models 
             return openai.Completion.create(**new_kwargs)
     except Exception as e:
         print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
         return None
     return None
 
-def fallback_request(fallback_strategy, kwargs):
+def fallback_request(args, kwargs, fallback_strategy):
     result = None
-    start_time = time.time()
-    # print(f"in fall req {fallback_strategy}")
     for model in fallback_strategy:
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
         result = make_LLM_request(new_kwargs)
         if result != None:
             return result    
     return None
 
-def handle_openAI_error(openAI_error, kwargs, fallback_strategy=[], graceful_string="Sorry, the OpenAI (GPT) failed"):
+def handle_openAI_error(args, kwargs, openAI_error, fallback_strategy, graceful_string):
     # Error Types from https://platform.openai.com/docs/guides/error-codes/python-library-error-types
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
     # 4. APIConnectionError - Check your network settings, proxy configuration, SSL certificates, or firewall rules.
     # 5. InvalidRequestError - User input was bad: context_length_exceeded, 
     # 6. AuthenticationError - API key not working, return default hardcoded message
     # 7. ServiceUnavailableError - retry, retry with fallback
-    if fallback_strategy == []:
-        fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002']
     error_type = openAI_error['type']
     if error_type == 'invalid_request_error' or error_type == 'InvalidRequestError':
         print(colored("ReliableGPT: invalid request error", "red"))
         # check if this is context window related, try with a 16k model
         if openAI_error.code == 'context_length_exceeded':
             fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
-            result = fallback_request(fallback_strategy=fallback_strategy, kwargs=kwargs)
+            result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
             if result == None:
                 return graceful_string
             else:
                 return result
 
     # todo: alert on user_email that there is now an auth error 
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
         print(colored("ReliableGPT: Auth error", "red"))
         return graceful_string
 
     # catch all 
-    result = fallback_request(fallback_strategy=fallback_strategy, kwargs=kwargs)
+    result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
-def reliable_create(fallback_strategy=[], retries=5):
-    def decorator(func):
-        @functools.wraps(func)
-        def decorator_wrapper(*args, **kwargs):
+class reliableGPT:
+    def __init__(self, openai_create_function, fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], graceful_string="Sorry, the OpenAI API is currently down"):
+        self.openai_create_function = openai_create_function
+        self.graceful_string = graceful_string
+        self.fallback_strategy = fallback_strategy
+
+    def __call__(self, *args, **kwargs):
+        try:
+            result = self.openai_create_function(*args, **kwargs)
+            return result
+        except Exception as e:
             try:
-                print(fallback_strategy)
-                print(retries)
-                response = func(*args, **kwargs)
-                return response
-            except Exception as e:
                 print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
                 print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
-                # print({e.code})
-                # print(e.error)
-                result = handle_openAI_error(e.error, fallback_strategy=fallback_strategy, kwargs=kwargs)
+                result = handle_openAI_error(
+                    args = args,
+                    kwargs = kwargs,
+                    openAI_error = e.error,
+                    fallback_strategy = self.fallback_strategy,
+                    graceful_string = self.graceful_string
+                )
                 print(colored(f"ReliableGPT: Recoverd got a successfull response {result}", "green"))
                 return result
-
-        return decorator_wrapper
-    return decorator
-
-
-
+            except:
+                return self.fallback_strategy
```

### Comparing `reliableGPT-0.1.6/reliablegpt/tests.py` & `reliableGPT-0.1.9/reliablegpt/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import openai
-from main import reliable_create
+from main import reliableGPT
 
-@reliable_create(fallback_strategy=['gpt-3.5-turbo', 'text-davinci-003', 'text-davinci-003'], retries=5)
-def reliable_openai_call(model, messages, temperature):
-   return openai.ChatCompletion.create(model=model,
-                                            messages=messages,
-                                            temperature=temperature)
+# make openAI reliable and safe
+openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create)
 
-
-openai.api_key = "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"
+openai.api_key = "<API KEY>"
 
 import concurrent.futures
 
 def test_multiple_calls():
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
@@ -25,15 +21,15 @@
     error_count = 0
     failure_count = 0  # Track the number of failures
 
     def call_reliable_openai():
         nonlocal error_count, failure_count
         try:
             print("Making OpenAI Call")
-            response = reliable_openai_call(model=model, messages=messages, temperature=temperature)
+            response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
             if response and "error" in response:
                 error_count += 1
             if response == "Sorry, the OpenAI (GPT) failed":
                 failure_count += 1
         except Exception as e:
             print("Exception occurred:", e)
             error_count += 1
@@ -51,9 +47,7 @@
 
     if error_count == 0:
         print("All calls executed successfully.")
     else:
         print("Some calls returned errors.")
 
 test_multiple_calls()
-
-
```

