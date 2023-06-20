# Comparing `tmp/codespeak-0.1.1.tar.gz` & `tmp/codespeak-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codespeak-0.1.1.tar", max compression
+gzip compressed data, was "codespeak-0.1.2.tar", max compression
```

## Comparing `codespeak-0.1.1.tar` & `codespeak-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,54 @@
--rw-r--r--   0        0        0     4797 2023-06-13 18:29:30.683863 codespeak-0.1.1/README.md
--rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.1/codespeak/.DS_Store
--rw-r--r--   0        0        0      226 2023-06-13 22:08:40.406442 codespeak-0.1.1/codespeak/__init__.py
--rw-r--r--   0        0        0     1375 2023-06-13 18:29:30.685025 codespeak-0.1.1/codespeak/config.py
--rw-r--r--   0        0        0        0 2023-06-13 18:29:30.685083 codespeak-0.1.1/codespeak/core/__init__.py
--rw-r--r--   0        0        0     7137 2023-06-13 22:08:40.406870 codespeak-0.1.1/codespeak/core/code_generator.py
--rw-r--r--   0        0        0     5738 2023-06-13 18:29:30.685471 codespeak-0.1.1/codespeak/core/codespeak_service.py
--rw-r--r--   0        0        0     1430 2023-06-13 18:29:30.685635 codespeak-0.1.1/codespeak/core/diff.py
--rw-r--r--   0        0        0     1395 2023-06-13 22:08:40.407101 codespeak-0.1.1/codespeak/core/executor.py
--rw-r--r--   0        0        0     3048 2023-06-13 18:29:30.685940 codespeak-0.1.1/codespeak/core/openai_service.py
--rw-r--r--   0        0        0     2723 2023-06-13 18:29:30.686115 codespeak-0.1.1/codespeak/core/prompt.py
--rw-r--r--   0        0        0     4042 2023-06-13 18:41:04.484074 codespeak-0.1.1/codespeak/core/results_collector.py
--rw-r--r--   0        0        0     2553 2023-06-13 18:29:30.686456 codespeak-0.1.1/codespeak/declaration/body_imports.py
--rw-r--r--   0        0        0     5129 2023-06-13 22:08:40.407367 codespeak-0.1.1/codespeak/declaration/codespeak_declaration.py
--rw-r--r--   0        0        0     6029 2023-06-13 22:08:40.407580 codespeak-0.1.1/codespeak/declaration/declaration_file_service.py
--rw-r--r--   0        0        0     1714 2023-06-13 18:29:30.687033 codespeak-0.1.1/codespeak/declaration/declaration_helpers.py
--rw-r--r--   0        0        0     2275 2023-06-13 22:08:40.407768 codespeak-0.1.1/codespeak/decorate.py
--rw-r--r--   0        0        0       91 2023-06-13 18:29:30.687444 codespeak-0.1.1/codespeak/definitions/__init__.py
--rw-r--r--   0        0        0     5649 2023-06-13 18:29:30.687657 codespeak-0.1.1/codespeak/definitions/classify.py
--rw-r--r--   0        0        0      919 2023-06-13 18:29:30.687955 codespeak-0.1.1/codespeak/definitions/definition.py
--rw-r--r--   0        0        0     1046 2023-06-13 18:29:30.688156 codespeak-0.1.1/codespeak/definitions/free_modules.py
--rw-r--r--   0        0        0      491 2023-06-13 18:29:30.688390 codespeak-0.1.1/codespeak/definitions/types/builtin.py
--rw-r--r--   0        0        0      671 2023-06-13 18:29:30.688578 codespeak-0.1.1/codespeak/definitions/types/custom_type_reference.py
--rw-r--r--   0        0        0      497 2023-06-13 18:29:30.688778 codespeak-0.1.1/codespeak/definitions/types/generic.py
--rw-r--r--   0        0        0      648 2023-06-13 18:29:30.688984 codespeak-0.1.1/codespeak/definitions/types/installed_class.py
--rw-r--r--   0        0        0     2982 2023-06-13 18:29:30.689217 codespeak-0.1.1/codespeak/definitions/types/local_class.py
--rw-r--r--   0        0        0     1195 2023-06-13 18:29:30.689426 codespeak-0.1.1/codespeak/definitions/types/local_class_as_self.py
--rw-r--r--   0        0        0      476 2023-06-13 18:29:30.689642 codespeak-0.1.1/codespeak/definitions/types/none.py
--rw-r--r--   0        0        0     1951 2023-06-13 18:29:30.689879 codespeak-0.1.1/codespeak/definitions/types/typing_type.py
--rw-r--r--   0        0        0      634 2023-06-13 18:29:30.690067 codespeak-0.1.1/codespeak/definitions/types/union_type.py
--rw-r--r--   0        0        0      560 2023-06-13 18:29:30.690265 codespeak-0.1.1/codespeak/definitions/utils/dedupe.py
--rw-r--r--   0        0        0      557 2023-06-13 18:29:30.690455 codespeak-0.1.1/codespeak/definitions/utils/flat_uniques.py
--rw-r--r--   0        0        0      276 2023-06-13 18:29:30.690644 codespeak-0.1.1/codespeak/definitions/utils/flatten.py
--rw-r--r--   0        0        0      399 2023-06-13 18:29:30.690802 codespeak-0.1.1/codespeak/definitions/utils/group.py
--rw-r--r--   0        0        0     1131 2023-06-13 18:29:30.690966 codespeak-0.1.1/codespeak/definitions/utils/swap_custom_types.py
--rw-r--r--   0        0        0     1261 2023-06-13 18:29:30.691278 codespeak-0.1.1/codespeak/generate.py
--rw-r--r--   0        0        0      632 2023-06-13 18:29:30.691432 codespeak-0.1.1/codespeak/generated_exception.py
--rw-r--r--   0        0        0        0 2023-06-13 18:29:30.691476 codespeak-0.1.1/codespeak/helpers/__init__.py
--rw-r--r--   0        0        0      495 2023-06-13 18:29:30.691686 codespeak-0.1.1/codespeak/helpers/gather_arguments.py
--rw-r--r--   0        0        0      363 2023-06-13 18:29:30.691856 codespeak-0.1.1/codespeak/helpers/get_attr_from_qualname.py
--rw-r--r--   0        0        0      529 2023-06-13 18:29:30.692022 codespeak-0.1.1/codespeak/helpers/self_type.py
--rw-r--r--   0        0        0      388 2023-06-13 18:29:30.692180 codespeak-0.1.1/codespeak/helpers/set_attr_for_qualname.py
--rw-r--r--   0        0        0      309 2023-06-13 18:29:30.692351 codespeak-0.1.1/codespeak/metadata/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-13 18:29:30.692500 codespeak-0.1.1/codespeak/metadata/digest.py
--rw-r--r--   0        0        0        0 2023-06-13 18:29:30.692545 codespeak-0.1.1/codespeak/static_cushion/__init__.py
--rw-r--r--   0        0        0       91 2023-06-13 18:29:30.692743 codespeak-0.1.1/codespeak/static_cushion/example_return.py
--rw-r--r--   0        0        0       50 2023-06-13 18:29:30.692883 codespeak-0.1.1/codespeak/static_cushion/preserve_imports.py
--rw-r--r--   0        0        0      500 2023-06-13 22:08:40.407903 codespeak-0.1.1/codespeak/unsafe_execute.py
--rw-r--r--   0        0        0      396 2023-06-13 22:09:59.627989 codespeak-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 codespeak-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5715 2023-06-20 19:39:40.677547 codespeak-0.1.2/README.md
+-rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.2/codespeak/.DS_Store
+-rw-r--r--   0        0        0      153 2023-06-20 19:39:40.677947 codespeak-0.1.2/codespeak/__init__.py
+-rw-r--r--   0        0        0     4411 2023-06-20 19:39:40.678280 codespeak-0.1.2/codespeak/_clean.py
+-rw-r--r--   0        0        0      541 2023-06-20 19:39:40.678546 codespeak-0.1.2/codespeak/_cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:39:40.678610 codespeak-0.1.2/codespeak/_core/__init__.py
+-rw-r--r--   0        0        0     7148 2023-06-20 19:39:40.678871 codespeak-0.1.2/codespeak/_core/code_generator.py
+-rw-r--r--   0        0        0     5755 2023-06-20 19:39:40.679073 codespeak-0.1.2/codespeak/_core/codespeak_service.py
+-rw-r--r--   0        0        0     1433 2023-06-20 19:39:40.679249 codespeak-0.1.2/codespeak/_core/diff.py
+-rw-r--r--   0        0        0     1444 2023-06-20 19:39:40.679443 codespeak-0.1.2/codespeak/_core/executor.py
+-rw-r--r--   0        0        0     3058 2023-06-20 19:39:40.679626 codespeak-0.1.2/codespeak/_core/openai_service.py
+-rw-r--r--   0        0        0     2723 2023-06-20 19:39:40.679773 codespeak-0.1.2/codespeak/_core/prompt.py
+-rw-r--r--   0        0        0     4043 2023-06-20 19:39:40.679962 codespeak-0.1.2/codespeak/_core/results_collector.py
+-rw-r--r--   0        0        0     2555 2023-06-20 19:39:40.680156 codespeak-0.1.2/codespeak/_declaration/body_imports.py
+-rw-r--r--   0        0        0     5144 2023-06-20 19:39:40.680337 codespeak-0.1.2/codespeak/_declaration/codespeak_declaration.py
+-rw-r--r--   0        0        0     6200 2023-06-20 19:39:40.680582 codespeak-0.1.2/codespeak/_declaration/declaration_file_service.py
+-rw-r--r--   0        0        0     1716 2023-06-20 19:39:40.680747 codespeak-0.1.2/codespeak/_declaration/declaration_helpers.py
+-rw-r--r--   0        0        0     3363 2023-06-20 19:39:40.681007 codespeak-0.1.2/codespeak/_decorate.py
+-rw-r--r--   0        0        0       91 2023-06-20 19:39:40.681118 codespeak-0.1.2/codespeak/_definitions/__init__.py
+-rw-r--r--   0        0        0     5659 2023-06-20 19:39:40.681303 codespeak-0.1.2/codespeak/_definitions/classify.py
+-rw-r--r--   0        0        0      919 2023-06-20 19:39:40.681422 codespeak-0.1.2/codespeak/_definitions/definition.py
+-rw-r--r--   0        0        0     1046 2023-06-20 19:39:40.681540 codespeak-0.1.2/codespeak/_definitions/free_modules.py
+-rw-r--r--   0        0        0      492 2023-06-20 19:39:40.681714 codespeak-0.1.2/codespeak/_definitions/types/builtin.py
+-rw-r--r--   0        0        0      672 2023-06-20 19:39:40.681864 codespeak-0.1.2/codespeak/_definitions/types/custom_type_reference.py
+-rw-r--r--   0        0        0      498 2023-06-20 19:39:40.682010 codespeak-0.1.2/codespeak/_definitions/types/generic.py
+-rw-r--r--   0        0        0      649 2023-06-20 19:39:40.682171 codespeak-0.1.2/codespeak/_definitions/types/installed_class.py
+-rw-r--r--   0        0        0     2987 2023-06-20 19:39:40.682339 codespeak-0.1.2/codespeak/_definitions/types/local_class.py
+-rw-r--r--   0        0        0     1196 2023-06-20 19:39:40.682503 codespeak-0.1.2/codespeak/_definitions/types/local_class_as_self.py
+-rw-r--r--   0        0        0      477 2023-06-20 19:39:40.682674 codespeak-0.1.2/codespeak/_definitions/types/none.py
+-rw-r--r--   0        0        0     1955 2023-06-20 19:39:40.682849 codespeak-0.1.2/codespeak/_definitions/types/typing_type.py
+-rw-r--r--   0        0        0      636 2023-06-20 19:39:40.683011 codespeak-0.1.2/codespeak/_definitions/types/union_type.py
+-rw-r--r--   0        0        0      561 2023-06-20 19:39:40.683191 codespeak-0.1.2/codespeak/_definitions/utils/dedupe.py
+-rw-r--r--   0        0        0      560 2023-06-20 19:39:40.683334 codespeak-0.1.2/codespeak/_definitions/utils/flat_uniques.py
+-rw-r--r--   0        0        0      277 2023-06-20 19:39:40.683486 codespeak-0.1.2/codespeak/_definitions/utils/flatten.py
+-rw-r--r--   0        0        0      400 2023-06-20 19:39:40.683646 codespeak-0.1.2/codespeak/_definitions/utils/group.py
+-rw-r--r--   0        0        0     1133 2023-06-20 19:39:40.683802 codespeak-0.1.2/codespeak/_definitions/utils/swap_custom_types.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:39:40.683843 codespeak-0.1.2/codespeak/_helpers/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-20 19:39:40.684119 codespeak-0.1.2/codespeak/_helpers/auto_detect_abspath_to_project_root.py
+-rw-r--r--   0        0        0      495 2023-06-20 19:39:40.684233 codespeak-0.1.2/codespeak/_helpers/gather_arguments.py
+-rw-r--r--   0        0        0      363 2023-06-20 19:39:40.684357 codespeak-0.1.2/codespeak/_helpers/get_attr_from_qualname.py
+-rw-r--r--   0        0        0      530 2023-06-20 19:39:40.684491 codespeak-0.1.2/codespeak/_helpers/self_type.py
+-rw-r--r--   0        0        0      388 2023-06-20 19:39:40.684583 codespeak-0.1.2/codespeak/_helpers/set_attr_for_qualname.py
+-rw-r--r--   0        0        0      310 2023-06-20 19:39:40.684732 codespeak-0.1.2/codespeak/_metadata/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-20 19:39:40.684841 codespeak-0.1.2/codespeak/_metadata/digest.py
+-rw-r--r--   0        0        0     2164 2023-06-20 19:39:40.685005 codespeak-0.1.2/codespeak/_settings/_settings.py
+-rw-r--r--   0        0        0       83 2023-06-20 19:39:40.685229 codespeak-0.1.2/codespeak/_settings/environment.py
+-rw-r--r--   0        0        0       74 2023-06-20 19:39:40.685405 codespeak-0.1.2/codespeak/public/codespeak_helpers/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-20 19:39:40.685580 codespeak-0.1.2/codespeak/public/codespeak_helpers/generate.py
+-rw-r--r--   0        0        0     2056 2023-06-20 19:39:40.685742 codespeak-0.1.2/codespeak/public/codespeak_helpers/unsafe_execute.py
+-rw-r--r--   0        0        0     1813 2023-06-20 19:39:40.685906 codespeak-0.1.2/codespeak/public/codespeak_settings.py
+-rw-r--r--   0        0        0      194 2023-06-20 19:39:40.686058 codespeak-0.1.2/codespeak/public/example_return.py
+-rw-r--r--   0        0        0      632 2023-06-20 19:39:40.686161 codespeak-0.1.2/codespeak/public/generated_exception.py
+-rw-r--r--   0        0        0      457 2023-06-20 19:40:57.543890 codespeak-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 codespeak-0.1.2/PKG-INFO
```

### Comparing `codespeak-0.1.1/README.md` & `codespeak-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,141 @@
-
-
-
-
 # <img src="https://raw.githubusercontent.com/nateshirley/codespeak-assets/main/speaker.png" style="zoom:17%;" /> Codespeak
 
