# Comparing `tmp/butter_backup-3.2.0.tar.gz` & `tmp/butter_backup-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butter_backup-3.2.0.tar", max compression
+gzip compressed data, was "butter_backup-3.3.0.tar", max compression
```

## Comparing `butter_backup-3.2.0.tar` & `butter_backup-3.3.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0    35106 2021-03-14 19:48:58.215845 butter_backup-3.2.0/LICENSE
--rw-r--r--   0        0        0     1688 2023-02-08 21:00:40.553947 butter_backup-3.2.0/pyproject.toml
--rw-r--r--   0        0        0       73 2022-10-04 09:00:10.876520 butter_backup-3.2.0/src/butter_backup/__init__.py
--rw-r--r--   0        0        0     4971 2022-12-21 00:19:23.284819 butter_backup-3.2.0/src/butter_backup/backup_backends.py
--rw-r--r--   0        0        0     7448 2023-02-08 20:55:41.741844 butter_backup-3.2.0/src/butter_backup/cli.py
--rw-r--r--   0        0        0     5144 2022-10-09 10:28:49.016730 butter_backup-3.2.0/src/butter_backup/config_parser.py
--rw-r--r--   0        0        0     7466 2022-10-09 10:28:49.016730 butter_backup-3.2.0/src/butter_backup/device_managers.py
--rw-r--r--   0        0        0        0 2022-10-04 09:00:10.876520 butter_backup-3.2.0/src/butter_backup/py.typed
--rw-r--r--   0        0        0     1851 2022-10-04 09:00:10.876520 butter_backup-3.2.0/src/butter_backup/shell_interface.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 butter_backup-3.2.0/setup.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 butter_backup-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35106 2021-03-14 19:48:58.215845 butter_backup-3.3.0/LICENSE
+-rw-r--r--   0        0        0     1531 2023-06-16 00:39:14.418292 butter_backup-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2022-10-04 09:00:10.876520 butter_backup-3.3.0/src/butter_backup/__init__.py
+-rw-r--r--   0        0        0     4964 2023-06-16 00:33:58.951231 butter_backup-3.3.0/src/butter_backup/backup_backends.py
+-rw-r--r--   0        0        0     7606 2023-06-16 00:34:04.879213 butter_backup-3.3.0/src/butter_backup/cli.py
+-rw-r--r--   0        0        0     4580 2023-06-16 00:34:04.879213 butter_backup-3.3.0/src/butter_backup/config_parser.py
+-rw-r--r--   0        0        0     2816 2023-06-16 00:39:14.406292 butter_backup-3.3.0/src/butter_backup/device_managers.py
+-rw-r--r--   0        0        0        0 2022-10-04 09:00:10.876520 butter_backup-3.3.0/src/butter_backup/py.typed
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 butter_backup-3.3.0/PKG-INFO
```

### Comparing `butter_backup-3.2.0/LICENSE` & `butter_backup-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `butter_backup-3.2.0/src/butter_backup/backup_backends.py` & `butter_backup-3.3.0/src/butter_backup/backup_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import abc
 import datetime as dt
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Union, overload
 
+import shell_interface as sh
 from loguru import logger
 
 from . import config_parser as cp
-from . import shell_interface as sh
 
 
 class BackupBackend(abc.ABC):
     @abc.abstractmethod
     def do_backup(self, mount_dir: Path) -> None:
         ...
```

### Comparing `butter_backup-3.2.0/src/butter_backup/cli.py` & `butter_backup-3.3.0/src/butter_backup/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import json
 import os
 import sys
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Any, Callable, Optional
 
+import storage_device_managers as sdm
 import typer
 from loguru import logger
 
 from . import __version__
 from . import backup_backends as bb
 from . import config_parser as cp
-from . import device_managers as dm
+from .device_managers import (
+    prepare_device_for_butterbackend,
+    prepare_device_for_resticbackend,
+)
 
 app = typer.Typer()
 DEFAULT_CONFIG_DIR = Path("~/.config/").expanduser()
 DEFAULT_CONFIG_NAME = "butter-backup.cfg"
 
 
 class ValidBackends(enum.Enum):
@@ -50,15 +54,17 @@
 
 
 CONFIG_OPTION = typer.Option(get_default_config_path(), exists=True, dir_okay=False)
 VERBOSITY_OPTION = typer.Option(0, "--verbose", "-v", count=True)
 
 
 @app.command()
