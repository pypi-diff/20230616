# Comparing `tmp/translategram-0.2.0.tar.gz` & `tmp/translategram-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translategram-0.2.0.tar", last modified: Mon Jun 12 15:54:32 2023, max compression
+gzip compressed data, was "translategram-0.3.0.tar", last modified: Fri Jun 16 20:17:19 2023, max compression
```

## Comparing `translategram-0.2.0.tar` & `translategram-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:54:23.000000 translategram-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 15:54:23.000000 translategram-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-12 15:54:32.959290 translategram-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-12 15:54:23.000000 translategram-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/auto_translategram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/service_libs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/auto_translategram/translator_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-12 15:54:23.000000 translategram-0.2.0/auto_translategram/python_telegram_bot_translator/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:54:32.959290 translategram-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 15:54:23.000000 translategram-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:54:32.959290 translategram-0.2.0/translategram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 15:54:32.000000 translategram-0.2.0/translategram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:19.552291 translategram-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 20:17:03.000000 translategram-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 20:17:03.000000 translategram-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-16 20:17:19.552291 translategram-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-16 20:17:03.000000 translategram-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:17:19.552291 translategram-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 20:17:03.000000 translategram-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:19.552291 translategram-0.3.0/translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:19.552291 translategram-0.3.0/translategram/python_telegram_bot_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/python_telegram_bot_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/python_telegram_bot_translator/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:19.552291 translategram-0.3.0/translategram/translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/translategram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/translategram/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/translategram/service_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/translategram/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-16 20:17:03.000000 translategram-0.3.0/translategram/translategram/translator_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:17:19.552291 translategram-0.3.0/translategram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-16 20:17:19.000000 translategram-0.3.0/translategram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-16 20:17:19.000000 translategram-0.3.0/translategram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:17:19.000000 translategram-0.3.0/translategram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 20:17:19.000000 translategram-0.3.0/translategram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 20:17:19.000000 translategram-0.3.0/translategram.egg-info/top_level.txt
```

### Comparing `translategram-0.2.0/LICENSE` & `translategram-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `translategram-0.2.0/PKG-INFO` & `translategram-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.2.0
+Version: 0.3.0
 Summary: Translategram is a Python library for translating messages are sent by your Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Auto Translategram
+# Translategram
 
-Auto Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
+Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
 
 ## Installation
 
-You can install Auto Translategram using pip:
+You can install Translategram using pip:
 
 ```
 pip install translategram
 ```
 
 ## Usage
 
@@ -47,26 +47,26 @@
 ```python
 login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 ```
 
 ### And finally your file should looks like this:
 
 ```python
 import logging
 from telegram.ext import ApplicationBuilder, ContextTypes, CommandHandler
 from telegram import Update
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 TOKEN = 'YOUR_TOKEN'
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
@@ -100,17 +100,14 @@
     application.run_polling()
 
 ```
 
 ## TODO
 
 * Implement cache system
-    - Create abstract base class for different cache systems.
-    - Cache System with Pickling and serialization (e.g. JSON).
-        - The Pickle module in Python can be used to serialize dataclasses and store them on disk. This approach is simple and suitable for small to medium-sized projects.
     - Cache System with Memcache.
     - Cache System with Redis.
 * Add aiogram framework adapter.
 * Add pyTelegramBotApi framework adapter.
 * Add support for more translation services.
```

### Comparing `translategram-0.2.0/README.md` & `translategram-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Auto Translategram
+# Translategram
 
-Auto Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
+Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
 
 ## Installation
 
-You can install Auto Translategram using pip:
+You can install Translategram using pip:
 
 ```
 pip install translategram
 ```
 
 ## Usage
 
@@ -26,26 +26,26 @@
 ```python
 login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 ```
 
 ### And finally your file should looks like this:
 
 ```python
 import logging
 from telegram.ext import ApplicationBuilder, ContextTypes, CommandHandler
 from telegram import Update
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 TOKEN = 'YOUR_TOKEN'
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
@@ -79,17 +79,14 @@
     application.run_polling()
 
 ```
 
 ## TODO
 
 * Implement cache system
-    - Create abstract base class for different cache systems.
-    - Cache System with Pickling and serialization (e.g. JSON).
-        - The Pickle module in Python can be used to serialize dataclasses and store them on disk. This approach is simple and suitable for small to medium-sized projects.
     - Cache System with Memcache.
     - Cache System with Redis.
 * Add aiogram framework adapter.
 * Add pyTelegramBotApi framework adapter.
 * Add support for more translation services.
```

### Comparing `translategram-0.2.0/auto_translategram/auto_translategram/translator.py` & `translategram-0.3.0/translategram/translategram/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Coroutine, Type, TypeVar, Union
 
