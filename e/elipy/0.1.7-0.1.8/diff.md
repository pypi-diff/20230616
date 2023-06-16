# Comparing `tmp/elipy-0.1.7.tar.gz` & `tmp/elipy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elipy-0.1.7.tar", max compression
+gzip compressed data, was "elipy-0.1.8.tar", max compression
```

## Comparing `elipy-0.1.7.tar` & `elipy-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1002 2023-02-03 11:02:34.583101 elipy-0.1.7/elipy/__init__.py
--rw-r--r--   0        0        0     6235 2023-02-03 10:32:59.943421 elipy-0.1.7/elipy/core/a2f_calculator.py
--rw-r--r--   0        0        0      841 2023-01-25 11:15:46.582987 elipy-0.1.7/elipy/core/constants.py
--rw-r--r--   0        0        0    11382 2023-02-07 14:20:10.129355 elipy-0.1.7/elipy/core/eliashberg.py
--rw-r--r--   0        0        0     7499 2023-02-07 14:19:04.969202 elipy-0.1.7/elipy/core/files_handling.py
--rw-r--r--   0        0        0     1301 2023-01-25 13:01:23.590241 elipy-0.1.7/elipy/core/grid.py
--rw-r--r--   0        0        0     3583 2023-02-07 13:33:54.465461 elipy-0.1.7/elipy/core/kpt_utils.py
--rw-r--r--   0        0        0     2795 2023-02-07 14:22:17.562604 elipy-0.1.7/elipy/core/messages.py
--rw-r--r--   0        0        0     1391 2023-01-25 13:15:53.505514 elipy-0.1.7/elipy/core/mpi.py
--rw-r--r--   0        0        0     1090 2023-02-03 10:49:12.836374 elipy-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      525 2023-02-07 14:28:17.717032 elipy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2427 2023-02-07 14:25:33.457975 elipy-0.1.7/README.md
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 elipy-0.1.7/setup.py
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 elipy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-09 08:02:09.061891 elipy-0.1.8/elipy/__init__.py
+-rw-r--r--   0        0        0     9686 2023-06-16 12:12:46.259774 elipy-0.1.8/elipy/core/a2f_calculator.py
+-rw-r--r--   0        0        0      841 2023-01-25 11:15:46.582987 elipy-0.1.8/elipy/core/constants.py
+-rw-r--r--   0        0        0    13084 2023-06-16 12:12:46.260787 elipy-0.1.8/elipy/core/eliashberg.py
+-rw-r--r--   0        0        0     8761 2023-06-16 12:12:46.263799 elipy-0.1.8/elipy/core/files_handling.py
+-rw-r--r--   0        0        0     1301 2023-01-25 13:01:23.590241 elipy-0.1.8/elipy/core/grid.py
+-rw-r--r--   0        0        0     3583 2023-02-07 13:33:54.465461 elipy-0.1.8/elipy/core/kpt_utils.py
+-rw-r--r--   0        0        0     3745 2023-06-16 12:13:58.979141 elipy-0.1.8/elipy/core/messages.py
+-rw-r--r--   0        0        0     1391 2023-01-25 13:15:53.505514 elipy-0.1.8/elipy/core/mpi.py
+-rw-r--r--   0        0        0     1090 2023-02-03 10:49:12.836374 elipy-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      525 2023-06-16 12:13:47.302719 elipy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2508 2023-06-16 12:15:15.160530 elipy-0.1.8/README.md
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 elipy-0.1.8/setup.py
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 elipy-0.1.8/PKG-INFO
```

### Comparing `elipy-0.1.7/elipy/__init__.py` & `elipy-0.1.8/elipy/__init__.py`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/elipy/core/a2f_calculator.py` & `elipy-0.1.8/elipy/core/a2f_calculator.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,14 +71,56 @@
         for j in range(Neps_pr):
             a2f_eew[i,j,:] = ( gaussian(w_arr[:], w_q, sigma_w) 
                             * gaussian(eps_pr_arr[j], eps_kq, sigma_eps_pr)
                             * gaussian(eps_arr[i], eps_k, sigma_eps) )
     return a2f_eew
 
 @njit()
+def get_ew_term(eps_k: np.float_, eps_kq: np.float_, w_q: np.float_, 
+                   sigma_eps: np.float_, sigma_w: np.float_, 
+                    eps_arr: np.ndarray, w_arr: np.ndarray,
+                    Neps: int, Nw: int, a2f_ew: np.ndarray) -> np.ndarray:
+    """get_ew_term calculate gaussian weights for all eigenvalues
+
+    Parameters
+    ----------
+    eps_k : np.float_
+        electron eigenvalue at k-point
+    eps_kq : np.float_
+        electron eigenvalue at k+q-point
+    w_q : np.float_
+        phonon eigenvalue at q-point
+    sigma_eps : np.float_
+        electron smearing for e
+    sigma_w : np.float_
+        phonon smearing
+    eps_arr : np.ndarray(Neps)
+        energy grid e
+    w_arr : np.ndarray(Nw)
+        frequency grid w
+    Neps : int
+        number of points in e grid
+    Nw : int
+        number of points in w grid
+    a2f_ew : np.ndarray(Neps, Nw)
+        array for gaussian weights, being rewritten every time
+
+    Returns
+    -------
+    np.ndarray
+        gaussian weights
+    """
+    # we don't require Nw, may change later
+    for i in range(Neps):
+        a2f_ew[i,:] = ( gaussian(w_arr[:], w_q, sigma_w) 
+                        * gaussian(eps_arr[i], eps_kq, sigma_eps)
+                        * gaussian(eps_arr[i], eps_k, sigma_eps) )
+    return a2f_ew
+
+@njit()
 def calculate_chunk(gkq_chunk: np.ndarray, eps_eig: np.ndarray, ph_eig: np.ndarray, 
                     nonzero_dims: tuple, ikqpts: list,
                     egrid: np.ndarray, e1grid: np.ndarray, phgrid: np.ndarray,
                     esmear: np.float_, e1smear: np.float_, phsmear: np.float_,
                     epoints: int, e1points: int, phpoints: int) -> np.ndarray:
     """calculate_chunk calculate a2F values for given |g|^2 chunk
 
@@ -127,25 +169,88 @@
         ik, iq, inu, ib, ibp = nk[i], nq[i], nnu[i], nb[i], nbp[i]
         ikq = ikqpts[iq][ik][0]
         w_q = ph_eig[iq, inu]
         eps_k = eps_eig[ik,ib]
         if (eps_k < ewindow_bounds[0])|(eps_k > ewindow_bounds[1]):
             continue # no need to account these values 
         eps_kq = eps_eig[ikq,ibp]
-        if (eps_k < e1window_bounds[0])|(eps_k > e1window_bounds[1]):
+        if (eps_kq < e1window_bounds[0])|(eps_kq > e1window_bounds[1]):
             continue # no need to account these values 
         g_kq = gkq_chunk[ik,iq,inu,ib,ibp]
         get_eew_term(eps_k, eps_kq, w_q,
                 esmear, e1smear, phsmear,
                 egrid, e1grid, phgrid,
                 epoints, e1points, phpoints,
                 a2f_temp)
         a2f_vals += a2f_temp * g_kq
     return a2f_vals
 
+@njit()
+def calculate_reduced_chunk(
+    gkq_chunk: np.ndarray, eps_eig: np.ndarray, ph_eig: np.ndarray, 
+    nonzero_dims: tuple, ikqpts: list,
+    egrid: np.ndarray, phgrid: np.ndarray,
+    esmear: np.float_, phsmear: np.float_,
+    epoints: int, phpoints: int
+) -> np.ndarray:
+    """calculate_chunk calculate a2F values for given |g|^2 chunk
+    for the special case e' == e
+
+    Parameters
+    ----------
+    gkq_chunk : np.ndarray
+        chunk of |g|^2 values
+    eps_eig : np.ndarray
+        electron eigenvalues
+    ph_eig : np.ndarray
+        phonon eigenvalues
+    nonzero_dims : tuple
+        indicies where |g|^2 != 0
+    ikqpts : list
+        maps of k->k+q points for every q
+    egrid : np.ndarray
+        energy grid e
+    phgrid : np.ndarray
+        frequency grid w
+    esmear : np.float_
+        electron smearing for e
+    phsmear : np.float_
+        phonon smearing
+    epoints : int
+        number of points in e grid
+    phpoints : int
+        number of points in w grid
+    Returns
+    -------
+    np.ndarray
+        a2F values for |g|^2 chunk
+    """
+    # countainers for a2f values
+    a2f_vals = np.zeros((epoints, phpoints))
+    a2f_temp = np.empty((epoints, phpoints))
+    ewindow_bounds = [np.amin(egrid), np.amax(egrid)]
+    nk, nq, nnu, nb, nbp = nonzero_dims
+    for i in range(len(nk)):
+        ik, iq, inu, ib, ibp = nk[i], nq[i], nnu[i], nb[i], nbp[i]
+        ikq = ikqpts[iq][ik][0]
+        w_q = ph_eig[iq, inu]
+        eps_k = eps_eig[ik,ib]
+        eps_kq = eps_eig[ikq,ibp]
+        if (eps_k < ewindow_bounds[0])|(eps_k > ewindow_bounds[1]):
+            continue # no need to account these values 
+        if (eps_kq < ewindow_bounds[0])|(eps_kq > ewindow_bounds[1]):
+            continue # no need to account these values 
+        g_kq = gkq_chunk[ik,iq,inu,ib,ibp]
+        get_ew_term(eps_k, eps_kq, w_q,
+                esmear, phsmear,
+                egrid, phgrid,
+                epoints, phpoints,
+                a2f_temp)
+        a2f_vals += a2f_temp * g_kq
+    return a2f_vals
     
 # def get_a2f_chunk(gkq_chunk: np.ndarray, kpts: np.ndarray, kpts_chunk: np.ndarray, qpts: np.ndarray,
 #                   eps_eig: np.ndarray, ph_eig: np.ndarray, 
 #                   egrid: Grid, e1grid: Grid, phgrid: Grid) -> np.ndarray:
 #     """get_a2f_chunk wrapper for calculate_chunk function
 
 #     Parameters
```

