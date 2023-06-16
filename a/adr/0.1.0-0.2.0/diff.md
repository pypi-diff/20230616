# Comparing `tmp/adr-0.1.0.tar.gz` & `tmp/adr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adr-0.1.0.tar", max compression
+gzip compressed data, was "adr-0.2.0.tar", max compression
```

## Comparing `adr-0.1.0.tar` & `adr-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3520 2023-04-16 19:30:46.662865 adr-0.1.0/README.md
--rw-r--r--   0        0        0     1229 2023-04-16 19:30:46.662865 adr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        1 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/entrypoints/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/entrypoints/cli.py
--rw-r--r--   0        0        0      311 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/injection/__init__.py
--rw-r--r--   0        0        0      720 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/injection/modules.py
--rw-r--r--   0        0        0      197 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/injection/settings.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/repositories/adr/__init__.py
--rw-r--r--   0        0        0      563 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/repositories/adr/base.py
--rw-r--r--   0        0        0     1487 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/repositories/adr/repository.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/services/template/__init__.py
--rw-r--r--   0        0        0      264 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/services/template/base.py
--rw-r--r--   0        0        0      512 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/services/template/service.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/__init__.py
--rw-r--r--   0        0        0      121 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/constants.py
--rw-r--r--   0        0        0      714 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/dtos.py
--rw-r--r--   0        0        0      951 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/settings.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/value_objects/__init__.py
--rw-r--r--   0        0        0      176 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/shared_kernel/value_objects/template.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/templates/__init__.py
--rw-r--r--   0        0        0      495 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/templates/initial-adr.md
--rw-r--r--   0        0        0      207 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/templates/new-adr.md
--rw-r--r--   0        0        0        0 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/use_cases/__init__.py
--rw-r--r--   0        0        0     1049 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/use_cases/creating.py
--rw-r--r--   0        0        0      981 2023-04-16 19:30:46.662865 adr-0.1.0/src/adrpy/use_cases/initializing.py
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 adr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3511 2023-06-16 19:13:06.172070 adr-0.2.0/README.md
+-rw-r--r--   0        0        0     1226 2023-06-16 19:13:06.172070 adr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/entrypoints/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/entrypoints/cli.py
+-rw-r--r--   0        0        0      219 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/injection/__init__.py
+-rw-r--r--   0        0        0      504 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/injection/modules.py
+-rw-r--r--   0        0        0      167 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/injection/settings.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.172070 adr-0.2.0/src/adrpy/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/repositories/adr/__init__.py
+-rw-r--r--   0        0        0      563 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/repositories/adr/base.py
+-rw-r--r--   0        0        0     1444 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/repositories/adr/repository.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/services/template/__init__.py
+-rw-r--r--   0        0        0      264 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/services/template/base.py
+-rw-r--r--   0        0        0      512 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/services/template/service.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/constants.py
+-rw-r--r--   0        0        0      714 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/dtos.py
+-rw-r--r--   0        0        0      951 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/settings.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/value_objects/__init__.py
+-rw-r--r--   0        0        0      176 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/shared_kernel/value_objects/template.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/templates/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/templates/initial-adr.md
+-rw-r--r--   0        0        0      207 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/templates/new-adr.md
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/use_cases/__init__.py
+-rw-r--r--   0        0        0     1061 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/use_cases/creating.py
+-rw-r--r--   0        0        0     1000 2023-06-16 19:13:06.176071 adr-0.2.0/src/adrpy/use_cases/initializing.py
+-rw-r--r--   0        0        0     4138 1970-01-01 00:00:00.000000 adr-0.2.0/PKG-INFO
```

### Comparing `adr-0.1.0/README.md` & `adr-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ## Prerequisites
 
 - Python 3.11 installed on your system.
 - Basic knowledge of command-line interface (CLI) usage.
 
 ## Installation
 
-- `pip install adrpy`
+- `pip install adr`
 
 ## How to Use
 
 **Usage**:
 
 ```console
-$ adrpy [OPTIONS] COMMAND [ARGS]...
+$ adr [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
@@ -39,15 +39,15 @@
 ## `init`
 
 Initialize ADR directory with first ADR in given PATH
 
 **Usage**:
 
 ```console
-$ adrpy init [OPTIONS] [PATH]
+$ adr init [OPTIONS] [PATH]
 ```
 
 **Arguments**:
 
 * `[PATH]`: Path in where ADRs should reside. If not provided Path will be extracted from pyproject.toml
 
 **Options**:
@@ -57,24 +57,24 @@
 ## `new`
 
 Create new ADR with given NAME
 
 **Usage**:
 
 ```console