-from auto_translategram.auto_translategram.cache import Cache
-from auto_translategram.auto_translategram.translator_services import TranslatorService
+from translategram.translategram.cache import Cache
+from translategram.translategram.translator_services import TranslatorService
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Translator(ABC):
     """
     Abstract base class for implementing translation functionality in various frameworks.
     This class provides a uniform interface for translation, allowing adapters to be written for different frameworks.
     This class is meant to be subclassed, and the `handler_translator` method should be implemented in the subclass.
     """
-    def __init__(self, translator_service: TranslatorService, cache_system: Union[Type[Cache], None] = None) -> None:
+
+    def __init__(
+        self,
+        translator_service: TranslatorService,
+        cache_system: Union[Type[Cache], None] = None,
+    ) -> None:
         """
         Initializes a new Translator instance using the specified `translator_service`.
 
-        :param translator_service: The `BaseTranslatorService` to use for translations.
+        :param translator_service: The `TranslatorService` to use for translations.
+        :param cache_system: The cache system to be used for caching translations. If None, caching is disabled.
         """
         ...
 
     @abstractmethod
     def handler_translator(
-        self,
-        message: str
-    ) -> Callable[[Callable[..., T]], Callable[[Any, Any, str], Coroutine[Any, Any, Any]]]:
+        self, message: str
+    ) -> Callable[
+        [Callable[..., T]], Callable[[Any, Any, str], Coroutine[Any, Any, Any]]
+    ]:
         """
         Translate a message based on the users' language
         :param func: The handler function that is used for handling commands by Frameworks.
         :param message: The message to translate.
         """
         ...
```

### Comparing `translategram-0.2.0/auto_translategram/python_telegram_bot_translator/adapter.py` & `translategram-0.3.0/translategram/python_telegram_bot_translator/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,113 @@
 import inspect
 from typing import Any, Coroutine, Callable, Type, TypeVar, Union
 from telegram.ext import ContextTypes
 
 from telegram import Update
 
-from auto_translategram.auto_translategram.cache import Cache
-from auto_translategram.auto_translategram.translator_services import TranslatorService
-from auto_translategram.auto_translategram.translator import Translator
+from translategram.translategram.cache import Cache
+from translategram.translategram.translator_services import TranslatorService
+from translategram.translategram.translator import Translator
 
-_T = TypeVar('_T')
+_T = TypeVar("_T")
 
 
 class PythonTelegramBotAdapter(Translator):
     """
     A Translator adapter for the python-telegram-bot framework.
 
     Inherits from the abstract class `Translator` and implements its `handler_translator` method
     to provide translation functionality for the python-telegram-bot framework.
-
-    :param translator_service: The `TranslatorService` to use for translations.
     """
 
-    def __init__(self,
-                 translator_service: Type[TranslatorService],
-                 cache_system: Union[Type[Cache], None] = None
-                 ) -> None:
+    def __init__(
+        self,
+        translator_service: Type[TranslatorService],
+        cache_system: Union[Type[Cache], None] = None,
+    ) -> None:
         """
         Initializes a new PythonTelegramBotAdapter instance using the specified `translator_service`.
 
         :param translator_service: The `TranslatorService` to use for translations.
+        :param cache_system: The cache system to be used for caching translations. If None, caching is disabled.
         """
         self._translator_service = translator_service()
         self._cache_system = cache_system
 
     def handler_translator(
-            self,
-            message: str
-            ) -> Callable[[Callable[[Any, Any, str], _T]], Callable[[Any, Any, str], Coroutine[Any, Any, Any]]]:
+        self, message: str
+    ) -> Callable[
+        [Callable[[Any, Any, str], _T]],
+        Callable[[Any, Any, str], Coroutine[Any, Any, Any]],
+    ]:
         """
         A decorator that wraps a python-telegram-bot `handler` function to provide translation functionality.
 
         The decorated function will be executed after being wrapped with a new function that translates
         the incoming message into the user's preferred language (if it is not already in that language).
         If the user does not have a preferred language set or if it is set to 'en', the message will not be translated.
 
         :param func: The handler function that is used for handling commands by the Python-telegram-bot framework.
         :param message: The message to translate.
         :return: A coroutine that wraps the handler function and provides translation functionality.
         """
-        def decorator(func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], _T]) \
-                -> Callable[[Any, Any, str], Coroutine[Any, Any, Any]]:
 