### Comparing `elipy-0.1.7/elipy/core/constants.py` & `elipy-0.1.8/elipy/core/constants.py`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/elipy/core/eliashberg.py` & `elipy-0.1.8/elipy/core/eliashberg.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 import numpy as np
 from numba.typed import List
 
 from .files_handling import *
 from .constants import *
 from .messages import *
 from .grid import Grid
-from .a2f_calculator import calculate_chunk #, get_a2f_chunk 
+from .a2f_calculator import calculate_chunk, calculate_reduced_chunk #, get_a2f_chunk 
 from .kpt_utils import get_kq2k
 
 from .mpi import MPI, comm, size, rank, master_only, mpi_watch, master
 
-class Elisahberg:
+class Eliashberg:
     """ contains methods for Eliashberg function a2F(e,e',w) calculation
     """
     def __init__(self, gkq_file: str|Path,
+                 ee1grid: bool = False,
                  ewindow: list = [default_emin, default_emax], esmear: float = default_esmear, 
                  epoints: int = default_epoints, eunits: str = 'Ha',
                  e1window: list = None, e1smear: float = None,
                  e1points: int = None, e1units: str = None,
                  phwindow: list = None, phsmear: float = default_phsmear,
                  phpoints: int = default_phpoints, phunits: str = 'Ha',
                  out_file: str|Path = Path.cwd()/'eliashberg_eew.nc') -> None:
         """__init__ parameters for Eliashberg class
 
         Parameters
         ----------
         gkq_file : str | Path
             Path to netCDF4 file with |g|^2 eph matrix elements
+        ee1grid: bool, optional
+            If true, code calculates a2F(e,e',w); otherwise, a2F(e,w) is calculated
         ewindow : list, optional
             window for electron energies,
             by default [default_emin, default_emax]
         esmear : float, optional
             smearing of electron delta function,
             by default default_esmear
         epoints : int, optional
@@ -65,21 +68,23 @@
         phunits : str, optional
             phonon frequency unit, by default 'Ha'
         out_file : str | Path, optional
             path to netCDF4 file for output storage,
             by default Path.cwd()/'eliashberg_eew.nc'
         """
         self.gkq_file = gkq_file
