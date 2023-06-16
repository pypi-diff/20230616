# Comparing `tmp/run_rx-0.0.8.tar.gz` & `tmp/run_rx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.8.tar", max compression
+gzip compressed data, was "run_rx-0.0.9.tar", max compression
```

## Comparing `run_rx-0.0.8.tar` & `run_rx-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.8/README.md
--rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.8/install/.rxignore
--rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.8/install/README.md
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.8/install/python-cpu
--rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.8/install/python-gpu
--rw-r--r--   0        0        0      736 2023-06-09 02:26:40.439644 run_rx-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.8/rx/__main__.py
--rw-r--r--   0        0        0     2850 2023-06-06 23:31:04.918753 run_rx-0.0.8/rx/client/commands/exec.py
--rw-r--r--   0        0        0     3782 2023-06-09 01:08:03.971935 run_rx-0.0.8/rx/client/commands/init.py
--rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.8/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     7016 2023-06-09 02:26:51.137891 run_rx-0.0.8/rx/client/configuration/local.py
--rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.8/rx/client/configuration/remote.py
--rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.8/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     9852 2023-06-09 00:46:28.253468 run_rx-0.0.8/rx/client/login.py
--rw-r--r--   0        0        0     2251 2023-06-09 01:11:45.554956 run_rx-0.0.8/rx/client/menu.py
--rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.8/rx/client/output_handler.py
--rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.8/rx/client/rsync.py
--rw-r--r--   0        0        0     4668 2023-06-08 21:15:48.685289 run_rx-0.0.8/rx/client/trex_client.py
--rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.8/rx/client/user.py
--rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.8/rx/client/worker_client.py
--rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.8/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.8/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.8/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.9/README.md
+-rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.9/install/.rxignore
+-rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.9/install/README.md
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.9/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.9/install/python-gpu
+-rw-r--r--   0        0        0      753 2023-06-16 21:15:22.264232 run_rx-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.9/rx/__main__.py
+-rw-r--r--   0        0        0     2850 2023-06-15 17:17:43.129031 run_rx-0.0.9/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     4059 2023-06-16 19:42:49.623110 run_rx-0.0.9/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.9/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7359 2023-06-16 21:15:30.004669 run_rx-0.0.9/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.9/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.9/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     9852 2023-06-09 00:46:28.253468 run_rx-0.0.9/rx/client/login.py
+-rw-r--r--   0        0        0     2673 2023-06-16 19:40:57.513477 run_rx-0.0.9/rx/client/menu.py
+-rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.9/rx/client/output_handler.py
+-rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.9/rx/client/rsync.py
+-rw-r--r--   0        0        0     4771 2023-06-15 20:17:35.649171 run_rx-0.0.9/rx/client/trex_client.py
+-rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.9/rx/client/user.py
+-rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.9/rx/client/worker_client.py
+-rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.9/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.9/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.9/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 run_rx-0.0.9/PKG-INFO
```

### Comparing `run_rx-0.0.8/LICENSE.txt` & `run_rx-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/README.md` & `run_rx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/pyproject.toml` & `run_rx-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.8"
+version = "0.0.9"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
@@ -24,14 +24,15 @@
 python = "^3.7"
 absl-py = "^1.4.0"
 grpcio = "^1.54.0"
 protobuf = "^4.22.3"
 PyJWT = "^2.6.0"
 requests = "^2.30.0"
 sty = "^1.0.4"
+tqdm = "^4.65.0"
 
 [tool.poetry.scripts]
 rx = 'rx.client.commands.exec:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `run_rx-0.0.8/rx/client/commands/exec.py` & `run_rx-0.0.9/rx/client/commands/exec.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/commands/init.py` & `run_rx-0.0.9/rx/client/commands/init.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,100 +15,108 @@
   'dry-run', False, 'Shows a list of files that would be uploaded by rx init')
 
 
 class InitCommand:
   """Initialize (or reinitialize) the remote."""
 
   def __init__(self):
-    self._cwd = (
-      pathlib.Path(config_base.RX_ROOT.value) if config_base.RX_ROOT.value else
-      pathlib.Path.cwd())
-    self._config = local.find_local_config(self._cwd)
+    if config_base.RX_ROOT.value:
+      rxroot = pathlib.Path(config_base.RX_ROOT.value)
+    else:
+      rxroot = local.find_rxroot(pathlib.Path.cwd())
+
+    if rxroot:
+      self._config_exists = local.get_local_config_path(rxroot).exists()
+      self._user_info_exists = not login.needs_login(rxroot)
+    else:
+      # Fall back on using this dir for rxroot.
+      rxroot = pathlib.Path.cwd()
+      self._config_exists = False
+      self._user_info_exists = False
+    self._rxroot = rxroot
+
+  @property
+  def rxroot(self) -> pathlib.Path:
+    return self._rxroot
 
   def _show_init_message(self):
