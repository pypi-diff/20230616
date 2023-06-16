# Comparing `tmp/cgroups_exporter-0.7.0.tar.gz` & `tmp/cgroups_exporter-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgroups_exporter-0.7.0.tar", max compression
+gzip compressed data, was "cgroups_exporter-0.8.0.tar", max compression
```

## Comparing `cgroups_exporter-0.7.0.tar` & `cgroups_exporter-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11342 2023-05-12 11:37:53.856745 cgroups_exporter-0.7.0/LICENSE
--rw-r--r--   0        0        0    19442 2023-05-12 11:37:53.857624 cgroups_exporter-0.7.0/README.md
--rw-r--r--   0        0        0        0 2021-06-18 16:25:57.000000 cgroups_exporter-0.7.0/cgroups_exporter/__init__.py
--rw-r--r--   0        0        0     2285 2023-05-12 11:37:53.858656 cgroups_exporter-0.7.0/cgroups_exporter/__main__.py
--rw-r--r--   0        0        0     1568 2023-05-12 11:37:53.860411 cgroups_exporter-0.7.0/cgroups_exporter/args.py
--rw-r--r--   0        0        0      825 2023-05-12 10:37:54.788008 cgroups_exporter-0.7.0/cgroups_exporter/metrics/__init__.py
--rw-r--r--   0        0        0     2371 2022-09-30 09:41:05.600451 cgroups_exporter-0.7.0/cgroups_exporter/metrics/_metrics.py
--rw-r--r--   0        0        0     3858 2023-05-12 10:37:54.788482 cgroups_exporter-0.7.0/cgroups_exporter/metrics/base.py
--rw-r--r--   0        0        0     4110 2021-11-29 21:16:37.000000 cgroups_exporter-0.7.0/cgroups_exporter/metrics/blkio.py
--rw-r--r--   0        0        0     1088 2023-05-12 10:37:54.789156 cgroups_exporter-0.7.0/cgroups_exporter/metrics/cpu.py
--rw-r--r--   0        0        0     1029 2021-10-18 13:31:10.000000 cgroups_exporter-0.7.0/cgroups_exporter/metrics/cpuset.py
--rw-r--r--   0        0        0     2265 2023-05-12 10:37:54.789614 cgroups_exporter-0.7.0/cgroups_exporter/metrics/meminfo.py
--rw-r--r--   0        0        0     2468 2021-10-18 13:31:10.000000 cgroups_exporter-0.7.0/cgroups_exporter/metrics/memory.py
--rw-r--r--   0        0        0      662 2023-05-12 10:37:54.790013 cgroups_exporter-0.7.0/cgroups_exporter/metrics/pids.py
--rw-r--r--   0        0        0     1594 2023-05-12 10:37:54.790375 cgroups_exporter-0.7.0/cgroups_exporter/metrics/unified.py
--rw-r--r--   0        0        0        1 2021-06-18 16:25:57.000000 cgroups_exporter-0.7.0/cgroups_exporter/services/__init__.py
--rw-r--r--   0        0        0     2435 2023-05-12 11:37:53.862567 cgroups_exporter-0.7.0/cgroups_exporter/services/collector.py
--rw-r--r--   0        0        0     1022 2022-05-30 19:37:57.353247 cgroups_exporter-0.7.0/cgroups_exporter/services/metrics.py
--rw-r--r--   0        0        0     1473 2023-05-12 11:37:53.866597 cgroups_exporter-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    21140 1970-01-01 00:00:00.000000 cgroups_exporter-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/LICENSE
+-rw-r--r--   0        0        0    19855 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/__init__.py
+-rw-r--r--   0        0        0     2285 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/__main__.py
+-rw-r--r--   0        0        0     1568 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/args.py
+-rw-r--r--   0        0        0      825 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/__init__.py
+-rw-r--r--   0        0        0     2423 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/_metrics.py
+-rw-r--r--   0        0        0     3858 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/base.py
+-rw-r--r--   0        0        0     4110 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/blkio.py
+-rw-r--r--   0        0        0     1088 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/cpu.py
+-rw-r--r--   0        0        0     1029 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/cpuset.py
+-rw-r--r--   0        0        0     2265 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/meminfo.py
+-rw-r--r--   0        0        0     2468 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/memory.py
+-rw-r--r--   0        0        0      662 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/pids.py
+-rw-r--r--   0        0        0     1594 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/metrics/unified.py
+-rw-r--r--   0        0        0        1 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/services/__init__.py
+-rw-r--r--   0        0        0     2435 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/services/collector.py
+-rw-r--r--   0        0        0     1022 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/cgroups_exporter/services/metrics.py
+-rw-r--r--   0        0        0     1473 2023-06-16 13:04:55.649553 cgroups_exporter-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    21354 1970-01-01 00:00:00.000000 cgroups_exporter-0.8.0/PKG-INFO
```

### Comparing `cgroups_exporter-0.7.0/LICENSE` & `cgroups_exporter-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/README.md` & `cgroups_exporter-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,26 @@
   --memory-tracer-interval MEMORY_TRACER_INTERVAL
                         (default: 5) [ENV: CGROUPS_EXPORTER_MEMORY_TRACER_INTERVAL]
 
 Default values will based on following configuration files ['cgroups-exporter.conf', '~/.cgroups-exporter.conf', '/etc/cgroups-exporter.conf']. The configuration files is INI-formatted files where configuration groups is INI
 sections.See more https://pypi.org/project/argclass/#configs
 ```
 
+Container Usage
+---------------
+
+`cgroups-exporter` is also available as a container image to be used in Docker, Kubernetes or other runtimes. It expects the host `/sys` directory to be mounted in the container (read only).
+
+Docker usage example:
+
+```shell
+docker run -p 9753:9753 -v /sys/:/host_sys/ ghcr.io/mosquito/cgroups-exporter:latest cgroups-exporter --cgroups-path "/host_sys/fs/cgroup/*/docker/*"
+```
+
+
 Metrics
 -------
 
 | Name | Description |
 | ------------ | ------------ |
 | `cgroups_blkio_bfq_service_bytes_async` | BlockIO service bytes ('async' field from 'blkio.bfq.io_service_bytes' file) |
 | `cgroups_blkio_bfq_service_bytes_discard` | BlockIO service bytes ('discard' field from 'blkio.bfq.io_service_bytes' file) |
```

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/__main__.py` & `cgroups_exporter-0.8.0/cgroups_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/args.py` & `cgroups_exporter-0.8.0/cgroups_exporter/args.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/__init__.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/_metrics.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,24 +61,27 @@
 
         # prevent change when iterating
         with self.lock:
             self.metrics[metric][record] = value
 
     def __iter__(self):
         with self.lock:
