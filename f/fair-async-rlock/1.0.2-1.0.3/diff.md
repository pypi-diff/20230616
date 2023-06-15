# Comparing `tmp/fair_async_rlock-1.0.2.tar.gz` & `tmp/fair_async_rlock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_async_rlock-1.0.2.tar", last modified: Thu Jun 15 00:21:19 2023, max compression
+gzip compressed data, was "fair_async_rlock-1.0.3.tar", last modified: Thu Jun 15 23:39:56 2023, max compression
```

## Comparing `fair_async_rlock-1.0.2.tar` & `fair_async_rlock-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.2/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.2/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock/
--rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.2/fair_async_rlock/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1998 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.2/fair_async_rlock/fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.2/fair_async_rlock/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12053 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.2/fair_async_rlock/tests/test_fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.2/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-15 00:16:05.000000 fair_async_rlock-1.0.2/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.3/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.3/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.609452 fair_async_rlock-1.0.3/fair_async_rlock/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.3/fair_async_rlock/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2043 2023-06-15 23:07:46.000000 fair_async_rlock-1.0.3/fair_async_rlock/fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/fair_async_rlock/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.3/fair_async_rlock/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15990 2023-06-15 23:27:05.000000 fair_async_rlock-1.0.3/fair_async_rlock/tests/test_fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 23:39:56.000000 fair_async_rlock-1.0.3/fair_async_rlock.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.3/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 23:39:56.613452 fair_async_rlock-1.0.3/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-15 23:33:49.000000 fair_async_rlock-1.0.3/setup.py
```

### Comparing `fair_async_rlock-1.0.2/LICENSE` & `fair_async_rlock-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.2/PKG-INFO` & `fair_async_rlock-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_async_rlock
-Version: 1.0.2
+Version: 1.0.3
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.2/README.md` & `fair_async_rlock-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.2/fair_async_rlock/fair_async_rlock.py` & `fair_async_rlock-1.0.3/fair_async_rlock/fair_async_rlock.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,47 +18,47 @@
             task = asyncio.current_task()
         return self._owner == task
 
     async def acquire(self):
         """Acquire the lock."""
         me = asyncio.current_task()
 
+        # If the lock is reentrant, acquire it immediately
         if self.is_owner(task=me):
             self._count += 1
             return
 
-        # If the lock is free or reentrant, acquire it immediately
+        # If the lock is free, acquire it immediately
         if self._count == 0:
-            # if self._count == 0  or self._owner == me: (redundant second clause)
             self._owner = me
-            self._count += 1
-        else:
-            # Create an event for this task
-            event = asyncio.Event()
-            self._queue.append(event)
-
-            # Wait for the lock to be free
-            try:
-                await event.wait()
-            except asyncio.CancelledError:
-                self._queue.remove(event)
-                raise
+            self._count = 1
+            return
 
+        # Create an event for this task, to notify when it's ready for acquire
+        event = asyncio.Event()
+        self._queue.append(event)
+
+        # Wait for the lock to be free, then acquire
+        try:
+            await event.wait()
             self._owner = me
             self._count = 1
+        except asyncio.CancelledError:
+            self._queue.remove(event)
+            raise
 
     async def release(self):
         """Release the lock"""
         me = asyncio.current_task()
 
         if self._owner is None:
-            raise RuntimeError("Cannot release un-acquired lock.")
+            raise RuntimeError(f"Cannot release un-acquired lock. {me} tried to release.")
 
         if not self.is_owner(task=me):
-            raise RuntimeError("Cannot release foreign lock.")
+            raise RuntimeError(f"Cannot release foreign lock. {me} tried to unlock {self._owner}.")
 
         self._count -= 1
         if self._count == 0:
             self._owner = None
             if self._queue:
                 # Wake up the next task in the queue
                 event = self._queue.popleft()
```

### Comparing `fair_async_rlock-1.0.2/fair_async_rlock/tests/test_fair_async_rlock.py` & `fair_async_rlock-1.0.3/fair_async_rlock/tests/test_fair_async_rlock.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import random
 from time import monotonic_ns, perf_counter
 
 import pytest
 
 from fair_async_rlock import FairAsyncRLock
 
 
@@ -276,15 +277,15 @@
             await asyncio.sleep(0.1)  # Sleep to ensure that task2 gets to the point where it's waiting for the lock
 
     async def task2():
         # Wait for both tasks to complete
         try:
             await lock.release()
         except RuntimeError as e:
-            assert str(e) == "Cannot release foreign lock."
+            assert str(e).startswith("Cannot release foreign lock.")
             return
 
     # Create the tasks and schedule them
     task1_handle = asyncio.create_task(task1())
     task2_handle = asyncio.create_task(task2())
 
     # Wait for both tasks to complete
