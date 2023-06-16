# Comparing `tmp/django_gem-1.1.0.tar.gz` & `tmp/django_gem-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.1.0.tar", max compression
+gzip compressed data, was "django_gem-1.1.1.tar", max compression
```

## Comparing `django_gem-1.1.0.tar` & `django_gem-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1067 2023-06-16 08:33:33.119767 django_gem-1.1.0/LICENSE
--rw-r--r--   0        0        0     2786 2023-06-16 08:33:33.119767 django_gem-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/apps.py
--rw-r--r--   0        0        0      535 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/constants.py
--rw-r--r--   0        0        0       71 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/__init__.py
--rw-r--r--   0        0        0      283 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/cutting_always_eager.py
--rw-r--r--   0        0        0      452 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/override_cutting_mode.py
--rw-r--r--   0        0        0      298 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/context/override_gem_setting.py
--rw-r--r--   0        0        0      218 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/core.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      220 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0     1536 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/__init__.py
--rw-r--r--   0        0        0      207 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/models.py
--rw-r--r--   0        0        0     1544 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/registry.py
--rw-r--r--   0        0        0      111 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/entities/source.py
--rw-r--r--   0        0        0     1108 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/logger.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/__init__.py
--rw-r--r--   0        0        0      893 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/cutmodel.py
--rw-r--r--   0        0        0      953 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/management/commands/cutqueryset.py
--rw-r--r--   0        0        0     2622 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/__init__.py
--rw-r--r--   0        0        0     1969 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2788 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1591 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1260 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     2274 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/save.py
--rw-r--r--   0        0        0      937 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      235 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      286 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      221 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      116 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      353 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      337 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2568 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     5072 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0     7313 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     5044 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0     1328 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1859 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     4198 2023-06-16 08:33:33.119767 django_gem-1.1.0/django_gem/validators.py
--rw-r--r--   0        0        0      811 2023-06-16 08:33:33.119767 django_gem-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-16 09:12:00.534564 django_gem-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2786 2023-06-16 09:12:00.534564 django_gem-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/apps.py
+-rw-r--r--   0        0        0      535 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/constants.py
+-rw-r--r--   0        0        0       71 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/context/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/context/cutting_always_eager.py
+-rw-r--r--   0        0        0      452 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/context/override_cutting_mode.py
+-rw-r--r--   0        0        0      298 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/context/override_gem_setting.py
+-rw-r--r--   0        0        0      225 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/core.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0     1536 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1706 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/entities/registry.py
+-rw-r--r--   0        0        0      132 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/entities/source.py
+-rw-r--r--   0        0        0     1108 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0      953 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     2622 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     2077 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2788 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1591 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1260 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     2274 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      937 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      286 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      221 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      353 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      337 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2568 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     5072 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0     7737 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     5843 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0     1328 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1859 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     4198 2023-06-16 09:12:00.534564 django_gem-1.1.1/django_gem/validators.py
+-rw-r--r--   0        0        0      811 2023-06-16 09:12:00.538564 django_gem-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.1.1/PKG-INFO
```

### Comparing `django_gem-1.1.0/LICENSE` & `django_gem-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/README.md` & `django_gem-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/constants.py` & `django_gem-1.1.1/django_gem/constants.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/cutters/base.py` & `django_gem-1.1.1/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/decorators/cutters.py` & `django_gem-1.1.1/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/decorators/models.py` & `django_gem-1.1.1/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/entities/models.py` & `django_gem-1.1.1/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/entities/registry.py` & `django_gem-1.1.1/django_gem/entities/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     propagate_triggers: typing.Dict[str, typing.List] = field(default_factory=lambda: {})
 
 
 @dataclass
 class CutterModel:
     model: typing.Type[models.Model] = None
     triggers: typing.List[CutterModelTrigger] = field(default_factory=lambda: [])
+    select_related_fields: typing.List[str] = field(default_factory=lambda: [])
+    prefetch_related_fields: typing.List[str] = field(default_factory=lambda: [])
 
 
 # endregion
 
 # region Reverse cutter entities
```

### Comparing `django_gem-1.1.0/django_gem/exceptions.py` & `django_gem-1.1.1/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/management/commands/cutmodel.py` & `django_gem-1.1.1/django_gem/management/commands/cutmodel.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/management/commands/cutqueryset.py` & `django_gem-1.1.1/django_gem/management/commands/cutqueryset.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/migrations/0001_initial.py` & `django_gem-1.1.1/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/models/base.py` & `django_gem-1.1.1/django_gem/models/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     model = None
     related_name = None
     cutter = None
     self_affected_fields: typing.List[str] = []
     propagate_triggers: typing.Dict[str, typing.List] = {}
     side_effects: typing.List[CutterSideEffect] = []
     related_gem_side_effects: typing.List[CutterRelatedGemSideEffect] = []
