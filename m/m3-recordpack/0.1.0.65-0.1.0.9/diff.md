# Comparing `tmp/m3-recordpack-0.1.0.65.tar.gz` & `tmp/m3-recordpack-0.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3-recordpack-0.1.0.65.tar", last modified: Fri Jun 16 12:16:54 2023, max compression
+gzip compressed data, was "dist/m3-recordpack-0.1.0.9.tar", last modified: Thu Oct  2 08:15:16 2014, max compression
```

## Comparing `m3-recordpack-0.1.0.65.tar` & `m3-recordpack-0.1.0.9.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:16:54.520131 m3-recordpack-0.1.0.65/
--rw-r--r--   0 root         (0) root         (0)     3459 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/LICENSE
--rw-r--r--   0 root         (0) root         (0)      825 2023-06-16 12:16:54.519131 m3-recordpack-0.1.0.65/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-16 12:16:46.000000 m3-recordpack-0.1.0.65/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:16:54.501131 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      825 2023-06-16 12:16:54.000000 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-16 12:16:54.000000 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 12:16:54.000000 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-16 12:16:54.000000 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-16 12:16:54.000000 m3-recordpack-0.1.0.65/m3_recordpack.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:16:54.511131 m3-recordpack-0.1.0.65/recordpack/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-16 12:16:46.000000 m3-recordpack-0.1.0.65/recordpack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11278 2023-06-16 12:16:46.000000 m3-recordpack-0.1.0.65/recordpack/be.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 12:16:54.518131 m3-recordpack-0.1.0.65/recordpack/demo/
--rw-r--r--   0 root         (0) root         (0)      609 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1523 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/actions.py
--rw-r--r--   0 root         (0) root         (0)     1271 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     1346 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/column_filter.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/controller.py
--rw-r--r--   0 root         (0) root         (0)     1785 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/models.py
--rw-r--r--   0 root         (0) root         (0)      757 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5837 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/demo/ui.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/encoder.py
--rw-r--r--   0 root         (0) root         (0)     1893 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5650 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/helpers.py
--rw-r--r--   0 root         (0) root         (0)    35317 2022-12-23 11:37:23.000000 m3-recordpack-0.1.0.65/recordpack/provider.py
--rw-r--r--   0 root         (0) root         (0)     8954 2023-03-22 06:06:18.000000 m3-recordpack-0.1.0.65/recordpack/proxy.py
--rw-r--r--   0 root         (0) root         (0)    64515 2023-03-21 08:58:06.000000 m3-recordpack-0.1.0.65/recordpack/recordpack.py
--rw-r--r--   0 root         (0) root         (0)      594 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/results.py
--rw-r--r--   0 root         (0) root         (0)     2542 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/signals.py
--rw-r--r--   0 root         (0) root         (0)     3888 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/recordpack/typecast.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 12:16:54.520131 m3-recordpack-0.1.0.65/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1236 2022-08-29 06:33:09.000000 m3-recordpack-0.1.0.65/setup.py
+drwxr-xr-x   0 prefer     (501) staff       (20)        0 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/
+drwxr-xr-x   0 prefer     (501) staff       (20)        0 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/
+-rw-r--r--   0 prefer     (501) staff       (20)        1 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/dependency_links.txt
+-rw-r--r--   0 prefer     (501) staff       (20)      824 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/PKG-INFO
+-rw-r--r--   0 prefer     (501) staff       (20)       20 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/requires.txt
+-rw-r--r--   0 prefer     (501) staff       (20)      632 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/SOURCES.txt
+-rw-r--r--   0 prefer     (501) staff       (20)       11 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/m3_recordpack.egg-info/top_level.txt
+-rw-r--r--   0 prefer     (501) staff       (20)      824 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/PKG-INFO
+-rw-r--r--   0 prefer     (501) staff       (20)       41 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/README.rst
+drwxr-xr-x   0 prefer     (501) staff       (20)        0 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/recordpack/
+-rw-r--r--   0 prefer     (501) staff       (20)      146 2014-09-24 09:45:02.000000 m3-recordpack-0.1.0.9/recordpack/__init__.py
+-rw-r--r--   0 prefer     (501) staff       (20)    10665 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/be.py
+drwxr-xr-x   0 prefer     (501) staff       (20)        0 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/recordpack/demo/
+-rw-r--r--   0 prefer     (501) staff       (20)      570 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/__init__.py
+-rw-r--r--   0 prefer     (501) staff       (20)     1468 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/actions.py
+-rw-r--r--   0 prefer     (501) staff       (20)     1215 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/app_meta.py
+-rw-r--r--   0 prefer     (501) staff       (20)     1274 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/column_filter.py
+-rw-r--r--   0 prefer     (501) staff       (20)      458 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/controller.py
+-rw-r--r--   0 prefer     (501) staff       (20)     1726 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/models.py
+-rw-r--r--   0 prefer     (501) staff       (20)      685 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/proxy.py
+-rw-r--r--   0 prefer     (501) staff       (20)     5765 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/demo/ui.py
+-rw-r--r--   0 prefer     (501) staff       (20)     1177 2014-09-24 09:45:02.000000 m3-recordpack-0.1.0.9/recordpack/exceptions.py
+-rw-r--r--   0 prefer     (501) staff       (20)     4326 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/helpers.py
+-rw-r--r--   0 prefer     (501) staff       (20)    25302 2014-09-24 09:45:02.000000 m3-recordpack-0.1.0.9/recordpack/provider.py
+-rw-r--r--   0 prefer     (501) staff       (20)     7526 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/proxy.py
+-rw-r--r--   0 prefer     (501) staff       (20)    56450 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/recordpack.py
+-rw-r--r--   0 prefer     (501) staff       (20)     2502 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/signals.py
+-rw-r--r--   0 prefer     (501) staff       (20)     3761 2014-09-24 09:40:41.000000 m3-recordpack-0.1.0.9/recordpack/typecast.py
+-rw-r--r--   0 prefer     (501) staff       (20)       59 2014-10-02 08:15:16.000000 m3-recordpack-0.1.0.9/setup.cfg
+-rw-r--r--   0 prefer     (501) staff       (20)     1212 2014-10-02 08:13:52.000000 m3-recordpack-0.1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `m3-recordpack-0.1.0.65/PKG-INFO` & `m3-recordpack-0.1.0.9/m3_recordpack.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: m3-recordpack
-Version: 0.1.0.65
+Version: 0.1.0.9
 Summary: Пак общего назначения, для формирования и управления журнальными окнами и окнами справочников
-Author: Bars Group
-Author-email: bars@bars-open.ru
-Maintainer: Torsunov Andrey
-Maintainer-email: torsunov@bars-open.ru
+Home-page: UNKNOWN
+Author: Torsunov Andrey
+Author-email: torsunov@bars-open.ru
 License: MIT
+Description: Recordpack
+        ==========
+        
+        :version: 0.1.0.0
+        
 Keywords: django m3
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-License-File: LICENSE
-
-Recordpack
-==========
-
-:version: 0.1.0.65
```

### Comparing `m3-recordpack-0.1.0.65/m3_recordpack.egg-info/PKG-INFO` & `m3-recordpack-0.1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: m3-recordpack
-Version: 0.1.0.65
+Version: 0.1.0.9
 Summary: Пак общего назначения, для формирования и управления журнальными окнами и окнами справочников
-Author: Bars Group
-Author-email: bars@bars-open.ru
-Maintainer: Torsunov Andrey
-Maintainer-email: torsunov@bars-open.ru
+Home-page: UNKNOWN
+Author: Torsunov Andrey
+Author-email: torsunov@bars-open.ru
 License: MIT
+Description: Recordpack
+        ==========
+        
+        :version: 0.1.0.0
+        
 Keywords: django m3
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-License-File: LICENSE
-
-Recordpack
-==========
-
-:version: 0.1.0.65
```

### Comparing `m3-recordpack-0.1.0.65/m3_recordpack.egg-info/SOURCES.txt` & `m3-recordpack-0.1.0.9/m3_recordpack.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-LICENSE
 README.rst
+setup.cfg
 setup.py
 m3_recordpack.egg-info/PKG-INFO
 m3_recordpack.egg-info/SOURCES.txt
 m3_recordpack.egg-info/dependency_links.txt
 m3_recordpack.egg-info/requires.txt
 m3_recordpack.egg-info/top_level.txt
 recordpack/__init__.py
 recordpack/be.py
-recordpack/encoder.py
 recordpack/exceptions.py
 recordpack/helpers.py
 recordpack/provider.py
 recordpack/proxy.py
 recordpack/recordpack.py
-recordpack/results.py
 recordpack/signals.py
 recordpack/typecast.py
 recordpack/demo/__init__.py
 recordpack/demo/actions.py
 recordpack/demo/app_meta.py
 recordpack/demo/column_filter.py
 recordpack/demo/controller.py
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/be.py` & `m3-recordpack-0.1.0.9/recordpack/be.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-from __future__ import (
-    absolute_import,
-)
+# coding: utf-8
 
-import six
+#------------------------------------------------------------------------------
+# Imports
+#------------------------------------------------------------------------------
+
+# Stdlib
+import string
 import operator
+from collections import Iterable
 
-from collections import (
-    Iterable,
-)
-
-from django.db.models import (
-    Q,
-)
-from django.utils.functional import (
-    LazyObject,
-)
+# 3rdparty
+from django.db.models import Q
 
+#------------------------------------------------------------------------------
 # Metadata
+#------------------------------------------------------------------------------
+
+__author__ = 'Andrey Torsunov'
+__contact__ = 'torsunov@bars-open.ru'
 __docformat__ = 'restructuredtext'
-__all__ = ['BooleanExpression', 'BE', 'expression_to_q', 'expression_to_bool', 'get_empty_filter_expression']
+
+__all__ = ['BooleanExpression', 'BE', 'expression_to_q', 'expression_to_bool']
 
 
+#------------------------------------------------------------------------------
+# Boolean expression class
+#------------------------------------------------------------------------------
+
 class BooleanExpression(object):
-    """Логическое выражение (для построения фильтров)."""
+    u""" Логическое выражение (для построения фильтров). """
 
     # Операторы сравнения
     AND = 'and'
     OR = 'or'
     NOT = 'not'
     EQ = 'eq'
     NE = 'neq'
     LT = 'lt'
     LE = 'lte'
     GT = 'gt'
     GE = 'gte'
     IC = 'icontains'
-    CT = 'contains'
-    OL = 'overlap'
     IN = 'in'
-    RE = 'regex'
 
     def __init__(self, left, operator=None, right=None):
-        """Инициализация выражения.
+        u""" Инициализация выражения.
 
-        Args:
-            left: Левый операнд.
-            operator: Необязательный; Оператор на операндами.
-            right: Необязательный; Правый операнд.
+        :param left: левый операнд
+        :param operator: оператор на операндами
+        :param right: правый операнд
 
         """
-
         self.left = left
         self.right = right
         self.operator = operator
 
     def __unicode__(self):
-        return f'{self.left} {self.operator} {self.right}'
+        return u'{left} {oper} {right}'.format(
+            left=self.left,
+            oper=self.operator,
+            right=self.right)
 
     def __str__(self):
-        return f'{self.left} {self.operator} {self.right}'
+        return '{left} {oper} {right}'.format(
+            left=self.left,
+            oper=self.operator,
+            right=self.right)
 
     # object & other
     def __and__(self, other):
         if isinstance(other, self.__class__):
             return self.__class__(self, self.AND, other)
         elif other is None:
             return self
@@ -92,70 +99,51 @@
     # other | object
     __ror__ = __or__
 
     def __invert__(self):
         return self.__class__(self, self.NOT)
 
     def find_value(self, value, in_left=True, in_right=False):
-        """Поиск выражения.
+        u""" Поиск выражения.
 
         Поиск выражения, в котором встречается *value*. Параметры *in_left*
         и *in_right* указывают где искать, в каких частях выражения.
 
-        Returns:
-            Если выражение найдено, то оно возвращается (первое
+        :return: Если выражение найдено, то оно возвращается (первое
             найденное), иначе возвращается :const:`None`.
-        """
 