-    needs_login = login.needs_login(self._cwd)
     steps = []
-    if self._config:
+    if self._config_exists:
       reinit = menu.bool_prompt(
         'Looks like you already have an rx workspace. Would you like to stop '
         'that one\nand start a new one?', 'y')
       if not reinit:
         print('Okay, goodbye!')
         sys.exit(0)
       message = 'Got it. To re-init this workspace, rx will:\n\n'
       steps.append('Shut down your existing virtual machine.')
     else:
       message = 'To set up rx, this command will:\n\n'
-    if needs_login:
+    if not self._user_info_exists:
       steps.append(
         'Create an account for you with rx (or log you into your existing '
         'account).')
     steps.append('Set up a virtual machine on the cloud (on AWS).')
     steps.append(
-      f'Copy over the files in this directory ({self._cwd}) to your\n'
+      f'Copy over the files in this directory ({self._rxroot}) to your\n'
       '   virtual machine.')
     for num, step in enumerate(steps, 1):
       message += f'{num}. {step}\n'
-    if needs_login:
+    if not self._user_info_exists:
       message += (
         '\nWould you like to proceed with logging in/creating an rx account?')
     else:
       message += ('\nWould you like to proceed?')
-    resp = menu.bool_prompt(message, 'y')
-    if resp:
-      local.install_local_files(self._cwd)
-    else:
+    if not menu.bool_prompt(message, 'y'):
       print('Okay, goodbye!')
       sys.exit(0)
 
   def run(self) -> int:
     self._show_init_message()
-    if self._config is None:
-      local.install_local_files(self._cwd)
-    else:
+    if self._config_exists:
       logging.info('Workspace already exists, resetting it.')
     try:
-      needs_login = login.needs_login(self._cwd)
-      self._config = local.create_local_config(self._cwd)
+      config = local.create_local_config(self._rxroot)
       with grpc_helper.get_channel(config_base.TREX_HOST.value) as ch:
-        client = trex_client.Client(ch, self._config)
+        client = trex_client.Client(ch, config)
         if _DRY_RUN.value:
           client.dry_run()
           return 0
-        if needs_login:
+        if not self._user_info_exists:
           ready_to_login = menu.bool_prompt(
             f"""
 Great! First rx will need to open a browser window for you to log in. rx uses
 Google's oauth to associate your email with your rx account.
 
 Press y to continue:""", 'y')
           if not ready_to_login:
             print('Okay, goodbye!')
             return 0
         client.create_user_or_log_in()
 
-        if needs_login:
+        if not self._user_info_exists:
           prefix = 'Next,'
         else:
           prefix = 'Great! First'
