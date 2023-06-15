# Comparing `tmp/rclone-python-0.1.5.tar.gz` & `tmp/rclone-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.5.tar", last modified: Fri May 26 21:20:29 2023, max compression
+gzip compressed data, was "rclone-python-0.1.6.tar", last modified: Thu Jun 15 23:04:22 2023, max compression
```

## Comparing `rclone-python-0.1.5.tar` & `rclone-python-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.191297 rclone-python-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 21:20:16.000000 rclone-python-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 21:20:29.187297 rclone-python-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-26 21:20:16.000000 rclone-python-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.187297 rclone-python-0.1.5/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-26 21:20:16.000000 rclone-python-0.1.5/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:20:29.187297 rclone-python-0.1.5/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 21:20:29.000000 rclone-python-0.1.5/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:20:29.191297 rclone-python-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-26 21:20:16.000000 rclone-python-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.088369 rclone-python-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 23:04:10.000000 rclone-python-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-15 23:04:22.088369 rclone-python-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-15 23:04:10.000000 rclone-python-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.084369 rclone-python-0.1.6/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.088369 rclone-python-0.1.6/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:04:22.088369 rclone-python-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 23:04:10.000000 rclone-python-0.1.6/setup.py
```

### Comparing `rclone-python-0.1.5/LICENSE` & `rclone-python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.5/PKG-INFO` & `rclone-python-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.5/README.md` & `rclone-python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.5/rclone_python/rclone.py` & `rclone-python-0.1.6/rclone_python/rclone.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,131 +11,216 @@
 from rclone_python.remote_types import RemoteTypes
 
 
 def __check_installed(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if not is_installed():
-            raise Exception('rclone is not installed on this system. Please install it here: https://rclone.org/')
+            raise Exception(
+                "rclone is not installed on this system. Please install it here: https://rclone.org/"
+            )
 
         return func(*args, **kwargs)
 
     return wrapper
 
 
 def is_installed() -> bool:
     """
     :return: True if rclone is correctly installed on the system.
     """
-    return which('rclone') is not None
+    return which("rclone") is not None
 
 
 @__check_installed
 def about(remote_name: str):
     """
     Executes the rclone about command and returns the retrieved json as a dictionary.
     :param remote_name: The name of the remote to examine.
     :return: Dictionary with remote properties.
     """
-    if not remote_name.endswith(':'):
+    if not remote_name.endswith(":"):
         # if the remote name missed the colon manually add it.
-        remote_name += ':'
+        remote_name += ":"
 
-    process = utils.run_cmd(f'rclone about {remote_name} --json')
+    process = utils.run_cmd(f"rclone about {remote_name} --json")
 
     if process.returncode == 0:
         return json.loads(process.stdout)
     else:
-        raise Exception(f'An error occurred while executing the about command: {process.stderr}')
+        raise Exception(
+            f"An error occurred while executing the about command: {process.stderr}"
+        )
 
 
 @__check_installed
 def check_remote_existing(remote_name: str) -> bool:
     """
     Returns True, if the specified rclone remote is already configured.
     :param remote_name: The name of the remote to check.
     :return: True if the remote exists, False otherwise.
     """
     # get the available remotes
     remotes = get_remotes()
 
     # add the trailing ':' if it is missing
-    if not remote_name.endswith(':'):
-        remote_name = f'{remote_name}:'
+    if not remote_name.endswith(":"):
+        remote_name = f"{remote_name}:"
 
     return remote_name in remotes
 
 
 @__check_installed
-def create_remote(remote_name, remote_type: Union[str, RemoteTypes], client_id=None, client_secret=None):
+def create_remote(
+    remote_name: str,
+    remote_type: Union[str, RemoteTypes],
+    client_id: Union[str, None] = None,
+    client_secret: Union[str, None] = None,
+    **kwargs,
+):
+    """Creates a new remote with name, type and options.
+
+    Args:
+        remote_name (str): Name of the new remote.
+        remote_type (Union[str, RemoteTypes]): The type of the remote (e.g. "onedrive", RemoteTypes.dropbox, ...)
+        client_id (str, optional): OAuth Client Id.
+        client_secret (str, optional): OAuth Client Secret.
+        **kwargs: Additional key value pairs that can be used with the "rclone config create" command.
+    """
     if isinstance(remote_type, RemoteTypes):
         remote_type = remote_type.value
 
     if not check_remote_existing(remote_name):
         # set up the selected cloud
-        command = f"rclone config create \"{remote_name}\" {remote_type}"
+        command = f'rclone config create "{remote_name}" "{remote_type}"'
 
         if client_id and client_secret:
-            logging.info('Using the provided client id and client secret.')
+            logging.info("Using the provided client id and client secret.")
 
-            command += f" --{remote_type}-client-id \"{client_id}\"" \
-                       f" --{remote_type}-client-secret \"{client_secret}\""
+            kwargs["client_id"] = client_id
+            kwargs["client_secret"] = client_secret
         else:
-            logging.warning('The drive client id and the client secret have not been set. Using defaults.')
+            logging.warning(
+                "The drive client id and the client secret have not been set. Using defaults."
+            )
+
+        # add the options as key-value pairs
+        for key, value in kwargs.items():
+            command += f' {key}="{value}"'
+
         # run the setup command
         process = utils.run_cmd(command)
 
         if process.returncode != 0:
             raise Exception(process.stderr)
     else:
-        raise Exception(f'A rclone remote with the name \'{remote_name}\' already exists!')
+        raise Exception(
+            f"A rclone remote with the name '{remote_name}' already exists!"
+        )
 
 
-def copy(in_path: str, out_path: str, ignore_existing=False, show_progress=True,
-         listener: Callable[[Dict], None] = None, args=None):
+def copy(
+    in_path: str,
+    out_path: str,
+    ignore_existing=False,
+    show_progress=True,
+    listener: Callable[[Dict], None] = None,
+    args=None,
+):
     """
     Copies a file or a directory from a src path to a destination path.
     :param in_path: The source path to use. Specify the remote with 'remote_name:path_on_remote'
     :param out_path: The destination path to use. Specify the remote with 'remote_name:path_on_remote'
     :param ignore_existing: If True, all existing files are ignored and not overwritten.
     :param show_progress: If true, show a progressbar.
     :param listener: An event-listener that is called with every update of rclone.
     :param args: List of additional arguments/ flags.
     """
     if args is None:
         args = []
 
-    _copy_move(in_path, out_path, ignore_existing=ignore_existing, move_files=False, show_progress=show_progress,
-               listener=listener, args=args)
-
-
-def move(in_path: str, out_path: str, ignore_existing=False, show_progress=True,
-         listener: Callable[[Dict], None] = None, args=None):
+    _rclone_transfer_operation(
+        in_path,
+        out_path,
+        ignore_existing=ignore_existing,
+        command="rclone copyto",
+        command_descr="Copying",
+        show_progress=show_progress,
+        listener=listener,
+        args=args,
+    )
+
+
+def move(
+    in_path: str,
+    out_path: str,
+    ignore_existing=False,
+    show_progress=True,
+    listener: Callable[[Dict], None] = None,
+    args=None,
+):
     """
     Moves a file or a directory from a src path to a destination path.
     :param in_path: The source path to use. Specify the remote with 'remote_name:path_on_remote'
     :param out_path: The destination path to use. Specify the remote with 'remote_name:path_on_remote'
     :param ignore_existing: If True, all existing files are ignored and not overwritten.
     :param show_progress: If true, show a progressbar.
     :param listener: An event-listener that is called with every update of rclone.
     :param args: List of additional arguments/ flags.
     """
     if args is None:
         args = []
 
-    _copy_move(in_path, out_path, ignore_existing=ignore_existing, move_files=True, show_progress=show_progress,
-               listener=listener, args=args)
+    _rclone_transfer_operation(
+        in_path,
+        out_path,
+        ignore_existing=ignore_existing,
+        command="rclone move",
+        command_descr="Moving",
+        show_progress=show_progress,
+        listener=listener,
+        args=args,
+    )
+
+
+def sync(
+    src_path: str,
+    dest_path: str,
+    show_progress=True,
+    listener: Callable[[Dict], None] = None,
+    args=None,
+):
+    """
+    Sync the source to the destination, changing the destination only. Doesn't transfer files that are identical on source and destination, testing by size and modification time or MD5SUM.
+    :param in_path: The source path to use. Specify the remote with 'remote_name:path_on_remote'
+    :param out_path: The destination path to use. Specify the remote with 'remote_name:path_on_remote'
+    :param show_progress: If true, show a progressbar.
+    :param listener: An event-listener that is called with every update of rclone.
+    :param args: List of additional arguments/ flags.
+    """
+    if args is None:
+        args = []
+
+    _rclone_transfer_operation(
+        src_path,
+        dest_path,
+        command="rclone sync",
+        command_descr="Syncing",
+        show_progress=show_progress,
+        listener=listener,
+        args=args,
+    )
 
 
 @__check_installed
 def get_remotes() -> List[str]:
     """
     :return: A list of all available remotes.
     """
-    command = 'rclone listremotes'
+    command = "rclone listremotes"
     remotes = utils.run_cmd(command).stdout.split()
     if remotes is None:
         remotes = []
 
     return remotes
 
 
@@ -148,18 +233,19 @@
     """
     if args is None:
         args = []
 
     command = f'rclone purge "{path}"'
     process = utils.run_cmd(command, args)
     if process.returncode == 0:
-        logging.info(f'Successfully purged {path}')
+        logging.info(f"Successfully purged {path}")
     else:
         raise Exception(
-            f'Purging path \"{path}\" failed with error message:\n{process.stderr}')
+            f'Purging path "{path}" failed with error message:\n{process.stderr}'
+        )
 
 
 @__check_installed
 def delete(path: str, args=None):
     """
     Deletes a file or a folder. When deleting a folder, all the files in it and it's subdirectories are removed,
     but not the folder structure itself.
@@ -169,22 +255,29 @@
     if args is None:
         args = []
 
     command = f'rclone delete "{path}"'
     process = utils.run_cmd(command, args)
 
     if process.returncode == 0:
-        logging.info(f'Successfully deleted {path}')
+        logging.info(f"Successfully deleted {path}")
     else:
-        raise Exception(f'Deleting path \"{path}\" failed with error message:\n{process.stderr}')
+        raise Exception(
+            f'Deleting path "{path}" failed with error message:\n{process.stderr}'
+        )
 
 
 @__check_installed
-def ls(path: str, max_depth: Union[int, None] = None, dirs_only=False, files_only=False, args=None) -> \
-        List[Dict[str, Union[int, str]]]:
+def ls(
+    path: str,
+    max_depth: Union[int, None] = None,
+    dirs_only=False,
+    files_only=False,
+    args=None,
+) -> List[Dict[str, Union[int, str]]]:
     """
     Lists the files in a directory.
     :param path: The path to the folder that should be examined.
     :param max_depth: The maximum depth for file search. If max_depth=1 only the files in the selected folder but not
     in its subdirectories will be included.
     :param files_only: If true only files will be returned.
     :param dirs_only: If true, only dirs will be returned.
@@ -198,132 +291,164 @@
 
     # add optional parameters
     if max_depth is not None:
         args.append(f"--max-depth {max_depth}")
     if dirs_only:
         args.append(f"--dirs-only")
     if files_only:
-        args.append('--files-only')
+        args.append("--files-only")
 
     process = utils.run_cmd(command, args)
 
     if process.returncode == 0:
         return json.loads(process.stdout)
     else:
-        raise Exception(f'ls operation on {path} failed with {process.stderr}')
+        raise Exception(f"ls operation on {path} failed with {process.stderr}")
 
 
 @__check_installed
-def _copy_move(in_path: str, out_path: str, ignore_existing=False, move_files=False, show_progress=True,
-               listener: Callable[[Dict], None] = None, args=None):
+def _rclone_transfer_operation(
+    in_path: str,
+    out_path: str,
+    command: str,
+    command_descr: str,
+    ignore_existing=False,
+    show_progress=True,
+    listener: Callable[[Dict], None] = None,
+    args=None,
+):
+    """Executes the rclone transfer operation (e.g. copyto, move, ...) and displays the progress of every individual file.
+
+    Args:
+        in_path (str): The source path to use. Specify the remote with 'remote_name:path_on_remote'
+        out_path (str): The destination path to use. Specify the remote with 'remote_name:path_on_remote'
+        command (str): The rclone command to execute (e.g. rclone copyto)
+        command_descr (str): The description to this command that should be displayed.
+        ignore_existing (bool, optional): If True, all existing files are ignored and not overwritten.
+        show_progress (bool, optional): If true, show a progressbar.
+        listener (Callable[[Dict], None], optional): An event-listener that is called with every update of rclone.
+        args: List of additional arguments/ flags.
+    """
     if args is None:
         args = []
 
-    if move_files:
-        command = f'rclone move'
-        prog_title = f'Moving'
-    else:
-        command = f'rclone copyto'
-        prog_title = f'Copying'
-
-    prog_title += f" [bold magenta]{utils.shorten_filepath(in_path, 20)}[/bold magenta] to [bold magenta]{utils.shorten_filepath(out_path, 20)}"
+    prog_title = f"{command_descr} [bold magenta]{utils.shorten_filepath(in_path, 20)}[/bold magenta] to [bold magenta]{utils.shorten_filepath(out_path, 20)}"
 
     # add global rclone flags
     if ignore_existing:
-        command += ' --ignore-existing'
-    command += ' --progress'
+        command += " --ignore-existing"
+    command += " --progress"
 
     # in path
     command += f' "{in_path}"'
     # out path
     command += f' "{out_path}"'
 
     # optional named arguments/flags
     command += utils.args2string(args)
 
     # execute the upload command
-    process = _rclone_progress(command, prog_title, listener=listener, show_progress=show_progress)
+    process = _rclone_progress(
+        command, prog_title, listener=listener, show_progress=show_progress
+    )
 
     if process.wait() == 0:
-        logging.info('Cloud upload completed.')
+        logging.info("Cloud upload completed.")
     else:
         _, err = process.communicate()
-        raise Exception(f'Copy/Move operation from {in_path} to {out_path}'
-                        f' failed with error message:\n{err.decode("utf-8")}')
-
+        raise Exception(
+            f"Copy/Move operation from {in_path} to {out_path}"
+            f' failed with error message:\n{err.decode("utf-8")}'
+        )
 
-def _rclone_progress(command: str, pbar_title: str, stderr=subprocess.PIPE, show_progress=True,
-                     listener: Callable[[Dict], None] = None) -> subprocess.Popen:
-    process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=stderr, shell=True)
 
+def _rclone_progress(
+    command: str,
+    pbar_title: str,
+    stderr=subprocess.PIPE,
+    show_progress=True,
+    listener: Callable[[Dict], None] = None,
+) -> subprocess.Popen:
     buffer = ""
     pbar = None
     total_progress_id = None
     subprocesses = {}
 
     if show_progress:
         pbar, total_progress_id = utils.create_progress_bar(pbar_title)
 
+    process = subprocess.Popen(
+        command, stdout=subprocess.PIPE, stderr=stderr, shell=True
+    )
+    for line in iter(process.stdout.readline, b""):
+        var = line.decode()
+
+        valid, update_dict = _extract_rclone_progress(buffer)
+
+        if valid:
+            if show_progress:
+                utils.update_tasks(pbar, total_progress_id, update_dict, subprocesses)
+
+            # call the listener
+            if listener:
+                listener(update_dict)
 
-    for c in iter(lambda: process.stdout.read(1), b''):
-        var = c.decode('utf-8', 'ignore')
-        if '\n' not in var:
-            buffer += var
+            # reset the buffer
+            buffer = ""
         else:
-            valid, update_dict = _extract_rclone_progress(buffer)
-
-            if valid:
-                if show_progress:
-                    utils.update_tasks(pbar, total_progress_id, update_dict, subprocesses)
-
-                # call the listener
-                if listener:
-                    listener(update_dict)
-
-                # reset the buffer
-                buffer = ""
+            # buffer until we
+            buffer += var
 
     if show_progress:
         utils.complete_task(total_progress_id, pbar)
+        for _, task_id in subprocesses.items():
+            # hide all subprocesses
+            pbar.update(task_id=task_id, visible=False)
         pbar.stop()
 
     return process
 
+
 def _extract_rclone_progress(buffer: str) -> Tuple[bool, Union[Dict[str, Any], None]]:
     # matcher that checks if the progress update block is completely buffered yet (defines start and stop)
     # it gets the sent bits, total bits, progress, transfer-speed and eta
     reg_transferred = re.findall(
-        r'Transferred:\s+(\d+.\d+ \w+) \/ (\d+.\d+ \w+), (\d{1,3})%, (\d+.\d+ \w+\/\w+), ETA (\S+)',
-        buffer)
+        r"Transferred:\s+(\d+.\d+ \w+) \/ (\d+.\d+ \w+), (\d{1,3})%, (\d+.\d+ \w+\/\w+), ETA (\S+)",
+        buffer,
+    )
 
     if reg_transferred:  # transferred block is completely buffered
         # get the progress of the individual files
         # matcher gets the currently transferring files and their individual progress
         # returns list of tuples: (name, progress, file_size, unit)
-        prog_transfering = []
-        prog_regex = re.findall(r'\* +(\S+):[ ]+(\d{1,2})% \/(\d+.\d+)([a-zA-Z]+),', buffer)
+        prog_transferring = []
+        prog_regex = re.findall(
+            r"\* +(\S+):[ ]+(\d{1,2})% \/(\d+.\d+)([a-zA-Z]+),", buffer
+        )
         for item in prog_regex:
-            prog_transfering.append(
+            prog_transferring.append(
                 (
                     item[0],
                     int(item[1]),
                     float(item[2]),
                     # the suffix B of the unit is missing for subprocesses
-                    item[3] + "B",  
+                    item[3] + "B",
                 )
             )
 
-        out = {'prog_transferring': prog_transfering}
+        out = {"prog_transferring": prog_transferring}
         sent_bits, total_bits, progress, transfer_speed_str, eta = reg_transferred[0]
-        out['progress'] = float(progress.strip())
-        out['total_bits'] = float(re.findall(r'\d+.\d+', total_bits)[0])
-        out['sent_bits'] = float(re.findall(r'\d+.\d+', sent_bits)[0])
-        out['unit_sent'] = re.findall(r'[a-zA-Z]+', sent_bits)[0]
-        out['unit_total'] = re.findall(r'[a-zA-Z]+', total_bits)[0]
-        out['transfer_speed'] = float(re.findall(r'\d+.\d+', transfer_speed_str)[0])
-        out['transfer_speed_unit'] = re.findall(r'[a-zA-Z]+/[a-zA-Z]+', transfer_speed_str)[0]
-        out['eta'] = eta
+        out["progress"] = float(progress.strip())
+        out["total_bits"] = float(re.findall(r"\d+.\d+", total_bits)[0])
+        out["sent_bits"] = float(re.findall(r"\d+.\d+", sent_bits)[0])
+        out["unit_sent"] = re.findall(r"[a-zA-Z]+", sent_bits)[0]
+        out["unit_total"] = re.findall(r"[a-zA-Z]+", total_bits)[0]
+        out["transfer_speed"] = float(re.findall(r"\d+.\d+", transfer_speed_str)[0])
+        out["transfer_speed_unit"] = re.findall(
+            r"[a-zA-Z]+/[a-zA-Z]+", transfer_speed_str
+        )[0]
+        out["eta"] = eta
 
         return True, out
 
     else:
         return False, None
```

### Comparing `rclone-python-0.1.5/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.6/rclone_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.5/setup.py` & `rclone-python-0.1.6/setup.py`

 * *Files identical despite different names*