+        self.ee1grid = ee1grid
         self.egrid = Grid(*ewindow, esmear, epoints, eunits)
         # use the same parameters for e and e1 by default
-        e1window = ewindow if not e1window else e1window
-        e1smear = esmear if not e1smear else e1smear
-        e1points = epoints if not e1points else e1points
-        e1units = eunits if not e1units else e1units
-        self.e1grid = Grid(*e1window, e1smear, e1points, e1units)
+        if self.ee1grid:
+            e1window = ewindow if not e1window else e1window
+            e1smear = esmear if not e1smear else e1smear
+            e1points = epoints if not e1points else e1points
+            e1units = eunits if not e1units else e1units
+            self.e1grid = Grid(*e1window, e1smear, e1points, e1units)
         # phonon grid is set according to phonon eigenvalues by default. 
         # If phonon window is chosen, use these values
         if phwindow:
             self.phgrid = Grid(*phwindow, phsmear, phpoints, phunits)
         else:
             self.phgrid = None # will be initialized later
         self.__phsmear = phsmear
@@ -97,14 +102,16 @@
         self.g_kpts, self.g_qpts, self.efermi = gkq_data['kpts'], gkq_data['qpts'], gkq_data['efermi']
         self.e_eigvals = gkq_data['e_eigs']
         self.ph_eigvals = gkq_data['ph_eigs']
         # if everything is OK, make electron eigenvalues Fermi energy centered
         self.e_eigvals = self.e_eigvals - self.efermi
         # g_kq has shape `[nq,nk,...]`, we swap 0th and 1st dimensions for convenience
         self.gkq_vals = np.swapaxes(gkq_vals, 0, 1)
+        # ensure gkq array to be C-contiguous in memory
+        self.gkq_vals = np.ascontiguousarray(self.gkq_vals)
         # and set up variables for all dimensions
        
     @mpi_watch
     def broadcast_dims(self):
         """broadcast_dims broadcasts dimensions of all arrays to cpus
         """               
         if master:
@@ -117,16 +124,16 @@
     @mpi_watch
     def broadcast_kqpoints(self):
         """broadcast_kqpoints broadcasts k- and q-point arrays to cpus
         """       
         if not master:
             self.g_kpts = np.empty((self.nkpt, 3), dtype=np.float64)
             self.g_qpts = np.empty((self.nqpt, 3), dtype=np.float64)
