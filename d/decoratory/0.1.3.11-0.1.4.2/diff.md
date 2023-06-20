# Comparing `tmp/decoratory-0.1.3.11.tar.gz` & `tmp/decoratory-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.3.11.tar", last modified: Mon Jun 19 16:30:58 2023, max compression
+gzip compressed data, was "decoratory-0.1.4.2.tar", last modified: Tue Jun 20 14:38:19 2023, max compression
```

## Comparing `decoratory-0.1.3.11.tar` & `decoratory-0.1.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.3.11/License.txt
--rw-rw-rw-   0        0        0    42585 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/PKG-INFO
--rw-rw-rw-   0        0        0    40959 2023-06-19 15:52:43.000000 decoratory-0.1.3.11/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.3.11/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.755034 decoratory-0.1.3.11/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.786288 decoratory-0.1.3.11/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.3.11/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     5467 2023-06-19 16:30:22.000000 decoratory-0.1.3.11/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    11946 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    37282 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7319 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0     9932 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.801921 decoratory-0.1.3.11/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    42585 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/Unittest/
--rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    21837 2023-06-19 16:04:04.000000 decoratory-0.1.3.11/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10504 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0     9098 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/setup.cfg
--rw-rw-rw-   0        0        0     4447 2023-06-19 16:30:22.000000 decoratory-0.1.3.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:38:19.837447 decoratory-0.1.4.2/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.4.2/License.txt
+-rw-rw-rw-   0        0        0    44214 2023-06-20 14:38:19.837447 decoratory-0.1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0    42589 2023-06-20 14:36:28.000000 decoratory-0.1.4.2/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.4.2/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:38:19.768456 decoratory-0.1.4.2/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:38:19.799704 decoratory-0.1.4.2/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.4.2/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     5466 2023-06-20 14:37:47.000000 decoratory-0.1.4.2/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.4.2/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.4.2/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12308 2023-06-20 14:08:32.000000 decoratory-0.1.4.2/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    37282 2023-06-19 16:25:39.000000 decoratory-0.1.4.2/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7939 2023-06-20 14:08:32.000000 decoratory-0.1.4.2/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0     9932 2023-06-19 15:55:21.000000 decoratory-0.1.4.2/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:38:19.815316 decoratory-0.1.4.2/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    44214 2023-06-20 14:38:19.000000 decoratory-0.1.4.2/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-06-20 14:38:19.000000 decoratory-0.1.4.2/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:38:19.000000 decoratory-0.1.4.2/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-20 14:38:19.000000 decoratory-0.1.4.2/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:38:19.830941 decoratory-0.1.4.2/Unittest/
+-rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.4.2/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23859 2023-06-20 14:08:32.000000 decoratory-0.1.4.2/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.4.2/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10729 2023-06-20 08:56:59.000000 decoratory-0.1.4.2/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0     9098 2023-06-19 16:25:39.000000 decoratory-0.1.4.2/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:38:19.837447 decoratory-0.1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     4446 2023-06-20 14:37:47.000000 decoratory-0.1.4.2/setup.py
```

### Comparing `decoratory-0.1.3.11/License.txt` & `decoratory-0.1.4.2/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/PKG-INFO` & `decoratory-0.1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.3.11
+Version: 0.1.4.2
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -69,44 +69,44 @@
 
     python -m decoratory --test
 
 .. _toc:
 
 **Package Contents**
 
-The *decoratory package* available here includes some classic decorators
+The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
-To illustrate the functionality of each module, a simple as well as a
-more complex example is presented. Even if only one particular module
+To illustrate the functionality of each module, simple as well as 
+more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
 more examples of the full range of possibilities, please refer to the
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
-across modules.
+across module boundaries.
 
-As a simple example serves the decoration of the class  ``Animal`` as
+As a simple example serves the decoration of the class  ``Animal`` as a 
 singleton. In the context of the `Decorator Arguments Pattern`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
@@ -118,16 +118,16 @@
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Teddy')        # Creates Teddy
-    b = Animal(name='Roxie')        # Returns Teddy
+    a = Animal(name='Teddy')        # Creates Teddy, the primary instance
+    b = Animal(name='Roxie')        # Returns Teddy, no Roxi is created
 
 If instances of the class ``Animal`` are now created, this is only done for the
 very first instantiation, and for all further instantiations always this
 *primary instance* is given back.
 
 .. code-block:: python
 
@@ -139,16 +139,16 @@
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
-code is used, additional parameters can be passed to the decorator for
-passing to the class constructor.
+code is used, additional parameters can be passed to the decorator for 
+passing to or through the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -160,30 +160,29 @@
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
-So far, this singleton implementation follows the concept of *once and
+So far, this singleton implementation follows the concept of *once 
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
-Although this behavior is consistent with the basic concept of a singleton,
-there are situations where it might be useful to reset a *singleton*. Such
-a *resettable singleton* could be useful to express in code that an instance
-is often retrieved but rarely changed.
+Although this behavior is consistent with the fundamental concept of a 
+singleton, there are situations where it might be useful to reset a 
+*singleton*. Such a *resettable singleton*, also called *semi-singleton*, 
+could be useful to express in code that an instance is often retrieved but 
+rarely changed.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as 'resettable singleton'
 
-    from decoratory.singleton import Singleton
-
     @Singleton(resettable=True)     # Exposes an additional reset method
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
@@ -191,54 +190,54 @@
     # Case 3: Decoration using @Singleton(resettable=True)
     print(Animal(name='Teddy'))     # Animal('Teddy')
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
-Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and
-the call ``Animal.reset()`` will fail raising an ``AttributeError``.
-
-With the same intention, the retrieval of the *primary instance* is also
-locked by default, but can be unlocked during decoration with the
-``accessible=True`` parameter, which allows ``Animal`` to expose the
-``get_instance()`` method.
+Without this striking ``resettable=True`` decoration ``Animal`` has no 
+``reset`` method and the call ``Animal.reset()`` will fail raising an 
+``AttributeError``. For situations where this concept really needs 
+to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
-    # *** example_singleton.py - decoration as 'accessible singleton'
+    # *** example_singleton.py - decoration as a 'semi singleton'
 
-    from decoratory.singleton import Singleton
+    from decoratory.singleton import SemiSingleton
 
-    @Singleton(accessible=True)     # Exposes a get_instance method
+    @SemiSingleton                  # or @SemiSingleton()
     class Animal:
-        def __init__(self, name):
-            self.name = name
+        pass                        # Some code ...
 
-        def __repr__(self):
-            return f"{self.__class__.__name__}('{self.name}')"
+Last but not least, both ``Singleton`` and ``SemiSingleton`` of course also 
+provide a ``get_instance()`` method to directly retrieve the primary instance,
+e.g. using ``Animal.get_instance()``. 
 
-    # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Teddy')        # Animal('Teddy')
-    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
-    print(a)                        # Animal('Teddy')
-    print(b)                        # Animal('Teddy')
+    **Hint** --- Using ``reset()`` and ``get_instance()`` in combination
+    
+    *It should be noted that the combination of* ``reset()`` *and immediately 
+    following* ``get_instance()`` *does not return a valid object, but*
+    ``None``. *So a* ``reset()`` *should always be followed by an 
+    instantiation to ensure that a valid singleton instance exists.*
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
 Whereas the singleton allows for exactly one instance per class, the multiton
-ensures one single (unique) *instance per key value of a dictionary*.
+ensures one single (unique) *instance per key*.
 