+        """
         expr = None
         if in_left and self.left == value:
             expr = self
         if not expr and in_right and self.right == value:
             expr = self
         if not expr and isinstance(self.left, self.__class__):
             expr = self.left.find_value(value, in_left, in_right)
         if not expr and isinstance(self.right, self.__class__):
             expr = self.right.find_value(value, in_left, in_right)
         return expr
 
-    def iter_nodes(self, left=False, right=False):
-        """
-        Итератор по листовым значениям. Параметры left и right
-        ограничивают, какие части выражения нужно выдавать.
-        """
-
-        if isinstance(self.left, self.__class__):
-            yield from self.left.iter_nodes(left, right)
-        elif left:
-            yield self.left
-
-        if isinstance(self.right, self.__class__):
-            yield from self.right.iter_nodes(left, right)
-        elif right:
-            yield self.right
-
     def remove(self, expression):
-        """
+        u"""
         Удаление вложенного выражения из текущего выражения.
         Оставшееся выражение заменяет родительское
         """
-
         parent_expr = self.__find_nested(expression)
         if parent_expr is not None:
             if parent_expr.left == expression:
                 new_parent_expression = parent_expr.right
             else:
                 new_parent_expression = parent_expr.left
             parent_expr.right = new_parent_expression.right
             parent_expr.operator = new_parent_expression.operator
             parent_expr.left = new_parent_expression.left
 
     def replace(self, expression, to_expression):
-        """Замена вложенного выражения на новое."""
-
+        u""" Замена вложенного выражения на новое. """
         parent_expr = self.__find_nested(expression)
         if parent_expr is not None:
             # если найденное выражение находится слева
             if parent_expr.left == expression:
                 parent_expr.left = to_expression
             else:
                 parent_expr.right = to_expression
@@ -163,59 +151,59 @@
     def to_bool(self, *a, **kw):
         return expression_to_bool(self, *a, **kw)
 
     def to_q(self, *a, **kw):
         return expression_to_q(self, *a, **kw)
 
     def __find_nested(self, expression):
-        """Поиск вложенного выражения.
+        u""" Поиск вложенного выражения.
 
         Ищется вложенное выражение (первое вхождение) и возвращается
         родительское выражение, в которое оно входит.
 
-        Returns:
-            Если не нашлось, или текущее выражение совпадает с
+        :return: Если не нашлось, или текущее выражение совпадает с
             искомым, то возвращается :const:`None`.
-        """
 
+        """
         result = None
         if expression == self:
             result = None
         elif isinstance(self.left, self.__class__) and expression == self.left:
             result = self
         elif isinstance(self.right, self.__class__) and expression == self.right:
             result = self
         if not result and isinstance(self.left, self.__class__):
             result = self.left.__find_nested(expression)
         if not result and isinstance(self.right, self.__class__):
             result = self.right.__find_nested(expression)
-
         return result
 
 
 BE = BooleanExpression
 
 
-def expression_to_q(boolexp):
-    """Преобразователь логического выражения в Q-объекты django."""
+#------------------------------------------------------------------------------
+# Boolean expression conversion
+#------------------------------------------------------------------------------
 
+def expression_to_q(boolexp):
+    """
+    Преобразователь логического выражения в Q-объекты django
+    """
     operators = {
         BE.AND: operator.and_,
         BE.OR: operator.or_,
         BE.LE: '__lte',
         BE.LT: '__lt',
         BE.GE: '__gte',
         BE.GT: '__gt',
         BE.EQ: '',
         BE.NE: '',
         BE.IN: '__in',
-        BE.IC: '__icontains',
-        BE.CT: '__contains',
-        BE.OL: '__overlap',
-        BE.RE: '__regex'
+        BE.IC: '__icontains'
     }
 
     operator_const = boolexp.operator
     negation = operator_const == BE.NE
 
     # Инициализация левого и правого операндов.
     left = _init_operand_q(boolexp.left)
@@ -229,37 +217,40 @@
     # меняется на :attr:`BE.IN`.
     operator_const = _eq2in(right, operator_const)
 
     if operator_const in operators:
         operator_postfix = operators[operator_const]
         if callable(operator_postfix):
             expr = operator_postfix(left, right)
-        elif isinstance(operator_postfix, six.string_types):
+        elif isinstance(operator_postfix, basestring):
             expr = Q((left + operator_postfix, right))
 
     elif expr is None:
-        raise ValueError(f"Handler for operator '{operator_const}' not exist.")
+        raise ValueError((
+            "Handler for operator '{operator}' not exist."
+        ).format(
+            operator=operator_const
+        ))
 
     return ~expr if negation else expr
 
 
 def expression_to_bool(boolexp, left_callback=None, right_callback=None):
-    """Преобразователь логического выражения в логическое значение."""
+    u""" Преобразователь логического выражения в логическое значение. """
 
     operators = {
         BE.AND: operator.and_,
         BE.OR: operator.or_,
         BE.LE: operator.le,
         BE.LT: operator.lt,
         BE.GE: operator.ge,
         BE.GT: operator.gt,
         BE.EQ: operator.eq,
         BE.NE: operator.ne,
-        BE.IN: lambda *a: operator.contains(*a[::-1]),
-        BE.OL: lambda a, b: bool(set(a) & set(b)),
+        BE.IN: lambda *a: operator.contains(*a[::-1])
     }
 
     operator_const = boolexp.operator
 
     # Инициализация левого и правого операндов.
     callbacks = (left_callback, right_callback)
     left = _init_operand(boolexp.left, left_callback, callbacks)
@@ -270,75 +261,54 @@
     expr = _neg_left(operator_const, left, boolexp.right)
 
     # Если правый операнд содержит перечисление, то оператор
     # меняется на :attr:`BE.IN`.
     operator_const = _eq2in(right, operator_const)
 
     if operator_const == BE.IC:
-        operator_callable = operators[BE.IN]
-        expr = operator_callable(six.text_type(right).upper(),
-                                 six.text_type(left).upper())
+        expr = string.find(string.upper(left), string.upper(right)) >= 0
 
     elif operator_const in operators:
         operator_callable = operators[operator_const]
         expr = operator_callable(left, right)
 
     elif expr is None:
-        raise ValueError(f"Handler for operator '{operator_const}' not exist.")
+        raise ValueError((
+            "Handler for operator '{operator}' not exist."
+        ).format(
+            operator=operator_const
+        ))
 
     return expr
 
 
 def _init_operand_q(value):
     if isinstance(value, BE):
         operand = expression_to_q(value)
     else:
         operand = value
-
     return operand
 
 
 def _init_operand(value, mutator, callbacks):
     if isinstance(value, BE):
         operand = expression_to_bool(value, *callbacks)
     else:
         operand = mutator(value) if mutator and mutator(value) else value
-
     return '' if operand is None else operand
 
 
 def _eq2in(right_operand, operator_const):
     if (
         isinstance(right_operand, Iterable) and
-        not isinstance(right_operand, LazyObject) and
-        not isinstance(right_operand, six.string_types) and
+        not isinstance(right_operand, basestring) and
         operator_const in (BE.EQ, BE.NE)
     ):
         operator_const = BE.IN
-
     return operator_const
 
 
 def _neg_left(operator_const, left_operand, right_operand):
     expr = None
     if right_operand is None:
         expr = ~left_operand if operator_const == BE.NOT else left_operand
-
     return expr
-
-
-def get_empty_filter_expression(attr):
-    """Возвращает выражение для фильтрации.
-
-    Возвращает выражение для фильтрации, если значение для фильтрации не пустое.
-
-    Args:
-        attr: Атрибут, по которому проходит фильтрация.
-
-    Returns:
-        Boolean expression или None.
-    """
-
-    def expression(value):
-        return BE(attr, BE.IN, value) if list(filter(None, value)) else None
-
-    return expression
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/__init__.py` & `m3-recordpack-0.1.0.9/recordpack/demo/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,11 +5,10 @@
 
 #: Патчинг m3_ext
 #: --------------
 #:
 #: В связи с тем, что в m3_blank.urls нет очевидной возможности
 #: расширить workspace, патчится workspace с указанием необходимого
 #: шаблона, для обеспечения работы "из коробки".
-from __future__ import absolute_import
 import functools
 import m3_ext
 m3_ext.workspace = functools.partial(m3_ext.workspace, template='demo_workspace.html')
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/actions.py` & `m3-recordpack-0.1.0.9/recordpack/demo/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
-from __future__ import absolute_import
 import datetime
 
 # Recordpack
 from recordpack import recordpack
 from recordpack.provider import DjangoProxyProvider
 from recordpack.be import BE
 from recordpack.typecast import cast_to_date
 
 # Demo
-from . import ui
-from . import column_filter
-from .proxy import PersonListProxy
-from .models import Person
+import ui
+import column_filter
+from proxy import PersonListProxy
+from models import Person
 
 #------------------------------------------------------------------------------
 # Demonstrative action packs
 #------------------------------------------------------------------------------
 
 class PersonPack(recordpack.BaseRecordListPack):
     u"""
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/app_meta.py` & `m3-recordpack-0.1.0.9/recordpack/demo/app_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # 3rdparty
-from __future__ import absolute_import
 from django.conf import urls
-from django.conf.urls import url
-
 from m3_ext.ui import app_ui
 from m3.actions import ControllerCache
 
 # Demo
-from . import actions
-from . import controller
+import actions
+import controller
 
 #------------------------------------------------------------------------------
 # Action packs registration
 #------------------------------------------------------------------------------
 
 def register_urlpatterns():
-    return (
-        url('^', controller.action_controller.process_request),
+    return urls.defaults.patterns(
+        '',
+        ('^', controller.action_controller.process_request),
     )
 
 
 def register_actions():
     controller.action_controller.extend_packs([
         actions.PersonPack(),
     ])
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/column_filter.py` & `m3-recordpack-0.1.0.9/recordpack/demo/column_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
-from __future__ import absolute_import
 import datetime
 
 # 3rdparty
 from django.db import models
 
 # Recordpack
-from m3_django_compat import get_model
-
 from recordpack.be import BE
 from recordpack.typecast import mute_typecast
 
 
 #------------------------------------------------------------------------------
 # Helpers functions
 #------------------------------------------------------------------------------
@@ -36,12 +33,12 @@
             date_string = date_string.lstrip(oper_code)
             birthday = mute_typecast(date_string, datetime.date)
             return birthday and BE('birthday', oper, birthday) or None
 
 
 def person_gender(gender_string):
     _filter = None
-    person_model = get_model('demo', 'Person')
+    person_model = models.get_model('demo', 'Person')
     for index, gender in person_model.GENDERS_LIST:
         if gender_string in gender:
             _filter |= BE('gender', BE.EQ, index)
     return _filter
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/models.py` & `m3-recordpack-0.1.0.9/recordpack/demo/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,45 @@
 Модели приложения
 """
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
-from __future__ import absolute_import
 import json
 
 # 3rdparty
 from django.db import models
-import six
 
 #------------------------------------------------------------------------------
 # Models
 #------------------------------------------------------------------------------
 
 class Person(models.Model):
     u"""
     Физическое лицо (человек)
     """
 
     GENDERS = {
         0: u'муж.',
         1: u'жен',
     }
-    GENDERS_LIST = list(GENDERS.items())
+    GENDERS_LIST = GENDERS.items()
 
     fname = models.CharField(
         u'Имя', max_length=255)
     sname = models.CharField(
         u'Фамилия', max_length=255)
     mname = models.CharField(
         u'Отчество', max_length=255)
     birthday = models.DateField(
         u'День рождения', null=True)
     gender = models.SmallIntegerField(
         u'Пол',
-        choices=six.iteritems(GENDERS),
+        choices=GENDERS.iteritems(),
         default=0)
     
 
     # Properties
     # -----------------------------------------------------------------
     
     @property
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/proxy.py` & `m3-recordpack-0.1.0.9/recordpack/demo/proxy.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 """
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # 3rdparty
-from __future__ import absolute_import
 from django.db import models
 
 # Recordpack
-from m3_django_compat import get_model
-
 from recordpack.provider import BaseProxy
 
 #------------------------------------------------------------------------------
 # Proxies
 #------------------------------------------------------------------------------
 
 class PersonListProxy(BaseProxy):
     def load(self, root):
-        person_model = get_model('demo', 'Person')
+        person_model = models.get_model('demo', 'Person')
         self.from_root()
         self.gender = person_model.GENDERS[self.gender]
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/demo/ui.py` & `m3-recordpack-0.1.0.9/recordpack/demo/ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 Пользовательский интерфейс (окошки).
 """
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # 3rdparty
-from __future__ import absolute_import
 from django.db import models
-from m3_django_compat import get_model
-
 from m3_ext.ui.windows.edit_window import ExtEditWindow
 from m3_ext.ui.controls.buttons import ExtButton
 from m3_ext.ui.containers.containers import ExtToolBar
 from m3_ext.ui.windows.window import ExtWindow
 from m3_ext.ui.panels.grids import ExtMultiGroupinGrid
 from m3_ext.ui.containers.forms import ExtForm
 from m3_ext.ui.fields import simple as fields
