# Comparing `tmp/xqute-0.2.1.tar.gz` & `tmp/xqute-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xqute-0.2.1.tar", max compression
+gzip compressed data, was "xqute-0.2.2.tar", max compression
```

## Comparing `xqute-0.2.1.tar` & `xqute-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-04-14 00:56:20.902778 xqute-0.2.1/LICENSE
--rw-r--r--   0        0        0     4751 2023-04-14 00:56:20.902778 xqute-0.2.1/README.md
--rw-r--r--   0        0        0     1173 2023-04-14 00:56:20.906779 xqute-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      246 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/defaults.py
--rw-r--r--   0        0        0     8595 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/job.py
--rw-r--r--   0        0        0     3017 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/plugin.py
--rw-r--r--   0        0        0     8109 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/scheduler.py
--rw-r--r--   0        0        0      633 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/__init__.py
--rw-r--r--   0        0        0     2361 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/local_scheduler.py
--rw-r--r--   0        0        0     4225 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/sge_scheduler.py
--rw-r--r--   0        0        0     7155 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/slurm_scheduler.py
--rw-r--r--   0        0        0       44 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/__init__.py
--rw-r--r--   0        0        0     3547 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/client.py
--rw-r--r--   0        0        0     2548 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/scheduler.py
--rw-r--r--   0        0        0      691 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/submitter.py
--rw-r--r--   0        0        0     2206 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/utils.py
--rw-r--r--   0        0        0     9380 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/xqute.py
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 xqute-0.2.1/setup.py
--rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 xqute-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-16 20:39:10.926349 xqute-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4751 2023-06-16 20:39:10.926349 xqute-0.2.2/README.md
+-rw-r--r--   0        0        0     1173 2023-06-16 20:39:10.930349 xqute-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/__init__.py
+-rw-r--r--   0        0        0     3378 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/defaults.py
+-rw-r--r--   0        0        0     8595 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/job.py
+-rw-r--r--   0        0        0     3017 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/plugin.py
+-rw-r--r--   0        0        0     8109 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/scheduler.py
+-rw-r--r--   0        0        0      633 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/__init__.py
+-rw-r--r--   0        0        0     2361 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/local_scheduler.py
+-rw-r--r--   0        0        0     4225 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/sge_scheduler.py
+-rw-r--r--   0        0        0     7155 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/slurm_scheduler.py
+-rw-r--r--   0        0        0       44 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/ssh_scheduler/__init__.py
+-rw-r--r--   0        0        0     3547 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/ssh_scheduler/client.py
+-rw-r--r--   0        0        0     2548 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/ssh_scheduler/scheduler.py
+-rw-r--r--   0        0        0      691 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/schedulers/ssh_scheduler/submitter.py
+-rw-r--r--   0        0        0     2206 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/utils.py
+-rw-r--r--   0        0        0     9380 2023-06-16 20:39:10.934349 xqute-0.2.2/xqute/xqute.py
+-rw-r--r--   0        0        0     5891 1970-01-01 00:00:00.000000 xqute-0.2.2/setup.py
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 xqute-0.2.2/PKG-INFO
```

### Comparing `xqute-0.2.1/LICENSE` & `xqute-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/README.md` & `xqute-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/pyproject.toml` & `xqute-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xqute"
-version = "0.2.1"
+version = "0.2.2"
 description = "A job management system for python"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 homepage = "https://github.com/pwwang/xqute"
 repository  = "https://github.com/pwwang/xqute"
 readme = "README.md"