-$ adrpy new [OPTIONS] NAME
+$ adr new [OPTIONS] NAME
 ```
 
 **Arguments**:
 
 * `NAME`: Name of new ADR. Longer names (with spaces) should be put in quotation marks.  [required]
 
 **Options**:
 
-* `adrpy --help`: Show this message and exit.
+* `adr --help`: Show this message and exit.
 
 
 ## **ADR Template**
 
 The generated ADR files follow the template proposed by Michael Nygard in his book "Documenting Architecture Decisions." The template consists of the following sections:
 
 - Title: The title of the ADR.
@@ -87,8 +87,8 @@
 
 Using ADRs has several benefits for software development teams, including:
 
 - Documentation: ADRs provide a written record of important architectural decisions, making it easier for team members to understand the reasons behind past decisions.
 - Communication: ADRs serve as a communication tool for discussing and documenting design decisions, facilitating collaboration among team members.
 - Decision-making: ADRs encourage thoughtful decision-making by requiring the team to consider the context, rationale, and potential consequences of each decision.
 - Transparency: ADRs promote transparency by making architectural decisions visible and accessible to the entire team, fostering a culture of shared understanding and accountability.
-- Knowledge sharing: ADRs help capture the collective knowledge and experience of the team, enabling future team members to learn from past decisions and avoid repeating mistakes.
+- Knowledge sharing: ADRs help capture the collective knowledge and experience of the team, enabling future team members to learn from past decisions and avoid repeating mistakes.
```

### Comparing `adr-0.1.0/pyproject.toml` & `adr-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "adr"
-version = "0.1.0"
+version = "0.2.0"
 description = "This Python script is designed to help software development teams document their architecture decisions using Architecture Decision Records (ADRs)."
 authors = ["Daniel Różycki <altosterino@gmail.com>"]
 readme = "README.md"
 packages = [{include = "adrpy", from = "src"}]
 
 [tool.poetry.scripts]
 adr = "adrpy.entrypoints.cli:cli_entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = "^0.7.0"
 loguru = "^0.7.0"
 rich = "^13.3.3"
 mako = "^1.2.4"
-injector = "^0.20.1"
+lidipy = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 ruff = "^0.0.261"
 typer-cli = "^0.0.13"
```

### Comparing `adr-0.1.0/src/adrpy/entrypoints/cli.py` & `adr-0.2.0/src/adrpy/entrypoints/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
-from adrpy.injection import injector
+from adrpy.injection import lidi
 from adrpy.shared_kernel.dtos import CreateADRDTO, InitializeADRDTO
 from adrpy.shared_kernel.settings import Settings
 from adrpy.use_cases.creating import CreatingADR
 from adrpy.use_cases.initializing import InitializingADR
 
 app = typer.Typer()
 
@@ -22,29 +22,27 @@
     )
 ) -> None:
     """
     Initialize ADR directory with first ADR in given PATH
     """
     if path:
         new_settings = Settings(initial_adr_dir=path)
-        injector.binder.bind(Settings, to=new_settings)
-    use_case = injector.get(InitializingADR)
+        lidi.bind(Settings, new_settings, singleton=True)
     dto = InitializeADRDTO(path=path)
-    use_case.execute(dto=dto)
+    InitializingADR().execute(dto=dto)
 
 
 @app.command()
 def new(
     name: str = typer.Argument(
         ..., help="Name of new ADR. Longer names (with spaces) should be put in quotation marks."
     ),
 ) -> None:
     """
     Create new ADR with given NAME
     """
-    use_case = injector.get(CreatingADR)
     dto = CreateADRDTO(name=name)
-    use_case.execute(dto=dto)
+    CreatingADR().execute(dto=dto)
 
 
 def cli_entrypoint() -> None:
     app()
```

### Comparing `adr-0.1.0/src/adrpy/repositories/adr/base.py` & `adr-0.2.0/src/adrpy/repositories/adr/base.py`

 * *Files identical despite different names*

### Comparing `adr-0.1.0/src/adrpy/repositories/adr/repository.py` & `adr-0.2.0/src/adrpy/repositories/adr/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 
-from adrpy.injection import Inject
 from adrpy.repositories.adr.base import BaseADRRepository
 from adrpy.shared_kernel.settings import Settings
 from adrpy.shared_kernel.value_objects.template import RenderedTemplate, Template
 
 
 class ADRFileRepository(BaseADRRepository):
-    def __init__(self, settings: Inject[Settings]) -> None:
+    def __init__(self, settings: Settings) -> None:
         self.settings = settings
 
     def get_template(self, name: str) -> Template:
         template_path = self.settings.APP_TEMPLATES_DIR / name
         with open(template_path, "r") as file:
             content = file.read()
         return Template(name=name, content=content)
```

### Comparing `adr-0.1.0/src/adrpy/services/template/service.py` & `adr-0.2.0/src/adrpy/services/template/service.py`

 * *Files identical despite different names*

### Comparing `adr-0.1.0/src/adrpy/shared_kernel/dtos.py` & `adr-0.2.0/src/adrpy/shared_kernel/dtos.py`

 * *Files identical despite different names*

### Comparing `adr-0.1.0/src/adrpy/shared_kernel/settings.py` & `adr-0.2.0/src/adrpy/shared_kernel/settings.py`

 * *Files identical despite different names*

### Comparing `adr-0.1.0/src/adrpy/use_cases/creating.py` & `adr-0.2.0/src/adrpy/use_cases/creating.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass
 from datetime import datetime
 
