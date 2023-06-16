# Comparing `tmp/atooms.active-1.0.2.tar.gz` & `tmp/atooms.active-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms.active-1.0.2.tar", last modified: Wed Jun 14 09:30:24 2023, max compression
+gzip compressed data, was "atooms.active-1.0.3.tar", last modified: Fri Jun 16 18:59:50 2023, max compression
```

## Comparing `atooms.active-1.0.2.tar` & `atooms.active-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-14 09:30:24.937619 atooms.active-1.0.2/
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)    35147 2023-06-14 09:25:07.000000 atooms.active-1.0.2/LICENSE
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3814 2023-06-14 09:30:24.937853 atooms.active-1.0.2/PKG-INFO
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3112 2023-06-14 09:25:07.000000 atooms.active-1.0.2/README.md
-drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-14 09:30:24.921001 atooms.active-1.0.2/atooms/
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       75 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/__init__.py
-drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-14 09:30:24.936690 atooms.active-1.0.2/atooms/active/
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      125 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/__init__.py
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     8648 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/api.py
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     2727 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/neighbor_list.f90
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     2859 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/neighbor_list_newton.f90
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3058 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/neighbor_list_newton_inline.f90
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     8542 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/neighbors.py
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     5286 2023-06-14 09:25:07.000000 atooms.active-1.0.2/atooms/active/vicsek.py
-drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-14 09:30:24.927439 atooms.active-1.0.2/atooms.active.egg-info/
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3814 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/PKG-INFO
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      500 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/SOURCES.txt
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        1 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/dependency_links.txt
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       50 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/entry_points.txt
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       56 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/requires.txt
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        7 2023-06-14 09:30:24.000000 atooms.active-1.0.2/atooms.active.egg-info/top_level.txt
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     1625 2023-06-14 09:25:07.000000 atooms.active-1.0.2/pyproject.toml
--rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      173 2023-06-14 09:30:24.938730 atooms.active-1.0.2/setup.cfg
+drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-16 18:59:50.989518 atooms.active-1.0.3/
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)    35147 2023-06-16 18:59:10.000000 atooms.active-1.0.3/LICENSE
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     4231 2023-06-16 18:59:50.989783 atooms.active-1.0.3/PKG-INFO
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3539 2023-06-16 18:59:10.000000 atooms.active-1.0.3/README.md
+drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-16 18:59:50.969638 atooms.active-1.0.3/atooms/
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       75 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/__init__.py
+drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-16 18:59:50.988683 atooms.active-1.0.3/atooms/active/
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      125 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/__init__.py
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     9047 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/api.py
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     2727 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/neighbor_list.f90
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     2859 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/neighbor_list_newton.f90
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     3058 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/neighbor_list_newton_inline.f90
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     8542 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/neighbors.py
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     5286 2023-06-16 18:59:10.000000 atooms.active-1.0.3/atooms/active/vicsek.py
+drwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        0 2023-06-16 18:59:50.980190 atooms.active-1.0.3/atooms.active.egg-info/
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     4231 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/PKG-INFO
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      500 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/SOURCES.txt
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        1 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/dependency_links.txt
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       50 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/entry_points.txt
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)       64 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/requires.txt
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)        7 2023-06-16 18:59:50.000000 atooms.active-1.0.3/atooms.active.egg-info/top_level.txt
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)     1625 2023-06-16 18:59:10.000000 atooms.active-1.0.3/pyproject.toml
+-rwxrwxrwx   0 iacopo    (1000) iacopo    (1000)      173 2023-06-16 18:59:50.990967 atooms.active-1.0.3/setup.cfg
```

### Comparing `atooms.active-1.0.2/LICENSE` & `atooms.active-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/PKG-INFO` & `atooms.active-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-Metadata-Version: 2.1
-Name: atooms.active
-Version: 1.0.2
-Summary: An atooms backend for simulating active matter
-Author-email: Iacopo Ricci <dummy.iricci@dummy.com>
-License: GPLv3
-Project-URL: repository, https://framagit.org/atooms/active
-Project-URL: changelog, https://framagit.org/atooms/active/-/blob/master/CHANGELOG.md
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # active 
 