-            self.ewin_ikpts = None
-            self.e1win_ikpts = None
+            # self.ewin_ikpts = None
+            # self.e1win_ikpts = None
         comm.Bcast([self.g_kpts, MPI.DOUBLE])
         comm.Bcast([self.g_qpts, MPI.DOUBLE])
         
     @mpi_watch
     def broadcast_eigvals(self):
         """broadcast_eigvals broadcasts electron and phonon eigenvalues to cpus
         """
@@ -136,97 +143,131 @@
         comm.Bcast([self.e_eigvals, MPI.DOUBLE])
         comm.Bcast([self.ph_eigvals, MPI.DOUBLE])
         # if phonon grid is not set, do it now    
         phmin = np.amin(self.ph_eigvals)
         phmin = 0 if phmin >= 0 else phmin - ph_delta
         if not self.phgrid:           
             self.phgrid = Grid(phmin, np.amax(self.ph_eigvals) + ph_delta,
-                               self.__phsmear*unit_conversion[self.__phunits], self.__phpoints, 'Ha')
+                               self.__phsmear*unit_conversion[self.__phunits],
+                               self.__phpoints, 'Ha')
 
 
-    # for some reason, scattering of n-dimensional array doesn't work
+    # here array is flatten to 1d and back to nd, but it may brake everything at some point
     # @mpi_watch
     # def scatter_gkq_vals(self):
-    #     # scatter gkq values to cpu-s over nkpt dimension
+    #     """scatter_gkq_vals distributes |g|^2 values over cpus
+    #     """
     #     # TODO: think about scattering over nqpt as well
-    #     if not master:
-    #         self.gkq_vals = None
+    #     if master: 
+    #         gkq_flatten = self.gkq_vals.flatten()
+    #     else:
+    #         gkq_flatten = None
     #     # find dimension of chunks per cpu and number dimension displacemen
     #     ave, res = divmod(self.nkpt, size)
     #     counts = np.array([ave + 1 if p < res else ave for p in range(size)], dtype=int)
     #     # self because will call it later
     #     self.__displ = np.array([sum(counts[:p]) for p in range(size)], dtype=int)
-    #     # allocate space for chunk
-    #     self.gkq_chunk = np.empty((counts[rank], self.nqpt, self.nbranch, self.nband, self.nband))
     #     rest_dims = self.nqpt*self.nbranch*self.nband*self.nband
-    #     comm.Scatterv([self.gkq_vals, counts*rest_dims, self.__displ*rest_dims, MPI.DOUBLE], self.gkq_chunk, root=0)
+    #     # allocate space for chunk
+    #     self.gkq_chunk = np.empty(counts[rank]*rest_dims)
+    #     comm.Scatterv([gkq_flatten, counts*rest_dims, self.__displ*rest_dims, MPI.DOUBLE],
+    #                   self.gkq_chunk, root=0)    
+    #     self.gkq_chunk = self.gkq_chunk.reshape((counts[rank], self.nqpt, self.nbranch,
+    #                                              self.nband, self.nband))
 
-    # here array is flatten to 1d and back to nd, but it may brake everything at some point
+    # TODO: think how to send LARGE amounts of data
     @mpi_watch
     def scatter_gkq_vals(self):
         """scatter_gkq_vals distributes |g|^2 values over cpus
         """
-        # TODO: think about scattering over nqpt as well
-        if master: 
-            gkq_flatten = self.gkq_vals.flatten()
-        else:
-            gkq_flatten = None
         # find dimension of chunks per cpu and number dimension displacemen
         ave, res = divmod(self.nkpt, size)
         counts = np.array([ave + 1 if p < res else ave for p in range(size)], dtype=int)
-        # self because will call it later
         self.__displ = np.array([sum(counts[:p]) for p in range(size)], dtype=int)
-        rest_dims = self.nqpt*self.nbranch*self.nband*self.nband
-        # allocate space for chunk
-        self.gkq_chunk = np.empty(counts[rank]*rest_dims)
-        comm.Scatterv([gkq_flatten, counts*rest_dims, self.__displ*rest_dims, MPI.DOUBLE], self.gkq_chunk, root=0)    
-        self.gkq_chunk = self.gkq_chunk.reshape((counts[rank], self.nqpt, self.nbranch, self.nband, self.nband))
+        if master:
+            for i in range(1, size):
+                if i != size-1:
+                    comm.Send([self.gkq_vals[self.__displ[i]:self.__displ[i+1]], MPI.REAL8],
+                            dest=i, tag=10+i)
+                else:
+                    comm.Send([self.gkq_vals[self.__displ[i]:], MPI.REAL8],
+                            dest=i, tag=10+i)
+            self.gkq_chunk = self.gkq_vals[:self.__displ[1]]
+        else:
+            chunk_shape = (counts[rank],self.nqpt,self.nbranch,self.nband,self.nband)
+            self.gkq_chunk = np.empty(chunk_shape, dtype=np.float64)
+            comm.Recv([self.gkq_chunk, MPI.REAL8], source=0, tag=10+rank)
         
     @mpi_watch
     def sum_chunks(self):
         """sum_chunks calculates a2f values for distributed |g|^2 chunk and sums them
         """
         # allocate array summing chunks from all cpu-s