@@ -107,15 +104,15 @@
         gender_field.value_field = 'id'
         gender_field.label = u'Пол'
         gender_field.name = 'gender'
         gender_field.anchor = '100%'
         gender_field.allow_blank = False
         gender_field.trigger_action = 'all'
 
-        person_model = get_model('demo', 'Person')
+        person_model = models.get_model('demo', 'Person')
         gender_field.set_store(
             stores.ExtDataStore(data=person_model.GENDERS_LIST))
 
         self.gender_field = gender_field
         self.form.items.append(gender_field)
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/helpers.py` & `m3-recordpack-0.1.0.9/recordpack/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
-from __future__ import absolute_import
-import six
-
 import collections
 
 # 3rdparty
 from m3.actions import Action
 
 #------------------------------------------------------------------------------
 # Metadata
@@ -22,25 +19,16 @@
 __docformat__ = 'restructuredtext'
 
 
 #------------------------------------------------------------------------------
 # Helper functions
 #------------------------------------------------------------------------------
 
-def make_action(
-    url,
-    run_method,
-    shortname='',
-    acd=None,
-    classname='SimpleAction',
-    bind_run=False,
-    bind_acd=False,
-    need_atomic=None,
-    category=None,
-):
+def make_action(url, run_method, shortname='', acd=None,
+                classname='SimpleAction', bind_run=False, bind_acd=False):
     u""" Конструктор Action'ов.
 
     Позволяет создать экшен без непосредственного объявления его класса.
     Пример:
 
     .. code-block:: python
 
@@ -71,22 +59,14 @@
         созданный экшн, по-умолчанию: `SimpleAction`.
     :param bind_run: (не обязательно) флаг, указывающий на необходимость
         передачи методу в `run_method` ссылки на сам экшн (self),
         по-умолчанию: :const:`False`.
     :param bind_acd: (не обязательно) флаг, указывающий на необходимость
         передачи методу в `acd` ссылки на сам экшн (self),
         по-умолчанию: :const:`False`.
-    :param need_atomic: (не обязательно) флаг, указывающий на необходимость
-        установки такого флага на экшене - для внешнего оборачивания в atomic,
-        по-умолчанию: :const:`None`.
-    :param category: (не обязательно) строка, категория поведения экшена,
-        например, можно указать 'readonly'.
-        эта категория может использоваться для разделения экшенов на "читающие"
-        и "пишущие", чтобы роутить запросы к разным БД.
-        по-умолчанию: :const:`None`.
 
     :return: Дочерний класс от :class:`Action`
     :rtype: class
 
     """
     # Генерация класса экшена
     cls = type(classname, (Action,), dict(
@@ -94,18 +74,14 @@
         shortname=shortname
     ))
     action = cls()
     # Привязка функций реализующих логику экшена
     action.run = bind_run and run_method.__get__(action) or run_method
     if acd is not None:
         action.context_declaration = bind_acd and acd.__get__(action) or acd
-    if need_atomic is not None:
-        action.need_atomic = need_atomic
-    if category is not None:
-        action.category = category
     return action
 
 
 def init_component(instance, **kwargs):
     u""" Инициализация атрибутов экземпляра.
 
     Используется для удобной инициализации атрибутов через конструктор
@@ -126,28 +102,16 @@
         Если передан None, то вернется пустой кортеж.
 
     :param item:
 
     :rtype tuple:
 
     """
-    if isinstance(item, six.string_types):
+    if isinstance(item, basestring):
         seq = (item,)
     elif item is None:
         seq = ()
     elif isinstance(item, collections.Iterable):
         seq = tuple(item)
     else:
         seq = (item,)
-    return seq
-
-
-class AttributedDict(dict):
-    """Словарь, позволяющий обращаться к своим элементам
-    как к атрибутам объекта.
-
-    """
-    def __getattr__(self, name):
-        return self[name]
-
-    def __setattr__(self, key, value):
-        self[key] = value
+    return seq
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/provider.py` & `m3-recordpack-0.1.0.9/recordpack/provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
-from __future__ import absolute_import
-import six
-import warnings
-
-from abc import (
-    ABCMeta,
-    abstractmethod,
-)
+from abc import ABCMeta, abstractmethod
+from itertools import imap, ifilter
 from operator import itemgetter
-from six.moves import (
-    map,
-    filter,
-)
 
 # 3rdparty
-from django.db.models import (
-    Count,
-    Sum,
-)
-from django.db.models.constants import LOOKUP_SEP
+from m3.actions import OperationResult
+from django.db.models import Count, Sum
+from django.utils.translation import ugettext as _
+from m3.db import ObjectState
 
 # Recordpack
-from . import signals
 from .be import BE
-from .exceptions import (
-    ObjectDoesNotExists,
-    MultipleObjects,
-)
-from .helpers import (
-    init_component,
-    AttributedDict,
-)
+from .exceptions import (ObjectDoesNotExists, MultipleObjects)
+from .helpers import init_component
+from .proxy import BaseProxy
+from . import signals
 
 #------------------------------------------------------------------------------
 # Metadata
 #------------------------------------------------------------------------------
 
 __author__ = 'Andrey Torsunov'
 __contact__ = 'torsunov@bars-open.com'
@@ -49,21 +33,14 @@
 #------------------------------------------------------------------------------
 # Constants
 #------------------------------------------------------------------------------
 
 SORT_ASC = 'ASC'
 SORT_DESC = 'DESC'
 
-# представление для полей выбора из справочника
-FIELD_VIEW = 'field'
-# представление для карточки
-CARD_VIEW = 'card'
-# представление для списка
-LIST_VIEW = 'list'
-
 
 #------------------------------------------------------------------------------
 # Provider classes
 #------------------------------------------------------------------------------
 
 class QueryObject(object):
     u""" Унифицированный интерфейс запросов.
@@ -92,72 +69,31 @@
         #: :class:`~django.db.models.Manager` или кастомный
         self.from_all = False
 
         #: Порядок сортировки: 
         #: `['field_a', '-field_b', 'field_c', ..]`
         self.sorting = []
 
-        self.select_related = []
-
-        self.prefetch_related = []
-
-        # Список only-полей для queryset.only()
-        self.only = []
-
-        # Список наименований полей, значения для которых требуется получить.
-        # Использует QuerySet.values()
-        self.values = []
+        #: Cвязанные объекты (будут добавлены как select_related)
+        self.related = []
 
         #: Описание итогов в формате:
         #: `{'field': 'aggregate_operation', ..}`
         self.totals = {}
 
         #: Контекст выполнения (:class:`~m3.actions.context.ActionContext`),
         #: будет передан всем прокси-объектам
         self.context = None
 
-        # Запрашиваемое представление
-        # может использоваться для подстановки proxy
-        self.view = None
-
-        # Признак выполнения distinct в запросе данных
-        # (накладывает дополнительную нагрузку на сервер БД)
-        # но иногда без него никак
-        self.distinct = False
-
         init_component(self, **kwargs)
 
-        # Удалить, когда будет удалено свойство related
-        self.select_related = self.select_related or kwargs.get('related', [])
 
-    # Удалить, когда будет удален параметр related при использовании объектов
-    # класса
-    @property
-    def related(self):
-        warnings.warn(
-            '`related` is deprecated. '
-            'Use `select_related` instead.',
-            DeprecationWarning)
-
-        return self.select_related
-
-    # Удалить, когда будет удален параметр related при использовании объектов
-    # класса
-    @related.setter
-    def related(self, related):
-        warnings.warn(
-            '`related` is deprecated. '
-            'Use `select_related` instead.',
-            DeprecationWarning)
-
-        self.select_related = related
-
-
-class BaseRecordProvider(six.with_metaclass(ABCMeta, object)):
+class BaseRecordProvider(object):
     u""" Базовый абстрактный класс провайдера данных. """
+    __metaclass__ = ABCMeta
 
     def __init__(self, **kwargs):
         #: Источник данных
         self.data_source = None
         init_component(self, **kwargs)
 
     @abstractmethod
@@ -184,62 +120,33 @@
     def delete_record(self, obj):
         u""" Удаление записи. """
 
 
 class DjangoModelProvider(BaseRecordProvider):
     u""" Базовый провайдер для моделей Django. """
     
-    def __init__(
-        self,
-        data_source,
-        key_field='id',
-        related=(),
-        select_related=None,
-        prefetch_related=None
-    ):
-        """
-        Инициализация провайдера моделей
-
-        :param data_source: модель-источник данных
-        :param key_field: имя поля первичного ключа
-        :param related: deprecated список полей внешних ключей для
-            select_related. Устаревший вариант, в дальнейшем будет удален.
-            Взамен использовать select_related.
-        :param select_related: список полей внешних ключей на связанные таблицы
-        :param prefetch_related: список обратных внешних ключей на связанные
-            таблицы.
-        """
+    def __init__(self, data_source, key_field='id', related=None):
         super(DjangoModelProvider, self).__init__()
         
         #: Источник данных.
         self.data_source = data_source
         
         #: Поле модели в :attr:`data_source`, которое является 
         #: первичным ключом.
         self.key_field = key_field
-
-        self.select_related = select_related or related
-        self.prefetch_related = prefetch_related
+        
+        #: Связные модели, логика та что и у :meth:`QuerySet.select_related`
+        self.related = related
         
         #: Агрегаторы данных для итоговой строки
         self.aggregators = {
             'sum': _aggregate_sum,
             'count': _aggregate_count,
         }
 
-    # Удалить после отказа от related в кодовой базе
-    @property
-    def related(self):
-        return self.select_related
-
-    # Удалить после отказа от related в кодовой базе
-    @related.setter
-    def related(self, related):
-        self.select_related = related
-
     def _create_filter_conditions(self, filter_):
         u""" Получение фильтра для модели по переданному выражению
         фильтра (BE).
         """
         filters = filter_.to_q() if isinstance(filter_, BE) else None
         return filters
 
@@ -292,293 +199,150 @@
             не найдена запись.
         :raises MultipleObjects: если по указанному ключу найдено
             более одной записи.
 
         """
         query_object = query_object if query_object else QueryObject()
         try:
-            manager = self.get_manager(query_object)
-            base_query = self.get_base_query(manager)
-
-            select_related = self._get_select_related_fields(
-                query_object=query_object,
-            )
-            if select_related:
-                base_query = base_query.select_related(*self.select_related)
-
-            prefetch_related = self._get_prefetch_related_fields(
-                query_object=query_object,
-            )
-            if prefetch_related:
-                base_query = base_query.prefetch_related(*self.prefetch_related)
-
-            record = base_query.get((self.key_field, key))
+            record = self.get_manager(query_object).get((self.key_field, key))
         except self.data_source.DoesNotExist:
-            raise ObjectDoesNotExists(
-                source=self.data_source,
-                field=self.key_field,
-                key=key
-            )
+            raise ObjectDoesNotExists
         except self.data_source.MultipleObjectsReturned:
-            raise MultipleObjects(
-                source=self.data_source,
-                field=self.key_field,
-                key=key
-            )
-        else:
-            return record
+            raise MultipleObjects
+
+        return record
 
     def _preprocess_record(self, obj, context=None):
         u"""
         Функция позволяет переопределить или дополнить объект,
         который является результатом работы :meth:`get_records`.
         """
         return obj
 
-    def _pre_process_records(self, data, context=None):
-        u"""
-        Функция позволяет переопределить или дополнить объекты,
-        которые являетсю результатом работы :meth:`get_records`.
-        """
-        return [self._preprocess_record(obj, context) for obj in data]
-
     def before_query(self, query_object, query):
         return query
 
-    def after_query(self, query_object, data):
-        return data
-
-    def get_data_source(self, query_object):
-        """Получение источника данных."""
-
-        return self.data_source
-
     def get_manager(self, query_object):
         u""" Получение менеджера модели.
         
         :param query_object:
         :type query_object: :class:`QueryObject`
 
         :return: менеджер модели
         :rtype: :class:`~django.db.models.manager.Manager`
 
         """
-
-        data_source = self.get_data_source(query_object)
-
         # иногда query_object может быть None
-        if (
-            getattr(query_object, 'from_all', None) and
-            hasattr(data_source, 'objects_all')
-        ):
-            model_manager = data_source.objects_all
+        if getattr(query_object, 'from_all', None) \
+                and hasattr(self.data_source, 'objects_all'):
+            model_manager = self.data_source.objects_all
         else:
-            model_manager = data_source.objects
+            model_manager = self.data_source.objects
 
         # [(receiver, result), ...]
         receivers_results = signals.provider_get_manager.send(
             sender=self,
             query_object=query_object,
             manager=model_manager)
 
         # Фильтрация по второму элементу, если есть хотябы один не None,
         # то он и будет возвращен, в ином случае - значение по-умолчанию.
         extract_manager = itemgetter(1)
         model_manager = next(
-            filter(None, map(extract_manager, receivers_results)),
+            ifilter(None, imap(extract_manager, receivers_results)),
             model_manager)
 
         return model_manager
 
-    @staticmethod
-    def get_query_select_related_fields(data):
-        u"""
-        Метод получения представления связей для проброса в select_related.
-        """
-        result = []
-
-        if (
-            hasattr(data, 'query') and
-            getattr(data.query, 'select_related', None)
-        ):
-            def combine_relations(d, attr='', res=[]):
-                if not d:
-                    res.append(attr)
-
-                attr = attr and attr + LOOKUP_SEP or ''
-
-                for k, v in d.items():
-                    combine_relations(v, attr + k)
-
-                return res
-
-            result = combine_relations(getattr(data.query, 'select_related'))
-
-        return result
-
-    def _get_select_related_fields(self, data=None, query_object=None):
-        u""" Возвращает список атрибутов для добавления в select_related. """
-        all_related = set()
-
-        if query_object and query_object.select_related:
-            all_related.update(query_object.select_related)
-
-        if self.select_related:
-            all_related.update(self.select_related)
-
-        if data is not None:
-            all_related.update(
-                self.get_query_select_related_fields(data)
-            )
-
-        return all_related
-
-    # Удалить после внедрения select_related и prefetch_related
-    def _related_fields(self, *args, **kwargs):
-        return self._get_select_related_fields(*args, **kwargs)
-
-    def _get_prefetch_related_fields(self, data=None, query_object=None):
-        u"""
-        Возвращает список атрибутов для добавления в prefetch_related
-        """
-        all_related = set()
-
-        if self.prefetch_related:
-            all_related.update(self.prefetch_related)
-
-        if query_object and query_object.prefetch_related:
-            all_related.update(query_object.prefetch_related)
-
-        return all_related
-
-    def extend_prefetch(self, prefetch):
-        """
-        Расширяет список prefetch_related
-        Args:
-            prefetch: список с расширенными prefetch'ами
-        """
-        self.prefetch_related = list(self.prefetch_related)
-        self.prefetch_related.extend(prefetch)
-
-    def get_base_query(self, manager):
-        """Извлекает строки из менеджера.
-
-        Args:
-            manager: Экземпляр 'django.db.models.manager.Manager'.
-
-        Returns:
-            Возвращает QuerySet.
-        """
-
-        return manager.all()
-
     def get_records(self, query_object):
         u"""
         Получение записей, которые удовлетворяют условию из *query_object*.
         
         :param query_object:
         :type query_object: :class:`QueryObject`
         
         :rtype: :class:`dict`
 
         """
         assert isinstance(query_object, QueryObject)
-        manager = self.get_manager(query_object)
-        data = self.get_base_query(manager)
+        data = self.get_manager(query_object).all()
 
         # Фильтрация
         # -------------------------------------------------------------
         filter_ = self._create_filter_conditions(query_object.filter)
         if filter_:
             data = data.filter(filter_)
 
-        search_filter = self._create_filter_conditions(
-            query_object.quick_filter,
-        )
+        search_filter = self._create_filter_conditions(query_object.quick_filter)
         if search_filter:
             data = data.filter(search_filter)
 
         # Связанные записи
         # -------------------------------------------------------------
-        select_related = self._get_select_related_fields(data, query_object)
-        if select_related:
-            data = data.select_related(*select_related)
-
-        prefetch_related = self._get_prefetch_related_fields(
-            data,
-            query_object,
-        )
-        if prefetch_related:
-            data = data.prefetch_related(*prefetch_related)
+        all_related = self._related_fields(data, query_object)
+        if all_related:
+            data = data.select_related(*all_related)
 
         # Сортировка
         # -------------------------------------------------------------
         sorting = self._create_sort_conditions(query_object.sorting)
         if sorting:
             # иначе при сортировке одинаковых значений возвращает разный порядок
             sorting.append('id')
             data = data.order_by(*sorting)
 
         # Избавление от дубликатов,
         # которые могут появится при наличии множества JOIN'ов
-        if query_object.distinct:
-            data = data.distinct()
-
-        values = query_object.values
-        if values:
-            data = data.values(*values)
-
-        # добавим поддержку only
-        if query_object.only:
-            data = data.only(*query_object.only)
+        data = data.distinct()
 
         # Обработка запроса перед выборкой
         # -------------------------------------------------------------
         data = self.before_query(query_object, data)
 
         # Срез
         # -------------------------------------------------------------
+        total = data.count()
         if query_object.end:
-            begin = max(query_object.begin, 0)
-            end = query_object.end
-            res_data = data.all()[begin:end]
-
-            # Если после пагинации БД отдала количество записей меньшее, чем
-            # мы запросили, дополнительный count-запрос нам не потребуется,
-            # т.к. это значит, что мы запросили данные с последней "страницы".
-            # Но если БД отдала 0 записей, это не значит ничего, т.к. мы могли
-            # запросить записи с 100 по 125, а всего их 80. Исключение - если
-            # мы запрашиваем записи начиная с нулевой.
-            rows_on_page_expected = end - begin
-            rows_on_page_got = len(res_data)
-            if (0 < rows_on_page_got < rows_on_page_expected or
-                    begin == 0 and rows_on_page_got == 0):
-                total = begin + rows_on_page_got
-            else:
-                total = self.__get_total(data)
+            res_data = data.all()[query_object.begin:query_object.end]
         else:
             res_data = data.all()
-            total = self.__get_total(data)
-
-        # Обработка запроса после выборки
-        # -------------------------------------------------------------
-        res_data = self.after_query(query_object, res_data)
 
         context = query_object.context
-        result = self._pre_process_records(res_data, context)
+        result = [self._preprocess_record(obj, context) for obj in res_data]
 
         # Подсчет итоговой строки
         # -------------------------------------------------------------
         total_row = self.calc_total(query_object, data)
 
         if total_row:
             return {'rows': result, 'total': total, 'totalRow': total_row}
         else:
             return {'rows': result, 'total': total}
 
+    def _related_fields(self, data, query_object):
+        u""" Возвращает список атрибутов для добавления в select_related. """
+        all_related = set()
+
+        if query_object.related:
+            all_related.update(query_object.related)
+
+        if self.related:
+            all_related.update(self.related)
+
+        if hasattr(data, 'query') and data.query.select_related:
+            def fn(d, attr='', res=[]):
+                if not d:
+                    res.append(attr)
+                attr = attr and attr + '___' or ''
+                for k, v in d.items():
+                    fn(v, attr + k)
+                return res
+            all_related.update(fn(data.query.select_related))
+        return list(all_related)
+
     def validate(self, obj):
         pass
 
     def save(self, obj):
         u""" Сохранение записи.
 
         :param obj: экземпляр :attr:`data_source`
@@ -612,33 +376,19 @@
         for field, aggregation_name in query_object.totals.items():
             if aggregation_name in self.aggregators:
                 expr = self.aggregators[aggregation_name](field)
                 expressions[field] = expr
 
         if expressions:
             total = results.model.objects.filter(
-                pk__in=list(results.values_list('pk', flat=True))
+                pk__in=results.values_list('pk', flat=True)
             ).aggregate(**expressions)
 
         return total
 
-    @staticmethod
-    def __get_total(data):
-        """Общее количество записей. Через SQL count.
-        """
-        # Новая Django не любит когда в extra что-то есть, когда считает count
-        if data.query.extra_select:
-            c = data.extra(select={})
-            c.query.extra_select.clear()
-            total = c.count()
-        else:
-            total = data.count()
-
-        return total
-
 
 class DjangoProxyProvider(DjangoModelProvider):
     u""" Провайдер данных c использованием прокси-объектов.
 
     Кто-то называет их прокси, кто-то view-model pattern, не суть, 
     главное, что представление строится на основе модели Django.
     Подгрузку и расчет дополнительных данных берет на себя 2 вида прокси:
@@ -654,33 +404,29 @@
     """
 
     def __init__(self, card_proxy=None, list_proxy=None, *a, **k):
         super(DjangoProxyProvider, self).__init__(*a, **k)
         self.card_proxy = card_proxy
         self.list_proxy = list_proxy
 
-    def _proxy_factory(self, proxy_class, obj, context=None):
-        """
-        Позволяет переопределить построение прокси для класса.
-        """
-        proxy = proxy_class(root=obj, context=context)
-        proxy.load(obj)
-        return proxy
-
     def _proxy_card_factory(self, obj, context=None):
         u"""
         Позволяет переопределить построение прокси для формы.
         """
-        return self._proxy_factory(self.card_proxy, obj, context)
+        proxy = self.card_proxy(root=obj, context=context)
+        proxy.load(obj)
+        return proxy
 
     def _proxy_list_factory(self, obj, context=None):
         u"""
         Позволяет переопределить построение прокси для списка.
         """
-        return self._proxy_factory(self.list_proxy, obj, context)
+        proxy = self.list_proxy(root=obj, context=context)
+        proxy.load(obj)
+        return proxy
 
     def new_record(self, **kwargs):
         u"""
         Возвращает новый экземпляр прокси.
         """
         context = kwargs.pop('context', None)
         obj = super(DjangoProxyProvider, self).new_record(**kwargs)
@@ -689,45 +435,23 @@
         return obj
 
     def get_record(self, key, query_object=None):
         u"""
         Получает экземпляр прокси, построенный по модели Django.
         """
         obj = super(DjangoProxyProvider, self).get_record(key, query_object)
-        return self._create_proxy(obj, query_object)
-
-    def get_query_proxy_class(self, query_object=None):
-        proxy_class = None
-        if query_object and query_object.view:
-            if query_object.view == CARD_VIEW:
-                proxy_class = self.card_proxy
-            if query_object.view == LIST_VIEW:
-                proxy_class = self.list_proxy
-        return proxy_class
-
-    def _create_proxy(self, obj, query_object):
-        context = query_object.context if query_object else None
-        # попробуем подобрать прокси по запросу
-        proxy_class = self.get_query_proxy_class(query_object)
-        if proxy_class:
-            obj = self._proxy_factory(proxy_class, obj, context)
-        elif self.card_proxy is not None:
-            obj = self._proxy_card_factory(obj, context=context)
+        if self.card_proxy is not None:
+            context = query_object.context if query_object else None
+            return self._proxy_card_factory(obj, context=context)
         return obj
 
     def _preprocess_record(self, obj, context=None):
         u"""
         Переопределяет возвращаемый провайдером класс на прокси объект.
         """
-        if isinstance(obj, dict):
-            # Словарь получен путём использования qs.values().
-            # Для обратной совместимости, включаем возможность
-            # работы с элементами этого словаря как с атрибутами объекта.
-            obj = AttributedDict(obj)
-
         if self.list_proxy is not None:
             return self._proxy_list_factory(obj, context=context)
         return obj
 
     def validate(self, obj):
         u"""
         Проверка сначала в прокси, затем если все хорошо в провайдере.
@@ -898,15 +622,14 @@
 #------------------------------------------------------------------------------
 # Aggregators
 #------------------------------------------------------------------------------
 
 def _aggregate_sum(field_name):
     return Sum(field_name)
 
-
 def _aggregate_count(field_name):
     return Count(field_name)
 
 
 #------------------------------------------------------------------------------
 # Decorators
 #------------------------------------------------------------------------------
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/proxy.py` & `m3-recordpack-0.1.0.9/recordpack/proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,35 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
-from abc import (
-    ABCMeta,
-)
-from operator import (
-    attrgetter,
-)
-
-import six
-from django.db.models import (
-    Model as DjangoModel,
-)
-from django.db.models.options import (
-    Options,
-)
-from six.moves import (
-    map,
-)
+# Stdlib
+from abc import ABCMeta
+from itertools import imap
+from operator import attrgetter
 
+# 3rdparty
+from django.db.models import Model
 
 #------------------------------------------------------------------------------
 # Metadata
 #------------------------------------------------------------------------------
 
 __author__ = 'Andrey Torsunov'
 __contact__ = 'torsunov@bars-open.com'
 __docformat__ = 'restructuredtext'
 
 
 #------------------------------------------------------------------------------
 # Proxy classes
 #------------------------------------------------------------------------------
 
