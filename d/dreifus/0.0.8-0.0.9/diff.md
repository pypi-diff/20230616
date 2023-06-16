# Comparing `tmp/dreifus-0.0.8.tar.gz` & `tmp/dreifus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-gdlwbtsm/dreifus-0.0.8.tar", last modified: Tue Jun  6 22:51:02 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-3h5abee6/dreifus-0.0.9.tar", last modified: Fri Jun 16 11:10:03 2023, max compression
```

## Comparing `dreifus-0.0.8.tar` & `dreifus-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.625413 dreifus-0.0.8/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-06 22:51:02.621402 dreifus-0.0.8/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.8/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-06 22:50:08.000000 dreifus-0.0.8/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-06 22:51:02.625413 dreifus-0.0.8/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.8/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:01.695326 dreifus-0.0.8/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.029315 dreifus-0.0.8/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.8/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.8/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5926 2023-06-06 18:50:08.000000 dreifus-0.0.8/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1550 2023-06-06 21:52:50.000000 dreifus-0.0.8/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.324371 dreifus-0.0.8/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.0.8/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.8/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.8/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.8/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17626 2023-06-06 18:45:27.000000 dreifus-0.0.8/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.8/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.0.8/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.8/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      952 2023-06-06 21:55:22.000000 dreifus-0.0.8/src/dreifus/render.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.8/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.379828 dreifus-0.0.8/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.8/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.8/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.494097 dreifus-0.0.8/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.8/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.8/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.8/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.8/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.134255 dreifus-0.0.8/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      922 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-06 22:51:01.000000 dreifus-0.0.8/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-06 22:51:02.599897 dreifus-0.0.8/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.8/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.0.8/test/test_camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.8/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.8/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.8/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:03.166873 dreifus-0.0.9/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-16 11:10:03.152836 dreifus-0.0.9/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.9/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-16 11:09:14.000000 dreifus-0.0.9/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-16 11:10:03.168617 dreifus-0.0.9/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.9/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:01.839337 dreifus-0.0.9/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.185717 dreifus-0.0.9/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.9/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.9/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6338 2023-06-16 11:08:44.000000 dreifus-0.0.9/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1550 2023-06-06 21:52:50.000000 dreifus-0.0.9/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.676022 dreifus-0.0.9/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      285 2023-06-06 17:30:54.000000 dreifus-0.0.9/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.9/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.9/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.9/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17626 2023-06-06 18:45:27.000000 dreifus-0.0.9/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.9/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4824 2023-06-06 17:53:09.000000 dreifus-0.0.9/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.9/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      952 2023-06-06 21:55:22.000000 dreifus-0.0.9/src/dreifus/render.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.9/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.772160 dreifus-0.0.9/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.9/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.9/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.961296 dreifus-0.0.9/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.9/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.9/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.9/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.9/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:02.342316 dreifus-0.0.9/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      922 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-16 11:10:01.000000 dreifus-0.0.9/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-16 11:10:03.121955 dreifus-0.0.9/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.9/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1398 2023-06-06 18:46:31.000000 dreifus-0.0.9/test/test_camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.9/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.9/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.9/test/test_vector.py
```

### Comparing `dreifus-0.0.8/pyproject.toml` & `dreifus-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.8"
+version = "0.0.9"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
```

### Comparing `dreifus-0.0.8/src/dreifus/camera.py` & `dreifus-0.0.9/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/camera_bundle.py` & `dreifus-0.0.9/src/dreifus/camera_bundle.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,16 +113,21 @@
     if up is not None:
         # Aligning the look direction might mess up the up direction again
         up_directions = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
         average_up_direction = np.mean(up_directions, axis=0)
         angle = angle_between_vectors(average_up_direction, up)
 
         # TODO: Here we assume that look direction should be z axis. Correct would be to rotate around look direction
-        rotator = Pose.from_euler(Vec3(0, 0, -angle), pose_type=PoseType.CAM_2_CAM)
+        rotator = Pose.from_euler(Vec3(0, 0, angle), pose_type=PoseType.CAM_2_CAM)
         cam_to_world_poses = [rotator @ cam_pose for cam_pose in cam_to_world_poses]
         transformation = rotator @ transformation
 
+        up_directions_after_alignment = [cam_pose.get_up_direction() for cam_pose in cam_to_world_poses]
+        average_up_direction_after_alignment = np.mean(up_directions_after_alignment, axis=0)
+        assert average_up_direction_after_alignment.dot(up) > 0.9, \
+            "Up directions could not be properly aligned. This can happen if the desired look direction is something else than the z-axis"
+
     if return_transformation:
         transformation = Pose(transformation, pose_type=PoseType.CAM_2_CAM)
         return cam_to_world_poses, transformation
     else:
         return cam_to_world_poses
```

### Comparing `dreifus-0.0.8/src/dreifus/graphics.py` & `dreifus-0.0.9/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.0.9/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.0.9/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/pose_base.py` & `dreifus-0.0.9/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.0.9/src/dreifus/matrix/pose_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/pose_torch.py` & `dreifus-0.0.9/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.0.9/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/pyvista.py` & `dreifus-0.0.9/src/dreifus/pyvista.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/render.py` & `dreifus-0.0.9/src/dreifus/render.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/trajectory.py` & `dreifus-0.0.9/src/dreifus/trajectory.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/vector/vector_base.py` & `dreifus-0.0.9/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/vector/vector_numpy.py` & `dreifus-0.0.9/src/dreifus/vector/vector_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus/vector/vector_torch.py` & `dreifus-0.0.9/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.0.9/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/test/test_camera.py` & `dreifus-0.0.9/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/test/test_camera_bundle.py` & `dreifus-0.0.9/test/test_camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/test/test_intrinsics.py` & `dreifus-0.0.9/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/test/test_pose.py` & `dreifus-0.0.9/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.8/test/test_vector.py` & `dreifus-0.0.9/test/test_vector.py`

 * *Files identical despite different names*