-In this implementation the key parameter can be either any immutable type
-or a callable returning such an immutable type which can be used as a key
-of a dictionary. In case of an invalid key, key is set ``None`` and with only
+In this implementation, the key parameter can be anything that is possible as 
+a key for a Python ``dict()`` dictionary, such as an immutable type or a 
+callable eventually returning such an immutable type etc. 
+
+In case of an invalid key, key is set ``None`` and with only
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
@@ -301,76 +300,88 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
     # Case 3: One unique instance per specie
     @Multiton(key="{0}".format)     # spec is args[0]
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 4: One unique instance per name
     @Multiton(key="{name}".format)  # name is kwargs['name']
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 5: One unique instance for all init values, i.e. no duplicates
     @Multiton(key=lambda spec, name: (spec, name))
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
-        ...
+        pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
 any new key raises a ``KeyError``.
 
-For deeper, special requirements on the equivalence classes of a multiton
-by setting the decorator parameter ``accessible=True``, the method
-``get_instances()`` is enabled, which grants direct access to the internal
-directory of the instances. This can be actively manipulated in this way,
-which of course should be done with care and is generally not recommended.
-
-.. code-block:: python
-
-    # *** example_multitonton.py - Accessibility to the internal directory
-
-    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
-    #                                   accessible=True)
-    print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') 
-    c = Animal('dog', name='Roxie') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
-                                    #  True:  Animal('cat', 'Molly')}
-
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. hint::
+Last but not least, ``Multiton`` provides a ``instances`` property and 
+associated getter and setter methods to directly retrieve the internal 
+dictionary of primary instances. It is obvious that manipulations on it can 
+corrupt the multiton itself, so it is a method for experts, but sometimes 
+they want or need to have exactly this freedom.
 
-    Classifications into the multiton directory are done only once on
+    **Hint** --- Changes affecting key values of classified objects
+
+    *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
-    corrupted by such modifications.
+    corrupted by such modifications.*
+
+    *Therefore,* **never change key related values of classified objects!**
 
-    Therefore, **never change key related values of classified objects**!
+This results in the following exemplary picture:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - seal, unseal, reset, get_instance
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: name,
+    #                                   resettable=True)
+    Animal.reset()                  # Because of resettable=True
+    print(Animal.get_instances())   # {}
+    print(Animal.issealed())        # False     (=default)
+    Animal('dog', name='Teddy')     # Animal('dog', 'Teddy')
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.seal()                   # Seal the multiton!
+    print(Animal.issealed())        # True
+    try:                            # Try to..
+        Animal('cat', name='Molly') # .. add a new animal
+    except  KeyError as ex:         # .. will fail
+        print(f"Sorry {ex.args[1]}, {ex.args[0]}")
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.unseal()                 # Unseal the multiton!
+    print(Animal.issealed())        # False
+    Animal('cat', name='Molly')     # Now, Molly is added
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'), 
+                                    #  'Molly': Animal('cat', 'Molly')}
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -503,21 +514,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. hint::
+    **Hint** --- Dynamic versus static decoration
 
-    Decorations to ``@staticmethod`` or ``@classmethod`` can be done
+    *Decorations to* ``@staticmethod`` *or* ``@classmethod`` *can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
     an object instance is created and must be decorated dynamically as an 
-    instance (e.g. see  `Instance Decoration`_ below).
+    instance (e.g. see*  `Instance Decoration`_ *below).*
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -819,19 +830,19 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-.. warning::
+    **Hint** --- Take care when decorating a class constructor
 
-    Calling **__init__()** results in a new instance! This means calling 
+    *Calling* ``__init__`` *results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior...
+    in not any case this is the desired behavior ...*
 
 So the decoration should not address a class but one (or more) target 
 methods of the class. As already mentioned, this is easy if this callback 
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -859,14 +870,16 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
 This is how it usually works: *one action* of the observed ``Dog``, here it's 
 the instantiation, triggers *many actions* at each observing ``Person``.
 
+.. _Class Decoration, Case 3:
+
 But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
@@ -946,19 +959,20 @@
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
 The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
-first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. On the other hand, the call ``dog.action2()`` fails because 
-this *instance method* was not registered. But, if this is what is to be 
-achieved, an instance method can first be created and registered, just as 
-seen above.
+first argument, ``self``. This works because internally the *class method* 
+``Dog.action2`` was registered instead of an instance method that didn't  
+exist at compile time. On the other hand, the call ``dog.action2()`` 
+fails because this *instance method* was not registered. But, if this is what 
+is to be achieved, an instance method can first be created and registered, 
+just as seen above in `Class Decoration, Case 3`_.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
@@ -1035,49 +1049,59 @@
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
     
 This method of instance decoration is certainly the most flexible. However, 
 it bears the risk of losing track of all dependencies. 
 
-    
+
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.4.*, Build: 2023-06-20**
+
+- A new subclass SemiSingleton for a resettable singleton
+- Accessible parameter for singleton and multiton removed
+- Additional test and documentation
+- Pre production state, version 0.9.* for modules
+    - singleton, [ ``python -m decoratory.singleton --version`` ]
+    - multiton,  [ ``python -m decoratory.multiton  --version`` ]
+
 **Version: 0.1.3.*, Build: 2023-06-19**
 
-- Enhancements for module observer: test and documentation
+- Extensions and improvements for module observer: test and documentation
 
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
-- accessible parameter for singleton and multiton, incl. documentation
-- resettable parameter for singleton and multiton, incl. documentation
+- Accessible parameter for singleton and multiton, incl. documentation
+- Resettable parameter for singleton and multiton, incl. documentation
 
 **Version: 0.1.0.2, Build: 2023-06-13**
 
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.3.11/Readme.rst` & `decoratory-0.1.4.2/Readme.rst`

 * *Files 3% similar despite different names*

```diff
@@ -30,44 +30,44 @@
 
     python -m decoratory --test
 
 .. _toc:
 
 **Package Contents**
 
-The *decoratory package* available here includes some classic decorators
+The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
-To illustrate the functionality of each module, a simple as well as a
-more complex example is presented. Even if only one particular module
+To illustrate the functionality of each module, simple as well as 
+more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
 more examples of the full range of possibilities, please refer to the
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
-across modules.
+across module boundaries.
 
-As a simple example serves the decoration of the class  ``Animal`` as
+As a simple example serves the decoration of the class  ``Animal`` as a 
 singleton. In the context of the `Decorator Arguments Pattern`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
@@ -79,16 +79,16 @@
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Teddy')        # Creates Teddy
-    b = Animal(name='Roxie')        # Returns Teddy
+    a = Animal(name='Teddy')        # Creates Teddy, the primary instance
+    b = Animal(name='Roxie')        # Returns Teddy, no Roxi is created
 
 If instances of the class ``Animal`` are now created, this is only done for the
 very first instantiation, and for all further instantiations always this
 *primary instance* is given back.
 
 .. code-block:: python
 
@@ -100,16 +100,16 @@
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
-code is used, additional parameters can be passed to the decorator for
-passing to the class constructor.
+code is used, additional parameters can be passed to the decorator for 
+passing to or through the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -121,30 +121,29 @@
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
-So far, this singleton implementation follows the concept of *once and
+So far, this singleton implementation follows the concept of *once 
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
-Although this behavior is consistent with the basic concept of a singleton,
-there are situations where it might be useful to reset a *singleton*. Such
-a *resettable singleton* could be useful to express in code that an instance
-is often retrieved but rarely changed.
+Although this behavior is consistent with the fundamental concept of a 
+singleton, there are situations where it might be useful to reset a 
+*singleton*. Such a *resettable singleton*, also called *semi-singleton*, 
+could be useful to express in code that an instance is often retrieved but 
+rarely changed.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as 'resettable singleton'
 