-class BaseProxy(six.with_metaclass(ABCMeta, object)):
+class BaseProxy(object):
     u""" Базовый прокси класс для объектов отвечающих за
     представление сущности в UI.
 
     Может перехватывать у провайдера ``save`` и ``delete``, если одноименные
     методы определены в дочернем классе.
 
     Жизненный цикл прокси:
@@ -48,32 +37,30 @@
     * ``Создание > Заполнение данными > Привязка к форме > JSON``
     * ``JSON > Привязка из формы > Ассоциация > Проверка > Сохранение``
 
     .. note::
         protected и private атрибуты не подлежат сериализации в JSON
 
     """
-
-    model_meta_fields_attr = 'local_fields'
-    _models_field_cache = {}
+    __metaclass__ = ABCMeta
 
     def __init__(self, root, context=None):
         #: Корневой объект сущности, который может тянуть за собой
         #: остальные подчиненные объекты.
         self._root = root
         #: Перемещенные поля от :attr:`_root` и обратно
         self._transferred_fields = []
         #: Контекст создания объекта, заполняется при создании в провайдере
         self._context = context
 
     def load(self, root):
         u"""
         Вызывается провайдером, для загрузки данных из полей root в атрибуты прокси.
         В процессе этого могут быть расчитаны вычисляемые поля.
-
+        
         :param root: экземпляр записи модели
         :type root: :class:`django.db.models.Model`
 
         """
         pass
 
     def associate(self):
@@ -93,21 +80,17 @@
         """
         pass
 
     #--------------------------------------------------------------------------
     # Перемещение атрибутов
     #--------------------------------------------------------------------------
 
-    def from_root(self, exclude=()):
-        """Перенос значений полей и json методов в атрибуты класса.
-
-        Args:
-            exclude: перечисление полей, которые следует исключить при перемещении
-        """
-        self.transfer_fields(self._root, self, exclude=exclude)
+    def from_root(self):
+        u""" Перенос значений всех полей и json методов в атрибуты класса. """
+        self.transfer_fields(self._root, self)
 
     def to_root(self):
         """ Перенос значений полей из прокси обратно в корневой объект.
 
         Переносятся только поля, которые изначально были перенесены с
         помощью :meth:`from_root` и сохранены в :attr:`_transferred_fields`.
 
@@ -120,86 +103,50 @@
         u"""
         .. deprecated:: 
            Рекомендуется использовать :meth:`from_root`.
         """
         self.from_root()
 
     def transfer_fields_back_to_root(self):
-        """
+        u""" 
         .. deprecated:: 
            Рекомендуется использовать :meth:`to_root`.
         """
         self.to_root()
 
     def transfer_fields(self, src_obj, dst_obj, exclude=()):
-        """
-        Перенос значений всех полей *src_obj* и json методов в
+        u""" Перенос значений всех полей *src_obj* и json методов в
         атрибуты объкта *dst_obj*
 
         :param src_obj: объект источник
         :param dst_obj: объект приемник
         :param tuple exclude: перечисление полей, которые
             следует исключить при перемещении
 
         """
+        source_is_model = isinstance(src_obj, Model)
+        attrname = attrgetter('attname')
 
-        fields = self._get_model_fields(src_obj)
-
-        if fields:
-            for attr in fields:
-                if attr in exclude:
-                    continue
-
-                value = getattr(src_obj, attr)
-                setattr(dst_obj, attr, value)
-                self._transferred_fields.append(attr)
+        if source_is_model:
+            for attr in imap(attrname, src_obj._meta.local_fields):
+                if attr not in exclude:
+                    value = getattr(src_obj, attr)
+                    setattr(dst_obj, attr, value)
+                    self._transferred_fields.append(attr)
 
         for attr in src_obj.__dict__.keys():
             if not attr.startswith('_'):
                 attr_value = getattr(src_obj, attr)
                 if hasattr(attr_value, 'json_encode') and callable(attr_value):
                     value = attr_value()
                     setattr(dst_obj, attr, value)
-                elif not fields:
+                elif not source_is_model:
                     setattr(dst_obj, attr, attr_value)
 
     #--------------------------------------------------------------------------
-    # Служебные методы
-    #--------------------------------------------------------------------------
-
-    @classmethod
-    def _get_model_fields(cls, src_obj: DjangoModel) -> list[str]:
-        """
-        Получение имен полей модели и формирование кеша.
-
-        Args:
-            src_obj: DjangoModel
-                Исходный объект
-
-        Returns: list[str]
-            Список полей модели
-        """
-
-        result: list[str] = []
-
-        if isinstance(src_obj, DjangoModel):
-            result: list[str] = cls._models_field_cache.get(src_obj.__class__, [])
-
-            if not result:
-                fields_source: Options = src_obj._meta
-                if fields_source.proxy:
-                    fields_source: Options = fields_source.proxy_for_model._meta
-
-                result = cls._models_field_cache[src_obj.__class__] = list(map(
-                    attrgetter('attname'),
-                    getattr(fields_source, cls.model_meta_fields_attr, [])))
-
-        return result
-
-    #--------------------------------------------------------------------------
     # Свойства
     #--------------------------------------------------------------------------
 
     @property
     def context(self):
         u""" Получение контекста запроса, в котором создан этот прокси. """
         return self._context
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/recordpack.py` & `m3-recordpack-0.1.0.9/recordpack/recordpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,129 +1,59 @@
+# coding: utf-8
+
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # Stdlib
 import json
 import operator
-import six
-from collections import (
-    Iterable,
-)
-from six.moves import (
-  filter,
-)
+import itertools
+from collections import Iterable
 
 # 3rdparty
-from django.conf import (
-    settings,
-)
-from django.core.exceptions import (
-    FieldDoesNotExist,
-)
-from django.db.models import (
-    ProtectedError,
-)
-from django.db.models.base import (
-    Model,
-)
-
-from m3 import (
-    ApplicationLogicException,
-)
-from m3.actions import (
-    ACD,
-    ActionPack,
-)
-from m3.actions.context import (
-    ActionContext,
-    ConversionFailed,
-)
-from m3.actions.interfaces import (
-    IMultiSelectablePack,
-)
-from m3.actions.results import (
-    OperationResult,
-)
-from m3.actions.urls import (
-    get_url,
-)
-from m3.actions.utils import (
-    extract_int,
-)
-from m3_ext.ui.containers.grids import (
-    ExtLiveGridCheckBoxSelModel,
-)
-from m3_ext.ui.fields import (
-    ExtComboBox,
-    ExtDictSelectField,
-)
-from m3_ext.ui.fields.complex import (
-    ExtMultiSelectField,
-)
-from m3_ext.ui.fields.simple import (
-    ExtCheckBox,
-    ExtRadio,
-    ExtStringField,
-    ExtTextArea,
-)
-from m3_ext.ui.misc.store import (
-    ExtDataStore,
-    ExtJsonStore,
-)
-from m3_ext.ui.panels.grids import (
-    ExtMultiGroupinGrid,
-    ExtObjectGrid,
-)
-from m3_ext.ui.results import (
-    ExtUIScriptResult,
-)
+from django.conf import settings
+from django.db.models import ProtectedError
+from django.db.models.base import Model
+from django.utils.translation import ugettext as _
+from django.db import transaction
+from m3 import ApplicationLogicException
+from m3.actions import ActionPack, ACD
+from m3.actions.context import ActionContext, ConversionFailed
+from m3_ext.ui.results import ExtUIScriptResult
+from m3.actions.results import OperationResult, PreJsonResult
+from m3.actions.utils import extract_int
+from m3_ext.ui.fields import ExtDictSelectField, ExtComboBox
+from m3_ext.ui.fields.simple import ExtCheckBox
+from m3_ext.ui.panels.grids import ExtMultiGroupinGrid, ExtObjectGrid
+from m3_ext.ui.misc.store import ExtJsonStore, ExtDataStore
+from m3.actions.urls import get_url
+from m3.actions.interfaces import IMultiSelectablePack
+from m3_ext.ui.containers.grids import ExtLiveGridCheckBoxSelModel
 
 # Recordpack
-from . import (
-    helpers,
-    signals,
-    typecast,
-)
-from .be import (
-    BE,
-)
-from .exceptions import (
-    MultipleObjects,
-    ObjectDoesNotExists,
-)
-from .provider import (
-    FIELD_VIEW,
-    QueryObject,
-)
-from .proxy import (
-    BaseProxy,
-)
-from .results import (
-    JsonSerializableResult,
-)
-
+from .be import BE
+from .provider import QueryObject
+from .exceptions import ObjectDoesNotExists, MultipleObjects
+from .proxy import BaseProxy
+from . import helpers, typecast, signals
 
 #------------------------------------------------------------------------------
 # Metadata
 #------------------------------------------------------------------------------
 
 __docformat__ = 'restructuredtext'
 
-# категория для экшенов с записью в БД
-WRITE_CATEGORY = 'write'
-# категория для readonly экшенов
-READONLY_CATEGORY = 'readonly'
 
 #------------------------------------------------------------------------------
 # Pack classes
 #------------------------------------------------------------------------------
 
 class BaseRecordPack(ActionPack):
-    """
+    u"""
     Экшенпак для работы с провайдерами записей
     """
     #: Заголовок пака, а так же окна редактирования по-умолчанию.
     title = ''
 
     #: Иконка для рабочего стола, которая будет соответствовать паку.
     icon_big = 'enterprise-icon-b'
@@ -208,20 +138,20 @@
     #:                            'type': datetime.date },
     context_attr_map = {}
 
     #: Список правил фильтрации для колонок грида.
     #:
     #: .. note::
     #:     Отличие :attr:`quick_filters` от :attr:`context_attr_map` в
-    #:     том, что :attr:`quick_filters` предназначен исключительно
-    #:     для грида, в то время, как :attr:`context_attr_map` для
+    #:     том, что :attr:`quick_filters` предназначен исключительно 
+    #:     для грида, в то время, как :attr:`context_attr_map` для 
     #:     обработки контекста в целом.
     #:
     #: Если требуется добавить фильтрацию для колонки в гриде, то
-    #: необходимо описать правило фильтрации в :attr:`quick_filters`,
+    #: необходимо описать правило фильтрации в :attr:`quick_filters`, 
     #: иначе "шапка" c полем (контролом) для фильтрации в колонке грида
     #: попросту не появится.
     #:
     #: Формат описания фильтров аналогичен :attr:`context_attr_map`, но
     #: еще можно указать контрол для фильтра в колонке, пример:
     #:
     #: .. code-block:: python
@@ -286,62 +216,50 @@
     def __init__(self):
         super(BaseRecordPack, self).__init__()
 
         # Экшн редактирования записи (отображение окна редактирования)
         self.action_edit = helpers.make_action(
             '/edit', self.request_edit_window,
             acd=self._get_edit_action_context_declaration,
-            classname='EditAction',
-            need_atomic=False,
-            category=READONLY_CATEGORY,
-        )
+            classname='EditAction')
 
         # Экшн удаления записи
         self.action_delete = helpers.make_action(
             '/delete',
             self.request_delete_rows,
             acd=self._get_delete_action_context_declaration,
-            classname='DeleteAction',
-            need_atomic=True,
-            category=WRITE_CATEGORY,
-        )
+            classname='DeleteAction')
 
         # Экшн сохранения записи
         self.action_save = helpers.make_action(
             '/save',
             self.request_save,
             acd=self._get_save_action_context_declaration,
-            classname='SaveAction',
-            need_atomic=True,
-            category=WRITE_CATEGORY,
-        )
+            classname='SaveAction')
 
         # Экшн подгружающий доступные записи
         self.action_rows = helpers.make_action(
             '/rows',
             self.request_rows,
             acd=self._get_rows_action_context_declaration,
-            classname='RowsAction',
-            need_atomic=False,
-            category=READONLY_CATEGORY,
-        )
+            classname='RowsAction')
 
         self.actions.extend([
             self.action_edit,
             self.action_delete,
             self.action_rows,
             self.action_save
         ])
 
     #--------------------------------------------------------------------------
     # Правила извлечения параметров из контекста
     #--------------------------------------------------------------------------
 
     def _get_edit_action_context_declaration(self):
-        """ Правила извлечения для :attr:`action_edit`. """
+        u""" Правила извлечения для :attr:`action_edit`. """
         result = [
             ACD(name='isGetData',
                 required=True,
                 type=bool,
                 default=False),
             ACD(name=self.context_id,
                 required=True,
@@ -354,15 +272,15 @@
                 ACD(name=self.context_master_id,
                     required=True,
                     type=self.context_master_type))
 
         return result
 
     def _get_save_action_context_declaration(self):
-        """ Правила извлечения для :attr:`action_save`. """
+        u""" Правила извлечения для :attr:`action_save`. """
         result = [
             ACD(name=self.context_id,
                 required=True,
                 type=self.context_type,
                 default=0),
         ]
         if self.context_master_id:
@@ -378,56 +296,30 @@
                 ACD(name=context_name,
                     required=True,
                     type=object))
 
         return result
 
     def _get_rows_action_context_declaration(self):
-        """ Правила извлечения для :attr:`action_rows`. """
+        u""" Правила извлечения для :attr:`action_rows`. """
         result = [
-            ACD(
-                name='multisort',
+            ACD(name='multisort',
                 required=False,
-                type=object,
-            ),
-            ACD(
-                name='start',
-                required=True,
-                default=0,
-                type=int,
-            ),
-            ACD(
-                name='limit',
-                required=True,
-                default=200,
-                type=int,
-            ),
-            ACD(
-                name='sort',
-                required=True,
-                default='',
-                type=str,
-            ),
-            ACD(
-                name='dir',
-                type=str,
-                required=True,
-                default='ASC',
-            ),
+                type=object),
         ]
         if self.context_master_id:
             result.append(
                 ACD(name=self.context_master_id,
                     required=True,
                     type=self.context_master_type))
 
         return result
 
     def _get_delete_action_context_declaration(self):
-        """ Правила извлечения для :attr:`action_delete`. """
+        u""" Правила извлечения для :attr:`action_delete`. """
         return [
             ACD(name=self.context_id,
                 required=True,
                 type=ActionContext.ValuesList(type=self.context_type),
                 default=0),
         ]
 
@@ -436,24 +328,24 @@
     #--------------------------------------------------------------------------
 
     def _extract_filter_from_request(self, request, context_map):
         _filter = None
 
         # Допускаются только те значения, которые описаны в context_map
         # и не явлюятся пустыми.
-        iter_context = filter(
-            lambda cn_cv: cn_cv[0] in context_map and cn_cv[1],
-            six.iteritems(request.POST)
+        iter_context = itertools.ifilter(
+            lambda (cn, cv): cn in context_map and cv,
+            request.REQUEST.iteritems()
         )
 
         for context_name, context_value in iter_context:
             oper = BE.IC
             name = context_name
             params = context_map[context_name]
-            if isinstance(params, six.string_types):
+            if isinstance(params, basestring):
                 params = {'attr': params}
 
             if 'type' in params:
                 context_value = typecast.typecast(
                     context_value, params['type'], self.custom_typecast)
                 if params['type'] == int:
                     oper = BE.EQ # для инта по дефолту EQ а не IC
@@ -472,89 +364,87 @@
                 if 'filter' in params and callable(params['filter']):
                     context_value = params['filter'](context_value)
                 _filter &= BE(name, oper, context_value)
 
         return _filter
 
     def extract_filter_context(self, request, context):
-        """ Извлечение фильтров из контекста запроса.
+        u""" Извлечение фильтров из контекста запроса.
 
         Извлечение фильтров происходит на основе правил описанных
         в ``context_attr_map``.
 
         :rtype: BooleanExpression or None
 
         """
         return self._extract_filter_from_request(request,
                                                  self.context_attr_map)
 
     def extract_quick_filter_context(self, request, context):