+    cut_select_related_fields: typing.List[str] = []
+    cut_prefetch_related_fields: typing.List[str] = []
 
 
 class CutterEngineBase(ModelBase):
     def __new__(cls, name, bases, attrs):
         if cutter_engine_meta := attrs.get("CutterEngineMeta"):
             if cutter_engine_meta and cutter_engine_meta.model:
                 related_name = (
```

### Comparing `django_gem-1.1.0/django_gem/models/gem_log_entry.py` & `django_gem-1.1.1/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.1.1/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/models/mixins.py` & `django_gem-1.1.1/django_gem/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/overrides/delete.py` & `django_gem-1.1.1/django_gem/overrides/delete.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/overrides/m2m_changed.py` & `django_gem-1.1.1/django_gem/overrides/m2m_changed.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/overrides/save.py` & `django_gem-1.1.1/django_gem/overrides/save.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/overrides/utils.py` & `django_gem-1.1.1/django_gem/overrides/utils.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/toolkit/chest.py` & `django_gem-1.1.1/django_gem/toolkit/chest.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/toolkit/forge.py` & `django_gem-1.1.1/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/toolkit/registry.py` & `django_gem-1.1.1/django_gem/toolkit/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,22 @@
         self.direct_cutters[model_key].triggers.append(
             CutterModelTrigger(
                 cutter=gem_class.CutterEngineMeta.cutter,
                 gem_class=gem_class,
                 propagate_triggers=gem_class.CutterEngineMeta.propagate_triggers,
             )
         )
+        self.direct_cutters[model_key].select_related_fields = {
+            *self.direct_cutters[model_key].select_related_fields,
+            *gem_class.CutterEngineMeta.cut_select_related_fields,
+        }
+        self.direct_cutters[model_key].prefetch_related_fields = {
+            *self.direct_cutters[model_key].prefetch_related_fields,
+            *gem_class.CutterEngineMeta.cut_prefetch_related_fields,
+        }
         for side_effect in gem_class.CutterEngineMeta.side_effects:
             self._add_side_effect_to_triggers(gem_class, side_effect)
 
     def _add_side_effect_to_triggers(
         self,
         gem_class: typing.Type[CutterEngineBaseModel],
         side_effect: CutterSideEffect,
```

### Comparing `django_gem-1.1.0/django_gem/toolkit/saw.py` & `django_gem-1.1.1/django_gem/toolkit/saw.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,30 @@
 from django_gem.models.mixins import GemModelMixin
 from django_gem.toolkit import forge, gem_settings
 from django_gem.toolkit.chest import SealedChestItem
 
 
 class Saw:
     @classmethod
+    def _get_queryset(cls, model_class, object_ids):
+        from django_gem.toolkit import cutter_registry
+
+        queryset = model_class.objects.filter(id__in=object_ids)
+        cutter_model = cutter_registry.get_cutter_for_model(model_class)
+        (select_related_fields, prefetch_related_fields) = (
+            cutter_model.select_related_fields,
+            cutter_model.prefetch_related_fields,
+        )
+        if select_related_fields:
+            queryset = queryset.select_related(*select_related_fields)
+        if prefetch_related_fields:
+            queryset = queryset.prefetch_related(*prefetch_related_fields)
+        return queryset
+
+    @classmethod
     def cut_content_type(cls, natural_key: str, field_names: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         try:
             content_type: ContentType = ContentType.objects.get_by_natural_key(
@@ -60,32 +76,36 @@
 
             sealed_chest_mapping: typing.Dict[str, SealedChestItem] = {
                 SealedChestItem(**item).object_id: SealedChestItem(**item) for item in chest_items
             }
             chest_item_object_ids = [chest_item for chest_item in sealed_chest_mapping]
 
             model_class = content_type.model_class()
+
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_started_at(chest_item_object_ids)
 
-            for model_instance in model_class.objects.filter(id__in=chest_item_object_ids):
+            queryset = cls._get_queryset(model_class, chest_item_object_ids)
+
+            for model_instance in queryset:
                 model_instance_id = str(model_instance.id)
                 if (sealed_chest_item := sealed_chest_mapping.get(str(model_instance_id))) is None:
                     continue
                 with contextlib.suppress(IntegrityError):
                     # Because of the distributed nature of cutting, the update to gem can happen
                     # after the referencing model was deleted. This will ensure we don't stop
                     # all the cuttings if something goes wrong.
                     forge.cut_model_fields(model_instance, sealed_chest_item.gem_fields)
                     cut_mapping[natural_key] += 1
 
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_completed_at(chest_item_object_ids)
 
-        logger.info(f"Cutting finished, cutting results: {json.dumps(cut_mapping)}")
+        cut_mapping = dict(cut_mapping)
+        logger.info(f"Cutting finished, cutting results: {cut_mapping}")
 
         return cut_mapping
 
     @classmethod
     def cut_queryset(cls, natural_key: str, object_ids: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
@@ -100,15 +120,17 @@
         except ContentType.DoesNotExist:
             return
 
         cut_mapping = defaultdict(int)
 
         model_class = content_type.model_class()
 
-        for model_instance in model_class.objects.filter(id__in=object_ids):
+        queryset = cls._get_queryset(model_class, object_ids)
+
+        for model_instance in queryset:
             reverse_cutter_model = forge.cutter_registry.get_reverse_cutter_for_model(
                 model_instance
             )
             if not reverse_cutter_model or not reverse_cutter_model.model:
                 continue
 
             for reverse_cutter_trigger in reverse_cutter_model.triggers:
@@ -120,8 +142,9 @@
                     natural_key=natural_key,
                     object_ids=object_ids,
                     gem_fields=reverse_cutter_trigger.gem_fields,
                 )
                 cut_mapping[natural_key] += 1
             with transaction.atomic():
                 smith.initiate_cutting()
+        cut_mapping = dict(cut_mapping)
         return cut_mapping
```

### Comparing `django_gem-1.1.0/django_gem/toolkit/settings.py` & `django_gem-1.1.1/django_gem/toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/toolkit/smith.py` & `django_gem-1.1.1/django_gem/toolkit/smith.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/django_gem/validators.py` & `django_gem-1.1.1/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.0/pyproject.toml` & `django_gem-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.1.0"
+version = "1.1.1"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.1.0/PKG-INFO` & `django_gem-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.1.0
+Version: 1.1.1
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