-    from decoratory.singleton import Singleton
-
     @Singleton(resettable=True)     # Exposes an additional reset method
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
@@ -152,54 +151,54 @@
     # Case 3: Decoration using @Singleton(resettable=True)
     print(Animal(name='Teddy'))     # Animal('Teddy')
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
-Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and
-the call ``Animal.reset()`` will fail raising an ``AttributeError``.
-
-With the same intention, the retrieval of the *primary instance* is also
-locked by default, but can be unlocked during decoration with the
-``accessible=True`` parameter, which allows ``Animal`` to expose the
-``get_instance()`` method.
+Without this striking ``resettable=True`` decoration ``Animal`` has no 
+``reset`` method and the call ``Animal.reset()`` will fail raising an 
+``AttributeError``. For situations where this concept really needs 
+to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
-    # *** example_singleton.py - decoration as 'accessible singleton'
+    # *** example_singleton.py - decoration as a 'semi singleton'
 
-    from decoratory.singleton import Singleton
+    from decoratory.singleton import SemiSingleton
 
-    @Singleton(accessible=True)     # Exposes a get_instance method
+    @SemiSingleton                  # or @SemiSingleton()
     class Animal:
-        def __init__(self, name):
-            self.name = name
+        pass                        # Some code ...
 
-        def __repr__(self):
-            return f"{self.__class__.__name__}('{self.name}')"
+Last but not least, both ``Singleton`` and ``SemiSingleton`` of course also 
+provide a ``get_instance()`` method to directly retrieve the primary instance,
+e.g. using ``Animal.get_instance()``. 
 
-    # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Teddy')        # Animal('Teddy')
-    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
-    print(a)                        # Animal('Teddy')
-    print(b)                        # Animal('Teddy')
+    **Hint** --- Using ``reset()`` and ``get_instance()`` in combination
+    
+    *It should be noted that the combination of* ``reset()`` *and immediately 
+    following* ``get_instance()`` *does not return a valid object, but*
+    ``None``. *So a* ``reset()`` *should always be followed by an 
+    instantiation to ensure that a valid singleton instance exists.*
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
 Whereas the singleton allows for exactly one instance per class, the multiton
-ensures one single (unique) *instance per key value of a dictionary*.
+ensures one single (unique) *instance per key*.
 
-In this implementation the key parameter can be either any immutable type
-or a callable returning such an immutable type which can be used as a key
-of a dictionary. In case of an invalid key, key is set ``None`` and with only
+In this implementation, the key parameter can be anything that is possible as 
+a key for a Python ``dict()`` dictionary, such as an immutable type or a 
+callable eventually returning such an immutable type etc. 
+
+In case of an invalid key, key is set ``None`` and with only
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
@@ -262,76 +261,88 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
     # Case 3: One unique instance per specie
     @Multiton(key="{0}".format)     # spec is args[0]
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 4: One unique instance per name
     @Multiton(key="{name}".format)  # name is kwargs['name']
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 5: One unique instance for all init values, i.e. no duplicates
     @Multiton(key=lambda spec, name: (spec, name))
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
-        ...
+        pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
 any new key raises a ``KeyError``.
 
-For deeper, special requirements on the equivalence classes of a multiton
-by setting the decorator parameter ``accessible=True``, the method
-``get_instances()`` is enabled, which grants direct access to the internal
-directory of the instances. This can be actively manipulated in this way,
-which of course should be done with care and is generally not recommended.
-
-.. code-block:: python
-
-    # *** example_multitonton.py - Accessibility to the internal directory
-
-    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
-    #                                   accessible=True)
-    print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') 
-    c = Animal('dog', name='Roxie') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
-                                    #  True:  Animal('cat', 'Molly')}
-
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. hint::
+Last but not least, ``Multiton`` provides a ``instances`` property and 
+associated getter and setter methods to directly retrieve the internal 
+dictionary of primary instances. It is obvious that manipulations on it can 
+corrupt the multiton itself, so it is a method for experts, but sometimes 
+they want or need to have exactly this freedom.
 
-    Classifications into the multiton directory are done only once on
+    **Hint** --- Changes affecting key values of classified objects
+
+    *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
-    corrupted by such modifications.
+    corrupted by such modifications.*
+
+    *Therefore,* **never change key related values of classified objects!**
 
-    Therefore, **never change key related values of classified objects**!
+This results in the following exemplary picture:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - seal, unseal, reset, get_instance
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: name,
+    #                                   resettable=True)
+    Animal.reset()                  # Because of resettable=True
+    print(Animal.get_instances())   # {}
+    print(Animal.issealed())        # False     (=default)
+    Animal('dog', name='Teddy')     # Animal('dog', 'Teddy')
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.seal()                   # Seal the multiton!
+    print(Animal.issealed())        # True
+    try:                            # Try to..
+        Animal('cat', name='Molly') # .. add a new animal
+    except  KeyError as ex:         # .. will fail
+        print(f"Sorry {ex.args[1]}, {ex.args[0]}")
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.unseal()                 # Unseal the multiton!
+    print(Animal.issealed())        # False
+    Animal('cat', name='Molly')     # Now, Molly is added
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'), 
+                                    #  'Molly': Animal('cat', 'Molly')}
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -464,21 +475,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. hint::
+    **Hint** --- Dynamic versus static decoration
 
-    Decorations to ``@staticmethod`` or ``@classmethod`` can be done
+    *Decorations to* ``@staticmethod`` *or* ``@classmethod`` *can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
     an object instance is created and must be decorated dynamically as an 
-    instance (e.g. see  `Instance Decoration`_ below).
+    instance (e.g. see*  `Instance Decoration`_ *below).*
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -780,19 +791,19 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-.. warning::
+    **Hint** --- Take care when decorating a class constructor
 
-    Calling **__init__()** results in a new instance! This means calling 
+    *Calling* ``__init__`` *results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior...
+    in not any case this is the desired behavior ...*
 
 So the decoration should not address a class but one (or more) target 
 methods of the class. As already mentioned, this is easy if this callback 
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -820,14 +831,16 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
 This is how it usually works: *one action* of the observed ``Dog``, here it's 
 the instantiation, triggers *many actions* at each observing ``Person``.
 
+.. _Class Decoration, Case 3:
+
 But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
@@ -907,19 +920,20 @@
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
 The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
-first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. On the other hand, the call ``dog.action2()`` fails because 
-this *instance method* was not registered. But, if this is what is to be 
-achieved, an instance method can first be created and registered, just as 
-seen above.
+first argument, ``self``. This works because internally the *class method* 
+``Dog.action2`` was registered instead of an instance method that didn't  
+exist at compile time. On the other hand, the call ``dog.action2()`` 
+fails because this *instance method* was not registered. But, if this is what 
+is to be achieved, an instance method can first be created and registered, 
+just as seen above in `Class Decoration, Case 3`_.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
@@ -996,49 +1010,59 @@
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
     
 This method of instance decoration is certainly the most flexible. However, 
 it bears the risk of losing track of all dependencies. 
 
-    
+
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.4.*, Build: 2023-06-20**
+
+- A new subclass SemiSingleton for a resettable singleton
+- Accessible parameter for singleton and multiton removed
+- Additional test and documentation
+- Pre production state, version 0.9.* for modules
+    - singleton, [ ``python -m decoratory.singleton --version`` ]
+    - multiton,  [ ``python -m decoratory.multiton  --version`` ]
+
 **Version: 0.1.3.*, Build: 2023-06-19**
 