-            for metric, records in self.metrics.items():
-                if metric.help:
-                    yield f"# HELP {metric.name} {metric.help}\n"
-
-                if metric.type:
-                    yield f"# TYPE {metric.name} {metric.type}\n"
-
-                for record, value in records.items():
-                    if record.labels:
-                        yield "%s{%s} %.3e\n" % (
-                            metric.name, record.labels, value,
-                        )
-                    else:
-                        yield "%s %.3e\n" % (metric.name, value)
+            # make a copy of metrics to avoid slow tcp attack
+            metrics = tuple(self.metrics.items())
+
+        for metric, records in metrics:
+            if metric.help:
+                yield f"# HELP {metric.name} {metric.help}\n"
+
+            if metric.type:
+                yield f"# TYPE {metric.name} {metric.type}\n"
+
+            for record, value in records.items():
+                if record.labels:
+                    yield "%s{%s} %.3e\n" % (
+                        metric.name, record.labels, value,
+                    )
+                else:
+                    yield "%s %.3e\n" % (metric.name, value)
 
 
 STORAGE = Storage()
```

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/base.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/base.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/blkio.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/blkio.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/cpu.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/cpu.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/cpuset.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/cpuset.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/meminfo.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/meminfo.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/memory.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/memory.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/pids.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/pids.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/metrics/unified.py` & `cgroups_exporter-0.8.0/cgroups_exporter/metrics/unified.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/services/collector.py` & `cgroups_exporter-0.8.0/cgroups_exporter/services/collector.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/cgroups_exporter/services/metrics.py` & `cgroups_exporter-0.8.0/cgroups_exporter/services/metrics.py`

 * *Files identical despite different names*

### Comparing `cgroups_exporter-0.7.0/pyproject.toml` & `cgroups_exporter-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgroups-exporter"
-version = "0.7.0"
+version = "0.8.0"
 description = "prometheus exporter for cgroups v1"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 license = "Apache Software License"
 homepage = "https://github.com/mosquito/cgroups-exporter"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `cgroups_exporter-0.7.0/PKG-INFO` & `cgroups_exporter-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgroups-exporter
-Version: 0.7.0
+Version: 0.8.0
 Summary: prometheus exporter for cgroups v1
 Home-page: https://github.com/mosquito/cgroups-exporter
 License: Apache Software License
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -16,19 +16,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiochannel (>=1.2.1,<2.0.0)
 Requires-Dist: aiohttp (==3.8.1)
 Requires-Dist: aiomisc (>=17.2.2,<18.0.0)
 Requires-Dist: argclass (>=0.9.2,<0.10.0)
@@ -152,14 +148,26 @@
   --memory-tracer-interval MEMORY_TRACER_INTERVAL
                         (default: 5) [ENV: CGROUPS_EXPORTER_MEMORY_TRACER_INTERVAL]
 
 Default values will based on following configuration files ['cgroups-exporter.conf', '~/.cgroups-exporter.conf', '/etc/cgroups-exporter.conf']. The configuration files is INI-formatted files where configuration groups is INI
 sections.See more https://pypi.org/project/argclass/#configs
 ```
 
+Container Usage
+---------------
+
+`cgroups-exporter` is also available as a container image to be used in Docker, Kubernetes or other runtimes. It expects the host `/sys` directory to be mounted in the container (read only).
+
+Docker usage example:
+
+```shell
+docker run -p 9753:9753 -v /sys/:/host_sys/ ghcr.io/mosquito/cgroups-exporter:latest cgroups-exporter --cgroups-path "/host_sys/fs/cgroup/*/docker/*"
+```
+
+
 Metrics
 -------
 
 | Name | Description |
 | ------------ | ------------ |
 | `cgroups_blkio_bfq_service_bytes_async` | BlockIO service bytes ('async' field from 'blkio.bfq.io_service_bytes' file) |
 | `cgroups_blkio_bfq_service_bytes_discard` | BlockIO service bytes ('discard' field from 'blkio.bfq.io_service_bytes' file) |
```