-            async def wrapper(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str = message) -> Any:
-                user_lang = update.effective_user.language_code if update.effective_user else 'en'
+        def decorator(
+            func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], _T]
+        ) -> Callable[[Any, Any, str], Coroutine[Any, Any, Any]]:
+            """
+            Decorator function that provides translation functionality to a Python-telegram-bot `handler` function.
+
+            The decorated function will be executed after being wrapped with a new function that translates
+            the incoming message into the user's preferred language (if it is not already in that language).
+            If the user does not have a preferred language set or if it is set to 'en', the message will
+            not be translated. # TODO: please get rid of this!
+
+            :param func: The handler function that is used for handling commands by the Python-telegram-bot framework.
+            :param message: The message to translate.
+            :return: A coroutine that wraps the handler function and provides translation functionality.
+            """
+
+            async def wrapper(
+                update: Update,
+                context: ContextTypes.DEFAULT_TYPE,
+                message: str = message,
+            ) -> Any:
+                user_lang = (
+                    update.effective_user.language_code
+                    if update.effective_user
+                    else "en"
+                )
                 message = message
                 msg = message
-                if user_lang != 'en' and user_lang is not None:  # TODO: get rid of this!
+                if (
+                    user_lang != "en" and user_lang is not None
+                ):  # TODO: get rid of this!
                     if self._cache_system is not None:
                         msg = await self._cache_system.retrieve(
-                            key=func.__name__ + '_' + user_lang
-                            )  # type: ignore
+                            key=func.__name__ + "_" + user_lang
+                        )  # type: ignore
                         if msg is None:
                             msg = await self._translator_service.translate_str(
                                 text=message,
                                 target_language=user_lang,
-                                source_language='en'
-                                )
+                                source_language="en",
+                            )
                             await self._cache_system.store(
-                                key=func.__name__ + '_' + user_lang, value=msg
-                                )  # type: ignore
+                                key=func.__name__ + "_" + user_lang, value=msg
+                            )  # type: ignore
                     else:
                         msg = await self._translator_service.translate_str(
                             text=message,
                             target_language=user_lang,
-                            source_language='en'
-                            )
+                            source_language="en",
+                        )
                 is_async = inspect.iscoroutinefunction(func)
                 if is_async:
                     result = await func(update, context, str(msg))  # type: ignore[misc]
                 else:
                     result = func(update, context, str(msg))  # type: ignore[misc]
                 return result
 
             return wrapper
+
         return decorator
```

### Comparing `translategram-0.2.0/setup.py` & `translategram-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r", encoding='utf-8') as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='translategram',
-    version='0.2.0',
-    description='Translategram is a Python library for translating messages are sent by your Bot in Telegram',
-    url='https://github.com/EkberHasanov/translategram',
-    author='Akbar',
-    author_email='hasanvakbar@gmail.com',
-    license='MIT',
+    name="translategram",
+    version="0.3.0",
+    description="Translategram is a Python library for translating messages are sent by your Bot in Telegram",
+    url="https://github.com/EkberHasanov/translategram",
+    author="Akbar",
+    author_email="hasanvakbar@gmail.com",
+    license="MIT",
     install_requires=[
-        'mtranslate',
+        "mtranslate",
     ],
     include_package_data=True,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests", "tests.*", "*.tests", "*.tests.*"]),
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `translategram-0.2.0/translategram.egg-info/PKG-INFO` & `translategram-0.3.0/translategram.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.2.0
+Version: 0.3.0
 Summary: Translategram is a Python library for translating messages are sent by your Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Auto Translategram
+# Translategram
 
-Auto Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
+Translategram is a Python package that provides translation capabilities for Telegram bots. It uses and supports multiple translation services.
 
 ## Installation
 
-You can install Auto Translategram using pip:
+You can install Translategram using pip:
 
 ```
 pip install translategram
 ```
 
 ## Usage
 
@@ -47,26 +47,26 @@
 ```python
 login_handler = CommandHandler('login', login)
 ```
 
 ### As well as you should create translator instance based on the framework you are using *(in this case python-telegram-bot)*.
 
 ```python
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 ```
 
 ### And finally your file should looks like this:
 
 ```python
 import logging
 from telegram.ext import ApplicationBuilder, ContextTypes, CommandHandler
 from telegram import Update
-from auto_translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
+from translategram import PythonTelegramBotTranslator, MtranslateTranslatorService
 
 translator = PythonTelegramBotTranslator(MtranslateTranslatorService)
 TOKEN = 'YOUR_TOKEN'
 logging.basicConfig(
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
     level=logging.INFO
 )
@@ -100,17 +100,14 @@
     application.run_polling()
 
 ```
 
 ## TODO
 
 * Implement cache system
-    - Create abstract base class for different cache systems.
-    - Cache System with Pickling and serialization (e.g. JSON).
-        - The Pickle module in Python can be used to serialize dataclasses and store them on disk. This approach is simple and suitable for small to medium-sized projects.
     - Cache System with Memcache.
     - Cache System with Redis.
 * Add aiogram framework adapter.
 * Add pyTelegramBotApi framework adapter.
 * Add support for more translation services.
```