-def open(config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION):  # noqa: A001
+def open(  # noqa: A001
+    config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION
+) -> None:
     """
     Öffne alle in der Konfiguration gelisteten Speichermedien
 
     Das Kommando `open` öffnet alle Speichermedien, deren UUID in der
     Konfiguration erwähnt wird.  Für jedes geöffnete Speichermedium wird die
     UUID und der Mount-Zielordner angegeben.
 
@@ -70,50 +76,50 @@
     kann das Speichermedium mit `butter-backup close` wieder entfernt werden.
     """
     setup_logging(verbose)
     configurations = cp.parse_configuration(config.read_text())
     for cfg in configurations:
         if cfg.device().exists():
             mount_dir = Path(mkdtemp())
-            decrypted = dm.open_encrypted_device(cfg.device(), cfg.DevicePassCmd)
-            dm.mount_btrfs_device(
+            decrypted = sdm.open_encrypted_device(cfg.device(), cfg.DevicePassCmd)
+            sdm.mount_btrfs_device(
                 decrypted, mount_dir=mount_dir, compression=cfg.Compression
             )
             typer.echo(f"Speichermedium {cfg.UUID} wurde in {mount_dir} geöffnet.")
 
 
 @app.command()
-def close(config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION):
+def close(config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION) -> None:
     """
     Schließe alle geöffneten Speichermedien
 
     Das Kommando `close` schließt alle gemounteten Speichermedien, deren UUIDs
     in der Konfiguration erwähnt werden. Es ist das Gegenstück des Kommandos
     `open`. Weitere Erklärungen finden sich dort.
     """
     setup_logging(verbose)
     configurations = cp.parse_configuration(config.read_text())
-    mounted_devices = dm.get_mounted_devices()
+    mounted_devices = sdm.get_mounted_devices()
     for cfg in configurations:
         mapped_device = f"/dev/mapper/{cfg.UUID}"
         if cfg.device().exists() and mapped_device in mounted_devices:
             mount_dirs = mounted_devices[mapped_device]
             if len(mount_dirs) != 1:
                 # TODO introduce custom exception
                 raise ValueError(
                     "Got several possible mount points. Expected exactly 1!"
                 )
             mount_dir = mount_dirs.pop()
-            dm.unmount_device(mount_dir)
-            dm.close_decrypted_device(Path(mapped_device))
+            sdm.unmount_device(mount_dir)
+            sdm.close_decrypted_device(Path(mapped_device))
             mount_dir.rmdir()
 
 
 @app.command()
-def backup(config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION):
+def backup(config: Path = CONFIG_OPTION, verbose: int = VERBOSITY_OPTION) -> None:
     """
     Führe Sicherheitskopien durch
 
     Für jedes angeschlossene Speichermedium wird eine Sicherheitskopie gemäß
     der Konfiguration durchgeführt. Das Speichermedium wird hierfür
     entschlüsselt und gemountet. Nachdem die Sicherungskopie durchgeführt
     wurde, wird es wieder vollständig geschlossen.
@@ -133,16 +139,16 @@
     for cfg in configurations:
         if not cfg.device().exists():
             logger.info(
                 f"Speichermedium {cfg.UUID} existiert nicht. Es wird kein Backup angelegt."
             )
             continue
         backend = bb.BackupBackend.from_config(cfg)
-        with dm.decrypted_device(cfg.device(), cfg.DevicePassCmd) as decrypted:
-            with dm.mounted_device(decrypted, cfg.Compression) as mount_dir:
+        with sdm.decrypted_device(cfg.device(), cfg.DevicePassCmd) as decrypted:
+            with sdm.mounted_device(decrypted, cfg.Compression) as mount_dir:
                 backend.do_backup(mount_dir)
 
 
 @app.command()
 def format_device(
     backend: ValidBackends = typer.Argument(...),  # noqa: B008
     device: Path = typer.Argument(  # noqa: B008
@@ -151,15 +157,15 @@
     config_to: Optional[Path] = typer.Option(  # noqa: B008
         None,
         help="Datei, in welche die generierte Konfiguration geschrieben werden"
         " soll. Die angegebene Datei darf nicht existieren. Wenn nicht"
         " angegeben, wird die Konfiguration auf STDOUT ausgegeben.",
     ),
     verbose: int = VERBOSITY_OPTION,
-):
+) -> None:
     """
     Richtet Speichermedium für butter-backup ein
 
     Das angegebene Speichermedium wird vollständig zur Erstellung von
     Sicherheitskopien mit `butter-backup` vorbereitet. Es wird eine
     Konfiguration ausgegeben, die nur noch um die zu sichernden Ordner bzw.
     Dateien ergänzt werden muss.
@@ -178,25 +184,25 @@
     else:
         if config_to.exists():
             raise ValueError(
                 "Zieldatei für ButterBackup-Konfiguration existiert schon!"
             )
         config_writer = config_to.write_text
     formatter = (
-        dm.prepare_device_for_butterbackend
+        prepare_device_for_butterbackend
         if backend == ValidBackends.btrfs_rsync
-        else dm.prepare_device_for_resticbackend
+        else prepare_device_for_resticbackend
     )
     config = formatter(device)
     json_serialisable = json.loads(config.json(exclude_none=True))
     config_writer(json.dumps([json_serialisable], indent=4, sort_keys=True))
 
 
 @app.command()
-def version():
+def version() -> None:
     """Gibt butter-backups aktuelle Version an"""
     typer.echo(__version__)
 
 
 def cli() -> None:
     app()
```

### Comparing `butter_backup-3.2.0/src/butter_backup/config_parser.py` & `butter_backup-3.3.0/src/butter_backup/config_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import enum
 import json
 import sys
 import uuid
 from collections import Counter
 from pathlib import Path
 from typing import ClassVar, Dict, List, Optional, Set, Union
 
@@ -13,58 +12,29 @@
     DirectoryPath,
     Extra,
     FilePath,
     parse_raw_as,
     root_validator,
     validator,
 )