-        """ Извлечение фильтров из контекста запроса.
+        u""" Извлечение фильтров из контекста запроса.
 
         Извлечение фильтров происходит на основе правил описанных
         в ``quick_filters``.
 
         :rtype: BooleanExpression or None
 
         """
         return self._extract_filter_from_request(request, self.quick_filters)
 
     def _convert_context_name_to_attr(self, context_name):
-        """ Преобразование имени из контекста в имя поля модели.
+        u""" Преобразование имени из контекста в имя поля модели.
 
         Преобразование происходит по правилам описанным в:
         - :attr:`context_attr_map`,
         - :attr:`quick_filters`.
 
         :param basestring context_name: имя атрибута в контексте
 
         :return: если правило преобразования не найдено, то вернется
             непреобразованное имя.
         :rtype: str
 
         """
-        context_maps = filter(
+        context_maps = itertools.ifilter(
             lambda m: context_name in m,
             (self.context_attr_map, self.quick_filters))
 
         real_name = context_name
         for context_map in context_maps:
             params = context_map[context_name]
-            if isinstance(params, dict) and 'sort_attr' in params:
-                real_name = params['sort_attr']
-                break
-            elif isinstance(params, dict) and 'attr' in params:
+            if isinstance(params, dict) and 'attr' in params:
                 real_name = params['attr']
                 break
-            elif isinstance(params, six.string_types):
+            elif isinstance(params, basestring):
                 real_name = params
                 break
+
         return real_name
 
     def _update_sorting_context(self, sort_name, direction, sorting=None):
-        """ Обновление информации для сортировки.
+        u""" Обновление информации для сортировки.
 
         :param basestring sort_name: поле для сортировки
         :param basestring direction: направление сортировки ("DESC", "ASC")
         :param list sorting: данные для сортировки
 
         :rtype: list
 
         """
         sorting = sorting or []
         attr = self._convert_context_name_to_attr(sort_name)
         sorting.append((attr, direction))
         return sorting
 
     def extract_sort_context(self, request, context):
-        """ Извлечение параметров сортировки из контекста.
+        u""" Извлечение параметров сортировки из контекста.
         """
         sorting = []
-        direction = request.POST.get('dir')
-        user_sort = request.POST.get('sort')
+        direction = request.REQUEST.get('dir')
+        user_sort = request.REQUEST.get('sort')
 
         # Множественная сортировка.
         if hasattr(context, 'multisort'):
             for sort in context.multisort:
                 sorting = self._update_sorting_context(
                     sort['field'], sort['direction'], sorting)
 
@@ -571,15 +461,15 @@
                 sort_name = sort_name.lstrip("-")
                 sorting = self._update_sorting_context(
                     sort_name, direction, sorting)
 
         return sorting
 
     def _convert_value(self, raw_value, arg_type):
-        """ Приведение значения к типу.
+        u""" Приведение значения к типу.
 
         :param raw_value: приводимое значение
         :param arg_type: приводимый тип
 
         """
         try:
             value = typecast.typecast(raw_value, arg_type)
@@ -589,15 +479,15 @@
         return value
 
     #--------------------------------------------------------------------------
     # Обработчики экшенов
     #--------------------------------------------------------------------------
 
     def get_row_from_request(self, request, context):
-        """ Получение / поиск редактируемой записи из `request`.
+        u""" Получение / поиск редактируемой записи из `request`.
 
         :return: (Model or BaseProxy, bool), первым элементом
             передается сама запись или ее прокси объект; если запись
             новая, то второй элемент кортежа будет :const:`True`, в
             ином случае :const:`False`.
         :rtype: tuple
 
@@ -608,29 +498,29 @@
         if is_new:
             row = self.new_row(request, context)
         else:
             row = self.get_row(request, context, key=row_id, query_object=qo)
         return row, is_new
 
     def get_query_object(self, request, context):
-        """
+        u"""
         Возвращает начальный объект для запроса к провайдеру.
         Используется для переопределения в потомках.
 
         :rtype: QueryObject
 
         """
         qo = QueryObject()
         qo.totals = self.totals
         return qo
 
     def request_rows(self, request, context):
-        """ Обработчик запроса на получение списка записей.
+        u""" Обработчик запроса на получение списка записей.
 
-        :rtype: JsonSerializableResult
+        :rtype: PreJsonResult
 
         """
         qo = self.get_query_object(request, context)
 
         # Если таблица подчиненная, то фильтруем по мастеру
         if self.context_master_id:
             master_id = getattr(context, self.context_master_id)
@@ -669,92 +559,21 @@
             sender=self.__class__,
             instance=self,
             request=request,
             context=context,
             query=qo,
             rows=result)
 
-        return JsonSerializableResult(result)
-
-    def _process_preview_field(self, field, data_object, complex_data):
-
-        if isinstance(field, ExtMultiSelectField):
-            # Для полей множественного выбора выделим список идентификаторов
-            # записей по аттрибуту value_field
-            # Выводить в поле будем либо объединённое выводимое значение
-            # записей (по аттрибуту display_field), либо указанное в нём
-            # кастомное текстовое сообщение
-            data = (json.loads(field.value)
-                    if isinstance(field.value, str) else field.value)
-            ids = [x[field.value_field] for x in data]
-            if field.multiple_display_value and len(data) > 1:
-                value = field.multiple_display_value
-            else:
-                value = ', '.join([
-                    str(x[field.display_field]) for x in data
-                ])
-
-            complex_data[field.name] = {
-                'id': ids,
-                'value': value
-            }
-
-        elif isinstance(field, ExtDictSelectField):
-            complex_data[field.name] = {
-                'id': field.value,
-                'value': field.default_text
-            }
-
-        elif isinstance(field, ExtComboBox):
-            if field.editable:
-                data_object[field.name] = field.value
-            elif field.store:
-                # Правила нахожджения записи в сторе
-                rules = (
-                    # Длина элементов записи должна быть болье 1го
-                    lambda r: len(r) > 1,
-                    # Первый элемент должен совпадать с искомым
-                    # значением
-                    lambda r: six.text_type(r[0]) == six.text_type(field.value),
-                )
-                try:
-                    # Поиск первой подходящей записи в сторе
-                    record = next(filter(
-                        lambda r: all(rl(r) for rl in rules),
-                        field.store.data
-                    ))
-                except StopIteration:
-                    # Если запись не удалось найти, данные
-                    # подстав ляются как есть.
-                    data_object[field.name] = field.value
-                else:
-                    if field.value_field == field.display_field:
-                        default_text = record[0]
-                    else:
-                        default_text = record[1]
-
-                    complex_data[field.name] = {
-                        'id': field.value,
-                        'value': default_text
-                    }
-
-        elif isinstance(field, ExtCheckBox):
-            data_object[field.name] = field.checked
-
-        elif isinstance(field, ExtRadio):
-            if field.checked:
-                data_object[field.name] = field.value
-
-        else:
-            data_object[field.name] = field.value
+        return PreJsonResult(result)
 
+    @transaction.commit_on_success
     def request_edit_window(self, request, context):
-        """ Обработчик запроса на окно редактирования / создания записи.
+        u""" Обработчик запроса на окно редактирования / создания записи.
 
-        :rtype: ExtUIScriptResult or JsonSerializableResult
+        :rtype: ExtUIScriptResult or PreJsonResult
 
         """
         row, is_new = self.get_row_from_request(request, context)
         # Запрашиваются ли данные для предпросмотра?
         is_preview = context.isGetData
 
         # Перенос данных из записи в форму редактирования
@@ -791,22 +610,61 @@
             data_object = {}
             complex_data = {}
             grid_data = {}
             all_fields = win.form._get_all_fields(win)
             all_grids = self._get_all_grids(win)
 
             for field in all_fields:
-                if field.name:
-                    self._process_preview_field(field, data_object, complex_data)
+                if isinstance(field, ExtDictSelectField):
+                    complex_data[field.name] = {
+                        'id': field.value,
+                        'value': field.default_text
+                    }
+                elif isinstance(field, ExtComboBox):
+                    if field.editable:
+                        data_object[field.name] = field.value
+                    elif field.store:
+                        # Правила нахожджения записи в сторе
+                        rules = (
+                            # Длина элементов записи должна быть болье 1го
+                            lambda r: len(r) > 1,
+                            # Первый элемент должен совпадать с искомым
+                            # значением
+                            lambda r: unicode(r[0]) == unicode(field.value),
+                        )
+                        try:
+                            # Поиск первой подходящей записи в сторе
+                            record = itertools.ifilter(
+                                lambda r: all(rl(r) for rl in rules),
+                                field.store.data
+                            ).next()
+                        except StopIteration:
+                            # Если запись не удалось найти, данные
+                            # подстав ляются как есть.
+                            data_object[field.name] = field.value
+                        else:
+                            if field.value_field == field.display_field:
+                                default_text = record[0]
+                            else:
+                                default_text = record[1]
+
+                            complex_data[field.name] = {
+                                'id': field.value,
+                                'value': default_text
+                            }
+                elif isinstance(field, ExtCheckBox):
+                    data_object[field.name] = field.checked
+                else:
+                    data_object[field.name] = field.value
 
             for grid in all_grids:
                 if isinstance(grid.store, ExtDataStore) and grid.name:
                     grid_data[grid.name] = grid.store.data
 
-            return JsonSerializableResult({
+            return PreJsonResult({
                 'success': True,
                 'data': data_object,
                 'complex_data': complex_data,
                 'grid_data': grid_data
             })
 
         else:
@@ -823,22 +681,20 @@
                 record=row,
                 window=win,
                 is_new=is_new)
 
             return ExtUIScriptResult(win, context)
 
     def _get_all_grids(self, item, lst=None):
-        """ Список всех гридов формы включая вложенные в контейнеры.
+        u""" Список всех гридов формы включая вложенные в контейнеры.
 
         :rtype: list
 
         """
-        if lst is None:
-            lst = []
-
+        lst = lst or []
         if isinstance(item, ExtObjectGrid):
             lst.append(item)
         elif hasattr(item, 'items'):
             for it in item.items:
                 self._get_all_grids(it, lst)
         return lst
 
@@ -871,27 +727,27 @@
             return self._local_save(request, context, row, is_new, qo)
         elif self.incremental_update:
             return self._incremental_save(request, context, row, is_new, qo)
         else:
             return self._natural_save(request, context, row, is_new, qo)
 
     def _local_save(self, request, context, row, is_new, qo):
-        """ Редактирование на клиенте.
+        u""" Редактирование на клиенте.
 
         :return: выдадим JSON записи
-        :rtype: JsonSerializableResult
+        :rtype: PreJsonResult
 
         """
-        return JsonSerializableResult({'success': True, 'data': row})
+        return PreJsonResult({'success': True, 'data': row})
 
     def _incremental_save(self, request, context, row, is_new, qo):
-        """ Обновление частями.
+        u""" Обновление частями.
 
         :return: JSON записи
-        :rtype: JsonSerializableResult or OperationResult
+        :rtype: PreJsonResult or OperationResult
 
         """
         self.save_row(request, context, row, is_new)
         # Для выдачи JSON надо получить объект списка, а не карточки,
         # но к сожалению провайдер устроен так, что ListProxy выдает
         # только get_rows.
         #
@@ -901,33 +757,35 @@
         rows = self.provider.get_records(qo)
 
         if isinstance(rows, dict) and 'rows' in rows:
             rows = rows['rows']
 
         if rows:
             list_obj = rows[0]
-            return JsonSerializableResult({'success': True, 'data': list_obj})
+            return PreJsonResult({'success': True, 'data': list_obj})
 
         return OperationResult()
 
     def _natural_save(self, request, context, row, is_new, qo):
-        """ Серверное редактирование. """
+        u""" Серверное редактирование. """
         self.save_row(request, context, row, is_new)
         return OperationResult()
 
+    @transaction.commit_on_success
     def request_save(self, request, context):
-        """ Обработчик запроса на сохранение записи.
+        u""" Обработчик запроса на сохранение записи.
 
-        :rtype: OperationResult or JsonSerializableResult
+        :rtype: OperationResult or PreJsonResult
 
         """
         return self._request_save(request, context)
 
+    @transaction.commit_on_success
     def request_delete_rows(self, request, context):
-        """ Обработчик запроса на удаление записей.
+        u""" Обработчик запроса на удаление записей.
 
         :rtype: OperationResult
 
         """
         rows_id = getattr(context, self.context_id)
         result = self.validate_delete_rows(request, context, rows_id)
 
@@ -941,22 +799,22 @@
         return OperationResult()
 
     #--------------------------------------------------------------------------
     # Взаимодействие с провайдером
     #--------------------------------------------------------------------------
 
     def new_row_defaults(self, request, context, defaults):
-        """
+        u"""
         Тут можно обновить/установить значения по-умолчанию для новых
         записей в зависимости от контекста
         """
         pass
 
     def new_row(self, request, context):
-        """ Оборачивает создание новой записи от провайдера.
+        u""" Оборачивает создание новой записи от провайдера.
 
         Позволяет создать запись с предопределенными значениями полей.
 
         :rtype: Model or BaseProxy
 
         """
         # Создаем новую запись с заполненным мастером по умолчанию
@@ -969,15 +827,15 @@
             default_values[master_field] = master_value
 
         self.new_row_defaults(request, context, default_values)
 
         return self.provider.new_record(**default_values)
 
     def get_row(self, request, context, key, query_object=None):
-        """ Оборачивает получение записи от провайдера.
+        u""" Оборачивает получение записи от провайдера.
 
         Метод нужнен чтобы обрабатывать возможные ошибки на
         пользовательском уровне.
 
         :raises: ObjectDoesNotExists, MultipleObjects
 
         """
@@ -986,233 +844,146 @@
             return self.new_row(request, context)
         else:
             try:
                 return self.provider.get_record(
                     key=key, query_object=query_object)
             except ObjectDoesNotExists:
                 raise ApplicationLogicException(
-                    f'Запись с id={key} не существует в базе данных.')
+                    _(u'Запись с id=%s не существует в базе данных.') % key)
             except MultipleObjects:
                 raise ApplicationLogicException(
-                    f'По id={key} найдено несколько записей. Возможно '
-                    f'целостность данных нарушена.')
+                    _(u'По id=%s найдено несколько записей. Возможно '
+                      u'целостность данных нарушена.') % key)
 
     def get_rows(self, request, context, query_object):
