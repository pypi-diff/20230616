# Comparing `tmp/django_gem-1.0.6.tar.gz` & `tmp/django_gem-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.0.6.tar", max compression
+gzip compressed data, was "django_gem-1.1.0.tar", max compression
```

## Comparing `django_gem-1.0.6.tar` & `django_gem-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
--rw-r--r--   0        0        0     1067 2023-06-16 04:43:16.658527 django_gem-1.0.6/LICENSE
--rw-r--r--   0        0        0     2786 2023-06-16 04:43:16.658527 django_gem-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/apps.py
--rw-r--r--   0        0        0      457 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/constants.py
--rw-r--r--   0        0        0       71 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/context/__init__.py
--rw-r--r--   0        0        0      283 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/context/cutting_always_eager.py
--rw-r--r--   0        0        0      298 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/context/override_gem_setting.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      220 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0     1536 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/entities/__init__.py
--rw-r--r--   0        0        0      106 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/entities/models.py
--rw-r--r--   0        0        0     1544 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/entities/registry.py
--rw-r--r--   0        0        0     1108 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/logger.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/management/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/management/commands/cutmodel.py
--rw-r--r--   0        0        0     1090 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/management/commands/cutqueryset.py
--rw-r--r--   0        0        0     2622 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/__init__.py
--rw-r--r--   0        0        0     1969 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2788 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1061 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     1522 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/overrides/save.py
--rw-r--r--   0        0        0      966 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      243 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      187 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      229 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      100 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      272 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      256 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2690 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     5072 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0     7337 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     4640 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0     1328 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1615 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     4198 2023-06-16 04:43:16.658527 django_gem-1.0.6/django_gem/validators.py
--rw-r--r--   0        0        0      811 2023-06-16 04:43:16.662527 django_gem-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-16 08:33:33.119767 django_gem-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2786 2023-06-16 08:33:33.119767 django_gem-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/apps.py
+-rw-r--r--   0        0        0      535 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/constants.py
+-rw-r--r--   0        0        0       71 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/cutting_always_eager.py
+-rw-r--r--   0        0        0      452 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/override_cutting_mode.py
+-rw-r--r--   0        0        0      298 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/override_gem_setting.py
+-rw-r--r--   0        0        0      218 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/core.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0     1536 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1544 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/registry.py
+-rw-r--r--   0        0        0      111 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/source.py
+-rw-r--r--   0        0        0     1108 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0      953 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     2622 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     1969 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2788 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1591 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1260 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     2274 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      937 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      286 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      221 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      353 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      337 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2568 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     5072 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0     7313 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     5044 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0     1328 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1859 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     4198 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/validators.py
+-rw-r--r--   0        0        0      811 2023-06-16 08:33:33.119767 django_gem-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.1.0/PKG-INFO
```

### Comparing `django_gem-1.0.6/LICENSE` & `django_gem-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/README.md` & `django_gem-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/cutters/base.py` & `django_gem-1.1.0/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/decorators/cutters.py` & `django_gem-1.1.0/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/decorators/models.py` & `django_gem-1.1.0/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/entities/models.py` & `django_gem-1.1.0/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/entities/registry.py` & `django_gem-1.1.0/django_gem/entities/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/exceptions.py` & `django_gem-1.1.0/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/management/commands/cutmodel.py` & `django_gem-1.1.0/django_gem/management/commands/cutmodel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 from django.contrib.auth import get_user_model
-from django.contrib.contenttypes.models import ContentType
 from django.core.management import BaseCommand
 
 from django_gem.toolkit.saw import Saw
 
 User = get_user_model()
 logger = logging.getLogger(__name__)
 
@@ -25,9 +24,8 @@
             help="Specify the object id to cut gems for.",
         )
 
     def handle(self, *args, **options):
         app_label = options["app_label"]
         model_name = options["model_name"]
         object_id = options["object_id"]
-        content_type = ContentType.objects.get(app_label=app_label, model=model_name)
-        Saw.cut_queryset(content_type_id=content_type.id, object_ids=[object_id])
+        Saw.cut_queryset(f"{app_label}.{model_name}", object_ids=[object_id])
```

### Comparing `django_gem-1.0.6/django_gem/migrations/0001_initial.py` & `django_gem-1.1.0/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/models/base.py` & `django_gem-1.1.0/django_gem/models/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/models/gem_log_entry.py` & `django_gem-1.1.0/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.1.0/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/models/mixins.py` & `django_gem-1.1.0/django_gem/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/overrides/delete.py` & `django_gem-1.1.0/django_gem/overrides/delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import typing
 
 from django.db import transaction
 
