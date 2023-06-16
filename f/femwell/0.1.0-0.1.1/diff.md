# Comparing `tmp/femwell-0.1.0.tar.gz` & `tmp/femwell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.0.tar", max compression
+gzip compressed data, was "femwell-0.1.1.tar", max compression
```

## Comparing `femwell-0.1.0.tar` & `femwell-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2023-04-29 13:21:37.219888 femwell-0.1.0/LICENSE
--rw-r--r--   0        0        0     2480 2023-04-29 13:21:37.219888 femwell-0.1.0/README.md
--rw-r--r--   0        0        0      255 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5762 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/fefd.py
--rw-r--r--   0        0        0     1304 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/laplace.py
--rw-r--r--   0        0        0    16525 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7713 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/waveguide.py
--rw-r--r--   0        0        0      974 2023-04-29 13:21:50.956002 femwell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 femwell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 21:17:55.657797 femwell-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2480 2023-06-16 21:17:55.657797 femwell-0.1.1/README.md
+-rw-r--r--   0        0        0      255 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5762 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/fefd.py
+-rw-r--r--   0        0        0     1304 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/laplace.py
+-rw-r--r--   0        0        0    17327 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7713 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4224 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/waveguide.py
+-rw-r--r--   0        0        0      974 2023-06-16 21:18:06.821815 femwell-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.1/PKG-INFO
```

### Comparing `femwell-0.1.0/LICENSE` & `femwell-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/README.md` & `femwell-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/culomb.py` & `femwell-0.1.1/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/eme.py.bak` & `femwell-0.1.1/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.1/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/fefd.py` & `femwell-0.1.1/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/fiber.py` & `femwell-0.1.1/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/laplace.py` & `femwell-0.1.1/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/maxwell/waveguide.py` & `femwell-0.1.1/femwell/maxwell/waveguide.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ElementTriN1,
     ElementTriN2,
     ElementTriP0,
     ElementTriP1,
     ElementTriP2,
     ElementVector,
     Functional,
+    InteriorFacetBasis,
     LinearForm,
     Mesh,
     condense,
     solve,
 )
 from skfem.helpers import cross, curl, dot, grad, inner
 from skfem.utils import solver_eigen_scipy
@@ -191,15 +192,15 @@
     *,
     mu_r=1,
     num_modes=1,
     order=1,
     metallic_boundaries=False,
     radius=np.inf,
     n_guess=None,
-    solver="slepc",
+    solver="scipy",
 ) -> Modes:
     if solver == "scipy":
         solver = solver_eigen_scipy
     elif solver == "slepc":
         from femwell.solver import solver_eigen_slepc
 
         solver = solver_eigen_slepc
@@ -236,15 +237,15 @@
 
     A = aform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
     B = bform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
 
     if n_guess:
         sigma = sigma = k0**2 * n_guess**2
     else:
-        sigma = sigma = k0**2 * np.max(epsilon_r) ** 2
+        sigma = sigma = k0**2 * np.max(epsilon_r)
 
     if metallic_boundaries:
         lams, xs = solve(
             *condense(
                 -A,
                 -B,
                 D=basis.get_dofs(None if metallic_boundaries is True else metallic_boundaries),
@@ -415,15 +416,15 @@
     plot_basis = et_basis.with_element(ElementVector(ElementDG(ElementTriP1())))
     et_xy = plot_basis.project(et_basis.interpolate(et))
     (et_x, et_x_basis), (et_y, et_y_basis) = plot_basis.split(et_xy)
 
     rc = (3, 1) if direction != "x" else (1, 3)
     fig, axs = plt.subplots(*rc, subplot_kw=dict(aspect=1))
     for ax in axs:
-        basis.mesh.draw(ax=ax, boundaries=True, boundaries_only=True)
+        basis.mesh.draw(ax=ax, boundaries_only=True)
         for subdomain in basis.mesh.subdomains.keys() - {"gmsh:bounding_entities"}:
             basis.mesh.restrict(subdomain).draw(ax=ax, boundaries_only=True)
 
     for ax, component in zip(axs, "xyz"):
         ax.set_title(f"${title}_{component}$")
 
     maxabs = max(np.max(np.abs(data.value)) for data in basis.interpolate(mode))
@@ -443,14 +444,41 @@
                 cax = divider.append_axes("right", size="5%", pad=0.05)
                 plt.colorbar(ax.collections[-1], cax=cax)
             plt.tight_layout()
 
     return fig, axs
 
 
+def eval_error_estimator(basis, u):
+    @Functional
+    def interior_residual(w):
+        h = w.h
+        x, y = w.x
+        return h**2  # * load_func(x, y) ** 2
+
+    eta_K = interior_residual.elemental(basis, w=basis.interpolate(u))
+
+    # facet jump
+    fbasis = [InteriorFacetBasis(basis.mesh, basis.elem, side=i) for i in [0, 1]]
+    w = {"u" + str(i + 1): fbasis[i].interpolate(u) for i in [0, 1]}
+
+    @Functional
+    def edge_jump(w):
+        return w.h * (
+            np.abs(dot(grad(w["u1"][1]) - grad(w["u2"][1]), w.n)) ** 2
+            + np.abs(dot(w["u1"][0] - w["u2"][0], w.n)) ** 2
+        )
+
+    tmp = np.zeros(basis.mesh.facets.shape[1])
+    tmp[fbasis[0].find] = edge_jump.elemental(fbasis[0], **w)
+    eta_E = np.sum(0.5 * tmp[basis.mesh.t2f], axis=0)
+
+    return eta_K + eta_E
+
+
 if __name__ == "__main__":
     from collections import OrderedDict
 
     from shapely.geometry import Polygon
 
     from femwell.mesh import mesh_from_OrderedDict
```

### Comparing `femwell-0.1.0/femwell/mesh/mesh.py` & `femwell-0.1.1/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mesh/meshtracker.py` & `femwell-0.1.1/femwell/mesh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mesh/slice.py` & `femwell-0.1.1/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mesh.py` & `femwell-0.1.1/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mode_solver_1d.py` & `femwell-0.1.1/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.1/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.1/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mode_solver_inplane.py` & `femwell-0.1.1/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/mode_solver_schrodinger.py` & `femwell-0.1.1/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/pn_analytical.py` & `femwell-0.1.1/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/solver.py` & `femwell-0.1.1/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/tcad.py` & `femwell-0.1.1/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/tests/test_mesh.py` & `femwell-0.1.1/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/thermal.py` & `femwell-0.1.1/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/thermal_transient.py` & `femwell-0.1.1/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/utils.py` & `femwell-0.1.1/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/visualization.py` & `femwell-0.1.1/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/femwell/waveguide.py` & `femwell-0.1.1/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.0/pyproject.toml` & `femwell-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "femwell"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.0/PKG-INFO` & `femwell-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.0
+Version: 0.1.1
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: gmsh
 Requires-Dist: matplotlib
 Requires-Dist: pygmsh
 Requires-Dist: scikit-fem (>=8.0.0)
 Requires-Dist: shapely (>=2.0.0)
 Project-URL: Documentation, https://HelgeGehring.github.io/femwell/
```