-        """ Получение списка записей.
+        u""" Получение списка записей.
 
         :rtype: list
 
         """
         return self.provider.get_records(query_object)
 
     def save_row(self, request, context, record, is_new):
-        """
+        u"""
         Сохранение записи.
         """
         return self.provider.save(record)
 
     def validate_row(self, request, context, record, is_new):
-        """
+        u"""
         Проверка записи на корректность заполнения.
         """
         return self.provider.validate(record)
 
     def validate_delete_rows(self, request, context, ids):
-        """
+        u"""
         Проверка возможности удаления записей.
         """
         return False
 
     def delete_rows(self, request, context, ids):
-        """Удаление записей.
-
-        Args:
-            request: запрос от клиента.
-            context: контекст выполнения.
-            ids: перечень id записей для удаления.
-
-        Returns:
-            Возвращает перечень ошибок, которые возникли при удалении записей.
+        u"""
+        Удаление записей.
         """
-
-        if isinstance(ids, six.string_types) or not isinstance(ids, Iterable):
-            ids = [ids, ]
-
-        results = []
-
         for _id in ids:
             obj = self.get_row(request, context, key=_id)
-            result = self.delete_row(request, context, obj)
-
-            if result:
-                results.append(result)
-
-        return results
+            self.delete_row(request, context, obj)
 
     def delete_row(self, request, context, record):
-        """
+        u"""
         Удаление записи.
-
-        Args:
-            request: запрос от клиента.
-            context: контекст выполнения.
-            record: запись для удаления.
-
-        Returns:
-            Может вернуть определенный результат (например, неблокирующую ошибку).
         """
         try:
             self.provider.delete_record(record)
         except ProtectedError as e:
-            err_msg = 'Нельзя удалить запись, так как она где-то используется!'
+            err_msg = _(u'Нельзя удалить запись, так как она где-то '
+                        u'используется!')
 
-            if settings.DEBUG or settings.TEST_APPLICATION:
-                if len(e.protected_objects) > 50:
-                    err_msg += '<br>(обнаружено более 50 зависимостей)'
-                err_msg = '{0}<br>{1}'.format(
-                    err_msg,
-                    '<br>'.join(
-                        ['{0} ID={1}'.format(po._meta.verbose_name, po.id) for
-                         po in list(e.protected_objects)[:50]]
-                    )
-                )
+            if settings.DEBUG:
+                err_msg = u'{0}<br>{1}'.format(err_msg, '<br>'.join(
+                    [u'{0} ID={1}'.format(po._meta.verbose_name, po.id) for
+                     po in e.protected_objects]))
 
             raise ApplicationLogicException(err_msg)
 
     #--------------------------------------------------------------------------
     # Взаимодействие с окнами
     #--------------------------------------------------------------------------
 
     def get_edit_window(self, request, context, record, is_new, **kwargs):
-        """
+        u"""
         Получение окна редактирования записи.
         """
         if is_new:
-            assert self.new_window, 'new_window должен быть задан'
+            assert self.new_window, u'new_window должен быть задан'
             win = self.new_window(create_new=is_new, **kwargs)
         else:
-            assert self.edit_window, 'edit_window должен быть задан'
+            assert self.edit_window, u'edit_window должен быть задан'
             win = self.edit_window(create_new=is_new, **kwargs)
 
         if not win.title:
             win.title = self.title
 
         if hasattr(self, 'icon') and self.icon:
             win.icon_cls = self.icon
 
         win.form.url = get_url(self.action_save)
 
         return win
 
     def update_context(self, request, context, window):
-        """
+        u"""
         Настройка контекста окна.
         """
         if not window.action_context:
             window.action_context = context
         else:
             window.action_context.__dict__.update(context.__dict__)
 
     def bind_record_to_window(self, request, context, record, window, is_new):
-        """
+        u"""
         Отображение записи на форму.
         """
         window.form.from_object(record)
 
-        def get_dbfield(obj, names):
-            """
-            Аналог функции get_value в ExtForm.from_object
-            Ищет в объекте obj поле с именем names.
-            Если соответствующего поля не оказалось, то возвращает None
-
-            names задается в виде списка, т.о. если его длина больше единицы,
-            то имеются вложенные объекты и их надо обработать
-            :param obj: объект или словарь
-            :type obj: object или dict
-            :param names: список имен
-            :type names: list
-            """
-            field_object = None
-
-            # hasattr не работает для dict'a
-            has_attr = (
-                hasattr(obj, names[0])
-                if not isinstance(obj, dict) else names[0] in obj)
-            if has_attr:
-                if len(names) == 1:
-                    if not isinstance(obj, dict):
-                        if isinstance(obj, BaseProxy):
-                            obj = obj._root
-                        if isinstance(obj, Model):
-                            try:
-                                field_object = obj._meta.get_field(names[0])
-                            except FieldDoesNotExist:
-                                pass
-                else:
-                    nested = (
-                        getattr(obj, names[0])
-                        if not isinstance(obj, dict) else obj[names[0]])
-                    field_object = get_dbfield(nested, names[1:])
-
-            return field_object
-
-        # помимо отображения, сделаем настройку полей
-        all_fields = window.form._get_all_fields(window.form)
-        for field in all_fields:
-            if not field.name:
-                continue
-            dbfield = get_dbfield(record, field.name.split('.'))
-            # выставим макс длину поля в соответствии с длиной поля БД
-            if (dbfield and isinstance(field, (ExtStringField, ExtTextArea)) and
-                    dbfield.max_length and (field.max_length is None
-                    or dbfield.max_length < field.max_length)):
-                field.max_length = dbfield.max_length
-
     def bind_request_to_window(self, request, context, window):
-        """
+        u"""
         Отображение запроса на форму.
         """
         window.form.bind_to_request(request)
 
     def bind_window_to_record(self, request, context, window, record, is_new):
-        """
+        u"""
         Отображение формы в запись.
         """
         window.form.to_object(record)
 
         # Привязка данных при локальном редактировании
         for k, v in self.local_edit_map.items():
             value = getattr(context, k)
             setattr(record, v, value)
 
     def create_column_filters(self, request, context, grid_or_tree):
-        """
+        u"""
         Построение фильтров в гриде.
         """
         columns = grid_or_tree.columns or ()
-        for col_name, params in six.iteritems(self.quick_filters):
+        for col_name, params in self.quick_filters.iteritems():
             params = params or {}
-            cmplx_control = params.get('complex_control')
-            if cmplx_control:
-                func = cmplx_control.get('func')
-                args = cmplx_control.get('args', [])
-                kwargs = cmplx_control.get('kwargs', {})
-                control = func(*args, **kwargs)
-            else:
-                control = params.get('control', {'xtype': 'textfield'})
+            control = params.get('control', {'xtype': 'textfield'})
 
             if isinstance(control, dict):
                 control['filterName'] = col_name
 
             for column in columns:
                 if column.data_index == col_name:
                     column.extra['filter'] = control
 
     def bind_to_grid(self, request, context, grid):
-        """
+        u"""
         Присоединение списка к гриду.
         """
         # настройка стора
         if not grid.get_store():
             grid_store = ExtJsonStore(
                 url=get_url(self.action_rows),
                 auto_load=True,
@@ -1243,28 +1014,28 @@
         self.create_column_filters(request, context, grid)
 
     #--------------------------------------------------------------------------
     # Геттеры адресов экшенов
     #--------------------------------------------------------------------------
 
     def get_edit_url(self):
-        """
+        u"""
         Возвращает адрес формы редактирования элемента справочника.
         """
         return get_url(self.action_edit)
 
     def get_rows_url(self):