-        self.a2f_vals = np.empty((self.egrid.npoints,
-                                self.e1grid.npoints,
-                                self.phgrid.npoints)) 
+        if rank == 0:
+            if self.ee1grid:
+                self.a2f_vals = np.empty((self.egrid.npoints,
+                                    self.e1grid.npoints,
+                                    self.phgrid.npoints)) 
+            else:
+                self.a2f_vals = np.empty((self.egrid.npoints,
+                                        self.phgrid.npoints)) 
+        else:
+            self.a2f_vals = None
+        
         # get the proper subset of kpoints
         if rank != size-1:
             kpts_chunk = self.g_kpts[self.__displ[rank]:self.__displ[rank+1],:]
         else:
             kpts_chunk = self.g_kpts[self.__displ[rank]:,:]
 
         # mapping of BZ: for every q get k+q -> k 
         ikqpts = List()
         [ikqpts.append(get_kq2k(self.g_kpts, kpts_chunk, qpt)) for qpt in self.g_qpts]
         # take only nonzero values of gkq_chunk
         where_nonzero = np.nonzero(self.gkq_chunk)
-        a2f_chunk = calculate_chunk(self.gkq_chunk, self.e_eigvals, self.ph_eigvals,
-                                where_nonzero, ikqpts,
-                                self.egrid.grid, self.e1grid.grid, self.phgrid.grid,
-                                self.egrid.smear, self.e1grid.smear, self.phgrid.smear,
-                                self.egrid.npoints, self.e1grid.npoints, self.phgrid.npoints)
-        
+        if self.ee1grid:
+            # calculate one chunk
+            a2f_chunk = calculate_chunk(
+                self.gkq_chunk, self.e_eigvals, self.ph_eigvals,
+                where_nonzero, ikqpts,
+                self.egrid.grid, self.e1grid.grid, self.phgrid.grid,
+                self.egrid.smear, self.e1grid.smear, self.phgrid.smear,
+                self.egrid.npoints, self.e1grid.npoints, self.phgrid.npoints
+                                        )
+        else:
+            a2f_chunk = calculate_reduced_chunk(
+                self.gkq_chunk, self.e_eigvals, self.ph_eigvals,
+                where_nonzero, ikqpts,
+                self.egrid.grid, self.phgrid.grid,
+                self.egrid.smear, self.phgrid.smear,
+                self.egrid.npoints, self.phgrid.npoints
+            )
+
         # calculate a2f values for given chunck        
         # a2f_chunk = get_a2f_chunk(self.gkq_chunk, self.g_kpts, kpts_chunk, self.g_qpts, 
         #                           self.e_eigvals, self.ph_eigvals,
         #                           self.egrid, self.e1grid, self.phgrid)
         
-        comm.Reduce([a2f_chunk, MPI.DOUBLE], [self.a2f_vals, MPI.DOUBLE], op=MPI.SUM, root=0)       
+        comm.Reduce([a2f_chunk, MPI.DOUBLE], [self.a2f_vals, MPI.DOUBLE],
+                    op=MPI.SUM, root=0)       
             
     @master_only
     def write_netcdf(self):
         """write_netcdf writes a2f to netCDF4 file
         """
         # multiply Eliashberg function to (almost) correct prefactor
         self.a2f_vals = self.a2f_vals * (2/self.nkpt/self.nqpt) # division to g(Ef) is up to user!
         # save computed Eliashberg function to netCDF file
-        store_a2f_values(self.out_file, self.efermi, 
-                         self.egrid, self.e1grid, self.phgrid, self.a2f_vals)
-        
+        if self.ee1grid:
+            store_a2f_values(self.out_file, self.efermi, 
+                            self.egrid, self.e1grid, self.phgrid, self.a2f_vals)
+        else:
+            store_a2f_reduced_values(self.out_file, self.efermi, 
+                            self.egrid, self.phgrid, self.a2f_vals)
+                    
     def compute_a2f(self):
         """compute_a2f gathers all previous methods together into united workflow
         """
         # and add status messages to log file
         if master:
         # we don't need to log everything 
             start = time()           
