# Comparing `tmp/notas_musicais-0.2.0.tar.gz` & `tmp/notas_musicais-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notas_musicais-0.2.0.tar", max compression
+gzip compressed data, was "notas_musicais-0.2.1.tar", max compression
```

## Comparing `notas_musicais-0.2.0.tar` & `notas_musicais-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      256 2023-02-14 06:46:12.366404 notas_musicais-0.2.0/LICENSE
--rw-r--r--   0        0        0     8416 2023-02-14 06:32:53.377199 notas_musicais-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-20 08:16:51.333910 notas_musicais-0.2.0/notas_musicais/__init__.py
--rw-r--r--   0        0        0     2951 2023-02-06 14:23:53.892679 notas_musicais-0.2.0/notas_musicais/acordes.py
--rw-r--r--   0        0        0     2242 2023-02-06 14:24:40.302708 notas_musicais-0.2.0/notas_musicais/campo_harmonico.py
--rw-r--r--   0        0        0     1314 2023-02-05 08:58:14.238745 notas_musicais-0.2.0/notas_musicais/cli.py
--rw-r--r--   0        0        0     2827 2023-02-06 14:14:12.149522 notas_musicais-0.2.0/notas_musicais/escalas.py
--rw-r--r--   0        0        0     1639 2023-02-14 06:56:32.980773 notas_musicais-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9446 1970-01-01 00:00:00.000000 notas_musicais-0.2.0/setup.py
--rw-r--r--   0        0        0     9451 1970-01-01 00:00:00.000000 notas_musicais-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      256 2023-02-14 06:46:12.366404 notas_musicais-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8600 2023-06-16 18:12:24.370596 notas_musicais-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-16 18:09:17.300607 notas_musicais-0.2.1/notas_musicais/__init__.py
+-rw-r--r--   0        0        0     2951 2023-02-06 14:23:53.892679 notas_musicais-0.2.1/notas_musicais/acordes.py
+-rw-r--r--   0        0        0     2242 2023-04-06 05:31:25.586178 notas_musicais-0.2.1/notas_musicais/campo_harmonico.py
+-rw-r--r--   0        0        0     2309 2023-06-16 18:08:27.413943 notas_musicais-0.2.1/notas_musicais/cli.py
+-rw-r--r--   0        0        0     2838 2023-04-06 05:34:59.990908 notas_musicais-0.2.1/notas_musicais/escalas.py
+-rw-r--r--   0        0        0     1639 2023-06-16 18:09:28.410606 notas_musicais-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9635 1970-01-01 00:00:00.000000 notas_musicais-0.2.1/PKG-INFO
```

### Comparing `notas_musicais-0.2.0/README.md` & `notas_musicais-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <img src="https://notas-musicais.readthedocs.io/en/latest/assets/logo.png" width="200">
 
 # Notas musicais
 [![Documentation Status](https://readthedocs.org/projects/notas-musicais/badge/?version=latest)](https://notas-musicais.readthedocs.io/en/latest/?badge=latest)
-![CI](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml/badge.svg)
+[![CI](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml)
 [![codecov](https://codecov.io/gh/dunossauro/notas-musicais/branch/main/graph/badge.svg?token=OVQQF4IQY2)](https://codecov.io/gh/dunossauro/notas-musicais)
+[![PyPI version](https://badge.fury.io/py/notas-musicais.svg)](https://badge.fury.io/py/notas-musicais)
 
 Notas musicais é um CLI para ajudar na formação de escalas, acordes e campos harmônicos.
 
 Toda a aplicação é baseada em um comando chamado `notas-musicais`. Esse comando tem um subcomando relacionado a cada ação que a aplicação pode realizar. Como `escalas`, `acordes` e `campo-harmonico`
 
 ## Instalação
 
@@ -19,15 +20,15 @@
 
 Embora isso seja somente uma recomendação! Você também pode instalar o projeto com o gerenciador de sua preferência. Como o pip:
 
 ```bash
 pip install notas-musicais
 ```
 
-## como usar?
+## Como usar?
 
 ### Escalas
 
 Você pode chamar as escalas via linha de comando. Por exemplo:
 
 
 ```bash
```

### Comparing `notas_musicais-0.2.0/notas_musicais/acordes.py` & `notas_musicais-0.2.1/notas_musicais/acordes.py`

 * *Files identical despite different names*

### Comparing `notas_musicais-0.2.0/notas_musicais/campo_harmonico.py` & `notas_musicais-0.2.1/notas_musicais/campo_harmonico.py`

 * *Files identical despite different names*

### Comparing `notas_musicais-0.2.0/notas_musicais/escalas.py` & `notas_musicais-0.2.1/notas_musicais/escalas.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Attributes:
    ESCALAS: Escalas implementadas usando a notação de inteiros
    NOTAS: Notas musicais
 
 # ESCALAS
 
-A escalas estão implementadas em uma constande chamada `ESCALAS`. Que é um dicionário onde as chaves são as escalas. Se quiser ver todas as escalas implementadas pode usar:
+As escalas estão implementadas em uma constante chamada `ESCALAS`. Que é um dicionário onde as chaves são os nomes das escalas. Se quiser ver todas as escalas implementadas pode usar:
 
 ```py title="No seu shell interativo"
 >>> from notas_musicais.escalas import ESCALAS
 >>> ESCALAS
 {'maior': (0, 2, 4, 5, 7, 9, 11), 'menor': (0, 2, 3, 5, 7, 8, 10)...}
 
 ```
@@ -21,15 +21,15 @@
 tip: Dica!
     Você pode contribuir com novas escalas usando a notação inteira:
     [Escalas wikipedia](https://en.wikipedia.org/wiki/List_of_musical_scales_and_modes).
     Todos os Pull Requests serão bem vindos! :heart:
 
 # NOTAS
 
-As notas estão sendo definidas em uma contasnte `NOTAS`. Foi optado por menter somente as notas no formato Natural e o Sustenido (#) para a simplificação do fluxo de trabalho. Embora não esteja totalmente correto. Para ver as 12 notas você pode:
+As notas estão sendo definidas em uma constante `NOTAS`. Foi optado por menter somente as notas no formato Natural e o Sustenido (#) para a simplificação do fluxo de trabalho. Embora não esteja totalmente correto. Para ver as 12 notas você pode:
 
 ```py title="No seu shell interativo"
 >>> from notas_musicais.escalas import NOTAS
 >>> NOTAS
 ['C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B']
 
 ```
```

### Comparing `notas_musicais-0.2.0/pyproject.toml` & `notas_musicais-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notas-musicais"
-version = "0.2.0"
+version = "0.2.1"
 description = "Notas musicais é um CLI para ajudar na formação de escalas, acordes e campos harmônicos"
 license = "BeerWare"
 authors = ["dunossauro <mendesxeduardo@gmail.com>"]
 readme = "README.md"
 packages = [{include = "notas_musicais"}]
 classifiers = [
     "Topic :: Education",
@@ -21,15 +21,15 @@
 "Doação" = "https://apoia.se/livedepython"
 
 
 [tool.poetry.scripts]
 notas-musicais = "notas_musicais.cli:app"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 typer = "^0.7.0"
 rich = "^13.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 blue = "^0.9.1"
```

### Comparing `notas_musicais-0.2.0/PKG-INFO` & `notas_musicais-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: notas-musicais
-Version: 0.2.0
+Version: 0.2.1
 Summary: Notas musicais é um CLI para ajudar na formação de escalas, acordes e campos harmônicos
 License: Beerware
 Author: dunossauro
 Author-email: mendesxeduardo@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Requires-Dist: rich (>=13.2.0,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/dunossauro/notas-musicais/issues
 Project-URL: Código, https://github.com/dunossauro/notas-musicais
 Project-URL: Documentação, https://notas-musicais.readthedocs.io/en/latest/
 Project-URL: Doação, https://apoia.se/livedepython
 Description-Content-Type: text/markdown
 
 <img src="https://notas-musicais.readthedocs.io/en/latest/assets/logo.png" width="200">
 
 # Notas musicais
 [![Documentation Status](https://readthedocs.org/projects/notas-musicais/badge/?version=latest)](https://notas-musicais.readthedocs.io/en/latest/?badge=latest)
-![CI](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml/badge.svg)
+[![CI](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/dunossauro/notas-musicais/actions/workflows/pipeline.yaml)
 [![codecov](https://codecov.io/gh/dunossauro/notas-musicais/branch/main/graph/badge.svg?token=OVQQF4IQY2)](https://codecov.io/gh/dunossauro/notas-musicais)
+[![PyPI version](https://badge.fury.io/py/notas-musicais.svg)](https://badge.fury.io/py/notas-musicais)
 
 Notas musicais é um CLI para ajudar na formação de escalas, acordes e campos harmônicos.
 
 Toda a aplicação é baseada em um comando chamado `notas-musicais`. Esse comando tem um subcomando relacionado a cada ação que a aplicação pode realizar. Como `escalas`, `acordes` e `campo-harmonico`
 
 ## Instalação
 
@@ -43,15 +44,15 @@
 
 Embora isso seja somente uma recomendação! Você também pode instalar o projeto com o gerenciador de sua preferência. Como o pip:
 
 ```bash
 pip install notas-musicais
 ```
 
-## como usar?
+## Como usar?
 
 ### Escalas
 
 Você pode chamar as escalas via linha de comando. Por exemplo:
 
 
 ```bash
```