-        """
+        u"""
         Возвращает адрес по которому запрашиваются элементы грида.
         """
         return get_url(self.action_rows)
 
 
 class BaseRecordListPack(BaseRecordPack, IMultiSelectablePack):
-    """ Прямой аналог линейного справочника.
+    u""" Прямой аналог линейного справочника.
 
     В дополнение к работе с данными из BaseRecordPack, содержит экшены
     форм списка и выбора, реализует интерфейс справочника ISelectablePack.
 
     """
     #: Заголовок окна списка записей по-умолчанию
     title_plural = ''
@@ -1290,86 +1061,77 @@
             self.title_plural = self.title
 
         # Экшн журнального окна.
         self.action_list = helpers.make_action(
             '/list',
             self.request_list_window,
             acd=self._get_list_action_context_declaration,
-            classname='ListAction',
-            need_atomic=False,
-            category=READONLY_CATEGORY,
-        )
+            classname='ListAction')
 
         # Экшн окна выбора записей. Обычно используется для
         # :class:`ExtDictSelectField`.
         self.action_select = helpers.make_action(
             '/select',
             self.request_select_window,
             acd=self._get_select_action_context_declaration,
-            classname='SelectAction',
-            need_atomic=False,
-            category=READONLY_CATEGORY,
-        )
+            classname='SelectAction')
 
         # Экшн окна множественного выбора записей. Обычно используется для
         # :class:`ExtDictSelectField`.
         self.action_multi_select = helpers.make_action(
             '/multi-select',
             self.request_multi_select_window,
             acd=self._get_select_action_context_declaration,
-            classname='MultiSelectAction',
-            need_atomic=False,
-            category=READONLY_CATEGORY,
-        )
+            classname='MultiSelectAction')
 
         self.actions.extend([
             self.action_list,
             self.action_select,
             self.action_multi_select
         ])
 
     #--------------------------------------------------------------------------
     # Правила извлечения параметров из контекста
     #--------------------------------------------------------------------------
 
     def _get_list_action_context_declaration(self):
-        """ Правила извлечения контекста для :attr:`action_list`. """
+        u""" Правила извлечения контекста для :attr:`action_list`. """
         return []
 
     def _get_select_action_context_declaration(self):
-        """ Правила извлечения контекста для :attr:`action_select`. """
+        u""" Правила извлечения контекста для :attr:`action_select`. """
         return [
             ACD(name='column_name_on_select',
                 required=True,
-                type=six.text_type,
+                type=unicode,
                 default=''),
         ]
 
     #--------------------------------------------------------------------------
     # Извлечение дополнительного контекста для фильтрации
     #--------------------------------------------------------------------------
 
     def extract_filter_context(self, request, context):
         _filter = super(BaseRecordListPack, self).extract_filter_context(
             request, context)
 
         if self.autocomplete_fields_name:
             # Введенные пользователем данные требующие автокомлита
-            user_text = request.POST.get(self.autocomplete_filter_name)
+            user_text = request.REQUEST.get(self.autocomplete_filter_name)
             if user_text:
                 _filter &= BE(self.autocomplete_fields_name, BE.IC, user_text)
 
         return _filter
 
     #--------------------------------------------------------------------------
     # Обработчики экшенов
     #--------------------------------------------------------------------------
 
     def request_list_window(self, request, context):
-        """
+        u"""
         Обработчик запроса на октрытие журнального окна.
         """
         self._clear_context(request, context)
         win = self.get_list_window(request, context, False)
 
         # Если у журнального окна есть метод настройки под запрос, то он
         # будет вызван.
@@ -1386,15 +1148,15 @@
             request=request,
             context=context,
             window=win)
 
         return ExtUIScriptResult(win, context)
 
     def request_select_window(self, request, context):
-        """
+        u"""
         Обработчик запроса на октрытие окна выбора записи.
         """
         self._clear_context(request, context)
         win = self.get_list_window(request, context, True)
 
         # Если у окна выбора записи есть метод настройки под запрос,
         # то он будет вызван.
@@ -1411,15 +1173,15 @@
             request=request,
             context=context,
             window=win)
 
         return ExtUIScriptResult(win, context)
 
     def request_multi_select_window(self, request, context):
-        """
+        u"""
         Обработчик запроса на октрытие окна множественного выбора записей.
         """
         self._clear_context(request, context)
         win = self.get_list_window(request, context, True)
 
         # Если у окна множественного выбора запией есть метод настройки
         # под запрос, то он будет вызван.
@@ -1432,114 +1194,113 @@
         # Модификация окна под множественный выбор.
         win.grid.sm = ExtLiveGridCheckBoxSelModel(check_only=True)
         win.set_multiselect_mode(True)
 
         return ExtUIScriptResult(win, context)
 
     def _clear_context(self, request, context):
-        """ Очистка контекста от лишних параметров.
+        u""" Очистка контекста от лишних параметров.
 
         В окно могут попасть оставшиеся в контексте значения quick-фильтров.
 
         """
         for context_name in self.quick_filters.keys():
             if hasattr(context, context_name):
                 delattr(context, context_name)
 
     #--------------------------------------------------------------------------
     # Взаимодействие с окнами
     #--------------------------------------------------------------------------
 
-    def get_list_window(self, request, context, is_select, *args, **kwargs):
+    def get_list_window(self, request, context, is_select):
         if is_select:
             if self.select_window is None:
                 raise AttributeError((
                     "'select_window' must be specified in '{}' class"
                 ).format(self.__class__.__name__))
-            win = self.select_window(*args, **kwargs)
+            win = self.select_window()
             win.modal = True
         else:
             if self.list_window is None:
                 raise AttributeError((
                     "'list_window' must be specified in '{}' class"
                 ).format(self.__class__.__name__))
-            win = self.list_window(*args, **kwargs)
+            win = self.list_window()
 
         if not win.title:
             win.title = self.title_plural
 
         if hasattr(self, 'icon') and self.icon:
             win.icon_cls = self.icon
 
         return win
 
     #--------------------------------------------------------------------------
     # Геттеры адресов экшенов
     #--------------------------------------------------------------------------
 
     def get_list_url(self):
-        """ Возвращает адрес формы списка элементов справочника.
+        u""" Возвращает адрес формы списка элементов справочника.
 
         Используется для присвоения адресов в прикладном приложении.
 
         """
         return get_url(self.action_list)
 
     #--------------------------------------------------------------------------
     # Реализация :class:`IMultiSelectablePack`
     #--------------------------------------------------------------------------
 
     def get_autocomplete_url(self):
-        """ Возвращает адрес для автоподбора элементов по введеному
+        u""" Возвращает адрес для автоподбора элементов по введеному
         пользователем тексту.
         """
         return self.get_rows_url()
 
     def get_edit_url(self):
-        """ Возвращает адрес диалога редактирования выбранного элемента. """
+        u""" Возвращает адрес диалога редактирования выбранного элемента. """
         return super(BaseRecordListPack, self).get_edit_url()
 
     def get_multi_select_url(self):
-        """ Возвращает адрес экшена окна для множественного выбора записей. """
+        u""" Возвращает адрес экшена окна для множественного выбора записей. """
         return get_url(self.action_multi_select)
 
     def get_select_url(self):
-        """ Возвращает адрес экшена окна для выбора записей. """
+        u""" Возвращает адрес экшена окна для выбора записей. """
         return get_url(self.action_select)
 
     def get_display_dict(self, key, value_field='id', display_field='name'):
-        """ Получает список словарей для отображения в компоненте
+        u""" Получает список словарей для отображения в компоненте
         множественного выбора.
 
         Метод работает по разному в зависимости от переданного ключа key:
         - json строка - переводится с список id и передается провайдеру;
         - список или кортеж - передается провайдеру;
         - запись ORM или прокси - не передается провайдеру, данные
         извлекаются из неё напрямую.
 
         """
         items = []
 
-        if isinstance(key, six.string_types):
+        if isinstance(key, basestring):
             try:
                 keys = json.loads(key)
             except ValueError:
                 keys = [key]
         elif isinstance(key, Iterable):
             keys = key
         else:
             keys = [key]
 
-        for key in filter(None, keys):
+        for key in itertools.ifilter(None, keys):
             if isinstance(key, (Model, BaseProxy)):
                 row = key
             else:
                 try:
-                    row = self.get_display_record(key, [value_field,
-                                                        display_field])
+                    row = self.provider.get_record(key=key)
                 except ObjectDoesNotExists:
                     row = None
                 if not row:
                     continue
 
             value = getattr(row, value_field, None)
             if value:
@@ -1549,46 +1310,29 @@
                 items.append({
                     value_field: value,
                     display_field: display})
 
         return items
 
     def get_display_text(self, key, attr_name=None):
-        """ Возвращает отображаемое значение записи (или :attr:`attr_name`)
+        u""" Возвращает отображаемое значение записи (или :attr:`attr_name`)
         по ключу `key`.
         """
+        row = self.get_record(key)
         name = attr_name or self.autocomplete_fields_name
-        row = self.get_display_record(key, [name])
 
         if name and row:
             try:
                 text = operator.attrgetter(name)(row)
             except AttributeError:
                 text = None
 
             return callable(text) and text() or text
         elif row:
-            return six.text_type(row)
+            return unicode(row)
         else:
             return
 
-    def get_display_record(self, key, attrs=None):
-        """
-        Специальный метод, вызываемый в биндинге формы (ExtForm.from_object)
-        для связки поля выбора из справочника с текущей выбранной записью.
-        В отличие от get_record, должен вытащить не полную запись, а
-        по возможности самый минимальный набор атрибутов.
-        Это должно регулироваться либо специальным proxy-объектом (listproxy),
-        либо query_object, в котором указываются нужные атрибуты
-        :param key: ключ записи
-        :param attrs: список атрибутов, которые требуются для отображения
-        :return: запись
-        """
-        qo = QueryObject()
-        # укажаем желаемое представление записи
-        qo.view = FIELD_VIEW
-        return self.get_record(key, query_object=qo)
-
     def get_record(self, key, query_object=None):
         if key == 0 or key == '':
             return None
         return self.provider.get_record(key=key, query_object=query_object)
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/signals.py` & `m3-recordpack-0.1.0.9/recordpack/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
 
 # 3rdparty
-from __future__ import absolute_import
-
 from django.dispatch import Signal
 
 #------------------------------------------------------------------------------
 # Metadata
 #------------------------------------------------------------------------------
 
 __author__ = 'Andrey Torsunov'
```

### Comparing `m3-recordpack-0.1.0.65/recordpack/typecast.py` & `m3-recordpack-0.1.0.9/recordpack/typecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # coding: utf-8
 
 #------------------------------------------------------------------------------
 # Imports
 #------------------------------------------------------------------------------
-from __future__ import absolute_import
 
 import decimal
 import datetime
 import json
-import six
-
-from six import string_types, text_type
 
 #------------------------------------------------------------------------------
 # Metadata
 #------------------------------------------------------------------------------
 
 __author__ = 'Andrey Torsunov'
 __contact__ = 'torsunov@bars-open.com'
@@ -91,19 +87,19 @@
         :class:`bool` и т.д), в качестве значение callable с одним аргументом
 
     :return: значение приведенное к *type_*
 
     :raise: ValueError, TypeError
 
     """
-    raw = six.text_type(raw)
-    if type_ != six.string_types:
+    raw = unicode(raw)
+    if type_ != basestring:
         raw = raw.strip()
     custom_cast = custom_cast or {}
-    cast_map = {**CAST_MAP, **custom_cast}
+    cast_map = dict(CAST_MAP, **custom_cast)
     cast = cast_map.get(type_)
     if cast is None:
         raise ValueError("Type converter to '%s' is not defined" % repr(type_))
     return cast(raw)
 
 
 def mute_typecast(raw, _type, custom_cast=None, default=None):
@@ -120,14 +116,13 @@
 
 
 CAST_MAP = {
     int: int,
     float: float,
     bool: lambda x: x.lower() in ('true', '1', 'on'),
     decimal.Decimal: lambda x: decimal.Decimal(x),
+    basestring: unicode,
     datetime.datetime: cast_to_datetime,
     datetime.date: cast_to_date,
     datetime.time: cast_to_time,
     object: json.loads
 }
-for t in string_types:
-    CAST_MAP[t] = text_type
```

### Comparing `m3-recordpack-0.1.0.65/setup.py` & `m3-recordpack-0.1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
-from __future__ import absolute_import
 from setuptools import setup, find_packages
+import sys, os
 import recordpack
 
 version = recordpack.__version__
 
 setup(name='m3-recordpack',
       version=version,
       description=u'Пак общего назначения, для формирования и управления журнальными окнами и окнами справочников',
```