-- Enhancements for module observer: test and documentation
+- Extensions and improvements for module observer: test and documentation
 
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
-- accessible parameter for singleton and multiton, incl. documentation
-- resettable parameter for singleton and multiton, incl. documentation
+- Accessible parameter for singleton and multiton, incl. documentation
+- Resettable parameter for singleton and multiton, incl. documentation
 
 **Version: 0.1.0.2, Build: 2023-06-13**
 
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.3.11/Sources/decoratory/__main__.py` & `decoratory-0.1.4.2/Sources/decoratory/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.11"
-__date__ = "2023-06-19"
-__time__ = "18:30:22"
+__version__ = "0.1.4.2"
+__date__ = "2023-06-20"
+__time__ = "16:37:47"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.3.11/Sources/decoratory/banner.py` & `decoratory-0.1.4.2/Sources/decoratory/banner.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Sources/decoratory/basic.py` & `decoratory-0.1.4.2/Sources/decoratory/basic.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Sources/decoratory/multiton.py` & `decoratory-0.1.4.2/Sources/decoratory/multiton.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,24 @@
 # vim: fileencoding=UTF-8 tabstop=8 expandtab shiftwidth=4 softtabstop=4
 # -----------------------------------------------------------------------------
 # Document Description
 """**Multiton**
 
     A multiton pattern is a design pattern that extends the singleton pattern.
     Whereas the singleton allows for exactly one instance per class, the
-    multiton ensures one single (unique) instance per key value of a
-    dictionary.
+    multiton ensures one single (unique) instance per key.
+
+    In this implementation, the key parameter can be anything that is possible
+    as a key for a Python dict() dictionary, such as an immutable type or a
+    callable eventually returning such an immutable type etc.
+
+    In case of an invalid key, key is set None and with only one key value the
+    multiton simply collapses to a singleton, therefore the decoration
+    @Multiton resp. @Multiton() or even @Multiton(key=17) or
+    @Multiton(key='some constant value') and so on always creates a singleton.
 
     Attributes
     ----------
     Multiton (class):
         Creates a multiton instance as a callable object.
 
     Methods
@@ -20,25 +28,24 @@
         None.
 
     Examples
     --------
 
     from decoratory.multiton import Multiton
 
-    # --- For alternative decorations see cases below!
-    @Multiton                       # Multiton(), Multiton(key=17), ...
+    @Multiton(key=lambda spec, name: name)
     class Animal:
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
-    # Create instances
+    # Create Instances
     a = Animal('dog', name='Teddy')
     b = Animal('cat', name='Molly')
     c = Animal('dog', name='Roxie')
 
     # Case 0: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
     #    ---> With no or fixed key the Multiton acts like a Singleton
     print(a)                        # Animal('dog', 'Teddy')
@@ -79,55 +86,55 @@
     #    ---> Late binding with F(classmethod_string)
     #         One unique instance from a @staticmethod or @classmethod
     class Animal:
         ...
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
+
     print(a)                        # Animal('dog', 'Teddy')
     print(b)                        # Animal('cat', 'Molly')
     print(c)                        # Animal('cat', 'Molly')
 
-    # Case 7: decoration @Multiton(key=lambda spec, name: name,
-    #                              accessible=True, resettable=True)
-    #    ---> Seal after Teddy
-    Animal.reset()                  # Reset/Clear the instance dictionary
+    # Case 7: with decoration @Multiton(key=lambda spec, name: name,
+    #                                   resettable=True)
+    Animal.reset()                  # Because of resettable=True
     print(Animal.get_instances())   # {}
-    print(Animal.issealed())        # False
-    a = Animal('dog', name='Teddy') # Animal('dog', 'Teddy')
-    Animal.seal()                   # Seal it!
+    print(Animal.issealed())        # False     (=default)
+    Animal('dog', name='Teddy')     # Animal('dog', 'Teddy')
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.seal()                   # Seal the multiton!
     print(Animal.issealed())        # True
-    b = Animal('dog', name='Teddy') # Returns primary instance
-    print(a is b)                   # True
-    try:
-        c = Animal('dog', name='Roxie')
-    except KeyError as ex:          # KeyError, Animal is sealed!
-        print(f"For '{ex.args[1]}' {ex.args[0]}")
+    try:                            # Try to..
+        Animal('cat', name='Molly') # .. add a new animal
+    except  KeyError as ex:         # .. will fail
+        print(f"Sorry {ex.args[1]}, {ex.args[0]}")
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
-    Animal.unseal()                 # Unseal it!
-    c = Animal('dog', name='Roxie') # Animal('dog', 'Teddy') now it's ok!
+    Animal.unseal()                 # Unseal the multiton!
+    print(Animal.issealed())        # False
+    Animal('cat', name='Molly')     # Now, Molly is added
     print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
-                                    #  'Roxie': Animal('dog', 'Roxie')}
+                                    #  'Molly': Animal('cat', 'Molly')}
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Multiton"
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.7"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-20"
+__time__ = "16:08:29"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -137,89 +144,78 @@
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Multiton:
     """**Multiton**
 
-    Multiton(substitute, *args, key, accessible, resettable, **kwargs)
+    Multiton(substitute, *args, key, resettable, **kwargs)
 
     Attributes
     ----------
     substitute (callable|type):
         A type to be made a multiton
 
     key (F|callable|object|None):
         An object building the instance key
 
-    accessible (bool):
-        If True exposes a get_instances() method
-
     resettable (bool):
         If True exposes a reset() method
 
     Methods
     -------
     seal(self) -> None:
         Seal the multiton
 
     unseal(self) -> None:
         Unseal the multiton
 
     issealed(self) -> bool:
         Multiton sealing state
 
-    get_instances(self) -> dict:    (if accessible=True, only!)
-        Return the multiton instance dictionary
+    get_instances(self) -> dict:    (property)
+        Returns the internal dictionary of instances
+
+    set_instances(self) -> None:    (property)
+        Sets the internal dictionary of instances
 
     reset(self) -> None:            (if resettable=True, only!)
         Resets the multiton instance dictionary
     """
 
     def __init__(self,
                  substitute: type = None,
                  *args: object,
                  key: Union[F, callable, object, None] = None,
-                 accessible: bool = False,
                  resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a multiton.
 
         Parameters:
             substitute (object): A type to be made a multiton
             key: (F|callable|object|None): An object building the instance key
-            accessible (bool): If True exposes a get_instance() method
             resettable (bool): If True exposes a reset() method
 
         Returns:
             self (object): Multiton decorator instance
         """
         self.__set__substitute(substitute)
         self.__key = key
 
         # Dictionary for unique key instances
-        self.__instances = dict()
+        self._instances = dict()
 
         # Sealing state
         self.__sealed = False
 
-        # If accessible == True exposes a get_instances() method
-        if bool(accessible):
-            def get_instances(s: object = self):
-                """Return dictionary of all instance representations."""
-                return s.__instances
-
-            # Add the instances method
-            setattr(self, 'get_instances', get_instances)
-
         # If resettable == True exposes a reset() method
         if bool(resettable):
-            def reset(s: object = self):
+            def reset(s: object = self) -> None:
                 """Define reset method"""
-                s.__instances.clear()
+                s.set_instances(None)
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
         # --- Decorator Arguments Pattern (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
@@ -253,60 +249,70 @@
                             getattr(self.substitute.callee, self.__key.callee),
                             *subst.callee_args, **subst.callee_kwargs).eval()
                 elif callable(self.__key):  # function
                     d_key = F(self.__key, *subst.callee_args,
                               **subst.callee_kwargs).eval()
                 else:  # Value
                     d_key = self.__key
-                instance = self.__instances.get(d_key, None)
+                instance = self._instances.get(d_key, None)
             except (TypeError, Exception):  # Default is None
                 d_key = None