@@ -234,15 +275,18 @@
         self.read_data()
         print_read_status(self.gkq_file)
         self.broadcast_dims()
         print_mpi_info(self.nkpt//size)
         self.broadcast_kqpoints()
         self.broadcast_eigvals()
         self.scatter_gkq_vals()
-        print_variables(self.egrid, self.e1grid, self.phgrid)
+        if self.ee1grid:
+            print_variables(self.egrid, self.phgrid, self.e1grid)
+        else:
+            print_variables(self.egrid, self.phgrid)
         
         # print_computation()
         self.sum_chunks()
         
         self.write_netcdf()
         print_save_status(self.out_file)
```

### Comparing `elipy-0.1.7/elipy/core/files_handling.py` & `elipy-0.1.8/elipy/core/files_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,11 +189,44 @@
     ncout.createDimension('number_of_frequencies', phgrid.npoints)
     evar = ncout.createVariable('energy','float64',('number_of_epoints'))
     evar[:] = egrid.grid
     e1var = ncout.createVariable('energy_pr','float64',('number_of_e1points'))
     e1var[:] = e1grid.grid
     phvar = ncout.createVariable('frequency','float64',('number_of_frequencies'))
     phvar[:] = phgrid.grid
-    a2fvar = ncout.createVariable('a2f','float64',('number_of_epoints','number_of_e1points','number_of_frequencies'))
-    a2fvar.setncattr('units','mm')
+    a2fvar = ncout.createVariable('a2f','float64',('number_of_epoints',
+                                                   'number_of_e1points','number_of_frequencies'))
     a2fvar[:] = a2f_vals
     ncout.close()      
+
+def store_a2f_reduced_values(out_path: str|Path, efermi: np.float_,
+                     egrid: Grid, phgrid: Grid, a2f_vals: np.ndarray) -> None:
+    """store_a2f_values saves output data no netCDF4 file
+    for the special case e' == e
+
+    Parameters
+    ----------
+    out_path : str | Path
+        path to output file
+    efermi : np.float_
+        Fermi energy of a system
+    egrid : Grid
+        electron energy grid e
+    phgrid : Grid
+        phonon frequency grid w
+    a2f_vals : np.ndarray
+        a2F(e,w) values
+    """
+    out_path = check_out_path(out_path)
+    ncout = nc.Dataset(out_path,'w')
+    efvar = ncout.createVariable('Fermi_energy', 'float64') 
+    efvar[0] = efermi
+    ncout.createDimension('number_of_epoints', egrid.npoints)
+    ncout.createDimension('number_of_frequencies', phgrid.npoints)
+    evar = ncout.createVariable('energy','float64',('number_of_epoints'))
+    evar[:] = egrid.grid
+    phvar = ncout.createVariable('frequency','float64',('number_of_frequencies'))
+    phvar[:] = phgrid.grid
+    a2fvar = ncout.createVariable('a2f','float64',
+                                  ('number_of_epoints','number_of_frequencies'))
+    a2fvar[:] = a2f_vals
+    ncout.close()
```

### Comparing `elipy-0.1.7/elipy/core/grid.py` & `elipy-0.1.8/elipy/core/grid.py`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/elipy/core/kpt_utils.py` & `elipy-0.1.8/elipy/core/kpt_utils.py`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/elipy/core/messages.py` & `elipy-0.1.8/elipy/core/messages.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from .grid import Grid
 from .mpi import master_only, size
 
 @master_only
 def print_header():
     __version__ = importlib.metadata.version("elipy")
-    # __version__ = "0.1.5"
+    # __version__ = "0.1.8"
     header_message = f"""
 elipy v{__version__} -- post-processing tool for ABINIT EPH package
 Started at: {datetime.now().strftime("%Y-%m-%d %H:%M:%S")}
     """
     print(header_message, flush=True)
 
 @master_only
@@ -26,38 +26,60 @@
 def print_read_status(g_file: Path) -> None:
     read_status_message = f"""
 Electron-phonon matrix elements, electron and phonon eigenvalues:\n{str(g_file)}
     """
     print(read_status_message, flush=True)
    
 @master_only   
-def print_variables(egrid: Grid, e1grid: Grid, phgrid: Grid) -> None:
-    variables_message = f"""
--------------------------------------------------------------------------------------
-                    Variables that govern the present computation
--------------------------------------------------------------------------------------
-
-all values in atomic units
-
-e_grid:
-    e_window    {egrid.g_min:.3e}  {egrid.g_max:.3e}
-    e_smearing  {egrid.smear:.3e} 
-    e_npoints    {egrid.npoints}
-e1_grid:
-    e1_window    {e1grid.g_min:.3e}  {e1grid.g_max:.3e}
-    e1_smearing  {e1grid.smear:.3e} 
-    e1_npoints    {e1grid.npoints}
-ph_grid:
-    ph_window    {phgrid.g_min:.3e}  {phgrid.g_max:.3e}
-    ph_smearing  {phgrid.smear:.3e} 
-    ph_npoints    {phgrid.npoints}
--------------------------------------------------------------------------------------
-
--------------------------------------------------------------------------------------
-    """
+def print_variables(egrid: Grid, phgrid: Grid, e1grid: Grid = None) -> None:
+    if e1grid:
+        variables_message = f"""
+    -------------------------------------------------------------------------------------
+                        Variables that govern the present computation
+    -------------------------------------------------------------------------------------
+
+    all values in atomic units
+
+    e_grid:
+        e_window    {egrid.g_min:.3e}  {egrid.g_max:.3e}
+        e_smearing  {egrid.smear:.3e} 
+        e_npoints    {egrid.npoints}
+    e1_grid:
+        e1_window    {e1grid.g_min:.3e}  {e1grid.g_max:.3e}
+        e1_smearing  {e1grid.smear:.3e} 
+        e1_npoints    {e1grid.npoints}
+    ph_grid:
+        ph_window    {phgrid.g_min:.3e}  {phgrid.g_max:.3e}
+        ph_smearing  {phgrid.smear:.3e} 
+        ph_npoints    {phgrid.npoints}
+    -------------------------------------------------------------------------------------
+
+    -------------------------------------------------------------------------------------
+        """
+    else:
+        variables_message = f"""
+    -------------------------------------------------------------------------------------
+                        Variables that govern the present computation
+    -------------------------------------------------------------------------------------
+
+    all values in atomic units
+
+    e_grid:
+        e_window    {egrid.g_min:.3e}  {egrid.g_max:.3e}
+        e_smearing  {egrid.smear:.3e} 
+        e_npoints    {egrid.npoints}
+    ph_grid:
+        ph_window    {phgrid.g_min:.3e}  {phgrid.g_max:.3e}
+        ph_smearing  {phgrid.smear:.3e} 
+        ph_npoints    {phgrid.npoints}
+    -------------------------------------------------------------------------------------
+
+    -------------------------------------------------------------------------------------
+        """
+        
     print(variables_message, flush=True)
 
 @master_only
 def print_computation() -> None:
     computation_message = """
 -------------------------------------------------------------------------------------
                                 Computation progress
```

### Comparing `elipy-0.1.7/elipy/core/mpi.py` & `elipy-0.1.8/elipy/core/mpi.py`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/LICENSE.txt` & `elipy-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elipy-0.1.7/pyproject.toml` & `elipy-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elipy"
-version = "0.1.7"
+version = "0.1.8"
 description = "Post-processing tool for Abinit >= 9.8.1 aiming to calculate energy-resolved Eliashberg function"
 authors = ["Fedor Akhmetov <f.akhmetov@utwente.nl>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "elipy"}]
 
 [tool.poetry.dependencies]
```

### Comparing `elipy-0.1.7/README.md` & `elipy-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 ## Authors
 
 [Fedor Akhmetov](https://github.com/Radioteddy)
 
 ## Version History
 
+* 0.1.8
+    * collective communication for matrix elements replaced by p2p one
 * 0.1.7
     * electron and phonon eigenvalues are taken from GSTORE
 * 0.1.6
     * minor bugfixes and improvements
 * 0.1.5
     * Working Release
 * 0.1.0
```

### Comparing `elipy-0.1.7/setup.py` & `elipy-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'netCDF4>=1.5.7,<2.0.0',
  'numba>=0.56.4,<0.57.0',
  'numpy>=1.23.5,<2.0.0',
  'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'elipy',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Post-processing tool for Abinit >= 9.8.1 aiming to calculate energy-resolved Eliashberg function',
-    'long_description': "# Elipy\n\nPost-processing tool for ABINIT >= 9.8.1 aiming for calculation of energy-resolved Eliashberg function\n\n## Description\n\nSince version 9.8.1 ABINIT provides easy-to-use methods within EPH package for the calculation of electron-phonon matrix elements on rectangular k- and q-point grids (optdriver 7, eph_task 11). The present package is a tool for calculation of electron-energy-resolved Eliashberg function on arbitrary electron and phonon grids. \n\n$$\n\\alpha^2 F(\\epsilon,\\epsilon',\\omega)=\\frac{1}{N_\\mathbf{k}N_\\mathbf{q}}\\sum_{\\mathbf{k}\\mathbf{q}mn\\nu}\\left|g_{mn\\nu}(\\mathbf{k},\\mathbf{q})\\right|^2\\delta(\\epsilon_{\\mathbf{k}n}-\\epsilon)\\delta(\\epsilon_{\\mathbf{k+q}m}-\\epsilon')\\delta(\\omega_{\\mathbf{q}\\nu}-\\omega)\n$$\n\nThe above-written definition does not include electron density of states at Fermi level. One needs to divide $\\alpha^2 F$ over $N_F$ to get physically meaningful results. \n\nProject uses mpi4py for many-core parallelization and Numba for acceleration of procedures dealing with iteration over numpy arrays.\n\nElipy is insipired by [ElectronPhononCoupling](https://github.com/GkAntonius/ElectronPhononCoupling) and [Abipy](https://github.com/abinit/abipy) projects, and uses some of their utility functions. Apologies for code copy-pasting, it allows to keep dependency list as short as possible.  \n\n### Limitations\n\n* only Gaussian smearing summation for delta functions\n* no account for spin of electron states\n\n## Getting Started\n\n### Dependencies\n\n* Numpy\n* Scipy\n* netCDF4\n* Numba\n* mpi4py\n\nThe actual versions of required packages are stored in pyproject.toml file.\n\n### Installation\n\n```\npip install elipy\n```\nALternatively, one can build code with [Poetry](https://python-poetry.org) package manager:\n\n```\ngit clone https://github.com/Radioteddy/elipy.git\ncd elipy\npoetry install\n```\n### Executing program\n\n* Use mpirun, mpiexec, srun,... for program execution\n```\nmpiexec -n X python filename.py > out 2> err\n```\n\n## Authors\n\n[Fedor Akhmetov](https://github.com/Radioteddy)\n\n## Version History\n\n* 0.1.7\n    * electron and phonon eigenvalues are taken from GSTORE\n* 0.1.6\n    * minor bugfixes and improvements\n* 0.1.5\n    * Working Release\n* 0.1.0\n    * Initial Release\n\n## Acknowledgments\n* [ElectronPhononCoupling](https://github.com/GkAntonius/ElectronPhononCoupling)\n* [Abipy](https://github.com/abinit/abipy)\n",
+    'long_description': "# Elipy\n\nPost-processing tool for ABINIT >= 9.8.1 aiming for calculation of energy-resolved Eliashberg function\n\n## Description\n\nSince version 9.8.1 ABINIT provides easy-to-use methods within EPH package for the calculation of electron-phonon matrix elements on rectangular k- and q-point grids (optdriver 7, eph_task 11). The present package is a tool for calculation of electron-energy-resolved Eliashberg function on arbitrary electron and phonon grids. \n\n$$\n\\alpha^2 F(\\epsilon,\\epsilon',\\omega)=\\frac{1}{N_\\mathbf{k}N_\\mathbf{q}}\\sum_{\\mathbf{k}\\mathbf{q}mn\\nu}\\left|g_{mn\\nu}(\\mathbf{k},\\mathbf{q})\\right|^2\\delta(\\epsilon_{\\mathbf{k}n}-\\epsilon)\\delta(\\epsilon_{\\mathbf{k+q}m}-\\epsilon')\\delta(\\omega_{\\mathbf{q}\\nu}-\\omega)\n$$\n\nThe above-written definition does not include electron density of states at Fermi level. One needs to divide $\\alpha^2 F$ over $N_F$ to get physically meaningful results. \n\nProject uses mpi4py for many-core parallelization and Numba for acceleration of procedures dealing with iteration over numpy arrays.\n\nElipy is insipired by [ElectronPhononCoupling](https://github.com/GkAntonius/ElectronPhononCoupling) and [Abipy](https://github.com/abinit/abipy) projects, and uses some of their utility functions. Apologies for code copy-pasting, it allows to keep dependency list as short as possible.  \n\n### Limitations\n\n* only Gaussian smearing summation for delta functions\n* no account for spin of electron states\n\n## Getting Started\n\n### Dependencies\n\n* Numpy\n* Scipy\n* netCDF4\n* Numba\n* mpi4py\n\nThe actual versions of required packages are stored in pyproject.toml file.\n\n### Installation\n\n```\npip install elipy\n```\nALternatively, one can build code with [Poetry](https://python-poetry.org) package manager:\n\n```\ngit clone https://github.com/Radioteddy/elipy.git\ncd elipy\npoetry install\n```\n### Executing program\n\n* Use mpirun, mpiexec, srun,... for program execution\n```\nmpiexec -n X python filename.py > out 2> err\n```\n\n## Authors\n\n[Fedor Akhmetov](https://github.com/Radioteddy)\n\n## Version History\n\n* 0.1.8\n    * collective communication for matrix elements replaced by p2p one\n* 0.1.7\n    * electron and phonon eigenvalues are taken from GSTORE\n* 0.1.6\n    * minor bugfixes and improvements\n* 0.1.5\n    * Working Release\n* 0.1.0\n    * Initial Release\n\n## Acknowledgments\n* [ElectronPhononCoupling](https://github.com/GkAntonius/ElectronPhononCoupling)\n* [Abipy](https://github.com/abinit/abipy)\n",
     'author': 'Fedor Akhmetov',
     'author_email': 'f.akhmetov@utwente.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `elipy-0.1.7/PKG-INFO` & `elipy-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elipy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Post-processing tool for Abinit >= 9.8.1 aiming to calculate energy-resolved Eliashberg function
 License: MIT
 Author: Fedor Akhmetov
 Author-email: f.akhmetov@utwente.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -73,14 +73,16 @@
 
 ## Authors
 
 [Fedor Akhmetov](https://github.com/Radioteddy)
 
 ## Version History
 
+* 0.1.8
+    * collective communication for matrix elements replaced by p2p one
 * 0.1.7
     * electron and phonon eigenvalues are taken from GSTORE
 * 0.1.6
     * minor bugfixes and improvements
 * 0.1.5
     * Working Release
 * 0.1.0
```