@@ -374,7 +375,116 @@
     task2.cancel()
     with pytest.raises(asyncio.CancelledError):
         await task2
     await task1  # Ensure task1 has a chance to release the lock
     # Ensure that lock is not owned and queue is empty after cancellation
     assert lock._owner is None
     assert len(lock._queue) == 0
+
+
+@pytest.mark.asyncio
+async def test_lock_cancellation_before_acquisition():
+    lock = FairAsyncRLock()
+    cancellation_event = asyncio.Event()
+
+    async def task_to_cancel():
+        try:
+            async with lock:
+                await asyncio.sleep(1)  # simulate some work
+        except asyncio.CancelledError:
+            cancellation_event.set()
+
+    task = asyncio.create_task(task_to_cancel())
+    await asyncio.sleep(0)  # yield control to let the task start
+    task.cancel()
+    await cancellation_event.wait()  # wait for the task to handle the cancellation
+
+    assert lock._owner is None  # lock should not be owned by any task
+
+
+@pytest.mark.asyncio
+async def test_lock_cancellation_during_acquisition():
+    lock = FairAsyncRLock()
+    acquisition_event = asyncio.Event()
+    cancellation_event = asyncio.Event()
+
+    async def task_acquiring_lock():
+        await lock.acquire()  # acquire the lock without releasing
+        acquisition_event.set()  # signal that lock has been acquired
+
+    async def task_to_cancel():
+        await acquisition_event.wait()  # wait for the other task to acquire the lock
+        try:
+            async with lock:  # attempt to acquire the lock
+                await asyncio.sleep(1)  # simulate some work
+        except asyncio.CancelledError:
+            cancellation_event.set()
+
+    first_task = asyncio.create_task(task_acquiring_lock())
+    task = asyncio.create_task(task_to_cancel())
+    await asyncio.sleep(0)  # yield control to let the tasks start
+    await acquisition_event.wait()  # wait for the lock to be acquired
+    task.cancel()
+    await cancellation_event.wait()  # wait for the task to handle the cancellation
+
+    assert lock.is_owner(task=first_task)  # lock should still be owned by the first task
+
+
+@pytest.mark.asyncio
+async def test_lock_cancellation_after_acquisition():
+    lock = FairAsyncRLock()
+    cancellation_event = asyncio.Event()
+
+    async def task_to_cancel():
+        async with lock:  # acquire the lock
+            try:
+                await asyncio.sleep(1)  # simulate some work
+            except asyncio.CancelledError:
+                cancellation_event.set()
+
+    task = asyncio.create_task(task_to_cancel())
+    await asyncio.sleep(0)  # yield control to let the task start
+    task.cancel()
+    await cancellation_event.wait()  # wait for the task to handle the cancellation
+
+    assert lock._owner is None  # lock should not be owned by any task
+
+
+@pytest.mark.asyncio
+async def test_stochastic_cancellation():
+    lock = FairAsyncRLock()
+    num_tasks = 10  # number of tasks to create
+    tasks = []
+    cancellation_occurred = asyncio.Event()
+
+    async def task_func(task_id):
+        """Function to be run in tasks. Tries to acquire and release the lock."""
+        try:
+            await asyncio.sleep(random.random())  # simulate work with random duration
+            async with lock:
+                print(f"Task {task_id} acquired lock")
+                await asyncio.sleep(random.random())  # simulate work with random duration
+        except asyncio.CancelledError:
+            print(f"Task {task_id} was cancelled")
+            cancellation_occurred.set()
+
+    async def monitor_func():
+        """Function to be run in monitor task. Randomly cancels one of the tasks."""
+        await asyncio.sleep(random.random())  # wait random duration before cancelling a task
+        task_to_cancel = random.choice(tasks)
+        task_to_cancel.cancel()
+
+    # Create tasks
+    for i in range(num_tasks):
+        tasks.append(asyncio.create_task(task_func(i)))
+
+    await asyncio.sleep(0)
+    # Create monitor task
+    monitor_task = asyncio.create_task(monitor_func())
+
+    # Wait for all tasks to complete or be cancelled
+    await asyncio.gather(*tasks, return_exceptions=True)
+
+    await monitor_task
+
+    # At least one cancellation should have occurred
+    assert cancellation_occurred.is_set()
```

### Comparing `fair_async_rlock-1.0.2/fair_async_rlock.egg-info/PKG-INFO` & `fair_async_rlock-1.0.3/fair_async_rlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-async-rlock
-Version: 1.0.2
+Version: 1.0.3
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fair_async_rlock-1.0.2/setup.py` & `fair_async_rlock-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='fair_async_rlock',
-      version='1.0.2',
+      version='1.0.3',
       description='A well-tested implementation of a fair asynchronous RLock for concurrent programming.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/Joshuaalbert/FairAsyncRLock",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=[],
```