-                instance = self.__instances.get(d_key, None)
+                instance = self._instances.get(d_key, None)
 
             # Create and store new or return existing instance (by key)
             if instance is None:
                 if self.__sealed:
                     raise KeyError(f"{self.__name__} is sealed.", d_key)
-                instance = self.__instances.setdefault(d_key, subst.eval())
+                instance = self._instances.setdefault(d_key, subst.eval())
 
             return instance
 
     # Getter, Setter, Properties
     def __get__substitute(self):
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
+    def get_instances(self) -> dict:
+        """Returns the internal dictionary of instances"""
+        return self._instances
+
+    def set_instances(self, value: dict = None) -> None:
+        """Sets the internal dictionary of instances"""
+        self._instances = value if isinstance(value, dict) else dict()
+
+    instances = property(get_instances, set_instances)
+
     # Methods
-    def seal(self):
+    def seal(self) -> None:
         """Seal multiton.
 
         Parameters:
             None.
 
         Returns:
             None.
         """
         self.__sealed = True
 
-    def unseal(self):
+    def unseal(self) -> None:
         """Unseal multiton .
 
         Parameters:
             None.
 
         Returns:
             None.
         """
         self.__sealed = False
 
-    def issealed(self):
+    def issealed(self) -> bool:
         """Multiton sealing state
 
         Parameters:
             None.
 
         Returns:
             True/False (bool): Sealing state.
```

### Comparing `decoratory-0.1.3.11/Sources/decoratory/observer.py` & `decoratory-0.1.4.2/Sources/decoratory/observer.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Sources/decoratory/singleton.py` & `decoratory-0.1.4.2/Sources/decoratory/singleton.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,156 +4,154 @@
 # -----------------------------------------------------------------------------
 # Document Description
 """**Singleton**
 
     A singleton pattern is a design pattern that limits the instantiation of a
     class to a single (unique) instance. This is useful when exactly one
     unique object is needed i.e. to manage an expensive resource or coordinate
-    actions across modules.
+    actions across module boundaries.
 
     Attributes
     ----------
     Singleton (class):
         Creates a singleton instance as a callable object.
 
+    SemiSingleton (class):
+        Creates a resettable semi singleton instance as a callable object.
+
     Methods
     -------
         None.
 
     Examples
     --------
 
     from decoratory.singleton import Singleton
 
+    # -------------------------------------------------------------------------
     @Singleton                      # or @Singleton()
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Teddy')        # Creates Teddy
-    b = Animal(name='Roxie')        # Returns Teddy
+    a = Animal(name='Teddy')        # Creates Teddy, the primary instance
+    b = Animal(name='Roxie')        # Returns Teddy, no Roxi is created
 
     # Case 1: Static decoration using @Singleton or @Singleton()
-    #    ---> One single object instance fits all.
     print(f"a = {a}")               # a = Animal('Teddy')
     print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
     # Case 2: Dynamic decoration providing extra initial default values
-    #    ---> Initial default values provided via the decorator
     Animal = Singleton(Animal, 'Teddy')
     Animal()                        # Using the decorator's default 'Teddy'
     a = Animal(name='Roxie')        # Returns Teddy
     print(a)                        # Animal('Teddy')
 
+    # -------------------------------------------------------------------------
+    @Singleton(resettable=True)     # Exposes an additional reset method
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+
+        def __repr__(self):
+            return f"{self.__class__.__name__}('{self.name}')"
+
     # Case 3: Decoration using @Singleton(resettable=True)
     print(Animal(name='Teddy'))     # Animal('Teddy')
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
-    # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Teddy')        # Animal('Teddy')
-    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
-    print(a)                        # Animal('Teddy')
-    print(b)                        # Animal('Teddy')
+    # -------------------------------------------------------------------------
+    from decoratory.singleton import SemiSingleton
+
+    @SemiSingleton                  # or @SemiSingleton()
+    class Animal:
+        pass                        # Some code ...
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Singleton"
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.9"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.9.0.1"
+__date__ = "2023-06-20"
+__time__ = "16:08:29"
 __state__ = "Beta"
 __license__ = "PSF"
 
-__all__ = ["Singleton"]
+__all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from functools import update_wrapper
 from decoratory.basic import F
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Singleton:
     """**Singleton**
 
-    Singleton(substitute, *args, accessible, resettable, **kwargs)
+    Singleton(substitute, *args, resettable, **kwargs)
 
     Attributes
     ----------
     substitute (callable|type):
         A type to be made a singleton
 
-    accessible (bool):
-        If True exposes a get_instance() method
-
     resettable (bool):
         If True exposes a reset() method
 
     Methods
     -------
-    get_instance(self) -> object:   (if accessible=True, only!)
-        Return the singleton instance
+    get_instance(self) -> object:
+        Return the singleton instance (primary instance)
 
     reset(self) -> None:            (if resettable=True, only!)
         Resets the singleton instance
     """
 
     def __init__(self,
                  substitute: object = None,
                  *args: object,
-                 accessible: bool = False,
                  resettable: bool = False,
                  **kwargs: object) -> None:
         """Set up a singleton.
 
         Parameters:
             substitute (object): A type to be made a singleton
-            accessible (bool): If True exposes a get_instance() method
             resettable (bool): If True exposes a reset() method
 
         Returns:
             self (object): Singleton decorator instance
         """
         self.__set__substitute(substitute)
 
         # The unique instance
         self.__instance = None
 
-        # If accessible == True exposes a get_instance() method
-        if bool(accessible):
-            def get_instance(s: object = self):
-                """Define get_instance method"""
-                return s.__instance
-
-            # Add the get_instance method
-            setattr(self, 'get_instance', get_instance)
-
         # If resettable == True exposes a reset() method
         if bool(resettable):
-            def reset(s: object = self):
+            def reset(s: object = self) -> None:
                 """Define reset method"""
                 s.__instance = None
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
         # --- Decorator Arguments Pattern (1/2)
@@ -187,14 +185,41 @@
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
+    # Methods
+    def get_instance(self) -> object:
+        """Returns the singleton instance"""
+        return self.__instance
+
+
+class SemiSingleton(Singleton):
+    """SemiSingleton
+
+    A subclass shortcut for a resettable singleton.
+    """
+
+    def __init__(self,
+                 substitute: object = None,
+                 *args: object,
+                 **kwargs: object) -> None:
+        """Set up a semi singleton.
+
+        Parameters:
+            substitute (object): A type to be made a semi singleton
+
+        Returns:
+            self (object): Semi singleton decorator instance
+        """
+        kwargs["resettable"] = True
+        super().__init__(substitute, *args, **kwargs)
+
 
 # -----------------------------------------------------------------------------
 # Entry Point
 if __name__ == '__main__':
     import decoratory.singleton as module
     from decoratory.banner import __banner as banner
```

### Comparing `decoratory-0.1.3.11/Sources/decoratory/wrapper.py` & `decoratory-0.1.4.2/Sources/decoratory/wrapper.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.4.2/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.3.11
+Version: 0.1.4.2
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -69,44 +69,44 @@
 
     python -m decoratory --test
 
 .. _toc:
 
 **Package Contents**
 
-The *decoratory package* available here includes some classic decorators
+The *decoratory package* includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
 This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
-To illustrate the functionality of each module, a simple as well as a
-more complex example is presented. Even if only one particular module
+To illustrate the functionality of each module, simple as well as 
+more complex examples are presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
 more examples of the full range of possibilities, please refer to the
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of
 a class to a single (unique) instance. This is useful when exactly one unique
 object is needed i.e. to manage an expensive resource or coordinate actions