-        ready_upload = menu.bool_prompt(
+        ready_to_upload = menu.bool_prompt(
           f"""
 {prefix} rx is going to start a virtual machine in the cloud for your user.
 This is your private machine and is currently free of charge (though limited in
 resources).
 
 The source code in this directory, will be copied to your virtual machine. To
 check what will be uploaded, you can rerun this command with --dry-run and
 modify .rxignore to exclude anything you don't want copied.
 
-Are you sure you want to upload {self._cwd} to the cloud?""", 'y')
-        if not ready_upload:
+Are you sure you want to upload {self._rxroot} to the cloud?""", 'y')
+        if not ready_to_upload:
           print('Okay, goodbye!')
           return 0
-        print('Great! Let\'s get down to business.')
+        if not menu._QUIET.value:
+          print('Great! Let\'s get down to business.')
         return client.init()
     except trex_client.InitError as e:
       sys.stderr.write(f'{e}\n')
       sys.stderr.flush()
       return e.code
 
 if __name__ == '__main__':
```

### Comparing `run_rx-0.0.8/rx/client/configuration/config_base.py` & `run_rx-0.0.9/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/configuration/local.py` & `run_rx-0.0.9/rx/client/configuration/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', None,
   'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
@@ -28,15 +28,15 @@
 
 
 class LocalConfigWriter(config_base.ReadWriteConfig):
   """This holds all of the configuration options that can be determined from
   the local machine."""
 
   def __init__(self, workspace_dir: pathlib.Path):
-    super().__init__(_get_local_config_file(workspace_dir))
+    super().__init__(get_local_config_path(workspace_dir))
     self._workspace_dir = workspace_dir
 
   def setup_remote(self):
     """Sets the "remote" field (and color) for the local config."""
     remote = str(_REMOTE.value if _REMOTE.value else _DEFAULT_REMOTE)
     remote_path = self._workspace_dir / remote
     try:
@@ -61,15 +61,15 @@
     self['color'] = {'r': r, 'g': g, 'b': b}
 
 
 class LocalConfig(config_base.ReadOnlyConfig):
   """Create the local configuration."""
 
   def __init__(self, working_dir: pathlib.Path):
-    super().__init__(_get_local_config_file(working_dir))
+    super().__init__(get_local_config_path(working_dir))
     self._cwd = working_dir
     self.config_dir = self.cwd / config_base.RX_DIR
     self._color = None
 
   @property
   def cwd(self) -> pathlib.Path:
     return self._cwd
@@ -114,23 +114,33 @@
 
   def color_str(self, s: str) -> str:
     color = self['color']
     fg = sty.fg(color['r'], color['g'], color['b'])
     return f'{fg}{s}{sty.rs.fg}'
 
 
-def create_local_config(cwd: pathlib.Path) -> LocalConfig:
+def create_local_config(rxroot: pathlib.Path) -> LocalConfig:
   """Gets or creates .rx directory."""
-  config_dir = _get_local_config_file(cwd).parent
+  _install_local_files(rxroot)
+  config_dir = get_local_config_path(rxroot).parent
   config_dir.mkdir(exist_ok=True, parents=True)
-  with LocalConfigWriter(cwd) as c:
+  with LocalConfigWriter(rxroot) as c:
     c.setup_remote()
-    c['project_name'] = _find_project_name(cwd)
+    c['project_name'] = _find_project_name(rxroot)
     c['rsync_path'] = _get_rsync_path()
-  return LocalConfig(cwd)
+  return LocalConfig(rxroot)
+
+
+def find_rxroot(working_dir: pathlib.Path) -> Optional[pathlib.Path]:
+  """Finds the rxroot, if it exists."""
+  cfg_path = config_base.get_config_dir(working_dir)
+  for parent in cfg_path.parents:
+    if config_base.get_config_dir(parent).exists():
+      return parent
+  return None
 
 
 def find_local_config(working_dir: pathlib.Path) -> Optional[LocalConfig]:
   """Factory to create a config by looking for .rx."""
   cfg_path = config_base.get_config_dir(working_dir)
   for parent in cfg_path.parents:
     if config_base.get_config_dir(parent).exists():
@@ -144,27 +154,27 @@
   return pathlib.Path(__file__).resolve().parent.parent.parent.parent
 
 
 def get_grpc_metadata() -> Tuple[Tuple[str, str]]:
   return (('cv', VERSION),)
 
 
-def install_local_files(cwd: pathlib.Path):
+def _install_local_files(rxroot: pathlib.Path):
   # Output directory.
-  (cwd / 'rx-out').mkdir(exist_ok=True)
+  (rxroot / 'rx-out').mkdir(exist_ok=True)
 
   install_dir = pathlib.Path(get_source_path() / 'install')
 
-  _install_file(install_dir, cwd, IGNORE)
+  _install_file(install_dir, rxroot, IGNORE)
 
-  config_dir = cwd / config_base.RX_DIR
+  config_dir = rxroot / config_base.RX_DIR
   config_dir.mkdir(exist_ok=True, parents=True)
   _install_file(install_dir, config_dir, 'README.md')
 
-  remotes = cwd / _REMOTE_DIR
+  remotes = rxroot / _REMOTE_DIR
   remotes.mkdir(exist_ok=True, parents=True)
 
   # Copy built-in configs.
   _install_file(install_dir, remotes, 'python-cpu')
   _install_file(install_dir, remotes, 'python-gpu')
   # Create soft link.
   default_config = remotes / 'default'
@@ -197,15 +207,15 @@
   for parent in start_dir.parents:
     if (parent / '.git').exists():
       return start_dir.name
   # Maybe we haven't initialized git yet, use out name.
   return start_dir.name
 
 
-def _get_local_config_file(rxroot: pathlib.Path) -> pathlib.Path:
+def get_local_config_path(rxroot: pathlib.Path) -> pathlib.Path:
   """Return .rx/trex-dev.run-rx.com/config/local."""
   return config_base.get_config_dir(rxroot) / 'local'
 
 
 def _install_file(install_dir, config_dir, base_name):
   """Installs a file if it doesn't already exist."""
   source_path = install_dir / base_name
```

### Comparing `run_rx-0.0.8/rx/client/configuration/remote.py` & `run_rx-0.0.9/rx/client/configuration/remote.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/login.py` & `run_rx-0.0.9/rx/client/login.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/menu.py` & `run_rx-0.0.9/rx/client/menu.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,25 @@
 2. Convert the response to the expected type.
 2. Validate the response. If validation fails, go back to 1.
 """
 
 import pathlib
 from typing import Any, Callable, List, Optional
 
+from absl import flags
+
+_QUIET = flags.DEFINE_bool(
+    'quiet', False, 'Don\'t prompt for user confirmation, go with the default '
+    'option automatically')
+
 
 def bool_prompt(prompt: str, default_opt: str = '') -> bool:
+  assert default_opt in ['', 'y', 'n']
+  if _QUIET.value and default_opt:
+    return default_opt == 'y'
   y = 'Y' if default_opt == 'y' else 'y'
   n = 'N' if default_opt == 'n' else 'n'
   response = input(f'{prompt} ({y}/{n}): ')
   if not response:
     response = default_opt
   response = response.lower()
   if response == 'y':
@@ -25,14 +34,16 @@
   print('Please choose "y" or "n".')
   return bool_prompt(prompt)
 
 
 def numbered_options_prompt(
     prompt: str, options: List[Any], default: int = 0) -> int:
   """Prompt with a numbered list of options."""
+  if _QUIET.value:
+    return default
 
   # Setup
   assert options
   print(prompt)
   for i, p in options:
     print(f'{i}: {p}')
   response = input(f'[{default}]: ')
@@ -51,14 +62,16 @@
 
 def path_prompt(
   prompt: str,
   default_path: Optional[pathlib.Path],
   validation: Callable[[Optional[pathlib.Path]], bool] = lambda x: True
 ) -> pathlib.Path:
   """Prompt for filesystem path."""
+  if _QUIET.value and default_path:
+    return default_path
 
   # Setup.
   if default_path:
     response = input(f'{prompt}\n[{default_path}]: ')
   else:
     response = input(f'{prompt}: ')
 
@@ -75,14 +88,17 @@
 
 
 def string_prompt(
   prompt: str,
   default_str: Optional[str] = None,
   validation:  Callable[[Optional[str]], bool] = lambda x: True
 ) -> str:
+  if _QUIET.value and default_str:
+    return default_str
+
   # Setup.
   if default_str:
     response = input(f'{prompt}\n[{default_str}]: ')
   else:
     response = input(f'{prompt}: ')
 
   # Convert.
```

### Comparing `run_rx-0.0.8/rx/client/output_handler.py` & `run_rx-0.0.9/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/rsync.py` & `run_rx-0.0.9/rx/client/rsync.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/trex_client.py` & `run_rx-0.0.9/rx/client/trex_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,41 +65,44 @@
     )
     # TODO: create a threaded UserStatus class with __enter__/__exit__.
     sys.stdout.write('Finding a remote worker... ')
     sys.stdout.flush()
     try:
       # Five minute timeout.
       resp = self._stub.Init(req, metadata=self._metadata, timeout=(5 * 60))
-      sys.stdout.write('Done.\n')
     except grpc.RpcError as e:
       e = cast(grpc.Call, e)
       raise InitError(f'Could not initialize worker: {e.details()}', -1)
     if resp.result.code != 0:
       raise InitError(resp.result.message, -1)
+    sys.stdout.write('Done.\n')
 
     with remote.WritableRemote(self._local_cfg.cwd) as r:
       r['workspace_id'] = resp.workspace_id
       r['worker_addr'] = resp.worker_addr
       r['daemon_module'] = resp.rsync_dest.daemon_module
 
     # Create a container on the worker.
+    sys.stdout.write('Setting up the container... ')
+    sys.stdout.flush()
     with grpc_helper.get_channel(resp.worker_addr) as ch:
       worker = worker_client.create_authed_client(ch, self._local_cfg)
       worker.init()
     sys.stdout.write('Done.\n')
     print('\nDone setting up rx! To use, run:\n\n\t$ rx <your command>\n')
     return 0
 
   def _create_username(self) -> str:
     username = user.username_prompt(self._login.id_token['email'])
     req = rx_pb2.SetUsernameRequest(username=username)
     try:
       resp = self._stub.SetUsername(
         req, metadata=self._metadata, timeout=_TIMEOUT)
     except grpc.RpcError as e:
+      e = cast(grpc.Call, e)
       raise InitError(f'Could not set username: {e.details()}', -1)
     if resp.result.code == rx_pb2.INVALID:
       raise InitError(
         f'{resp.result.message}\nInvalid username: {username}', rx_pb2.INVALID)
     return username
 
   def _get_username(self) -> str:
```

### Comparing `run_rx-0.0.8/rx/client/user.py` & `run_rx-0.0.9/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/client/worker_client.py` & `run_rx-0.0.9/rx/client/worker_client.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/proto/rx_pb2.py` & `run_rx-0.0.9/rx/proto/rx_pb2.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/proto/rx_pb2.pyi` & `run_rx-0.0.9/rx/proto/rx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.9/rx/proto/rx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.8/PKG-INFO` & `run_rx-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: absl-py (>=1.4.0,<2.0.0)
 Requires-Dist: grpcio (>=1.54.0,<2.0.0)
 Requires-Dist: protobuf (>=4.22.3,<5.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sty (>=1.0.4,<2.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/run-rx/rx
 Description-Content-Type: text/markdown
 
 # rx
 
 [rx](https://www.run-rx.com) is a command-line tool to help make remote
 execution easy.
```