+from django_gem.constants import GemCuttingMode
+from django_gem.core import get_model_natural_key
+from django_gem.entities.context import gem_cutting_context
 from django_gem.entities.registry import CutterBatchItem
+from django_gem.entities.source import CutSource
 from django_gem.models.mixins import GemCutConditionalMixin
 from django_gem.overrides.utils import add_cut_items
 
 
 def delete_cutting_hook(
     delete_func,
     cut_batch_items: typing.List[CutterBatchItem],
@@ -20,20 +24,24 @@
         if isinstance(self, GemCutConditionalMixin):
             should_cut = self.should_cut_on_delete(*args, **kwargs)
 
         if should_cut:
             for cut_batch_item in cut_batch_items:
                 cut_batch_item.load_object_ids(self)
 
+            smith.add_source(
+                get_model_natural_key(self), CutSource(object_id=str(self.id), affected_fields=[])
+            )
+
         with transaction.atomic():
             result = delete_func(self, *args, **kwargs)
             if not gem_cutting_enabled or not should_cut:
                 return result
 
             add_cut_items(smith, cut_batch_items)
-
-            transaction.on_commit(
-                lambda: smith.initiate_cutting(),
-            )
+            if gem_cutting_context.cutting_mode == GemCuttingMode.TRANSACTION:
+                transaction.on_commit(
+                    lambda: smith.initiate_cutting(),
+                )
             return result
 
     return wrapped_trigger
```

### Comparing `django_gem-1.0.6/django_gem/overrides/m2m_changed.py` & `django_gem-1.1.0/django_gem/overrides/m2m_changed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import typing
 
 from django.db import transaction
 
+from django_gem.constants import GemCuttingMode
+from django_gem.entities.context import gem_cutting_context
 from django_gem.entities.registry import CutterBatchItem
 from django_gem.overrides.utils import add_cut_items
 
 CUTTER_M2M_SIGNAL_ACTIONS = ["pre_add", "pre_remove", "pre_clear"]
 
 
 def m2m_changed_hook(
@@ -26,12 +28,13 @@
                 changed_cut_batch_items.append(cut_batch_item)
 
             if not gem_cutting_enabled:
                 return
 
             add_cut_items(smith, changed_cut_batch_items)
 
-            transaction.on_commit(
-                lambda: smith.initiate_cutting(),
-            )
+            if gem_cutting_context.cutting_mode == GemCuttingMode.TRANSACTION:
+                transaction.on_commit(
+                    lambda: smith.initiate_cutting(),
+                )
 
     return m2m_changed
```

### Comparing `django_gem-1.0.6/django_gem/overrides/save.py` & `django_gem-1.1.0/django_gem/overrides/save.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import typing
 
+from dirtyfields import DirtyFieldsMixin
 from django.db import transaction
 
+from django_gem.constants import GemCuttingMode
+from django_gem.core import get_model_natural_key
+from django_gem.entities.context import gem_cutting_context
 from django_gem.entities.registry import CutterBatchItem
+from django_gem.entities.source import CutSource
 from django_gem.models.mixins import GemCutConditionalMixin
 from django_gem.overrides.utils import add_cut_items, is_cutting_needed
 
 
 def save_cutting_hook(
     save_func,
     cut_batch_items: typing.List[CutterBatchItem],
@@ -35,13 +40,24 @@
                 return
 
             for cut_batch_item in prepared_cut_batch_items:
                 cut_batch_item.load_object_ids(self)
                 changed_cut_batch_items.append(cut_batch_item)
 
             add_cut_items(smith, changed_cut_batch_items)
-
-            transaction.on_commit(
-                lambda: smith.initiate_cutting(),
+            affected_fields = []
+            if isinstance(self, DirtyFieldsMixin):
+                affected_fields = self.get_dirty_fields(check_relationship=True)
+
+            smith.add_source(
+                get_model_natural_key(self),  # noqa
+                CutSource(
+                    object_id=str(self.id),  # noqa
+                    affected_fields=affected_fields,
+                ),
             )
+            if gem_cutting_context.cutting_mode == GemCuttingMode.TRANSACTION:
+                transaction.on_commit(
+                    lambda: smith.initiate_cutting(),
+                )
 
     return wrapped_trigger
```

### Comparing `django_gem-1.0.6/django_gem/toolkit/forge.py` & `django_gem-1.1.0/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/toolkit/registry.py` & `django_gem-1.1.0/django_gem/toolkit/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 from collections import defaultdict
 
 from django.db.models.fields.related_descriptors import ManyToManyDescriptor
 from django.db.models.signals import m2m_changed
 from django.utils.module_loading import autodiscover_modules
 
+from django_gem.core import get_model_natural_key
 from django_gem.entities.registry import (
     CutterBatchItem,
     CutterModel,
     CutterModelTrigger,
     EagerGemItem,
     ReverseCutterModel,
 )
@@ -29,16 +30,16 @@
     direct_cutters = defaultdict(CutterModel)
     # Reverse cutters contains the related models mapping that should trigger updates
     reverse_cutters = defaultdict(ReverseCutterModel)
 
     @classmethod
     def get_model_key(cls, model_class):
         if isinstance(model_class, ManyToManyDescriptor):
-            return f"{model_class.through._meta.app_label}.{model_class.through._meta.model_name}"  # noqa
-        return f"{model_class._meta.app_label}.{model_class._meta.model_name}"  # noqa
+            return get_model_natural_key(model_class.through)
+        return get_model_natural_key(model_class)  # noqa
 
     def get_cutter_for_model(self, model_class):
         autodiscover_modules("apps")
         return self.direct_cutters.get(self.get_model_key(model_class))
 
     def get_reverse_cutter_for_model(self, model_class):
         autodiscover_modules("apps")
```

### Comparing `django_gem-1.0.6/django_gem/toolkit/saw.py` & `django_gem-1.1.0/django_gem/toolkit/saw.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 import contextlib
 import json
 import typing
+from collections import defaultdict
 
 from django.contrib.contenttypes.models import ContentType
 from django.db import IntegrityError, transaction
 
+from django_gem.core import get_model_natural_key
+from django_gem.logger import logger
 from django_gem.models.mixins import GemModelMixin
 from django_gem.toolkit import forge, gem_settings
 from django_gem.toolkit.chest import SealedChestItem
 
 
 class Saw:
     @classmethod
-    def cut_content_type(cls, content_type_id: int, field_names: list):
+    def cut_content_type(cls, natural_key: str, field_names: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         try:
-            content_type: ContentType = ContentType.objects.get(id=content_type_id)
+            content_type: ContentType = ContentType.objects.get_by_natural_key(
+                *natural_key.split(".")
+            )
         except ContentType.DoesNotExist:
             return
 
         model_class = content_type.model_class()
         for model_instance in model_class.objects.all():
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_started_at([model_instance.id])
-            with transaction.atomic():
-                for field_name in field_names:
-                    forge.cut_model_field(model_instance, field_name)
+            forge.cut_model_fields(model_instance, field_names)
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_completed_at([model_instance.id])
 
     @classmethod
-    def cut_models(cls, sealed_chest: str):
+    def cut_models(cls, sealed_chest: str, sealed_sources: str):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
+        cut_mapping = defaultdict(int)
+
         if not gem_cutting_enabled:
             return
         try:
-            unsealed_chest: typing.Dict[int, typing.List[typing.Dict]] = json.loads(sealed_chest)
+            unsealed_chest: typing.Dict[str, typing.List[typing.Dict]] = json.loads(sealed_chest)
         except json.JSONDecodeError:
             return
 
-        for content_type_id, chest_items in unsealed_chest.items():
+        logger.info(f"Cutting initiated by: {sealed_sources}; for: {sealed_chest}")
+
+        for natural_key, chest_items in unsealed_chest.items():
             try:
-                content_type: ContentType = ContentType.objects.get(id=content_type_id)
+                content_type: ContentType = ContentType.objects.get_by_natural_key(
+                    *natural_key.split(".")
+                )
             except ContentType.DoesNotExist:
                 continue
 
             sealed_chest_mapping: typing.Dict[str, SealedChestItem] = {
                 SealedChestItem(**item).object_id: SealedChestItem(**item) for item in chest_items
             }
             chest_item_object_ids = [chest_item for chest_item in sealed_chest_mapping]
@@ -58,55 +67,61 @@
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_started_at(chest_item_object_ids)
 
             for model_instance in model_class.objects.filter(id__in=chest_item_object_ids):
                 model_instance_id = str(model_instance.id)
                 if (sealed_chest_item := sealed_chest_mapping.get(str(model_instance_id))) is None:
                     continue
-                with contextlib.suppress(IntegrityError), transaction.atomic():
+                with contextlib.suppress(IntegrityError):
                     # Because of the distributed nature of cutting, the update to gem can happen
                     # after the referencing model was deleted. This will ensure we don't stop
                     # all the cuttings if something goes wrong.
-                    forge.cut_model_fields(
-                        model_instance,
-                        sealed_chest_item.gem_fields,
-                    )
+                    forge.cut_model_fields(model_instance, sealed_chest_item.gem_fields)
+                    cut_mapping[natural_key] += 1
 
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_completed_at(chest_item_object_ids)
 
+        logger.info(f"Cutting finished, cutting results: {json.dumps(cut_mapping)}")
+
+        return cut_mapping
+
     @classmethod
-    def cut_queryset(cls, content_type_id: int, object_ids: list):
+    def cut_queryset(cls, natural_key: str, object_ids: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         from django_gem.toolkit import forge, smith
 
         try:
-            content_type: ContentType = ContentType.objects.get(id=content_type_id)
+            content_type: ContentType = ContentType.objects.get_by_natural_key(
+                *natural_key.split(".")
+            )
         except ContentType.DoesNotExist:
             return
 
+        cut_mapping = defaultdict(int)
+
         model_class = content_type.model_class()
 
         for model_instance in model_class.objects.filter(id__in=object_ids):
             reverse_cutter_model = forge.cutter_registry.get_reverse_cutter_for_model(
                 model_instance
             )
             if not reverse_cutter_model or not reverse_cutter_model.model:
                 continue
 
             for reverse_cutter_trigger in reverse_cutter_model.triggers:
                 object_ids = list(reverse_cutter_trigger.callback(model_instance))
                 if not object_ids:
                     continue
-                reversed_cutter_model_content_type = ContentType.objects.get_for_model(
-                    reverse_cutter_trigger.model
-                )
+                natural_key = get_model_natural_key(reverse_cutter_trigger.model)
                 smith.add_item(
-                    content_type_id=reversed_cutter_model_content_type.id,
+                    natural_key=natural_key,
                     object_ids=object_ids,
                     gem_fields=reverse_cutter_trigger.gem_fields,
                 )
+                cut_mapping[natural_key] += 1
             with transaction.atomic():
                 smith.initiate_cutting()
+        return cut_mapping
```

### Comparing `django_gem-1.0.6/django_gem/toolkit/settings.py` & `django_gem-1.1.0/django_gem/toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/django_gem/toolkit/smith.py` & `django_gem-1.1.0/django_gem/toolkit/smith.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import importlib
 import typing
 
+from django_gem.entities.source import CutSource
 from django_gem.logger import logger
 from django_gem.toolkit import gem_settings
 from django_gem.toolkit.anvils.base import BaseAnvil
 from django_gem.toolkit.chest import Chest
 
 
 class Smith:
     """Handles data collection and initiates cut process"""
 
     chest = Chest()
     anvils: typing.List[BaseAnvil] = []
 
-    def add_item(self, content_type_id: int, object_ids: list, gem_fields: list):
-        self.chest.add(content_type_id, object_ids, gem_fields)
+    def add_item(self, natural_key: str, object_ids: list, gem_fields: list):
+        self.chest.add_chest_item(natural_key, object_ids, gem_fields)
+
+    def add_source(self, natural_key: str, source: CutSource):
+        self.chest.add_cut_source(natural_key, source)
 
     def add_anvil(self, anvil: BaseAnvil):
         self.anvils.append(anvil)
 
     def load(self):
         for anvil_import in gem_settings.GEM_ANVILS:
             try:
@@ -39,13 +43,14 @@
             self.add_anvil(anvil())
 
     def initiate_cutting(self):
         if self.chest.is_empty():
             return
 
         sealed_chest = self.chest.get_sealed_chest()
+        sealed_sources = self.chest.get_sealed_sources()
         for anvil in self.anvils:
-            anvil.cut(sealed_chest)
+            anvil.cut(sealed_chest, sealed_sources)
         self.chest.reset()
 
 
 smith = Smith()
```

### Comparing `django_gem-1.0.6/django_gem/validators.py` & `django_gem-1.1.0/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.6/pyproject.toml` & `django_gem-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.0.6"
+version = "1.1.0"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.0.6/PKG-INFO` & `django_gem-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.0.6
+Version: 1.1.0
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