-across modules.
+across module boundaries.
 
-As a simple example serves the decoration of the class  ``Animal`` as
+As a simple example serves the decoration of the class  ``Animal`` as a 
 singleton. In the context of the `Decorator Arguments Pattern`_, this can be
 done both without brackets (decorator class) and with brackets (decorator
 instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
 
     # *** example_singleton.py - class Animal with Singleton decoration
@@ -118,16 +118,16 @@
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Teddy')        # Creates Teddy
-    b = Animal(name='Roxie')        # Returns Teddy
+    a = Animal(name='Teddy')        # Creates Teddy, the primary instance
+    b = Animal(name='Roxie')        # Returns Teddy, no Roxi is created
 
 If instances of the class ``Animal`` are now created, this is only done for the
 very first instantiation, and for all further instantiations always this
 *primary instance* is given back.
 
 .. code-block:: python
 
@@ -139,16 +139,16 @@
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 .. _dynamic-decoration:
 
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
-code is used, additional parameters can be passed to the decorator for
-passing to the class constructor.
+code is used, additional parameters can be passed to the decorator for 
+passing to or through the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values
     Animal = Singleton(Animal, 'Teddy')
@@ -160,30 +160,29 @@
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 #. Decoration as a class (without parentheses) and Decoration as an instance
    (with empty parentheses) are equivalent
 #. For dynamic decoration, extra parameters can be passed, e.g. for the
    class constructor
 
-So far, this singleton implementation follows the concept of *once and
+So far, this singleton implementation follows the concept of *once 
 forever*, i.e. whenever a new instance of a class is created, one always
 gets the *primary instance* back - without any possibility of ever changing
 it again.
 
-Although this behavior is consistent with the basic concept of a singleton,
-there are situations where it might be useful to reset a *singleton*. Such
-a *resettable singleton* could be useful to express in code that an instance
-is often retrieved but rarely changed.
+Although this behavior is consistent with the fundamental concept of a 
+singleton, there are situations where it might be useful to reset a 
+*singleton*. Such a *resettable singleton*, also called *semi-singleton*, 
+could be useful to express in code that an instance is often retrieved but 
+rarely changed.
 
 .. code-block:: python
 
     # *** example_singleton.py - decoration as 'resettable singleton'
 
-    from decoratory.singleton import Singleton
-
     @Singleton(resettable=True)     # Exposes an additional reset method
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
@@ -191,54 +190,54 @@
     # Case 3: Decoration using @Singleton(resettable=True)
     print(Animal(name='Teddy'))     # Animal('Teddy')
     print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
     print(Animal(name='Roxie'))     # Animal('Roxie')
     print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
-Without ``resettable=True`` decoration ``Animal`` has no ``reset`` method and
-the call ``Animal.reset()`` will fail raising an ``AttributeError``.
-
-With the same intention, the retrieval of the *primary instance* is also
-locked by default, but can be unlocked during decoration with the
-``accessible=True`` parameter, which allows ``Animal`` to expose the
-``get_instance()`` method.
+Without this striking ``resettable=True`` decoration ``Animal`` has no 
+``reset`` method and the call ``Animal.reset()`` will fail raising an 
+``AttributeError``. For situations where this concept really needs 
+to be used more often, a subclass shortcut ``SemiSingleton`` is provided.
 
 .. code-block:: python
 
-    # *** example_singleton.py - decoration as 'accessible singleton'
+    # *** example_singleton.py - decoration as a 'semi singleton'
 
-    from decoratory.singleton import Singleton
+    from decoratory.singleton import SemiSingleton
 
-    @Singleton(accessible=True)     # Exposes a get_instance method
+    @SemiSingleton                  # or @SemiSingleton()
     class Animal:
-        def __init__(self, name):
-            self.name = name
+        pass                        # Some code ...
 
-        def __repr__(self):
-            return f"{self.__class__.__name__}('{self.name}')"
+Last but not least, both ``Singleton`` and ``SemiSingleton`` of course also 
+provide a ``get_instance()`` method to directly retrieve the primary instance,
+e.g. using ``Animal.get_instance()``. 
 
-    # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Teddy')        # Animal('Teddy')
-    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
-    print(a)                        # Animal('Teddy')
-    print(b)                        # Animal('Teddy')
+    **Hint** --- Using ``reset()`` and ``get_instance()`` in combination
+    
+    *It should be noted that the combination of* ``reset()`` *and immediately 
+    following* ``get_instance()`` *does not return a valid object, but*
+    ``None``. *So a* ``reset()`` *should always be followed by an 
+    instantiation to ensure that a valid singleton instance exists.*
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
 Whereas the singleton allows for exactly one instance per class, the multiton
-ensures one single (unique) *instance per key value of a dictionary*.
+ensures one single (unique) *instance per key*.
 
-In this implementation the key parameter can be either any immutable type
-or a callable returning such an immutable type which can be used as a key
-of a dictionary. In case of an invalid key, key is set ``None`` and with only
+In this implementation, the key parameter can be anything that is possible as 
+a key for a Python ``dict()`` dictionary, such as an immutable type or a 
+callable eventually returning such an immutable type etc. 
+
+In case of an invalid key, key is set ``None`` and with only
 one key value the multiton simply collapses to a singleton, therefore the
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)``
 or  ``@Multiton(key='some constant value')`` and so on always creates a
 singleton.
 
 Normally, the key is part of or is composed from the initial values of the
 classified object, as in the following example, where the key function matches
@@ -301,76 +300,88 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Alternative decoration examples
 
     # Case 3: One unique instance per specie
     @Multiton(key="{0}".format)     # spec is args[0]
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 4: One unique instance per name
     @Multiton(key="{name}".format)  # name is kwargs['name']
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 5: One unique instance for all init values, i.e. no duplicates
     @Multiton(key=lambda spec, name: (spec, name))
     class Animal:
-        ...
+        pass                        # Some code ...
 
     # Case 6: One unique instance from a @staticmethod or @classmethod
     @Multiton(key=F("my_key"))      # Late binding with F(classmethod_string)
     class Animal:
-        ...
+        pass                        # Some code ...
 
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
 
 To actively control access to new equivalence classes, ``Multiton`` provides
 the ``seal()``, ``unseal()``, and ``issealed()`` methods for sealing, unsealing,
 and checking the sealing state of the ``Multiton``. By default, the sealing
 state is set ``False``, so for every new key a new (unique) object is
 instantiated. When sealed (e.g. later in the process) is set ``True`` the
 dictionary has completed, i.e. restricted to the current object set and
 any new key raises a ``KeyError``.
 
-For deeper, special requirements on the equivalence classes of a multiton
-by setting the decorator parameter ``accessible=True``, the method
-``get_instances()`` is enabled, which grants direct access to the internal
-directory of the instances. This can be actively manipulated in this way,
-which of course should be done with care and is generally not recommended.
-
-.. code-block:: python
-
-    # *** example_multitonton.py - Accessibility to the internal directory
-
-    # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
-    #                                   accessible=True)
-    print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') 
-    c = Animal('dog', name='Roxie') 
-    print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
-                                    #  True:  Animal('cat', 'Molly')}
-
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. hint::
+Last but not least, ``Multiton`` provides a ``instances`` property and 
+associated getter and setter methods to directly retrieve the internal 
+dictionary of primary instances. It is obvious that manipulations on it can 
+corrupt the multiton itself, so it is a method for experts, but sometimes 
+they want or need to have exactly this freedom.
 
-    Classifications into the multiton directory are done only once on
+    **Hint** --- Changes affecting key values of classified objects
+
+    *Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
-    corrupted by such modifications.
+    corrupted by such modifications.*
+
+    *Therefore,* **never change key related values of classified objects!**
 