```

### Comparing `xqute-0.2.1/xqute/defaults.py` & `xqute-0.2.2/xqute/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 DEFAULT_JOB_METADIR: Path = Path('./.xqute')
 DEFAULT_JOB_ERROR_STRATEGY: str = JobErrorStrategy.IGNORE
 DEFAULT_JOB_NUM_RETRIES: int = 3
 DEFAULT_JOB_SUBMISSION_BATCH: int = 8
 DEFAULT_JOB_CMD_WRAPPER_SHELL: str = '/bin/bash'
 DEFAULT_JOB_CMD_WRAPPER_TEMPLATE: str = r"""{shebang}
 
+set -u -e -E -o pipefail
+
 # Trap command to capture status, rc
 # And remove job id file
 cleanup() {{
     rc=$?
     echo $rc > {job.rc_file}
     if [[ $rc -eq 0 ]]; then
         echo {status.FINISHED} > {job.status_file}
```

### Comparing `xqute-0.2.1/xqute/job.py` & `xqute-0.2.2/xqute/job.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/plugin.py` & `xqute-0.2.2/xqute/plugin.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/scheduler.py` & `xqute-0.2.2/xqute/scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/__init__.py` & `xqute-0.2.2/xqute/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/local_scheduler.py` & `xqute-0.2.2/xqute/schedulers/local_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/sge_scheduler.py` & `xqute-0.2.2/xqute/schedulers/sge_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/slurm_scheduler.py` & `xqute-0.2.2/xqute/schedulers/slurm_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/ssh_scheduler/client.py` & `xqute-0.2.2/xqute/schedulers/ssh_scheduler/client.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/ssh_scheduler/scheduler.py` & `xqute-0.2.2/xqute/schedulers/ssh_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/schedulers/ssh_scheduler/submitter.py` & `xqute-0.2.2/xqute/schedulers/ssh_scheduler/submitter.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/utils.py` & `xqute-0.2.2/xqute/utils.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/xqute/xqute.py` & `xqute-0.2.2/xqute/xqute.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.1/setup.py` & `xqute-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['diot>=0.1,<0.2', 'rich>=13,<14', 'simplug>=0.3,<0.4', 'uvloop>=0,<1']
 
 extras_require = \
-{':python_version < "3.10"': ['aiopath>=0.5.0,<0.6.0'],
+{':python_version < "3.10"': ['aiopath==0.5.*'],
  ':python_version >= "3.10"': ['aiopath>=0.6,<0.7']}
 
 setup_kwargs = {
     'name': 'xqute',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A job management system for python',
     'long_description': '# xqute\n\nA job management system for python\n\n## Features\n\n- Written in async\n- Plugin system\n- Scheduler adaptor\n- Job retrying/pipeline halting when failed\n\n## Installation\n\n```\npip install xqute\n```\n\n## A toy example\n```python\nimport asyncio\nfrom xqute import Xqute\n\nasync def main():\n    # 3 jobs allowed to run at the same time\n    xqute = Xqute(scheduler_forks=3)\n    for _ in range(10):\n        await xqute.put(\'sleep 1\')\n    await xqute.run_until_complete()\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n![xqute](./xqute.png)\n\n\n## API\nhttps://pwwang.github.io/xqute/\n\n## Usage\n\n### Xqute object\n\nAn xqute is initialized by:\n```python\nxqute = Xqute(...)\n```\nAvailable arguments are:\n\n- scheduler: The scheduler class or name\n- plugins: The plugins to enable/disable for this session\n- job_metadir: The job meta directory (Default: `./.xqute/`)\n- job_error_strategy: The strategy when there is error happened\n- job_num_retries: Max number of retries when job_error_strategy is retry\n- job_submission_batch: The number of consumers to submit jobs\n- scheduler_forks: Max number of job forks\n- **scheduler_opts: Additional keyword arguments for scheduler\n\nNote that the producer must be initialized in an event loop.\n\nTo push a job into the queue:\n```python\nawait xqute.put([\'echo\', 1])\n```\n\n### Using SGE scheduler\n```python\nxqute = Xqute(\n    \'sge\',\n    scheduler_forks=100,\n    qsub=\'path to qsub\',\n    qdel=\'path to qdel\',\n    qstat=\'path to qstat\',\n    sge_q=\'1-day\',  # or qsub_q=\'1-day\'\n    ...\n)\n```\nKeyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:\n`sge_l=[\'h_vmem=2G\', \'gpu=1\']` will be expanded in wrapped script like this:\n```shell\n# ...\n\n#$ -l h_vmem=2G\n#$ -l gpu=1\n\n# ...\n```\n\n\n### Using Slurm scheduler\n\n```python\nxqute = Xqute(\n    \'slurm\',\n    scheduler_forks=100,\n    sbatch=\'path to sbatch\',\n    scancel=\'path to scancel\',\n    squeue=\'path to squeue\',\n    sbatch_partition=\'1-day\',  # or slurm_partition=\'1-day\'\n    sbatch_time=\'01:00:00\',\n    ...\n)\n```\n\n### Using ssh scheduler\n\n```python\nxqute = Xqute(\n    \'ssh\',\n    scheduler_forks=100,\n    ssh=\'path to ssh\',\n    ssh_servers={\n        "server1": {\n            "user": ...,\n            "port": 22,\n            "keyfile": ...,\n            # How long to keep the ssh connection alive\n            "ctrl_persist": 600,\n            # Where to store the control socket\n            "ctrl_dir": "/tmp",\n        },\n        ...\n    }\n    ...\n)\n```\n\nSSH servers must share the same filesystem and using keyfile authentication.\n\n### Plugins\n\nTo write a plugin for `xqute`, you will need to implement the following hooks:\n\n- `on_init(scheduler)`: Right after scheduler object is initialized\n- `on_shutdown(scheduler, sig)`: When scheduler is shutting down\n- `on_job_init(scheduler, job)`: When the job is initialized\n- `on_job_queued(scheduler, job)`: When the job is queued\n- `on_job_submitted(scheduler, job)`: When the job is submitted\n- `on_job_killing(scheduler, job)`: When the job is being killed\n- `on_job_killed(scheduler, job)`: When the job is killed\n- `on_job_failed(scheduler, job)`: When the job is failed\n- `on_job_succeeded(scheduler, job)`: When the job is succeeded\n\nNote that all hooks are corotines except `on_init` and `on_shutdown`, that means you should also implement them as corotines (sync implementations are allowed but will be warned).\n\nTo implement a hook, you have to fetch the plugin manager:\n\n```python\nfrom simplug import Simplug\npm = Simplug(\'xqute\')\n\n# or\nfrom xqute import simplug as pm\n```\n\nand then use the decorator `pm.impl`:\n\n```python\n@pm.impl\ndef on_init(scheduler):\n    ...\n```\n\n### Implementing a scheduler\n\nCurrently there are only 2 builtin schedulers: `local` and `sge`.\n\nOne can implement a scheduler by subclassing the `Scheduler` abstract class. There are three abstract methods that have to be implemented in the subclass:\n\n```python\nfrom xqute import Scheduer\n\nclass MyScheduler(Scheduler):\n    name = \'my\'\n    job_class: MyJob\n\n    async def submit_job(self, job):\n        """How to submit a job, return a unique id in the scheduler system\n        (the pid for local scheduler for example)\n        """\n\n    async def kill_job(self, job):\n        """How to kill a job"""\n\n    async def job_is_running(self, job):\n        """Check if a job is running"""\n```\n\nAs you may see, we may also need to implement a job class before `MyScheduler`. The only abstract method to be implemented is `wrap_cmd`:\n```python\nfrom xqute import Job\n\nclass MyJob(Job):\n\n    async def wrap_cmd(self, scheduler):\n        ...\n```\n\nYou have to use the trap command in the wrapped script to update job status, return code and clear the job id file.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/xqute',
```

### Comparing `xqute-0.2.1/PKG-INFO` & `xqute-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: xqute
-Version: 0.2.1
+Version: 0.2.2
 Summary: A job management system for python
 Home-page: https://github.com/pwwang/xqute
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiopath (>=0.5.0,<0.6.0) ; python_version < "3.10"
+Requires-Dist: aiopath (==0.5.*) ; python_version < "3.10"
 Requires-Dist: aiopath (>=0.6,<0.7) ; python_version >= "3.10"
 Requires-Dist: diot (>=0.1,<0.2)
 Requires-Dist: rich (>=13,<14)
 Requires-Dist: simplug (>=0.3,<0.4)
 Requires-Dist: uvloop (>=0,<1)
 Project-URL: Repository, https://github.com/pwwang/xqute
 Description-Content-Type: text/markdown
```

