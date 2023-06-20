# Comparing `tmp/reliableGPT-0.1.1.tar.gz` & `tmp/reliableGPT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reliableGPT-0.1.1.tar", last modified: Tue Jun 20 02:01:14 2023, max compression
+gzip compressed data, was "dist/reliableGPT-0.1.2.tar", last modified: Tue Jun 20 05:54:16 2023, max compression
```

## Comparing `reliableGPT-0.1.1.tar` & `reliableGPT-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.441614 reliableGPT-0.1.1/
--rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.1/LICENSE
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 02:01:14.441419 reliableGPT-0.1.1/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.1/README.md
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.440401 reliableGPT-0.1.1/reliableGPT.egg-info/
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)      259 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       17 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.440831 reliableGPT-0.1.1/reliablegpt/
--rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.1/reliablegpt/__init__.py
--rw-r--r--   0 daddyish   (501) staff       (20)     4035 2023-06-20 01:44:48.000000 reliableGPT-0.1.1/reliablegpt/main.py
--rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 02:01:14.441654 reliableGPT-0.1.1/setup.cfg
--rw-r--r--   0 daddyish   (501) staff       (20)      275 2023-06-20 02:00:56.000000 reliableGPT-0.1.1/setup.py
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.441141 reliableGPT-0.1.1/tests/
--rw-r--r--   0 daddyish   (501) staff       (20)     1804 2023-06-20 01:26:23.000000 reliableGPT-0.1.1/tests/tests.py
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 05:54:16.349253 reliableGPT-0.1.2/
+-rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.2/LICENSE
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 05:54:16.348986 reliableGPT-0.1.2/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.2/README.md
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 05:54:16.342096 reliableGPT-0.1.2/reliableGPT.egg-info/
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 05:54:16.000000 reliableGPT-0.1.2/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)      265 2023-06-20 05:54:16.000000 reliableGPT-0.1.2/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 05:54:16.000000 reliableGPT-0.1.2/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       24 2023-06-20 05:54:16.000000 reliableGPT-0.1.2/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 05:54:16.000000 reliableGPT-0.1.2/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 05:54:16.342787 reliableGPT-0.1.2/reliablegpt/
+-rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.2/reliablegpt/__init__.py
+-rw-r--r--   0 daddyish   (501) staff       (20)     4003 2023-06-20 05:52:39.000000 reliableGPT-0.1.2/reliablegpt/main.py
+-rw-r--r--   0 daddyish   (501) staff       (20)     2105 2023-06-20 05:31:15.000000 reliableGPT-0.1.2/reliablegpt/tests.py
+-rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 05:54:16.349306 reliableGPT-0.1.2/setup.cfg
+-rw-r--r--   0 daddyish   (501) staff       (20)      293 2023-06-20 05:54:02.000000 reliableGPT-0.1.2/setup.py
```

### Comparing `reliableGPT-0.1.1/LICENSE` & `reliableGPT-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.1.1/reliablegpt/main.py` & `reliableGPT-0.1.2/reliablegpt/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,39 @@
 import openai
 from termcolor import colored
 import time
 import functools
 import copy
 
-CHAT_MODELS = [
-    'gpt-4',
-    'gpt-4-0613',
-    'gpt-4-32k',
-    'gpt-4-32k-0613'
-    'gpt-3.5-turbo'
-    'gpt-3.5-turbo-16k',
-    'gpt-3.5-turbo-0613'
-]
-
-TEXT_MODELS = [
-    'text-davinci-003',
-    'text-davinci-002',
-    'text-curie-001',
-    'ada',
-    'babbage'
-]
-
 def make_LLM_request(new_kwargs):
     try:
         model = new_kwargs['model']
-        #print(kwargs)
-        # print(model)
-        if "3.5" or "4" in model:
+        if "3.5" or "4" in model: # call ChatCompletion
             print(colored(f"ReliableGPT: Retrying request with model CHAT {model}", "blue"))
             return openai.ChatCompletion.create(**new_kwargs)
         else:
             print(colored(f"ReliableGPT: Retrying request with model TEXT {model}", "blue"))
             new_kwargs['prompt'] = " ".join([message["content"] for message in new_kwargs['messages']])
             new_kwargs.pop('messages', None) # remove messages for completion models 
             return openai.Completion.create(**new_kwargs)
     except Exception as e:
-        print(colored(f"ReliableGPT: Got 2nd Error {e}", "red"))
+        print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
         return None
     return None
 
 def fallback_request(fallback_strategy, kwargs):
     result = None
     start_time = time.time()
     # print(fallback_strategy)
     for model in fallback_strategy:
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
         result = make_LLM_request(new_kwargs)
         if result != None:
-            return result
+            return result    
     return None
 
 def handle_openAI_error(openAI_error, kwargs, fallback_strategy=[], graceful_string="Sorry, the OpenAI (GPT) failed"):
     # Error Types from https://platform.openai.com/docs/guides/error-codes/python-library-error-types
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
@@ -71,39 +51,43 @@
             fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
             result = fallback_request(fallback_strategy, kwargs)
             if result == None:
                 return graceful_string
             else:
                 return result
 
+    # todo: alert on user_email that there is now an auth error 
     elif error_type == 'authentication_error' or error_type == 'AuthenticationError':
         print(colored("ReliableGPT: Auth error", "red"))
         return graceful_string
 
     # catch all 
     result = fallback_request(fallback_strategy, kwargs)
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
+def reliable_create(fallback_strategy=[], retries=5):
+    def decorator(func):
+        @functools.wraps(func)
+        def decorator_wrapper(*args, **kwargs):
+            try:
+                print(fallback_strategy)
+                print(retries)
+                response = func(*args, **kwargs)
+                return response
+            except Exception as e:
+                print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
+                print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
+                # print({e.code})
+                # print(e.error)
+                result = handle_openAI_error(e.error, fallback_strategy, kwargs)
+                print(colored(f"ReliableGPT: Recoverd got a successfull response {result}", "green"))
+                return result
 
-def reliable_create(func):
-    @functools.wraps(func)
-    def decorator_wrapper(*args, **kwargs):
-        try:
-            response = func(*args, **kwargs)
-            return response
-        except Exception as e:
-            print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
-            print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
-            # print({e.code})
-            # print(e.error)
-            result = handle_openAI_error(e.error, kwargs)
-            print(colored(f"ReliableGPT: Recoverd got a successfull response {result}", "green"))
-            return handle_openAI_error(e.error, kwargs)
-
-    return decorator_wrapper
+        return decorator_wrapper
+    return decorator
```

### Comparing `reliableGPT-0.1.1/tests/tests.py` & `reliableGPT-0.1.2/reliablegpt/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import openai
 from main import reliable_create
 
-@reliable_create
+@reliable_create(fallback_strategy=['gpt-3.5', 'text-davinci-003', 'text-davinci-003'], retries=5)
 def reliable_openai_call(model, messages, temperature):
    return openai.ChatCompletion.create(model=model,
                                             messages=messages,
                                             temperature=temperature)
 
 
-openai.api_key = "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"
+openai.api_key = "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"
 
 import concurrent.futures
 
 def test_multiple_calls():
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Who won the world series in 2020?"*400},
         {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
         {"role": "user", "content": "Where was it played?"}
     ]
     temperature = 0.7
 
     error_count = 0
+    failure_count = 0  # Track the number of failures
 
     def call_reliable_openai():
-        nonlocal error_count
+        nonlocal error_count, failure_count
         try:
             print("Making OpenAI Call")
             response = reliable_openai_call(model=model, messages=messages, temperature=temperature)
             if response and "error" in response:
                 error_count += 1
+            if response == "Sorry, the OpenAI (GPT) failed":
+                failure_count += 1
         except Exception as e:
             print("Exception occurred:", e)
             error_count += 1
 
     # Create a ThreadPoolExecutor with a maximum of 10 threads
     with concurrent.futures.ThreadPoolExecutor(max_workers=10) as executor:
         # Submit the callable to the executor for each call
-        future_calls = [executor.submit(call_reliable_openai) for _ in range(200)]
+        future_calls = [executor.submit(call_reliable_openai) for _ in range(20)]
 
         # Wait for all the futures to complete
         concurrent.futures.wait(future_calls)
 
     print(f"Error Count: {error_count}")
+    print(f"Fallback response count: {failure_count}")
 
     if error_count == 0:
         print("All calls executed successfully.")
     else:
         print("Some calls returned errors.")
 
 test_multiple_calls()
```