-    Therefore, **never change key related values of classified objects**!
+This results in the following exemplary picture:
+
+.. code-block:: python
+
+    # *** example_multitonton.py - seal, unseal, reset, get_instance
+
+    # Case 7: with decoration @Multiton(key=lambda spec, name: name,
+    #                                   resettable=True)
+    Animal.reset()                  # Because of resettable=True
+    print(Animal.get_instances())   # {}
+    print(Animal.issealed())        # False     (=default)
+    Animal('dog', name='Teddy')     # Animal('dog', 'Teddy')
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.seal()                   # Seal the multiton!
+    print(Animal.issealed())        # True
+    try:                            # Try to..
+        Animal('cat', name='Molly') # .. add a new animal
+    except  KeyError as ex:         # .. will fail
+        print(f"Sorry {ex.args[1]}, {ex.args[0]}")
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
+    Animal.unseal()                 # Unseal the multiton!
+    print(Animal.issealed())        # False
+    Animal('cat', name='Molly')     # Now, Molly is added
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'), 
+                                    #  'Molly': Animal('cat', 'Molly')}
 
 
 ******************************************************************************
 Wrapper
 ******************************************************************************
 
 As the name implies, a wrapper encloses the original function with an
@@ -503,21 +514,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. hint::
+    **Hint** --- Dynamic versus static decoration
 
-    Decorations to ``@staticmethod`` or ``@classmethod`` can be done
+    *Decorations to* ``@staticmethod`` *or* ``@classmethod`` *can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
     an object instance is created and must be decorated dynamically as an 
-    instance (e.g. see  `Instance Decoration`_ below).
+    instance (e.g. see*  `Instance Decoration`_ *below).*
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -819,19 +830,19 @@
     # Case 1: Dog is an observable to Person
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe arrived.
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
-.. warning::
+    **Hint** --- Take care when decorating a class constructor
 
-    Calling **__init__()** results in a new instance! This means calling 
+    *Calling* ``__init__`` *results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired behavior...
+    in not any case this is the desired behavior ...*
 
 So the decoration should not address a class but one (or more) target 
 methods of the class. As already mentioned, this is easy if this callback 
 function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
@@ -859,14 +870,16 @@
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
 This is how it usually works: *one action* of the observed ``Dog``, here it's 
 the instantiation, triggers *many actions* at each observing ``Person``.
 
+.. _Class Decoration, Case 3:
+
 But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
@@ -946,19 +959,20 @@
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
 The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
-first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. On the other hand, the call ``dog.action2()`` fails because 
-this *instance method* was not registered. But, if this is what is to be 
-achieved, an instance method can first be created and registered, just as 
-seen above.
+first argument, ``self``. This works because internally the *class method* 
+``Dog.action2`` was registered instead of an instance method that didn't  
+exist at compile time. On the other hand, the call ``dog.action2()`` 
+fails because this *instance method* was not registered. But, if this is what 
+is to be achieved, an instance method can first be created and registered, 
+just as seen above in `Class Decoration, Case 3`_.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
@@ -1035,49 +1049,59 @@
     # Case 7: Unregister nti.info from tgi
     tgi.inc.observable.unregister(nti.info)
     print(tgi.inc.observable.observers(classbased=True))    # {}
     
 This method of instance decoration is certainly the most flexible. However, 
 it bears the risk of losing track of all dependencies. 
 
-    
+
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.4.*, Build: 2023-06-20**
+
+- A new subclass SemiSingleton for a resettable singleton
+- Accessible parameter for singleton and multiton removed
+- Additional test and documentation
+- Pre production state, version 0.9.* for modules
+    - singleton, [ ``python -m decoratory.singleton --version`` ]
+    - multiton,  [ ``python -m decoratory.multiton  --version`` ]
+
 **Version: 0.1.3.*, Build: 2023-06-19**
 
-- Enhancements for module observer: test and documentation
+- Extensions and improvements for module observer: test and documentation
 
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
-- accessible parameter for singleton and multiton, incl. documentation
-- resettable parameter for singleton and multiton, incl. documentation
+- Accessible parameter for singleton and multiton, incl. documentation
+- Resettable parameter for singleton and multiton, incl. documentation
 
 **Version: 0.1.0.2, Build: 2023-06-13**
 
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
 ~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
 
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.3.11/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.1.4.2/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Unittest/test_basic.py` & `decoratory-0.1.4.2/Unittest/test_basic.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Unittest/test_multiton.py` & `decoratory-0.1.4.2/Unittest/test_multiton.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.9"
-__date__ = "2023-06-19"
-__time__ = "18:04:04"
+__version__ = "0.1.3.10"
+__date__ = "2023-06-20"
+__time__ = "16:08:29"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -238,15 +238,15 @@
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
     def test_decoration_with_valid_parameter_id(self):
-        """Unittest: Decoration with a valid key parameter:
+        """Unittest: Decoration with a valid key parameter: args[0]
             -> key = "name" attribute from args[0]
         """
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(key="{0}".format)(TestClass)  # args[0]
 
         # Instances
         a = TestClassMultiton("a")  # New single object a
@@ -269,15 +269,15 @@
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
     def test_decoration_with_valid_parameter_name(self):
-        """Unittest: Decoration with a valid key parameter:
+        """Unittest: Decoration with a valid key parameter: kwargs['name']
             --> key = "name" attribute from kwargs['name']
         """
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(key="{name}".format)(
             TestClass)  # kwargs['name']
 
         # Instances
@@ -301,15 +301,15 @@
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
     def test_decoration_with_valid_parameter_inherited(self):
-        """Unittest: Decoration with a valid key parameter:
+        """Unittest: Decoration with a valid key parameter: lambda name: name
             --> key = "name" attribute from lambda name: name
         """
 
         class TestClass(TestMultiton.TestClass):
             """Inherited test class"""
             pass
 
@@ -336,15 +336,15 @@
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
     def test_decoration_with_callable_parameter(self):
-        """Unittest: Decoration with a valid key callable
+        """Unittest: Decoration with a valid key callable: f = lambda name: name
             --> key = "name" attribute from function f = lambda name: name
         """
         f = lambda name: name  # Mapping as a function
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(key=f)(TestClass)
 
         # Instances
@@ -406,15 +406,15 @@
         self.assertNotEqual(a, c)
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
-    def test_decoration_sealed(self):
+    def test_sealed(self):
         """Unittest: Decoration with a valid key parameter: "name" attribute
             --> Method test for seal(), unseal() and issealed()
         """
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(key=lambda name: name)(TestClass)
 
         # Instances
@@ -469,14 +469,56 @@
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
         self.assertEqual(TestClass.__doc__, d.__doc__)
         self.assertEqual(TestClass.__doc__, e.__doc__)
 