-from adrpy.injection import Inject
+from adrpy.injection import lidi
 from adrpy.repositories.adr.base import BaseADRRepository
 from adrpy.services.template.base import BaseTemplateService
 from adrpy.shared_kernel.dtos import CreateADRDTO
 
 
 @dataclass
 class CreatingADR:
-    template_service: Inject[BaseTemplateService]
-    adr_repository: Inject[BaseADRRepository]
+    template_service = lidi.resolve(BaseTemplateService)
+    adr_repository = lidi.resolve(BaseADRRepository)
 
     def execute(self, dto: CreateADRDTO) -> None:
         template = self.adr_repository.get_template(name=dto.adr_template_name)
         rendered_template = self.template_service.render(
             template_file=template,
             data={
                 "date_created": datetime.now(),
```

### Comparing `adr-0.1.0/src/adrpy/use_cases/initializing.py` & `adr-0.2.0/src/adrpy/use_cases/initializing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 
-from adrpy.injection import Inject
+from adrpy.injection import lidi
 from adrpy.repositories.adr.base import BaseADRRepository
 from adrpy.services.template.base import BaseTemplateService
 from adrpy.shared_kernel.dtos import InitializeADRDTO
 from adrpy.shared_kernel.settings import Settings
 
 
 @dataclass
 class InitializingADR:
-    template_service: Inject[BaseTemplateService]
-    file_service: Inject[BaseADRRepository]
-    settings: Inject[Settings]
+    template_service = lidi.resolve(BaseTemplateService)
+    file_service = lidi.resolve(BaseADRRepository)
+    settings = lidi.resolve(Settings)
     INITIAL_ADR_NAME: str = field(init=False, default="0001-record-architecture-decisions")
 
     def execute(self, dto: InitializeADRDTO) -> None:
         app_template = self.file_service.get_template(name=dto.adr_template_name)
         rendered_template = self.template_service.render(
             template_file=app_template, data={"date_created": datetime.now(), "status": "ACCEPTED"}
         )
```

### Comparing `adr-0.1.0/PKG-INFO` & `adr-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: adr
-Version: 0.1.0
+Version: 0.2.0
 Summary: This Python script is designed to help software development teams document their architecture decisions using Architecture Decision Records (ADRs).
 Author: Daniel Różycki
 Author-email: altosterino@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: injector (>=0.20.1,<0.21.0)
+Requires-Dist: lidipy (>=0.1.1,<0.2.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: mako (>=1.2.4,<2.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # ADR-py
@@ -27,22 +27,22 @@
 ## Prerequisites
 
 - Python 3.11 installed on your system.
 - Basic knowledge of command-line interface (CLI) usage.
 
 ## Installation
 
-- `pip install adrpy`
+- `pip install adr`
 
 ## How to Use
 
 **Usage**:
 
 ```console
-$ adrpy [OPTIONS] COMMAND [ARGS]...
+$ adr [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
@@ -55,15 +55,15 @@
 ## `init`
 
 Initialize ADR directory with first ADR in given PATH
 
 **Usage**:
 
 ```console
-$ adrpy init [OPTIONS] [PATH]
+$ adr init [OPTIONS] [PATH]
 ```
 
 **Arguments**:
 
 * `[PATH]`: Path in where ADRs should reside. If not provided Path will be extracted from pyproject.toml
 
 **Options**:
@@ -73,24 +73,24 @@
 ## `new`
 
 Create new ADR with given NAME
 
 **Usage**:
 
 ```console
-$ adrpy new [OPTIONS] NAME
+$ adr new [OPTIONS] NAME
 ```
 
 **Arguments**:
 
 * `NAME`: Name of new ADR. Longer names (with spaces) should be put in quotation marks.  [required]
 
 **Options**:
 
-* `adrpy --help`: Show this message and exit.
+* `adr --help`: Show this message and exit.
 
 
 ## **ADR Template**
 
 The generated ADR files follow the template proposed by Michael Nygard in his book "Documenting Architecture Decisions." The template consists of the following sections:
 
 - Title: The title of the ADR.
@@ -104,7 +104,8 @@
 Using ADRs has several benefits for software development teams, including:
 
 - Documentation: ADRs provide a written record of important architectural decisions, making it easier for team members to understand the reasons behind past decisions.
 - Communication: ADRs serve as a communication tool for discussing and documenting design decisions, facilitating collaboration among team members.
 - Decision-making: ADRs encourage thoughtful decision-making by requiring the team to consider the context, rationale, and potential consequences of each decision.
 - Transparency: ADRs promote transparency by making architectural decisions visible and accessible to the entire team, fostering a culture of shared understanding and accountability.
 - Knowledge sharing: ADRs help capture the collective knowledge and experience of the team, enabling future team members to learn from past decisions and avoid repeating mistakes.
+
```