+from storage_device_managers import ValidCompressions
 
 FoldersT = Dict[DirectoryPath, str]
 
 
 def path_aware_btrfs_json_decoding(v, *, default) -> str:
     v["Folders"] = {str(key): val for key, val in v["Folders"].items()}
     return json.dumps(v, default=default)
 
 
 def path_aware_restic_json_decoding(v, *, default) -> str:
     v["FilesAndFolders"] = {str(cur) for cur in v["FilesAndFolders"]}
     return json.dumps(v, default=default)
 
 
-class ValidCompressions(enum.Enum):
-    LZO = "lzo"
-    ZLIB = "zlib"
-    ZLIB1 = "zlib:1"
-    ZLIB2 = "zlib:2"
-    ZLIB3 = "zlib:3"
-    ZLIB4 = "zlib:4"
-    ZLIB5 = "zlib:5"
-    ZLIB6 = "zlib:6"
-    ZLIB7 = "zlib:7"
-    ZLIB8 = "zlib:8"
-    ZLIB9 = "zlib:9"
-    ZSTD = "zstd"
-    ZSTD1 = "zstd:1"
-    ZSTD2 = "zstd:2"
-    ZSTD3 = "zstd:3"
-    ZSTD4 = "zstd:4"
-    ZSTD5 = "zstd:5"
-    ZSTD6 = "zstd:6"
-    ZSTD7 = "zstd:7"
-    ZSTD8 = "zstd:8"
-    ZSTD9 = "zstd:9"
-    ZSTD10 = "zstd:10"
-    ZSTD11 = "zstd:11"
-    ZSTD12 = "zstd:12"
-    ZSTD13 = "zstd:13"
-    ZSTD14 = "zstd:14"
-    ZSTD15 = "zstd:15"
-
-
 class BaseConfig(BaseModel):
     BackupRepositoryFolder: str
     DevicePassCmd: str
     ExcludePatternsFile: Optional[FilePath] = None
     UUID: uuid.UUID
     Compression: Optional[ValidCompressions] = None
```

### Comparing `butter_backup-3.2.0/PKG-INFO` & `butter_backup-3.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: butter-backup
-Version: 3.2.0
+Version: 3.3.0
 Summary: Vollverschlüsselte, pseudoinkrementelle Sicherungskopien leicht gemacht
 License: GPL-3.0-or-later
 Author: Max Görner
 Author-email: max@familie-goerner.eu
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: shell-interface (>=0.10.0,<0.11.0)
+Requires-Dist: storage-device-managers (>=0.10.0,<0.11.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
```