+[![pypi](https://img.shields.io/pypi/v/atooms.active)](https://pypi.org/project/atooms.active/)
+[![version](https://img.shields.io/pypi/pyversions/atooms.active)](https://pypi.org/project/atooms.active/)
 [![license](https://img.shields.io/pypi/l/atooms.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-[![pipeline status](https://framagit.org/activematter/active/badges/master/pipeline.svg)](https://framagit.org/activematter/active/-/commits/master)
+[![pipeline](https://framagit.org/activematter/active/badges/master/pipeline.svg)](https://framagit.org/activematter/active/-/commits/master)
 [![coverage report](https://framagit.org/activematter/active/badges/master/coverage.svg)](https://framagit.org/activematter/active/-/commits/master)
 
 **active** is a simulation backend for [atooms](https://framagit.org/atooms/atooms), a high-level framework for particle-based simulations. This backend implements active matter systems, e.g. the Vicsek model as described in [Vicsek _et al._ (1995)](https://doi.org/10.1103/PhysRevLett.75.1226) and in [Grégoire _and_ Chaté (2004)](https://doi.org/10.1103/PhysRevLett.92.025702).
 
 ## Quick start
 Here we have a simulation of an active matter system based on the Vicsek model. First of all, we need to setup a 2D _atooms_ system.
 
@@ -62,21 +47,21 @@
 This simulation employs the so-called 'vectorial' noise implementation (discussed in Grégoire and Chaté) and the _scipy_-based kD-tree neighbor search algorithm.
 
 A basic API is also available. We can run the same simulation as follows
 
 ```python
 from atooms.active.api import vm
 
-vm('input.xyz', 'output.xyz', npart=2048, eta=0.4, rho=2.0, nsteps=1000, config_number=10)
+vm('input.xyz', file_out='output.xyz', npart=2048, eta=0.4, rho=2.0, nsteps=1000, config_number=10)
 ```
 
 or, from the command line 
 
 ```python
-api.py input.xyz output.xyz --npart 2048 --eta 0.4 --rho 2.0 --nsteps 1000 --config-number 10
+api.py input.xyz --file-out output.xyz --npart 2048 --eta 0.4 --rho 2.0 --nsteps 1000 --config-number 10
 ```
 
 ## Features
 
 - Seamless integration with _atooms_ framework
 - Various nearest neighbors algorithms available
 - Easy extension to new variations of the Vicsek model
@@ -93,15 +78,27 @@
 	- scipy (optional)
  
 ## Documentation
 
 Check out the [tutorial](https://atooms.frama.io/active/tutorial) for more detailed examples and the [public API](https://atooms.frama.io/active/api/atooms/active/) for more detail.
 
 ## Installation
-From the code repository:
+From the Python Package Index
+
+```
+pip install atooms.active[full]
+```
+
+to get all optional dependencies (*i.e.* `scipy`). A lightweight installation can be performed as well
+
+```
+pip install atooms.active
+```
+
+From the code repository
 
 ```
 git clone https://framagit.org/atooms/active.git
 cd active
 make install
 ```
```

### Comparing `atooms.active-1.0.2/atooms/active/api.py` & `atooms.active-1.0.3/atooms/active/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         log.removeHandler(h)
 
 def _initialize_system(dim, L, npart, file_inp, load=False, save=False):
     """
     System initialization.
     The system can be generated on the spot, loaded from an input file or saved to disk
     """
+    # TODO: add metadata read
     # TODO: move to utilities module
     # Import pkgs
     from atooms.system import System
     from atooms.system.cell import Cell
 
     # Set input trajectory file path
     input_file = os.path.join(os.path.dirname(__file__), file_inp)
@@ -95,27 +96,28 @@
     return norm/v0
 
 # API
 
 
 @argh.arg('--load', action='store_true')
 @argh.arg('--save', action='store_true')
-def vm(file_inp, file_out, load=False, save=False, noise='vectorial',
+def vm(file_inp, file_out=None, load=False, save=False, noise='vectorial',
        neighbors='kdtree', dim=2, npart=2048, eta=0.4, rho=2., v0=1.,
        nsteps=1000, checkpoint_interval=0, config_number=0, verbose=False,
-       seed=1, seed_inp='data/seed.txt', block='', restart=False, dry=False, log=True):
+       seed=1, seed_inp='data/seed.txt', block='', restart=False, dry=False, 
+       log=True, data_log='data/metadata.log'):
     """
     Simple API with logging facilities for Vicsek model simulations.
 
     Parameters
     ----------
     file_inp:               string
                             Input file path.
-    file_out:               string
-                            Output file path.
+    file_out:               string, default None
+                            Output file path. If None, output files are created in `data/`, using a randomly generated unique identifier as file name.
     load:                   bool, default False
                             Enable loading of starting trajectory from `file_inp`
     save:                   bool, default False
                             Enable saving of starting trajectory to `file_out`
     noise:                  string, default 'vectorial'
                             Orientation update method. See `active.vicsek` module.
     neighbors:              string, default `kdtree`
@@ -143,25 +145,30 @@
     seed_inp:               string, default 'data/seed.txt'
                             Seed file path. It has priority over `seed` variable.
     restart:                bool, default False
                             Enable simulation restarting from checkpoint.
     dry:                    bool, default False
                             Enable dry run. No simulation is performed.
     log:                    bool, default True
-                            Enable system parameters logging in path given by `file_out + '.param'`.
+                            Enable system parameters logging in `data_log`.
+    data_log:               string, default 'data/metadata.log'
+                            System parameters logging path.
     """
 
-    # Initialize seed
+    # Initialize seed and generate uid
     if os.path.exists(seed_inp):
         f = open(seed_inp, 'r')
         seed = int(f.read())
     random.seed(seed)
     numpy.random.seed(seed)
+    uid = _random_choice_id(length=16)
 
-    # Initialize directory structure
+    # Initialize filenames and directory structure
+    if file_out == None:
+        file_out = 'data/'+uid+'.xyz'
     mkdir(os.path.dirname(file_out))
 
     # Always log to file
     if not restart:
         rmf(file_out + '.log')
     setup_logging(level=20, filename=file_out + '.log')
     if verbose:
@@ -184,15 +191,15 @@
     sim = Simulation(bck, output_path=file_out, steps=nsteps,
                      enable_speedometer=True, restart=restart,
                      checkpoint_interval=checkpoint_interval)
     sim.checkpoint_variables = ['position', 'orientation', 'velocity']
 
     # Trajectory class instantiation with proper metadata
     trajectory = TrajectoryXYZ(file_out, mode='w')
-    trajectory.metadata = {'eta': eta, 'v0': v0, 'neighbors': neighbors}
+    trajectory.metadata = {'eta': eta, 'v0': v0, 'seed': seed, 'noise': noise, 'neighbors': neighbors}
 
     # Writing trajectory file
     if config_number == 0:
         if len(block) > 0:
             sim.add(write_trajectory, Scheduler(block=[int(_) for _ in block.split(',')]),
                     variables=['position', 'orientation', 'velocity'],
                     trajectory=trajectory)
@@ -207,21 +214,20 @@
 
     # TODO: fix write to file - cbk tuple doesn't work properly
     # cbk = ('phi', _order_parameter)
     # sim.add(write, Scheduler(calls=config_number), cbk, suffix='phi')
 
     # Create/update parameter log
     if log:
-        uuid = _random_choice_id(length=16)
-        with open(file_out+'.param', 'a') as f:
+        with open(data_log, 'a') as f:
             write = csv.writer(f)
             # Add header if file is empty
             if os.stat(data_log).st_size == 0:
-                write.writerow(['npart', 'rho', 'eta', 'v0', 'nsteps', 'noise', 'seed', 'uuid'])
-            write.writerow([npart, rho, eta, v0, nsteps, noise, seed, uuid])
+                write.writerow(['npart', 'rho', 'eta', 'v0', 'nsteps', 'noise', 'seed', 'uid'])
+            write.writerow([npart, rho, eta, v0, nsteps, noise, seed, uid])
 
     # Run
     if not dry:
         sim.run()
         _clear_logging()
 
     return sim
```

### Comparing `atooms.active-1.0.2/atooms/active/neighbor_list.f90` & `atooms.active-1.0.3/atooms/active/neighbor_list.f90`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/atooms/active/neighbor_list_newton.f90` & `atooms.active-1.0.3/atooms/active/neighbor_list_newton.f90`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/atooms/active/neighbor_list_newton_inline.f90` & `atooms.active-1.0.3/atooms/active/neighbor_list_newton_inline.f90`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/atooms/active/neighbors.py` & `atooms.active-1.0.3/atooms/active/neighbors.py`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/atooms/active/vicsek.py` & `atooms.active-1.0.3/atooms/active/vicsek.py`

 * *Files identical despite different names*

### Comparing `atooms.active-1.0.2/atooms.active.egg-info/PKG-INFO` & `atooms.active-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: atooms.active
-Version: 1.0.2
+Version: 1.0.3
 Summary: An atooms backend for simulating active matter
-Author-email: Iacopo Ricci <dummy.iricci@dummy.com>
+Author: Iacopo Ricci
 License: GPLv3
 Project-URL: repository, https://framagit.org/atooms/active
 Project-URL: changelog, https://framagit.org/atooms/active/-/blob/master/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE
 
 # active 
 
+[![pypi](https://img.shields.io/pypi/v/atooms.active)](https://pypi.org/project/atooms.active/)
+[![version](https://img.shields.io/pypi/pyversions/atooms.active)](https://pypi.org/project/atooms.active/)
 [![license](https://img.shields.io/pypi/l/atooms.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-[![pipeline status](https://framagit.org/activematter/active/badges/master/pipeline.svg)](https://framagit.org/activematter/active/-/commits/master)
+[![pipeline](https://framagit.org/activematter/active/badges/master/pipeline.svg)](https://framagit.org/activematter/active/-/commits/master)
 [![coverage report](https://framagit.org/activematter/active/badges/master/coverage.svg)](https://framagit.org/activematter/active/-/commits/master)
 
 **active** is a simulation backend for [atooms](https://framagit.org/atooms/atooms), a high-level framework for particle-based simulations. This backend implements active matter systems, e.g. the Vicsek model as described in [Vicsek _et al._ (1995)](https://doi.org/10.1103/PhysRevLett.75.1226) and in [Grégoire _and_ Chaté (2004)](https://doi.org/10.1103/PhysRevLett.92.025702).
 
 ## Quick start
 Here we have a simulation of an active matter system based on the Vicsek model. First of all, we need to setup a 2D _atooms_ system.
 
@@ -62,21 +65,21 @@
 This simulation employs the so-called 'vectorial' noise implementation (discussed in Grégoire and Chaté) and the _scipy_-based kD-tree neighbor search algorithm.
 
 A basic API is also available. We can run the same simulation as follows
 
 ```python
 from atooms.active.api import vm
 
-vm('input.xyz', 'output.xyz', npart=2048, eta=0.4, rho=2.0, nsteps=1000, config_number=10)
+vm('input.xyz', file_out='output.xyz', npart=2048, eta=0.4, rho=2.0, nsteps=1000, config_number=10)
 ```
 
 or, from the command line 
 
 ```python
-api.py input.xyz output.xyz --npart 2048 --eta 0.4 --rho 2.0 --nsteps 1000 --config-number 10
+api.py input.xyz --file-out output.xyz --npart 2048 --eta 0.4 --rho 2.0 --nsteps 1000 --config-number 10
 ```
 
 ## Features
 
 - Seamless integration with _atooms_ framework
 - Various nearest neighbors algorithms available
 - Easy extension to new variations of the Vicsek model
@@ -93,15 +96,27 @@
 	- scipy (optional)
  
 ## Documentation
 
 Check out the [tutorial](https://atooms.frama.io/active/tutorial) for more detailed examples and the [public API](https://atooms.frama.io/active/api/atooms/active/) for more detail.
 
 ## Installation
-From the code repository:
+From the Python Package Index
+
+```
+pip install atooms.active[full]
+```
+
+to get all optional dependencies (*i.e.* `scipy`). A lightweight installation can be performed as well
+
+```
+pip install atooms.active
+```
+
+From the code repository
 
 ```
 git clone https://framagit.org/atooms/active.git
 cd active
 make install
 ```
```

### Comparing `atooms.active-1.0.2/pyproject.toml` & `atooms.active-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 # https://github.com/pypa/sampleproject/blob/main/pyproject.toml
 
 [project]
 name = "atooms.active"
 description = "An atooms backend for simulating active matter"
 readme = "README.md"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
-    {name = "Iacopo Ricci", email = "dummy.iricci@dummy.com"}
+    {name = "Iacopo Ricci"}
 ]
 requires-python = ">=3.10"
 license = {text = "GPLv3"}
 dependencies = [
     "argh>=0.28.1",
     "atooms>=3.15.0",
     "f2py-jit>=0.9.1",
-    "numpy",
-    "scipy",
+    "numpy"
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.10",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
+[project.optional-dependencies]
+full = ["scipy"]
+
 [project.urls]
 repository = "https://framagit.org/atooms/active"
 changelog = "https://framagit.org/atooms/active/-/blob/master/CHANGELOG.md"
 # homepage = ""
 # documentation = ""
 
 # The following would provide a command line executable called `mypackage`
@@ -38,15 +40,14 @@
 [project.scripts]
 active = "atooms.active.cli:main"
 
 # Package building
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
- 
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = {"atooms.active" = ["*.f90"]}
```