-Codespeak lets you write python in natural language while maintaining complete interop with your existing stack and preserving real-time, deterministic execution.
-
-
+Write python in natural language. Maintain complete interop with your existing stack and preserve real-time, deterministic execution.
 
 ## Installation
 
 `pip install codespeak` or `poetry add codespeak`
 
 See [getting started](#getting-started) for API key config.
 
 ## Usage
 
-Declare a function with the `@codespeak()` decorator and describe its goal with a docstring. Then, call the function:
+Declare a function with the `@codespeak` decorator and describe its goal with a docstring. Then, call the function:
 
 ```python
 from codespeak import codespeak
 
-@codespeak()
+@codespeak
 def add_two(x: int, y: int) -> int:
   """add two numbers together"""
-  
- 
-result = add_two(1, 3) 
-print(result) # output: 4  
+
+
+result = add_two(1, 3)
+print(result) # output: 4
 ```
 
 Codespeak uses function declarations to understand program intent and write corresponding implementations. When Codespeak functions are called, their generated implementations are executed.
 
 ### Use type hints to create reliable, highly-capable functions
 
 Proper type hints allow Codespeak to write more complex code inside your existing projects. Let's look at another example:
 
 ```python
 from sqlalchemy.orm.session import Session
 from datetime import datetime
 from my_models import User, Order
 
-@codespeak()
+@codespeak
 def orders_for_user_since_date(session: Session, user: User, since_date: datetime) -> List[Order]:
   """return all of the orders for the user placed after the given date"""
 ```
 
-When compared to the first example, this function requires more advanced logic, but its type hints contain much richer information about the data that the function will operate on. 
+When compared to the first example, this function requires more advanced logic, but its type hints contain much richer information about the data that the function will operate on.
 
 To generate code for the above function, Codespeak will navigate through the function's types and use them to understand how to accomplish its goal. Here, the types should contain plenty of information to implement the function.
 
 If using this function, simply declare it as shown above, and then call it.
 
 ### Maintain real-time, deterministic execution
 
-When Codespeak detects a new and/or different function, it writes new code for it. Otherwise, functions are executed deterministically and in real-time.
+The first time a Codespeak function is executed, the appropriate implementation is generated. From then on, the function is executed deterministically and in real-time.
 
 Here's fizzbuzz in Codespeak:
 
 ```python
-@codespeak()
+@codespeak
 def fizzbuzz(limit: int) -> None:
   """
   Iterate from 1 to the limit.
   If the number is divisible by 3, print "Fizz".
   If the number is divisible by 5, print "Buzz".
   If the number is divisible by both 3 and 5, print "FizzBuzz".
   Otherwise, print the number.
   """
 ```
 
-The first time fizzbuzz() is called in your project, Codespeak will generate its implementation and execute it. When the function is called anytime thereafter, the current version is compared with the previous using a checksum. 
+The first time fizzbuzz() is called, Codespeak will generate its implementation and execute it. When the function is called anytime thereafter, the current version is compared with the previous using a checksum.
 
 When changes are detected, new code is generated and executed. Otherwise, the previous implementation is executed in real-time.
 
 In production environments, Codespeak assumes all functions are unchanged and executes them with near-zero overhead.
 
 To configure production settings, use an environment variable `ENVIRONMENT=PROD` or call `codespeak.set_environment("prod")`
 
 ### Use tests to guarantee execution properties
 
 Alongside type hints, tests allow Codespeak to guarantee specific properties in your functions.
 
 When writing code for a function with tests, Codespeak will rewrite and execute its code until the tests pass.
 
-To apply a test to a function, simply pass it into the `@codespeak()` decorator as an argument:
+To attach a test to a function, simply assign it with the function's built-in "assign_pytest_function" method:
 
 ```python
-def test_add_two():
-  assert add_two(1, 3) == 4
- 
-@codespeak(test_add_two)
+@codespeak
 def add_two(x: int, y: int) -> int:
   """add two numbers together"""
+
+def test_add_two():
+  assert add_two(1, 3) == 4
+
+add_two.assign_pytest_function(test_add_two)
+
 ```
 
-Currently, Codespeak tests are run exclusively as pytest functions.
+Currently, Codespeak receives tests exclusively in the form of pytest functions.
 
 ### Access and manipulate generated logic in your file system
 
-When Codespeak implements your functions, they are written to the file system in a `codespeak_generated/` directory under the same hiearchy as they are defined.
+When Codespeak implements your functions, they're written to the file system in a `codespeak_generated/` directory under the same hiearchy as they are defined.
 
 Each function is implemented in its own file, named after the function. To view or edit logic for a function, simply visit the file at [function_name].
 
+## Why would I use this?
+
+#### The right syntax is whatever makes sense to you.
 
+Stop crawling your memory for syntax and data structures. Whatever makes sense to you, just works, so you can stay focused on your program's goals.
 
-## Why would I use this?
+#### Choose the best-fit abstraction for your work.
+
+Maintain the flexibility to delegate as much—or as little—programming as you'd like to an LLM, and adjust your choice on a case-by-case basis. Let a model control an entire endpoint, or a single SQL query.
 
-- English is easy to write
-- Explicitly pairing prompt-context to programming logic ensures that any information used to create a block of code is easily accessible and editable in the future
-- Programmers have full control over the quantity of work they are abstracting to a language-model
-- Automated file management
+#### Always know what you wrote and what you didn't.
 
+Stop digging through blocks of code that Copilot wrote last month and sending them to ChatGPT. Let your code clarify your responsibilities.
 
+#### Modify AI-generated code with simple comment revisions.
+
+With Codespeak, everything that's required to generate new code for your existing programs is declared in your codebase. This means your codegen can be immediately re-produced or updated on any machine, simply by adjusting your code comments.
+
+#### Accomplish more with your programs in fewer declared-lines.
+
+Compress your exposure to program logic. Fewer lines means fewer files and fewer functions to manage, so you can stop wasting your time re-organzing and re-naming. Stay focused on your program's goals.
 
 ## Getting started
 
-Codespeak needs to be configured with an OpenAI API key (access your keys [here](https://platform.openai.com/account/api-keys)). 
+Codespeak needs to be configured with an OpenAI API key (access your keys [here](https://platform.openai.com/account/api-keys)).
 
 The library will automatically use an environment variable `OPENAI_API_KEY` if one exists:
 
 ```python
 export OPENAI_API_KEY='sk-...'
 ```
 
 Otherwise, set it explicitly with `codespeak.set_openai_api_key()`:
 
 ```python
 import codespeak
 
 codespeak.set_openai_api_key("sk-...")
 ```
-
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codespeak-0.1.1/codespeak/.DS_Store` & `codespeak-0.1.2/codespeak/.DS_Store`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/codespeak/config.py` & `codespeak-0.1.2/codespeak/public/codespeak_settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-from enum import Enum
-import os
 from pydantic import BaseModel
+from codespeak._settings.environment import Environment
+from codespeak._settings._settings import _settings
 
 
-class Environment(Enum):
-    PROD = "prod"
-    DEV = "dev"
-
-
-class Config(BaseModel):
-    openai_api_key: str | None = None
-    environment: Environment
-    verbose: bool = False
-
-    @staticmethod
-    def from_env():
-        env = os.getenv("ENVIRONMENT")
-        if env:
-            env = env.lower()
-            if env in [e.value for e in Environment]:
-                return Config(
-                    openai_api_key=os.getenv("OPENAI_API_KEY"),
-                    environment=Environment(env),
-                )
-        return Config(
-            openai_api_key=os.getenv("OPENAI_API_KEY"), environment=Environment.DEV
-        )
-
-
-_config = Config.from_env()
+def set_openai_api_key(key: str):
+    _settings.openai_api_key = key
 
 
-def set_openai_api_key(key: str):
-    _config.openai_api_key = key
+def set_verbose(verbose: bool):
+    _settings.verbose = verbose
 
 
-def get_openai_api_key() -> str | None:
-    return _config.openai_api_key
+def set_auto_clean(auto_clean: bool):
+    _settings.auto_clean = auto_clean
 
 
-def set_verbose(verbose: bool):
-    _config.verbose = verbose
+def set_openai_model(model: str):
+    _settings.openai_model = model
 
 
-def get_verbose() -> bool:
-    return _config.verbose
+def manually_set_abspath_to_project_root(abspath: str):
+    _settings.abspath_to_project_root = abspath
 
 
 def set_environment(env: Environment | str):
     if isinstance(env, Environment):
-        _config.environment = env
+        _settings.environment = env
     else:
         if env not in [e.value for e in Environment]:
             raise Exception("Environment doesn't exist, use 'prod' or 'dev'")
-        _config.environment = Environment(env)
+        _settings.environment = Environment(env)
 
 
-def get_environment() -> Environment:
-    return _config.environment
+class Settings(BaseModel):
+    """
+    Public settings obj for codespeak.
+
+    - openai_api_key: your openai api key, NOT required in prod
+    - environment: 'prod' or 'dev'
+    - verbose: whether to print out debug statements
+    - auto_clean: whether to auto clean the codegen dir after each run
+    - openai_model: the openai model to use
+    """
+
+    openai_api_key: str | None
+    environment: Environment | str | None
+    verbose: bool | None
+    auto_clean: bool | None
+    openai_model: str | None
+
+
+def set(settings: Settings):
+    if settings.openai_api_key is not None:
+        set_openai_api_key(settings.openai_api_key)
+    if settings.environment is not None:
+        set_environment(settings.environment)
+    if settings.verbose is not None:
+        set_verbose(settings.verbose)
+    if settings.auto_clean is not None:
+        set_auto_clean(settings.auto_clean)
+    if settings.openai_model is not None:
+        set_openai_model(settings.openai_model)
```

### Comparing `codespeak-0.1.1/codespeak/core/code_generator.py` & `codespeak-0.1.2/codespeak/_core/code_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # need to give it import paths
 
 import inspect
 from typing import Any, Callable, Dict, List
 from pydantic import BaseModel
 import pytest
-from codespeak.core.codespeak_service import CodespeakService
-from codespeak.generated_exception import GeneratedException
-from codespeak.core.executor import execute_unsafe
-from codespeak.core.results_collector import TestRunner
-from codespeak.declaration.codespeak_declaration import CodespeakDeclaration
+from codespeak._core.codespeak_service import CodespeakService
+from codespeak.public.generated_exception import GeneratedException
+from codespeak._core.executor import execute_unsafe
+from codespeak._core.results_collector import TestRunner
+from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
 
 
 class ExecutionResponse(BaseModel):
     result: Any
     did_regenerate_source: bool = False
```

### Comparing `codespeak-0.1.1/codespeak/core/codespeak_service.py` & `codespeak-0.1.2/codespeak/_core/codespeak_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from pydantic import BaseModel
-from codespeak.core import prompt
-from codespeak.core.openai_service import OpenAIService, Roles
-from codespeak.core.results_collector import CrashReport
-from codespeak.config import get_verbose
-from codespeak.declaration.codespeak_declaration import CodespeakDeclaration
+from codespeak._core import prompt
+from codespeak._core.openai_service import OpenAIService, Roles
+from codespeak._core.results_collector import CrashReport
+from codespeak._settings._settings import get_verbose
+from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
 
 
 class IterationState(BaseModel):
     num_code_versions: int = 0
     max_code_versions: int = 3
     num_test_versions: int = 0
     max_test_versions: int = 3
```

### Comparing `codespeak-0.1.1/codespeak/core/diff.py` & `codespeak-0.1.2/codespeak/_core/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Callable
-from codespeak.declaration.declaration_file_service import DeclarationFileService
-from codespeak.metadata import FunctionMetadata
-from codespeak.metadata.digest import DeclarationDigest
+from codespeak._declaration.declaration_file_service import DeclarationFileService
+from codespeak._metadata import FunctionMetadata
+from codespeak._metadata.digest import DeclarationDigest
 
 
 def require_new_codegen(
     file_service: DeclarationFileService,
     active_digest: DeclarationDigest,
     require_deep_hash_match: bool = False,
 ) -> bool:
```

### Comparing `codespeak-0.1.1/codespeak/core/executor.py` & `codespeak-0.1.2/codespeak/_core/executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from importlib import import_module
 from typing import Any, Callable
-from codespeak.generated_exception import GeneratedException
+from codespeak.public.generated_exception import GeneratedException
 
 
 def load_generated_logic_from_module_qualname(
-    modulepath: str, func_name: str
+    module_qualname: str, func_name: str
 ) -> Callable:
     try:
-        module = import_module(modulepath)
+        module = import_module(module_qualname)
     except Exception as e:
-        raise Exception(f"Could not import module path at {modulepath}. e: {e}")
+        raise Exception(f"Could not import module path at {module_qualname}. e: {e}")
     try:
         return getattr(module, func_name)
     except AttributeError:
-        raise Exception(f"Could not find function {func_name} on module {modulepath}")
+        raise Exception(
+            f"Could not find function {func_name} on module {module_qualname}"
+        )
 
 
 def execute_unsafe(codegen_module_qualname: str, func_name: str, *args, **kwargs):
     logic = load_generated_logic_from_module_qualname(
         codegen_module_qualname, func_name=func_name
     )
     return logic(*args, **kwargs)
```

### Comparing `codespeak-0.1.1/codespeak/core/openai_service.py` & `codespeak-0.1.2/codespeak/_core/openai_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import openai
-from typing import Any, Callable, Dict, List, Literal
+from typing import Any, List
 
 from pydantic import BaseModel, validator
-from codespeak.config import get_openai_api_key
+from codespeak._settings import _settings
 
 
 class Roles:
     @staticmethod
     def user():
         return "user"
 
@@ -36,15 +36,15 @@
     model: str
     messages: List[Message]
     num_retries: int = 0
 
     @staticmethod
     def with_defaults():
         return OpenAIService(
-            model="gpt-4",
+            model=_settings.get_openai_model(),
             messages=[
                 Message(
                     role=Roles.system(),
                     content="You are a competent and diligent python programmer.",
                 ),
             ],
             num_retries=0,
@@ -59,20 +59,20 @@
         self.add_message(content=completion, role=Roles.assistant())
         return completion
 
     def add_message(self, content: str, role: str):
         self.messages.append(Message(role=role, content=content))
 
     def get_completion(self) -> str:
-        openai_key = get_openai_api_key()
+        openai_key = _settings.get_openai_api_key()
         if openai_key is None or openai_key == "":
             raise Exception(
                 "OpenAI API key not configured, use codespeak.set_openai_key() to set it, or load an env variable OPENAI_API_KEY",
             )
-        openai.api_key = get_openai_api_key()
+        openai.api_key = _settings.get_openai_api_key()
         try:
             response: Any = openai.ChatCompletion.create(
                 model=self.model,
                 messages=self.json_messages(),
                 stream=True,
             )
             result = ""
```

### Comparing `codespeak-0.1.1/codespeak/core/prompt.py` & `codespeak-0.1.2/codespeak/_core/prompt.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/codespeak/core/results_collector.py` & `codespeak-0.1.2/codespeak/_core/results_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # run.py
 import importlib
 import inspect
 import time
 from typing import Callable, List
 from pydantic import BaseModel
-from codespeak.helpers.set_attr_for_qualname import set_attr_for_qualname
+from codespeak._helpers.set_attr_for_qualname import set_attr_for_qualname
 import pytest
 
 
 class ResultsCollector:
     def __init__(self):
         self.reports = []
         self.collected = 0
```

### Comparing `codespeak-0.1.1/codespeak/declaration/body_imports.py` & `codespeak-0.1.2/codespeak/_declaration/body_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import inspect
 from pydantic import BaseModel
 from typing import Dict, List, Optional, Any
-from codespeak.definitions.definition import Definition
-from codespeak.definitions import classify
+from codespeak._definitions.definition import Definition
+from codespeak._definitions import classify
 
 import importlib
 import astor
 
 
 class BodyImports(BaseModel):
     defs: List[Definition]
```

### Comparing `codespeak-0.1.1/codespeak/declaration/codespeak_declaration.py` & `codespeak-0.1.2/codespeak/_declaration/codespeak_declaration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import ast
 import inspect
 import json
 import textwrap
 from typing import Any, Callable, Dict, List, Optional
 from pydantic import BaseModel, validator
-from codespeak.declaration.declaration_file_service import DeclarationFileService
-from codespeak.declaration import declaration_helpers
-from codespeak.definitions import classify
-from codespeak.definitions.definition import Definition
+from codespeak._declaration.declaration_file_service import DeclarationFileService
+from codespeak._declaration import declaration_helpers
+from codespeak._definitions import classify
+from codespeak._definitions.definition import Definition
 
-from codespeak.definitions.utils.dedupe import dedupe
-from codespeak.definitions.utils.group import group_by_module
-from codespeak.declaration.body_imports import BodyImports
-from codespeak import generated_exception
-from codespeak.metadata.digest import DeclarationDigest
+from codespeak._definitions.utils.dedupe import dedupe
+from codespeak._definitions.utils.group import group_by_module
+from codespeak._declaration.body_imports import BodyImports
+from codespeak.public import generated_exception
+from codespeak._metadata.digest import DeclarationDigest
 
 
 class CodespeakDeclaration(BaseModel):
     name: str
     qualname: str
     module_name: str
     docstring: str
```

### Comparing `codespeak-0.1.1/codespeak/declaration/declaration_file_service.py` & `codespeak-0.1.2/codespeak/_declaration/declaration_file_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import inspect
 import json
 import os
 from types import ModuleType
 from typing import Any, Callable
 from pydantic import BaseModel
 
-from codespeak.metadata import FunctionMetadata
-from codespeak.metadata.digest import DeclarationDigest
+from codespeak._settings import _settings
+from codespeak._metadata import FunctionMetadata
+from codespeak._metadata.digest import DeclarationDigest
 
-generated_directory_stem = "codespeak_generated"
+codegen_dirname = "codespeak_generated"
+metadata_file_prefix = "_metadata_"
 
 
 class DeclarationFileService(BaseModel):
     declaration_filesystem_name: str
     generated_module_qualname: str
     codegen_absolute_dirpath: str
     generated_entrypoint: str
@@ -56,34 +58,45 @@
 
     @property
     def codegen_metadata_dirpath(self) -> str:
         return f"{self.codegen_absolute_dirpath}/metadata"
 
     @property
     def codegen_metadata_filepath(self) -> str:
-        return f"{self.codegen_metadata_dirpath}/metadata___{self.declaration_filesystem_name}.json"
+        return f"{self.codegen_metadata_dirpath}/{metadata_file_prefix}{self.declaration_filesystem_name}.json"
+
+    @staticmethod
+    def gather_generated_module_qualname(decorated_func: Callable) -> str:
+        module = inspect.getmodule(decorated_func)
+        if not module:
+            raise Exception("module not found for func: ", decorated_func.__name__)
+        declared_module_qualname = get_declared_module_qualname(decorated_func)
+        return build_generated_module_qualname(
+            declared_module_qualname=declared_module_qualname,
+            func_qualname=decorated_func.__qualname__,
+        )
 
     @staticmethod
     def from_callable(func: Callable) -> "DeclarationFileService":
         module = inspect.getmodule(func)
         if not module:
             raise Exception("module not found for func: ", func.__name__)
-        abspath_to_proj = abspath_to_project_root(func)
+        abspath_to_proj = _settings.get_abspath_to_project_root(func)
         declared_module_qualname = get_declared_module_qualname(func)
         declared_module_as_filepath = declared_module_qualname.replace(".", "/")
         return DeclarationFileService(
             declaration_filesystem_name=func_qualname_to_filesystem_name(
                 func.__qualname__
             ),
             generated_entrypoint=func.__name__,
             generated_module_qualname=build_generated_module_qualname(
                 declared_module_qualname=declared_module_qualname,
                 func_qualname=func.__qualname__,
             ),
-            codegen_absolute_dirpath=f"{abspath_to_proj}/{generated_directory_stem}/{declared_module_as_filepath}",
+            codegen_absolute_dirpath=f"{abspath_to_proj}/{codegen_dirname}/{declared_module_as_filepath}",
         )
 
     def does_metadata_exist(self) -> bool:
         return os.path.exists(self.codegen_logic_filepath) and os.path.exists(
             self.codegen_metadata_filepath
         )
 
@@ -95,33 +108,36 @@
         return FunctionMetadata.parse_obj(data)
 
     def load_logic(self) -> str:
         with open(self.codegen_logic_filepath, "r") as file:
             return file.read()
 
 
+# this func assumes generated directory is in project root
+# could also add flexibity here to configure this in a toml, later
 def build_generated_module_qualname(declared_module_qualname: str, func_qualname: str):
-    return f"{generated_directory_stem}.{declared_module_qualname}.{func_qualname_to_filesystem_name(func_qualname)}"
+    return f"{codegen_dirname}.{declared_module_qualname}.{func_qualname_to_filesystem_name(func_qualname)}"
 
 
 def func_qualname_to_filesystem_name(qualname: str) -> str:
     return qualname.replace(".", "___")
 
 
 def derive_generated_module_qualname_from_func(func: Callable) -> str:
     declared_mod_qualname = get_declared_module_qualname(func)
     return build_generated_module_qualname(declared_mod_qualname, func.__qualname__)
 
 
+# want to leave this as an attribute on the wrapper, just want to get rid of abspath to root
 def get_declared_module_qualname(func: Callable):
     source_file = inspect.getsourcefile(func)
     if not source_file:
         raise Exception("unable to get source file for func: ", func.__name__)
     return derive_declared_module_qualname_from_filepaths(
-        source_file, abspath_to_project_root(func)
+        source_file, _settings.get_abspath_to_project_root(func)
     )
 
 
 def derive_declared_module_qualname_from_filepaths(
     declaration_filepath: str, project_root: str
 ):
     # Make sure both paths are absolute and normalized
@@ -142,28 +158,7 @@
     module_qualname = module_qualname.replace(os.sep, ".")
 
     # If the function is in '__init__', use the parent directory as the module
     if module_qualname.endswith(".__init__"):
         module_qualname = module_qualname[: -len(".__init__")]
 
     return module_qualname
-
-
-def abspath_to_project_root(func: Callable):
-    import os
-
-    func_path = inspect.getabsfile(func)
-    current_directory = func_path
-    installed_root = None
-
-    while current_directory != "/":
-        if os.path.exists(os.path.join(current_directory, "pyproject.toml")):
-            installed_root = current_directory
-            break
-
-        current_directory = os.path.dirname(current_directory)
-
-    if installed_root is None:
-        raise Exception(
-            "Unable to find root directory of project where codespeak is installed. make sure you have a pyproject.toml file in your project root."
-        )
-    return installed_root
```

### Comparing `codespeak-0.1.1/codespeak/declaration/declaration_helpers.py` & `codespeak-0.1.2/codespeak/_declaration/declaration_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 import re
 from typing import Any, Callable, List
-from codespeak.definitions import classify
-from codespeak.definitions.definition import Definition
+from codespeak._definitions import classify
+from codespeak._definitions.definition import Definition
 import inspect
 
 
 def insert_after_self(text, insert_text):
     def replace(match):
         return match.group() + ":" + insert_text
```

### Comparing `codespeak-0.1.1/codespeak/decorate.py` & `codespeak-0.1.2/codespeak/_decorate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,86 @@
-import inspect
-import os
-from typing import Callable, List, Any
-from codespeak.core.codespeak_service import CodespeakService
-from codespeak.declaration.codespeak_declaration import CodespeakDeclaration
+from typing import Any, Callable
+
+from pydantic import BaseModel
+from codespeak._core.codespeak_service import CodespeakService
+from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
 from functools import wraps
-from codespeak.core import diff, executor
-from codespeak.core.code_generator import CodeGenerator
-from codespeak.declaration.declaration_file_service import (
+from codespeak._core import diff, executor
+from codespeak._core.code_generator import CodeGenerator
+from codespeak._declaration.declaration_file_service import (
     DeclarationFileService,
 )
-from codespeak.helpers.self_type import self_type_if_exists
-from codespeak.core.code_generator import TestFunc
-from codespeak.config import get_environment, Environment
-
-
-def codespeak(pytest_func: Callable | None = None):
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            if not hasattr(wrapper, "file_service"):
-                raise Exception("file service not found")
-            if get_environment() == Environment.DEV:
-                self_type = self_type_if_exists(func, list(args), kwargs)
-                declaration = CodespeakDeclaration.from_callable(
-                    func, self_type, wrapper.file_service
-                )
-                should_generate_new_source_code = diff.require_new_codegen(
-                    wrapper.file_service, declaration.digest
-                )
-                test_func = TestFunc.from_callable(pytest_func) if pytest_func else None
-                if should_generate_new_source_code:
-                    code_generator = CodeGenerator(
-                        declaration=declaration,
-                        service=CodespeakService.with_defaults(declaration),
-                        should_execute=True,
-                        test_func=test_func,
-                        args=list(args),
-                        kwargs=kwargs,
-                    )
-                    generation = code_generator.generate()
-                    return generation.execution_result
+from codespeak._helpers.self_type import self_type_if_exists
+from codespeak._core.code_generator import TestFunc
+from codespeak._settings import _settings
+from codespeak._clean import clean
+from codespeak._settings.environment import Environment
+
+
+def codespeak(func):
+    @wraps(func)
+    def dev_execute(*args, **kwargs):
+        if not hasattr(codespeak_function, "file_service"):
+            raise Exception("file service not found")
+        file_service = codespeak_function.file_service
+        self_type = self_type_if_exists(func, list(args), kwargs)
+        declaration = CodespeakDeclaration.from_callable(func, self_type, file_service)
+        should_generate_new_source_code = diff.require_new_codegen(
+            file_service, declaration.digest
+        )
+        pytest_func: TestFunc | None = getattr(codespeak_function, "pytest_func", None)
+        if should_generate_new_source_code:
+            code_generator = CodeGenerator(
+                declaration=declaration,
+                service=CodespeakService.with_defaults(declaration),
+                should_execute=True,
+                test_func=pytest_func,
+                args=list(args),
+                kwargs=kwargs,
+            )
+            generation = code_generator.generate()
+            if _settings.should_auto_clean():
+                clean(_settings.abspath_to_codegen_dir())
+            return generation.execution_result
+        else:
             return executor.execute_with_attributes(
-                wrapper.file_service.generated_module_qualname,
-                func.__name__,
+                file_service.generated_module_qualname,
+                file_service.generated_entrypoint,
                 *args,
-                **kwargs
+                **kwargs,
             )
 
-        setattr(
-            wrapper,
-            "file_service",
-            DeclarationFileService.from_callable(func),
-        )
-        return wrapper
+    class _CodespeakFunction:
+        file_service: DeclarationFileService
+        pytest_func: TestFunc
+        is_prod: bool
+        logic: Callable
 
-    return decorator
+        def __call__(self, *args, **kwargs):
+            if self.is_prod:
+                return self.logic(*args, **kwargs)
+            else:
+                return dev_execute(*args, **kwargs)
+
+        def assign_pytest_function(self, _pytest_func: Callable):
+            self.pytest_func = TestFunc.from_callable(_pytest_func)
+
+    codespeak_function = _CodespeakFunction()
+    assign_default_attributes(codespeak_function, func)
+    return codespeak_function
+
+
+def assign_default_attributes(codespeak_function: Callable, decorated_func: Callable):
+    env = _settings.get_environment()
+    codespeak_function.is_prod = env == Environment.PROD
+    if env == _settings.Environment.PROD:
+        logic = executor.load_generated_logic_from_module_qualname(
+            DeclarationFileService.gather_generated_module_qualname(
+                decorated_func=decorated_func
+            ),
+            decorated_func.__name__,
+        )
+        codespeak_function.logic = logic
+    elif env == _settings.Environment.DEV:
+        codespeak_function.file_service = DeclarationFileService.from_callable(
+            decorated_func
+        )
```

### Comparing `codespeak-0.1.1/codespeak/definitions/classify.py` & `codespeak-0.1.2/codespeak/_definitions/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import types
 from typing import Any, Callable, Dict, Tuple, get_origin
 import builtins
 from typing import Any, Union, get_args, get_origin, List, get_type_hints
 import inspect
-from codespeak.definitions.free_modules import FREE_MODULES
+from codespeak._definitions.free_modules import FREE_MODULES
 import os
 import types
-from codespeak.definitions.definition import Definition
-from codespeak.definitions.types.generic import Generic
-from codespeak.definitions.types.local_class import LocalClass
-from codespeak.definitions.types.local_class_as_self import LocalClassAsSelf
-from codespeak.definitions.types.installed_class import InstalledClass
-from codespeak.definitions.types.builtin import Builtin
-from codespeak.definitions.types.none import NoneDef
-from codespeak.definitions.types.typing_type import TypingType
-from codespeak.definitions.types.union_type import UnionType
+from codespeak._definitions.definition import Definition
+from codespeak._definitions.types.generic import Generic
+from codespeak._definitions.types.local_class import LocalClass
+from codespeak._definitions.types.local_class_as_self import LocalClassAsSelf
+from codespeak._definitions.types.installed_class import InstalledClass
+from codespeak._definitions.types.builtin import Builtin
+from codespeak._definitions.types.none import NoneDef
+from codespeak._definitions.types.typing_type import TypingType
+from codespeak._definitions.types.union_type import UnionType
 import pkg_resources
 
 
 def to_union_type(definition: Any) -> UnionType:
     args = get_args(definition)
     _types = []
     for _type in args:
```

### Comparing `codespeak-0.1.1/codespeak/definitions/definition.py` & `codespeak-0.1.2/codespeak/_definitions/definition.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/codespeak/definitions/free_modules.py` & `codespeak-0.1.2/codespeak/_definitions/free_modules.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/codespeak/definitions/types/custom_type_reference.py` & `codespeak-0.1.2/codespeak/_definitions/types/custom_type_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Literal
-from codespeak.definitions.definition import Definition
+from codespeak._definitions.definition import Definition
 
 
 class CustomTypeReference(Definition):
     type: Literal["ComplexTypeReference"] = "ComplexTypeReference"
 
     def ref(self):
         return "$ref: complex_types/" + self.module + "." + self.qualname
```

### Comparing `codespeak-0.1.1/codespeak/definitions/types/installed_class.py` & `codespeak-0.1.2/codespeak/_definitions/types/installed_class.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Callable, Dict
 from typing import Literal
-from codespeak.definitions.definition import Definition
+from codespeak._definitions.definition import Definition
 
 
 class InstalledClass(Definition):
     type: Literal["InstalledClass"] = "InstalledClass"
     origin: str = "installed"
 
     def annotate(self) -> Dict:
```

### Comparing `codespeak-0.1.1/codespeak/definitions/types/local_class.py` & `codespeak-0.1.2/codespeak/_definitions/types/local_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, List, Tuple
 
 from typing import Literal
-from codespeak.definitions.definition import Definition
-from codespeak.definitions.types.custom_type_reference import CustomTypeReference
-from codespeak.definitions.utils.dedupe import dedupe
-from codespeak.definitions.utils.flat_uniques import flat_uniques
-from codespeak.definitions.utils.flatten import flatten_definitions
+from codespeak._definitions.definition import Definition
+from codespeak._definitions.types.custom_type_reference import CustomTypeReference
+from codespeak._definitions.utils.dedupe import dedupe
+from codespeak._definitions.utils.flat_uniques import flat_uniques
+from codespeak._definitions.utils.flatten import flatten_definitions
 import ast
 
 
 class LocalClass(Definition):
     type: Literal["LocalClass"] = "LocalClass"
     source_code: str
     bases: List[Definition]
```

### Comparing `codespeak-0.1.1/codespeak/definitions/types/local_class_as_self.py` & `codespeak-0.1.2/codespeak/_definitions/types/local_class_as_self.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ast
 from typing import Dict
-from codespeak.definitions.types.local_class import LocalClass
+from codespeak._definitions.types.local_class import LocalClass
 
 
 class RemoveFunction(ast.NodeTransformer):
     def __init__(self, function_name):
         self.function_name = function_name
 
     def visit_FunctionDef(self, node):
```

### Comparing `codespeak-0.1.1/codespeak/definitions/types/typing_type.py` & `codespeak-0.1.2/codespeak/_definitions/types/typing_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from typing import Any, Dict, List, Tuple
 
 from typing import Literal
-from codespeak.definitions.types.generic import Generic
-from codespeak.definitions.utils.flat_uniques import flat_uniques
-from codespeak.definitions.definition import Definition
-from codespeak.definitions.utils.swap_custom_types import (
+from codespeak._definitions.types.generic import Generic
+from codespeak._definitions.utils.flat_uniques import flat_uniques
+from codespeak._definitions.definition import Definition
+from codespeak._definitions.utils.swap_custom_types import (
     recursively_swap_custom_types_for_references,
 )
 
 
 class TypingType(Definition):
     qualname: str
     module: str
```

### Comparing `codespeak-0.1.1/codespeak/definitions/types/union_type.py` & `codespeak-0.1.2/codespeak/_definitions/types/union_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable, Dict, List
 from typing import Literal
 
-from codespeak.definitions.types.typing_type import TypingType
-from codespeak.definitions.definition import Definition
+from codespeak._definitions.types.typing_type import TypingType
+from codespeak._definitions.definition import Definition
 
 
 class UnionType(TypingType):
     qualname: str = "UnionType"
     module: str = "types"
     args: List[Definition]
     type: Literal["UnionType"] = "UnionType"
```

### Comparing `codespeak-0.1.1/codespeak/definitions/utils/dedupe.py` & `codespeak-0.1.2/codespeak/_definitions/utils/dedupe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from codespeak.definitions.definition import Definition
+from codespeak._definitions.definition import Definition
 
 
 def dedupe(definitions: List[Definition]) -> List[Definition]:
     uniques = []
     paths = {}
     for _def in definitions:
         if hasattr(_def, "module") and hasattr(_def, "qualname"):
```

### Comparing `codespeak-0.1.1/codespeak/definitions/utils/flat_uniques.py` & `codespeak-0.1.2/codespeak/_definitions/utils/flat_uniques.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flat_uniques = dedupe(
 #     flatten_definitions(self.args, include_local_classes=False)
 # )
 from typing import List
-from codespeak.definitions.utils.dedupe import dedupe
-from codespeak.definitions.utils.flatten import flatten_definitions
-from codespeak.definitions.definition import Definition
+from codespeak._definitions.utils.dedupe import dedupe
+from codespeak._definitions.utils.flatten import flatten_definitions
+from codespeak._definitions.definition import Definition
 
 
 def flat_uniques(definitions: List[Definition], locals_only: bool) -> List[Definition]:
     f_u = dedupe(flatten_definitions(definitions))
     if locals_only:
         return [local for local in f_u if local.type == "LocalClass"]
     else:
```

### Comparing `codespeak-0.1.1/codespeak/definitions/utils/swap_custom_types.py` & `codespeak-0.1.2/codespeak/_definitions/utils/swap_custom_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple
 
-from codespeak.definitions.definition import Definition
-from codespeak.definitions.types.custom_type_reference import CustomTypeReference
+from codespeak._definitions.definition import Definition
+from codespeak._definitions.types.custom_type_reference import CustomTypeReference
 
 
 def recursively_swap_custom_types_for_references(
     args: List[Definition],
 ) -> Tuple[List[Definition], List[Definition]]:
     swapped = []
     for i, _def in enumerate(args):
```

### Comparing `codespeak-0.1.1/codespeak/generate.py` & `codespeak-0.1.2/codespeak/public/codespeak_helpers/generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable, Dict, List
-from codespeak.core.code_generator import CodeGenerator, TestFunc
-from codespeak.core.codespeak_service import CodespeakService
-from codespeak.declaration.codespeak_declaration import CodespeakDeclaration
-from codespeak.helpers.self_type import self_type_if_exists
+from codespeak._core.code_generator import CodeGenerator, TestFunc
+from codespeak._core.codespeak_service import CodespeakService
+from codespeak._declaration.codespeak_declaration import CodespeakDeclaration
+from codespeak._helpers.self_type import self_type_if_exists
 
 
 def generate(
     func: Callable,
     args: List[Any] | None = None,
     kwargs: Dict[str, Any] | None = None,
     pytest_func: Callable | None = None,
```

### Comparing `codespeak-0.1.1/codespeak/generated_exception.py` & `codespeak-0.1.2/codespeak/public/generated_exception.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/codespeak/helpers/self_type.py` & `codespeak-0.1.2/codespeak/_helpers/self_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from typing import Any, Callable, Dict, List
-from codespeak.helpers.gather_arguments import gather_arguments
+from codespeak._helpers.gather_arguments import gather_arguments
 
 
 def self_type_if_exists(
     func: Callable, args: List[Any], kwargs: Dict[str, Any]
 ) -> Any | None:
     bounded_args = gather_arguments(func, args, kwargs)
     for index, arg in enumerate(bounded_args):
```

### Comparing `codespeak-0.1.1/codespeak/metadata/digest.py` & `codespeak-0.1.2/codespeak/_metadata/digest.py`

 * *Files identical despite different names*

### Comparing `codespeak-0.1.1/PKG-INFO` & `codespeak-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codespeak
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: nateshirley
 Author-email: nate.00.shirley@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,133 +12,141 @@
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.13,<3.0.0)
 Description-Content-Type: text/markdown
 
-
-
-
-
 # <img src="https://raw.githubusercontent.com/nateshirley/codespeak-assets/main/speaker.png" style="zoom:17%;" /> Codespeak
 
-Codespeak lets you write python in natural language while maintaining complete interop with your existing stack and preserving real-time, deterministic execution.
-
-
+Write python in natural language. Maintain complete interop with your existing stack and preserve real-time, deterministic execution.
 
 ## Installation
 
 `pip install codespeak` or `poetry add codespeak`
 
 See [getting started](#getting-started) for API key config.
 
 ## Usage
 
-Declare a function with the `@codespeak()` decorator and describe its goal with a docstring. Then, call the function:
+Declare a function with the `@codespeak` decorator and describe its goal with a docstring. Then, call the function:
 
 ```python
 from codespeak import codespeak
 
-@codespeak()
+@codespeak
 def add_two(x: int, y: int) -> int:
   """add two numbers together"""
-  
- 
-result = add_two(1, 3) 
-print(result) # output: 4  
+
+
+result = add_two(1, 3)
+print(result) # output: 4
 ```
 
 Codespeak uses function declarations to understand program intent and write corresponding implementations. When Codespeak functions are called, their generated implementations are executed.
 
 ### Use type hints to create reliable, highly-capable functions
 
 Proper type hints allow Codespeak to write more complex code inside your existing projects. Let's look at another example:
 
 ```python
 from sqlalchemy.orm.session import Session
 from datetime import datetime
 from my_models import User, Order
 
-@codespeak()
+@codespeak
 def orders_for_user_since_date(session: Session, user: User, since_date: datetime) -> List[Order]:
   """return all of the orders for the user placed after the given date"""
 ```
 
-When compared to the first example, this function requires more advanced logic, but its type hints contain much richer information about the data that the function will operate on. 
+When compared to the first example, this function requires more advanced logic, but its type hints contain much richer information about the data that the function will operate on.
 
 To generate code for the above function, Codespeak will navigate through the function's types and use them to understand how to accomplish its goal. Here, the types should contain plenty of information to implement the function.
 
 If using this function, simply declare it as shown above, and then call it.
 
 ### Maintain real-time, deterministic execution
 
-When Codespeak detects a new and/or different function, it writes new code for it. Otherwise, functions are executed deterministically and in real-time.
+The first time a Codespeak function is executed, the appropriate implementation is generated. From then on, the function is executed deterministically and in real-time.
 
 Here's fizzbuzz in Codespeak:
 
 ```python
-@codespeak()
+@codespeak
 def fizzbuzz(limit: int) -> None:
   """
   Iterate from 1 to the limit.
   If the number is divisible by 3, print "Fizz".
   If the number is divisible by 5, print "Buzz".
   If the number is divisible by both 3 and 5, print "FizzBuzz".
   Otherwise, print the number.
   """
 ```
 
-The first time fizzbuzz() is called in your project, Codespeak will generate its implementation and execute it. When the function is called anytime thereafter, the current version is compared with the previous using a checksum. 
+The first time fizzbuzz() is called, Codespeak will generate its implementation and execute it. When the function is called anytime thereafter, the current version is compared with the previous using a checksum.
 
 When changes are detected, new code is generated and executed. Otherwise, the previous implementation is executed in real-time.
 
 In production environments, Codespeak assumes all functions are unchanged and executes them with near-zero overhead.
 
 To configure production settings, use an environment variable `ENVIRONMENT=PROD` or call `codespeak.set_environment("prod")`
 
 ### Use tests to guarantee execution properties
 
 Alongside type hints, tests allow Codespeak to guarantee specific properties in your functions.
 
 When writing code for a function with tests, Codespeak will rewrite and execute its code until the tests pass.
 
-To apply a test to a function, simply pass it into the `@codespeak()` decorator as an argument:
+To attach a test to a function, simply assign it with the function's built-in "assign_pytest_function" method:
 
 ```python
-def test_add_two():
-  assert add_two(1, 3) == 4
- 
-@codespeak(test_add_two)
+@codespeak
 def add_two(x: int, y: int) -> int:
   """add two numbers together"""
+
+def test_add_two():
+  assert add_two(1, 3) == 4
+
+add_two.assign_pytest_function(test_add_two)
+
 ```
 
-Currently, Codespeak tests are run exclusively as pytest functions.
+Currently, Codespeak receives tests exclusively in the form of pytest functions.
 
 ### Access and manipulate generated logic in your file system
 
-When Codespeak implements your functions, they are written to the file system in a `codespeak_generated/` directory under the same hiearchy as they are defined.
+When Codespeak implements your functions, they're written to the file system in a `codespeak_generated/` directory under the same hiearchy as they are defined.
 
 Each function is implemented in its own file, named after the function. To view or edit logic for a function, simply visit the file at [function_name].
 
+## Why would I use this?
+
+#### The right syntax is whatever makes sense to you.
 
+Stop crawling your memory for syntax and data structures. Whatever makes sense to you, just works, so you can stay focused on your program's goals.
 
-## Why would I use this?
+#### Choose the best-fit abstraction for your work.
+
+Maintain the flexibility to delegate as much—or as little—programming as you'd like to an LLM, and adjust your choice on a case-by-case basis. Let a model control an entire endpoint, or a single SQL query.
 
-- English is easy to write
-- Explicitly pairing prompt-context to programming logic ensures that any information used to create a block of code is easily accessible and editable in the future
-- Programmers have full control over the quantity of work they are abstracting to a language-model
-- Automated file management
+#### Always know what you wrote and what you didn't.
 
+Stop digging through blocks of code that Copilot wrote last month and sending them to ChatGPT. Let your code clarify your responsibilities.
 
+#### Modify AI-generated code with simple comment revisions.
+
+With Codespeak, everything that's required to generate new code for your existing programs is declared in your codebase. This means your codegen can be immediately re-produced or updated on any machine, simply by adjusting your code comments.
+
+#### Accomplish more with your programs in fewer declared-lines.
+
+Compress your exposure to program logic. Fewer lines means fewer files and fewer functions to manage, so you can stop wasting your time re-organzing and re-naming. Stay focused on your program's goals.
 
 ## Getting started
 
-Codespeak needs to be configured with an OpenAI API key (access your keys [here](https://platform.openai.com/account/api-keys)). 
+Codespeak needs to be configured with an OpenAI API key (access your keys [here](https://platform.openai.com/account/api-keys)).
 
 The library will automatically use an environment variable `OPENAI_API_KEY` if one exists:
 
 ```python
 export OPENAI_API_KEY='sk-...'
 ```
 
@@ -146,10 +154,7 @@
 
 ```python
 import codespeak
 
 codespeak.set_openai_api_key("sk-...")
 ```
 
-
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