+    def test_reset_instances(self):
+        """Unittest: Decoration with a valid key parameter: "name" attribute
+            --> Method test for instances and reset()
+        """
+        TestClass = TestMultiton.TestClass
+        TestClassMultiton = Multiton(key=lambda name: name,
+                                     resettable=True)(TestClass)
+
+        # Instances
+        a = TestClassMultiton(name="a")  # New single object a
+        b = TestClassMultiton(name="b")  # New single object b
+
+        # Tests
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a, 'b': b})
+        TestClassMultiton.reset()
+        self.assertDictEqual(TestClassMultiton.instances, {})
+        self.assertFalse(TestClassMultiton.issealed())
+        a = TestClassMultiton(name="a")  # New single object a
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a})
+        TestClassMultiton.seal()
+        self.assertTrue(TestClassMultiton.issealed())
+        try:
+            TestClassMultiton(name="b")
+        except KeyError as ex:
+            self.assertTupleEqual(ex.args, ('TestClass is sealed.', 'b'))
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a})
+        TestClassMultiton.unseal()
+        self.assertFalse(TestClassMultiton.issealed())
+        c = TestClassMultiton(name="c")
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a, 'c': c})
+        TestClassMultiton.instances.pop("a")
+        self.assertDictEqual(TestClassMultiton.instances, {'c': c})
+        TestClassMultiton.reset()
+        self.assertDictEqual(TestClassMultiton.instances, {})
+
+        TestClassMultiton.instances = {'a': a}
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a})
+        a = TestClassMultiton(name="a")
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a})
+        TestClassMultiton(name="a")
+        self.assertDictEqual(TestClassMultiton.instances, {'a': a})
+
     def test_concurrency(self):
         """Unittest: Decoration with a valid key parameter: "name" attribute
             --> Two parallel multitons do not interfere with each other!
         """
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(key=lambda name: name)(TestClass)
         AltClass = TestMultiton.AltClass
```

### Comparing `decoratory-0.1.3.11/Unittest/test_observer.py` & `decoratory-0.1.4.2/Unittest/test_observer.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/Unittest/test_singleton.py` & `decoratory-0.1.4.2/Unittest/test_singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.8"
-__date__ = "2023-06-19"
-__time__ = "17:55:21"
+__version__ = "0.1.3.9"
+__date__ = "2023-06-20"
+__time__ = "10:56:59"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
-from decoratory.singleton import Singleton
+from decoratory.singleton import Singleton, SemiSingleton
 
 
 # -----------------------------------------------------------------------------
 # Test Class
 # noinspection PyPep8Naming
 class TestSingleton(unittest.TestCase):
     class TestClass:
@@ -84,16 +84,16 @@
         self.assertEqual(repr(a), "TestClass('a', None, 'any stuff')")
         self.assertEqual(repr(b), "TestClass('a', None, 'any stuff')")
         self.assertEqual(a, b)
         self.assertEqual(TestClass.__doc__, TestClassSingleton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
 
-    def test_decoration_with_brackets(self):
-        """Unittest: Decoration with brackets"""
+    def test_decoration_with_empty_brackets(self):
+        """Unittest: Decoration with empty brackets"""
 
         TestClass = TestSingleton.TestClass
         TestClassSingleton = Singleton()(TestClass)
 
         # Instances
         a = TestClassSingleton(name="a")  # New single object a
         b = TestClassSingleton(name="b")  # Singleton: b is a
@@ -144,28 +144,44 @@
         a = TestClassSingleton(name="a")  # New single object a (default)
 
         # Tests
         self.assertFalse(hasattr(TestClass, "reset"))
         self.assertFalse(hasattr(TestClassSingleton, "reset"))
         self.assertFalse(hasattr(a, "reset"))
 
+        # Test exception
+        try:
+            TestClassSingleton.reset()
+        except AttributeError:
+            pass
+        else:
+            raise AssertionError
+
         # ---------------------------------------------------------------------
         # Set: resettable = False
         TestClass = TestSingleton.TestClass
         # noinspection PyArgumentEqualDefault
         TestClassSingleton = Singleton(TestClass, resettable=False)
 
         # Instances
         a = TestClassSingleton(name="a")  # New single object a (default)
 
         # Tests
         self.assertFalse(hasattr(TestClass, "reset"))
         self.assertFalse(hasattr(TestClassSingleton, "reset"))
         self.assertFalse(hasattr(a, "reset"))
 
+        # Test exception
+        try:
+            TestClassSingleton.reset()
+        except AttributeError:
+            pass
+        else:
+            raise AssertionError
+
         # ---------------------------------------------------------------------
         # Set: resettable = True
         TestClass = TestSingleton.TestClass
         TestClassSingleton = Singleton(TestClass, resettable=True)
 
         # Instances
         a = TestClassSingleton(name="a")  # New single object a (default)
@@ -185,50 +201,49 @@
 
         c = TestClassSingleton(name="c")  # New single object c (default)
         self.assertEqual(repr(a), "TestClass('a', None, 'any stuff')")
         self.assertEqual(repr(c), "TestClass('c', None, 'any stuff')")
         self.assertNotEqual(a, c)
         self.assertIsNot(a, c)
 
-    def test_decoration_with_accessible(self):
-        """Unittest: Decoration with accessible"""
+    def test_semi_singleton(self):
+        """Unittest: Decoration as a semi singleton"""
 
-        # ---------------------------------------------------------------------
-        # Default: accessible = False
         TestClass = TestSingleton.TestClass
-        TestClassSingleton = Singleton(TestClass)
+        TestClassSingleton = SemiSingleton(TestClass)
 
         # Instances
         a = TestClassSingleton(name="a")  # New single object a (default)
 
         # Tests
-        self.assertFalse(hasattr(TestClass, "get_instance"))
-        self.assertFalse(hasattr(TestClassSingleton, "get_instance"))
-        self.assertFalse(hasattr(a, "get_instance"))
+        self.assertFalse(hasattr(TestClass, "reset"))
+        self.assertTrue(hasattr(TestClassSingleton, "reset"))  # The only one!
+        self.assertFalse(hasattr(a, "reset"))
 
-        # ---------------------------------------------------------------------
-        # Set: accessible = False
-        TestClass = TestSingleton.TestClass
-        # noinspection PyArgumentEqualDefault
-        TestClassSingleton = Singleton(TestClass, accessible=False)
+        b = TestClassSingleton(name="b")  # Singleton: b is a
+        self.assertEqual(repr(a), "TestClass('a', None, 'any stuff')")
+        self.assertEqual(repr(b), "TestClass('a', None, 'any stuff')")
+        self.assertEqual(a, b)
+        self.assertIs(a, b)
 
-        # Instances
-        a = TestClassSingleton(name="a")  # New single object a (default)
+        TestClassSingleton.reset()
 
-        # Tests
-        self.assertFalse(hasattr(TestClass, "get_instance"))
-        self.assertFalse(hasattr(TestClassSingleton, "get_instance"))
-        self.assertFalse(hasattr(a, "get_instance"))
+        c = TestClassSingleton(name="c")  # New single object c (default)
+        self.assertEqual(repr(a), "TestClass('a', None, 'any stuff')")
+        self.assertEqual(repr(c), "TestClass('c', None, 'any stuff')")
+        self.assertNotEqual(a, c)
+        self.assertIsNot(a, c)
+
+    def test_get_instance(self):
+        """Unittest: Decoration get_instance"""
 
-        # ---------------------------------------------------------------------
-        # Set: accessible = True
         TestClass = TestSingleton.TestClass
-        TestClassSingleton = Singleton(TestClass, accessible=True)
+        TestClassSingleton = Singleton(TestClass)
 
-        # Instances
+        # Instance
         a = TestClassSingleton(name="a")  # New single object a (default)
 
         # Tests
         self.assertFalse(hasattr(TestClass, "get_instance"))
         self.assertTrue(hasattr(TestClassSingleton, "get_instance"))  # This!
         self.assertFalse(hasattr(a, "get_instance"))
```

### Comparing `decoratory-0.1.3.11/Unittest/test_wrapper.py` & `decoratory-0.1.4.2/Unittest/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.3.11/setup.py` & `decoratory-0.1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.3.11"
-__date__ = "2023-06-19"
-__time__ = "18:30:22"
+__version__ = "0.1.4.2"
+__date__ = "2023-06-20"
+__time__ = "16:37:47"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
```

