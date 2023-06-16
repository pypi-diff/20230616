# Comparing `tmp/storage_device_managers-0.11.1.tar.gz` & `tmp/storage_device_managers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage_device_managers-0.11.1.tar", max compression
+gzip compressed data, was "storage_device_managers-0.9.0.tar", max compression
```

## Comparing `storage_device_managers-0.11.1.tar` & `storage_device_managers-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35106 2023-06-15 19:36:56.857826 storage_device_managers-0.11.1/LICENSE
--rw-r--r--   0        0        0     1250 2023-06-16 01:31:22.029633 storage_device_managers-0.11.1/pyproject.toml
--rw-r--r--   0        0        0      801 2023-06-16 01:30:54.473618 storage_device_managers-0.11.1/src/storage_device_managers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 20:47:57.614397 storage_device_managers-0.11.1/src/storage_device_managers/py.typed
--rw-r--r--   0        0        0    10724 2023-06-16 01:30:54.473618 storage_device_managers-0.11.1/src/storage_device_managers/storage_device_managers.py
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 storage_device_managers-0.11.1/PKG-INFO
+-rw-r--r--   0        0        0    35106 2023-06-15 19:36:56.857826 storage_device_managers-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1249 2023-06-15 21:36:15.761780 storage_device_managers-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-06-15 20:47:57.614397 storage_device_managers-0.9.0/src/storage_device_managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 20:47:57.614397 storage_device_managers-0.9.0/src/storage_device_managers/py.typed
+-rw-r--r--   0        0        0     8726 2023-06-15 21:31:36.242303 storage_device_managers-0.9.0/src/storage_device_managers/storage_device_managers.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 storage_device_managers-0.9.0/PKG-INFO
```

### Comparing `storage_device_managers-0.11.1/LICENSE` & `storage_device_managers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `storage_device_managers-0.11.1/pyproject.toml` & `storage_device_managers-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "storage-device-managers"
-version = "0.11.1"
+version = "0.9.0"
 description = "Helpful context managers for managing decryption and mounts of storage devices"
 authors = ["Max Görner <max@familie-goerner.eu>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 loguru = "^0.7.0"
```

### Comparing `storage_device_managers-0.11.1/src/storage_device_managers/__init__.py` & `storage_device_managers-0.9.0/src/storage_device_managers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from importlib import metadata
 
 from .storage_device_managers import (
     InvalidDecryptedDevice,
     ValidCompressions,
-    chown,
     close_decrypted_device,
     decrypted_device,
     encrypt_device,
     generate_passcmd,
     get_mounted_devices,
     is_mounted,
     mkfs_btrfs,
@@ -16,23 +15,22 @@
     open_encrypted_device,
     symbolic_link,
     unmount_device,
 )
 
 __version__ = metadata.version(__name__)
 __all__ = [
-    "chown",
+    "InvalidDecryptedDevice",
+    "ValidCompressions",
     "close_decrypted_device",
     "decrypted_device",
     "encrypt_device",
     "generate_passcmd",
     "get_mounted_devices",
-    "InvalidDecryptedDevice",
     "is_mounted",
     "mkfs_btrfs",
     "mount_btrfs_device",
     "mounted_device",
     "open_encrypted_device",
     "symbolic_link",
     "unmount_device",
-    "ValidCompressions",
 ]
```

### Comparing `storage_device_managers-0.11.1/src/storage_device_managers/storage_device_managers.py` & `storage_device_managers-0.9.0/src/storage_device_managers/storage_device_managers.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import contextlib
 import enum
 import secrets
 import string
 from collections import defaultdict
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Iterator, Optional, Union
+from typing import Iterator, Optional
 from uuid import UUID, uuid4
 
 import shell_interface as sh
 from loguru import logger
 
 
 class InvalidDecryptedDevice(ValueError):
@@ -80,15 +80,15 @@
         logger.success(
             f"Verschlüsselung des Speichermediums {device} erfolgreich geschlossen."
         )
 
 
 @contextlib.contextmanager
 def mounted_device(
-    device: Path, compression: Optional[ValidCompressions] = None
+    device: Path, compression: Optional[ValidCompressions]
 ) -> Iterator[Path]:
     """Mount a given BtrFS device
 
     Given a path pointing to a file-like object, this context manager will
     mount it to some temporary directory and return its path. Upon exit, the
     file-like object is unmounted again.
 
@@ -164,15 +164,15 @@
         # all, the aimed for state has been reached.
         rm_cmd: sh.StrPathList = ["sudo", "rm", "-f", absolute_dest]
         sh.run_cmd(cmd=rm_cmd)
         logger.success(f"Symlink von {src} nach {dest} erfolgreich entfernt.")
 
 
 def mount_btrfs_device(
-    device: Path, mount_dir: Path, compression: Optional[ValidCompressions] = None
+    device: Path, mount_dir: Path, compression: Optional[ValidCompressions]
 ) -> None:
     cmd: sh.StrPathList = [
         "sudo",
         "mount",
         device,
         mount_dir,
     ]
@@ -238,41 +238,32 @@
     if device.parent != Path("/dev/mapper"):
         raise InvalidDecryptedDevice
     map_name = device.name
     close_cmd = ["sudo", "cryptsetup", "close", map_name]
     sh.run_cmd(cmd=close_cmd)
 
 
-def encrypt_device(
-    device: Path, password_cmd: str, *, fast_and_insecure: bool = False
-) -> UUID:
+def encrypt_device(device: Path, password_cmd: str) -> UUID:
     """Encrypt a device
 
     This function will encrypt a device. The device can be any valid file-like
     object like real devices in `/dev/` or suitably sized files in $HOME.
 
     In order to retrieve the necessary password, the input `password_cmd` is
     executed in a subshell and its STDOUT used as password. Therefore, DO NOT
     USE UNTRUSTED `password_cmd`!
 
-    The argument `fast_and_insecure` is for internal use only. If set to
-    `True`, `cryptsetup`'s PBKDF is configured to be as fast as possible. This
-    renders it useless for any real-world use cases but is extremely helpful in
-    the test suite.
-
     In order to obtain a safe password_cmd, refer to `generate_passcmd`.
 
     Parameters:
     -----------
     device
         file-like object to be encrypted
     password_cmd
         Shell command that prints the password to be used to STDOUT
-    fast_and_insecure
-        for internal use only
 
     Returns:
     --------
     UUID
         UUID of the new LUKS partition
     """
     new_uuid = uuid4()
@@ -280,26 +271,14 @@
         "sudo",
         "cryptsetup",
         "luksFormat",
         "--uuid",
         str(new_uuid),
         device,
     ]
-    if fast_and_insecure:
-        format_cmd.extend(
-            [
-                "--pbkdf-force-iterations",
-                "4",
-                "--pbkdf-memory",
-                "32",
-                "--pbkdf-parallel",
-                "1",
-            ]
-        )
-
     sh.pipe_pass_cmd_to_real_cmd(pass_cmd=password_cmd, command=format_cmd)
     return new_uuid
 
 
 def mkfs_btrfs(device: Path) -> None:
     """Format device with BtrFS
 
@@ -322,54 +301,7 @@
     str
         password command producing the password
     """
     n_chars = 16
     alphabet = string.ascii_letters + string.digits
     passphrase = "".join(secrets.choice(alphabet) for _ in range(n_chars))
     return f"echo {passphrase}"
-
-
-def chown(
-    file_or_folder: Path,
-    /,
-    user: Union[int, str],
-    group: Optional[Union[int, str]] = None,
-    *,
-    recursive: bool,
-) -> None:
-    """Change user and group of a device or folder
-
-    This function will change the ownership as specified. It requires root
-    privileges and will ask for them if not available. If no group is given,
-    only the owner is changed.
-
-    If recursive is true, ownership information of all files and folders
-    contained by `file_or_folder` will be adapted.
-
-    If `file_or_folder` points to a file, `recursive` must be `False`.
-    Otherwise a ValueError will be raised.
-
-
-    Parameters:
-    -----------
-    user
-        user ID, either as name or as UID
-    group
-        group ID, either as name or as GID
-    recursive
-        whether or not to change ownership for content
-
-    Raises:
-    --------
-    ValueError
-        if `file_or_folder` is a file but `recursive` is `True`
-    """
-    if file_or_folder.is_file() and recursive:
-        raise ValueError(
-            "First argument must point to a directory if `recursive` is `True`!"
-        )
-
-    user_spec = str(user) if group is None else f"{user}:{group}"
-    chown_cmd: sh.StrPathList = ["sudo", "chown", user_spec, file_or_folder]
-    if recursive is not None:
-        chown_cmd.append("--recursive")
-    sh.run_cmd(cmd=chown_cmd)
```

### Comparing `storage_device_managers-0.11.1/PKG-INFO` & `storage_device_managers-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage-device-managers
-Version: 0.11.1
+Version: 0.9.0
 Summary: Helpful context managers for managing decryption and mounts of storage devices
 License: GPL-3.0-or-later
 Author: Max Görner
 Author-email: max@familie-goerner.eu
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

