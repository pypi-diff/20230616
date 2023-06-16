# Comparing `tmp/pit30m-0.0.1.tar.gz` & `tmp/pit30m-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pit30m-0.0.1.tar", max compression
+gzip compressed data, was "pit30m-0.0.2.tar", max compression
```

## Comparing `pit30m-0.0.1.tar` & `pit30m-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1096 2023-04-21 03:48:21.893274 pit30m-0.0.1/LICENSE
--rw-r--r--   0        0        0     4153 2023-04-21 04:02:31.637592 pit30m-0.0.1/README.md
--rw-r--r--   0        0        0       45 2023-04-21 03:48:21.909274 pit30m-0.0.1/pit30m/__init__.py
--rw-r--r--   0        0        0    56166 2023-02-13 02:34:48.514354 pit30m-0.0.1/pit30m/all_logs.txt
--rw-r--r--   0        0        0      989 2023-04-21 03:48:21.873274 pit30m-0.0.1/pit30m/camera.py
--rw-r--r--   0        0        0     3821 2023-04-21 04:06:55.127244 pit30m-0.0.1/pit30m/cli.py
--rw-r--r--   0        0        0        0 2022-10-20 01:06:11.851040 pit30m-0.0.1/pit30m/data/__init__.py
--rw-r--r--   0        0        0    15838 2023-04-21 03:48:21.917274 pit30m-0.0.1/pit30m/data/log_reader.py
--rw-r--r--   0        0        0     4379 2023-04-21 03:48:21.909274 pit30m-0.0.1/pit30m/data/submap.py
--rw-r--r--   0        0        0   183837 2023-04-21 03:48:21.909274 pit30m-0.0.1/pit30m/data/submap_utm.pkl
--rw-r--r--   0        0        0     1011 2023-04-21 03:48:21.873274 pit30m-0.0.1/pit30m/fs_util.py
--rw-r--r--   0        0        0      334 2023-01-29 01:48:14.740506 pit30m-0.0.1/pit30m/indexing.hh
--rw-r--r--   0        0        0    23888 2023-04-21 03:48:21.881274 pit30m-0.0.1/pit30m/indexing.py
--rw-r--r--   0        0        0    25163 2023-02-11 22:09:27.574350 pit30m-0.0.1/pit30m/monkeywrench.bak.py
--rw-r--r--   0        0        0    56704 2023-04-21 03:48:21.909274 pit30m-0.0.1/pit30m/monkeywrench.py
--rw-r--r--   0        0        0     1549 2023-04-21 03:48:21.873274 pit30m-0.0.1/pit30m/time_utils.py
--rw-r--r--   0        0        0     4628 2023-04-21 04:06:55.143243 pit30m-0.0.1/pit30m/torch/dataset.py
--rw-r--r--   0        0        0      191 2023-04-21 04:06:55.083244 pit30m-0.0.1/pit30m/torch/dataset_test.py
--rw-r--r--   0        0        0      801 2023-04-21 03:48:21.873274 pit30m-0.0.1/pit30m/util.py
--rw-r--r--   0        0        0     2002 2023-04-21 04:03:21.549147 pit30m-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 pit30m-0.0.1/setup.py
--rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 pit30m-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-21 03:48:21.893274 pit30m-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6806 2023-06-16 02:25:56.023827 pit30m-0.0.2/README.md
+-rw-r--r--   0        0        0       45 2023-06-11 22:50:33.715106 pit30m-0.0.2/pit30m/__init__.py
+-rw-r--r--   0        0        0    56166 2023-02-13 02:34:48.514354 pit30m-0.0.2/pit30m/all_logs.txt
+-rw-r--r--   0        0        0      989 2023-04-21 03:48:21.873274 pit30m-0.0.2/pit30m/camera.py
+-rw-r--r--   0        0        0     3781 2023-06-11 22:40:08.627741 pit30m-0.0.2/pit30m/cli.py
+-rw-r--r--   0        0        0        0 2022-10-20 01:06:11.851040 pit30m-0.0.2/pit30m/data/__init__.py
+-rw-r--r--   0        0        0    26678 2023-06-16 01:48:37.558680 pit30m-0.0.2/pit30m/data/log_reader.py
+-rw-r--r--   0        0        0     2593 2023-06-16 01:48:37.558680 pit30m-0.0.2/pit30m/data/partitions.py
+-rw-r--r--   0        0        0     7328 2023-06-16 01:48:37.558680 pit30m-0.0.2/pit30m/data/submap.py
+-rw-r--r--   0        0        0   183837 2023-05-31 03:08:00.918096 pit30m-0.0.2/pit30m/data/submap_utm.pkl
+-rw-r--r--   0        0        0     1117 2023-05-31 03:08:00.918096 pit30m-0.0.2/pit30m/fs_util.py
+-rw-r--r--   0        0        0      334 2023-01-29 01:48:14.740506 pit30m-0.0.2/pit30m/indexing.hh
+-rw-r--r--   0        0        0    31840 2023-06-16 01:48:37.558680 pit30m-0.0.2/pit30m/indexing.py
+-rw-r--r--   0        0        0    57780 2023-06-16 01:48:33.282720 pit30m-0.0.2/pit30m/monkeywrench.py
+-rw-r--r--   0        0        0     1573 2023-06-03 03:35:22.368588 pit30m-0.0.2/pit30m/time_utils.py
+-rw-r--r--   0        0        0     4742 2023-06-16 02:22:10.817619 pit30m-0.0.2/pit30m/torch/dataset.py
+-rw-r--r--   0        0        0      191 2023-05-31 03:35:40.070516 pit30m-0.0.2/pit30m/torch/dataset_test.py
+-rw-r--r--   0        0        0      801 2023-04-21 03:48:21.873274 pit30m-0.0.2/pit30m/util.py
+-rw-r--r--   0        0        0     2749 2023-06-16 01:48:33.282720 pit30m-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 pit30m-0.0.2/PKG-INFO
```

### Comparing `pit30m-0.0.1/LICENSE` & `pit30m-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pit30m-0.0.1/pit30m/all_logs.txt` & `pit30m-0.0.2/pit30m/all_logs.txt`

 * *Files identical despite different names*

### Comparing `pit30m-0.0.1/pit30m/camera.py` & `pit30m-0.0.2/pit30m/camera.py`

 * *Files identical despite different names*

### Comparing `pit30m-0.0.1/pit30m/cli.py` & `pit30m-0.0.2/pit30m/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import multiprocessing as mp
 import os
 import shlex
-import shutil
 import subprocess
 import tempfile
 from functools import cached_property
-from typing import Tuple, Union
+from typing import Iterable, Union
 from urllib.parse import urlparse
 
 import fire
 import fsspec
 from joblib import Parallel, delayed
 
 
@@ -25,33 +24,30 @@
 
     @cached_property
     def all_log_ids(self) -> list[str]:
         """Return a list of all log IDs in the dataset."""
         with open(self._log_list_fpath, "r") as f:
             return [line.strip() for line in f]
 
-    def woof(self):
-        print("bow wow")
-
     def multicam_demo(
         self,
         out_dir: str,
         log_id: str = "e9511854-f657-47bd-c9d3-047187cfc663",
-        chunks: Union[int, tuple[int]] = (17, 18),
+        chunks: Union[int, Iterable[int]] = (17, 18),
     ) -> None:
         """Bakes a multicam video from a log URI. Requires `ffmpeg` to be installed.
 
         chunks = 100-image chunks of log to include
 
         TODO(andrei): Port to use the log reader.
         """
-        in_fs = fsspec.filesystem(urlparse(self._data_root).scheme)
+        in_fs = fsspec.filesystem(urlparse(self._data_root).scheme, anon=True)
         out_fs = fsspec.filesystem(urlparse(out_dir).scheme)
         if isinstance(chunks, int):
-            chunks = chunks
+            chunks = (chunks,)
 
         # Clockwise wide camera names, with the front wide in the middle
         cams_clockwise = [
             "hdcam_08_port_rear_roof_wide",
             "hdcam_10_port_front_roof_wide",
             "hdcam_12_middle_front_roof_wide",
             "hdcam_02_starboard_front_roof_wide",
@@ -61,29 +57,29 @@
         video_fpaths = []
         with tempfile.TemporaryDirectory() as tmp_dir:
             for cam in cams_clockwise:
                 ld = self._data_root + log_id + "/cameras/" + cam
 
                 sample_img_uris = [
                     entry
-                    for chunk in chunks
+                    for chunk in list(chunks)
                     for entry in in_fs.ls(os.path.join(ld, f"{chunk:04d}"))
                     if entry.endswith("webp")
                 ]
 
                 def copy_img(img_uri, out_dir):
                     with in_fs.open(img_uri, "rb") as f:
                         with out_fs.open(out_dir + "/" + img_uri.split("/")[-1], "wb") as out_f:
                             out_f.write(f.read())
 
                 out_img_dir = tmp_dir + "/frames/" + cam
                 if not out_fs.exists(out_img_dir):
                     out_fs.mkdir(out_img_dir)
                 print("ETL for", cam)
-                res = self._read_pool(delayed(copy_img)(img_uri, out_img_dir) for img_uri in sample_img_uris)
+                self._read_pool(delayed(copy_img)(img_uri, out_img_dir) for img_uri in sample_img_uris)
 
                 framerate = 10
                 subprocess.run(
                     shlex.split(
                         f"ffmpeg -framerate {framerate} -i {out_img_dir}/%*.day.webp -crf 20 -pix_fmt yuv420p "
                         f"-filter:v 'scale=-1:800' {out_img_dir}.mp4"
                     )
```

### Comparing `pit30m-0.0.1/pit30m/data/submap_utm.pkl` & `pit30m-0.0.2/pit30m/data/submap_utm.pkl`

 * *Files identical despite different names*

### Comparing `pit30m-0.0.1/pit30m/fs_util.py` & `pit30m-0.0.2/pit30m/fs_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 @memory.cache(ignore=["fs"])
 def cached_glob(
     root_dir: str,
     extension: str,
     fs: Optional[fsspec.AbstractFileSystem] = None,
 ) -> list[str]:
     scheme = urlparse(root_dir).scheme
+    storage_options = {}
+    if scheme == "s3":
+        storage_options["anon"] = True
     if fs is None:
-        fs = fsspec.filesystem(scheme)
+        fs = fsspec.filesystem(scheme, **storage_options)
     entries = sorted(fs.glob(os.path.join(root_dir, "*", "*" + extension)))
     if scheme is None or 0 == len(scheme):
         return entries
     else:
         return [f"{scheme}://{entry}" for entry in entries]
```

### Comparing `pit30m-0.0.1/pit30m/indexing.py` & `pit30m-0.0.2/pit30m/indexing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,81 @@
 """Utility functions for timing, data association, and indexing."""
 
+import logging
+import math
 import multiprocessing as mp
 import os
+from typing import TYPE_CHECKING, Tuple
 from urllib.parse import urlparse
 
 import fsspec
-import ipdb
 import lz4
 import numpy as np
 from joblib import Memory, Parallel, delayed
 
 from pit30m.fs_util import cached_glob_images, cached_glob_lidar_sweeps
 from pit30m.util import print_list_with_limit
 
+if TYPE_CHECKING:
+    # To prevent circular import
+    from pit30m.data.log_reader import LogReader
+
 # 1M images in a log would mean 100k seconds = A 27h nonstop log. We can't overflow this max length.
 MAX_IMG_RELPATH_LEN = 22  # = len("0090/000000.night.webp")
-MAX_LIDAR_RELPATH_LEN = 14  # = len("007959.npz.lz4")
+MAX_LIDAR_RELPATH_LEN = 15  # = len("0000/007959.npz")
+START_OF_2011_UNIX = 1293861600
 
 memory = Memory(location=os.path.expanduser("~/.cache/pit30m"), verbose=0)
 
 # Please refer to the NumPy documentation for exact details on type dimensions.
 # https://numpy.org/doc/stable/reference/arrays.dtypes.html
+
+# Deprecated, please use V0.
 CAM_INDEX_V0_0_DTYPE = np.dtype(
     [
+        ("rel_path", str, MAX_LIDAR_RELPATH_LEN),
+        # NOTE(andrei): GPS timestamp in the pre-release index.
+        ("img_time", np.double),
+        ("shutter_s", np.double),
+        ("seq_counter", np.int64),
+        ("gain_db", np.double),
+        ("cp_present", bool),
+        ("cp_valid", bool),
+        ("cp_time_s", np.double),
+        ("cp_x", np.double),
+        ("cp_y", np.double),
+        ("cp_z", np.double),
+        ("cp_roll", np.double),
+        ("cp_pitch", np.double),
+        ("cp_yaw", np.double),
+        ("mrp_present", bool),
+        ("mrp_valid", bool),
+        ("mrp_time", np.double),
+        ("mrp_submap_id", bytes, 16),
+        ("mrp_x", np.double),
+        ("mrp_y", np.double),
+        ("mrp_z", np.double),
+        ("mrp_roll", np.double),
+        ("mrp_pitch", np.double),
+        ("mrp_yaw", np.double),
+        # UTM coordinates are provided for CONVENIENCE, computed from MRP based on the v0 (unrefined)
+        # submap UTM coordinates. Ideally you'll eventually want to use the 'Map' class and compute your
+        # own UTMs once Andrei B. manages to release refined submap UTMs.
+        ("utm_present", bool),
+        ("utm_valid", bool),
+        ("utm_x", np.double),  # Easting
+        ("utm_y", np.double),  # Northing
+        ("utm_z", np.double),  # TODO(andrei): Make sure you populate UTM Z (altitude) eventually
+    ]
+)
+CAM_INDEX_V1_0_DTYPE = np.dtype(
+    [
         # TODO-LOW(andrei): Index a number and day/night to save space.
         ("rel_path", str, MAX_IMG_RELPATH_LEN),
-        # TODO(andrei): This is currently a GPS timestamp. Need to update to UNIX when (re)building the index.
+        # GPS timestamp
         ("img_time", np.double),
         ("shutter_s", np.double),
         ("seq_counter", np.int64),
         ("gain_db", np.double),
         ("cp_present", bool),
         ("cp_valid", bool),
         ("cp_time_s", np.double),
@@ -52,20 +98,60 @@
         # UTM coordinates are provided for CONVENIENCE, computed from MRP based on the v0 (unrefined)
         # submap UTM coordinates. Ideally you'll eventually want to use the 'Map' class and compute your
         # own UTMs once Andrei B. manages to release refined submap UTMs.
         ("utm_present", bool),
         ("utm_valid", bool),
         ("utm_x", np.double),  # Easting
         ("utm_y", np.double),  # Northing
-        ("utm_z", np.double),  # TODO(andrei): Make sure you populate UTM Z (altitude) eventually
+        ("utm_z", np.double),  # Altitude
     ]
 )
+CAM_INDEX_V2_0_DTYPE = CAM_INDEX_V1_0_DTYPE
+
 
 LIDAR_INDEX_V0_0_DTYPE = np.dtype(
     [
+        ("rel_path", str, 14),
+        ("lidar_time", np.double),
+        ("lidar_min_time", np.double),
+        ("lidar_max_time", np.double),
+        ("lidar_mean_time", np.double),
+        ("lidar_median_time", np.double),
+        ("num_points", np.int64),
+        ("cp_present", bool),
+        ("cp_valid", bool),
+        ("cp_time_s", np.double),
+        ("cp_x", np.double),
+        ("cp_y", np.double),
+        ("cp_z", np.double),
+        ("cp_roll", np.double),
+        ("cp_pitch", np.double),
+        ("cp_yaw", np.double),
+        ("mrp_present", bool),
+        ("mrp_valid", bool),
+        ("mrp_time", np.double),
+        ("mrp_submap_id", bytes, 16),
+        ("mrp_x", np.double),
+        ("mrp_y", np.double),
+        ("mrp_z", np.double),
+        ("mrp_roll", np.double),
+        ("mrp_pitch", np.double),
+        ("mrp_yaw", np.double),
+        # UTM coordinates are provided for CONVENIENCE, computed from MRP based on the v0 (unrefined)
+        # submap UTM coordinates. Ideally you'll eventually want to use the 'Map' class and compute your
+        # own UTMs once Andrei B. manages to release refined submap UTMs.
+        ("utm_present", bool),
+        ("utm_valid", bool),
+        ("utm_x", np.double),  # Easting
+        ("utm_y", np.double),  # Northing
+        ("utm_z", np.double),  # Altitude
+    ]
+)
+LIDAR_INDEX_V1_0_DTYPE = np.dtype(
+    [
         ("rel_path", str, MAX_LIDAR_RELPATH_LEN),
         ("lidar_time", np.double),
         ("lidar_min_time", np.double),
         ("lidar_max_time", np.double),
         ("lidar_mean_time", np.double),
         ("lidar_median_time", np.double),
         ("num_points", np.int64),
@@ -91,17 +177,18 @@
         # UTM coordinates are provided for CONVENIENCE, computed from MRP based on the v0 (unrefined)
         # submap UTM coordinates. Ideally you'll eventually want to use the 'Map' class and compute your
         # own UTMs once Andrei B. manages to release refined submap UTMs.
         ("utm_present", bool),
         ("utm_valid", bool),
         ("utm_x", np.double),  # Easting
         ("utm_y", np.double),  # Northing
-        ("utm_z", np.double),  # TODO(andrei): Make sure you populate UTM Z (altitude) eventually
+        ("utm_z", np.double),  # Altitude
     ]
 )
+LIDAR_INDEX_V2_0_DTYPE = LIDAR_INDEX_V1_0_DTYPE
 
 
 def fetch_metadata_for_image(img_uri: str) -> tuple[str, tuple]:
     """Returns the original URI and the image metadata.
 
     Used in indexing operations. Average users should not be reading metadata files directly
     as there are many of them and they are tiny, so it is very inefficient. Users should be
@@ -110,30 +197,44 @@
 
     The many tiny metadata files were just dumped originally for simplicity and maximum
     robustness.
     """
     meta_uri = img_uri.replace(".day", ".night").replace(".night.webp", ".meta.npy").replace(".webp", ".meta.npy")
     with fsspec.open(meta_uri) as meta_f:
         meta = np.load(meta_f, allow_pickle=True).tolist()
-        timestamp_s = float(meta["capture_seconds"])
+        timestamp_gps_s = float(meta["capture_seconds"])
+
+        # We basically assert the timestamp we read is actually GPS time. Uber ATG did not exist in 2010!
+        assert timestamp_gps_s < START_OF_2011_UNIX
         # Not used
         # transmission_s = float(meta["transmission_seconds"])
+        # timestamp_unix_s = gps_seconds_to_utc(timestamp_gps_s).timestamp()
 
-        entry = (timestamp_s, float(meta["shutter_seconds"]), int(meta["sequence_counter"]), float(meta["gain_db"]))
+        entry = (
+            timestamp_gps_s,
+            float(meta["shutter_seconds"]),
+            int(meta["sequence_counter"]),
+            float(meta["gain_db"]),
+        )
         return img_uri, entry
 
 
 @memory.cache(verbose=0)
-def fetch_metadata_for_lidar(lidar_uri: str) -> tuple[str, tuple]:
-    """Returns LiDAR timing metadata."""
+def fetch_metadata_for_lidar(lidar_uri: str) -> tuple[str, ...]:
+    """Returns LiDAR timing metadata.
+
+    All returned timestamps are GPS timestamps.
+    """
     # meta_uri = lidar_uri.replace(".day", ".night").replace(".night.webp", ".meta.npy").replace(".webp", ".meta.npy")
     with fsspec.open(lidar_uri) as compressed_f:
         with lz4.frame.open(compressed_f, "rb") as f:
             lidar_data = np.load(f)
-            point_times = lidar_data["seconds"]
+            point_times_gps = lidar_data["seconds"]
+            # See the camera metadata function for why we assert this.
+            assert np.min(point_times_gps) < START_OF_2011_UNIX
 
             if lidar_data["points"].ndim != 2 or lidar_data["points"].shape[-1] != 3:
                 return (
                     "Error",
                     lidar_uri,
                     "unexpected-points-shape",
                     "{}".format(lidar_data["points"].shape),
@@ -165,37 +266,107 @@
                 return (
                     "Error",
                     lidar_uri,
                     "unexpected-point-time-shape",
                     "{} vs. {} points".format(lidar_data["seconds"].shape, lidar_data["points"].shape),
                 )
 
+            # Assumption - no leap second during the sweep.
+            # first_point_gps = point_times_gps[0]
+            # first_point_unix = gps_seconds_to_utc(first_point_gps).timestamp()
+            # assert first_point_unix > first_point_gps
+            # naive_delta = first_point_unix - point_times_gps[0]
+            # assert naive_delta > 0
+
+            # point_times_unix = point_times_gps + naive_delta
+
             return (
                 "OK",
                 lidar_uri,
-                point_times.min(),
-                point_times.max(),
-                point_times.mean(),
-                np.median(point_times),
+                point_times_gps.min(),
+                point_times_gps.max(),
+                point_times_gps.mean(),
+                np.median(point_times_gps),
                 lidar_data["points"].shape,
             )
 
 
+def associate_np(
+    query_timestamps: np.ndarray, target_timestamps: np.ndarray, max_delta_s: float = 0.5
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Similar associate, but fully vectorized
+
+    Returns:
+        np.ndarray: The same length as query_timestamps, with the index of the associated target_timestamps
+        np.ndarray: The same length as query_timestamps, True if the association is over max_delta_s
+
+    NOTE(julieta)
+    This is called every time we load an index, and therefore it matters that it be fast.
+    We could take advantage of both arrays being sorted and implement this in C or Rust to speed things up.
+    """
+    result = np.zeros(query_timestamps.shape, dtype=np.int64)
+
+    assert target_timestamps.shape[0] > 0
+    assert target_timestamps.dtype == np.float64 or target_timestamps.dtype == np.float32
+    assert query_timestamps.dtype == np.float64 or query_timestamps.dtype == np.float32
+
+    target_idx = np.searchsorted(target_timestamps, query_timestamps)
+    prv = target_idx - 1
+    nxt = target_idx
+
+    # If the target timestamp is past the end of the target timestamps, we'll just use the last
+    idx_past = nxt >= len(target_timestamps)
+    target_idx[idx_past] = len(target_timestamps) - 1
+
+    # Now do interpolation for the rest
+    rest = np.logical_not(idx_past)
+
+    delta_prev = np.abs(query_timestamps - target_timestamps[prv])
+    delta_next = np.abs(query_timestamps - target_timestamps[nxt])
+
+    smaller_idx = delta_prev < delta_next
+    set_with_smaller = np.logical_and(rest, smaller_idx)
+    target_idx[set_with_smaller] = prv[set_with_smaller]
+
+    set_with_larger = np.logical_and(rest, np.logical_not(smaller_idx))
+    target_idx[set_with_larger] = nxt[set_with_larger]
+
+    # NOTE(julieta) we could re-use the appropriate entries from delta_prev and delta_next here, but this is clearer
+    delta_s = np.abs(query_timestamps - target_timestamps[target_idx])
+
+    over = delta_s > max_delta_s
+
+    if max_delta_s > 0:
+        n_over = np.sum(over)
+        # breakpoint()
+        # NOTE(julieta) log instead of print
+        if n_over:
+            print(
+                f"WARNING: There are {n_over} / {len(over)} ({100*n_over/len(over):.2f}%) timestamp associations with gap > {max_delta_s:.3f}s. Max is {delta_s.max():.3f}s"
+            )
+
+    result = target_idx
+    return result, over
+
+
 def associate(query_timestamps: np.ndarray, target_timestamps: np.ndarray, max_delta_s: float = 0.5) -> np.ndarray:
     """Associates timestamps from two arrays, returning the indices of the closest matches.
 
-    The result will contain an index into 'db_ts' for each entry in 'q_ts' (query timestamps).
+    The result will contain an index into 'target_timestamps' for each entry in 'query_timestamps'.
     All timestamps are expected to be float64, seconds.
 
     Args:
         query_timestamps:   The timestamps to find matches for.
         target_timestamps:  The timestamps to match against. Must be sorted!!
         max_delta_s:        Warn if the gap between the query and the result is bigger than this. Note that we will
                             still return this index, so the end user is responsible for filtering out the results.
+    Returns:
+        An array of the same size as query_timestamps, with the indices of the matching entries in target_timestamps.
     """
+
     # TODO(andrei): Within a few ms at worst, poses are evenly spaced. We can use
     # arithmetic to dramatically constrain our search range to turn log n binary search
     # into a constant time look-up.
     #
     # TODO(andrei): Interpolate poses linearly. Poses are 100Hz so nearest-neighbor lookups can
     # be at most 10-ish ms off which can cause 0.33m of error for 33 mps driving (120kph) in
     # a worst-case scenario, so not trivial.
@@ -221,47 +392,57 @@
             else:
                 target_idx = next
         else:
             target_idx = target_idx - 1
 
         delta_s = abs(q_ts - target_timestamps[target_idx])
         if max_delta_s > 0 and delta_s > max_delta_s:
-            print(f"WARNING: Timestamp association gap is {delta_s:.3f}s for query {q_idx}.")
+            print(f"WARNING: Timestamp association gap is {delta_s:.3f}s > {max_delta_s:.3f} for query {q_idx}.")
         result[q_idx] = target_idx
 
     return result
 
 
-def build_camera_index(in_root, log_reader, cam_dir, _logger):
+def build_camera_index(
+    in_root: str, log_reader: "LogReader", cam_dir: str, logger: logging.Logger, index_version: int
+) -> np.ndarray:
     """Internal function to build an index for a sensor in a log.
 
     Grabs all available images and tries to associate them with poses by timestamp, creating an index in numpy binary
     format (easy to parse in C++ as well, for instance). The index has an entry for every image - if that image did not
     have a matching pose (especially common at the start and end of logs), then the appropriate fields `mrp_present`
     and `cp_present` will be set to False.
 
     Please refer to the LogReader documentation and the project README for details on how poses work and what MRP and CP
     means.
     """
-    _logger.info("Reading continuous pose data")
+    logger.info("Reading continuous pose data")
     cp_dense = log_reader.continuous_pose_dense
     cp_times = np.array(cp_dense[:, 0])
     in_scheme = urlparse(in_root).scheme
     in_fs = fsspec.filesystem(in_scheme)
+    if index_version == 0:
+        camera_index_dtype = CAM_INDEX_V0_0_DTYPE
+    elif index_version == 1:
+        camera_index_dtype = CAM_INDEX_V1_0_DTYPE
+    elif index_version == 2:
+        camera_index_dtype = CAM_INDEX_V2_0_DTYPE
+    else:
+        raise ValueError(f"Unknown index version {index_version}")
 
-    _logger.info("Reading UTM and MRP")
+    logger.info("Reading UTM and MRP")
     # Note that UTM is inferred from MRP via (very much imperfect) submap UTMs
-    utm_poses = log_reader.utm_poses_dense
+    _, utm_poses = log_reader.utm_poses_dense
     mrp_poses = log_reader.map_relative_poses_dense
-    assert len(mrp_poses) == len(utm_poses)
+    assert len(mrp_poses) == len(utm_poses), f"{len(mrp_poses) = } != {len(utm_poses) = }"
     mrp_times = np.array(mrp_poses["time"])
 
-    _logger.info("Listing all images from %s", cam_dir)
+    logger.info("Listing all images from %s", cam_dir)
     image_uris = cached_glob_images(cam_dir, in_fs)
-    _logger.info("There are %d images in %s", len(image_uris), cam_dir)
+    logger.info("There are %d images in %s", len(image_uris), cam_dir)
 
     h = len(image_uris) / 10.0 / 3600.0
     print(f"{h:.2f} hours of driving")
 
     # NOTE(andrei): Seems to be worth over-subscribing!
     #
     # Coarse numbers from my personal machine, 16 core 1Gbps connection to S3.
@@ -272,65 +453,70 @@
     # 128, 30s = 29k
     # 256, 30s = 54k (though I think my upload speed is unnaturally fast... (for the requests))
     # 256, 15s (bs = 4) = 23.5k, 28k, ...
     # 256, 15s, bs = 8  = 28.8k
     # 512, 15s = 14.9k
     #
     # This subsequently got a fair bit slower once I actually parsed the npy, oh well
-    pool = Parallel(n_jobs=mp.cpu_count() * 8, verbose=1, batch_size=8)
-    _logger.info("Fetching metadata...")
+    # Lower factor when running inside AWS (4) vs locally (8).
+    factor = 4
+    pool = Parallel(n_jobs=mp.cpu_count() * factor, verbose=1, batch_size=8)
+    logger.info("Fetching metadata...")
     res = pool(delayed(fetch_metadata_for_image)(x) for x in image_uris)
-    _logger.info("Fetched %d results", len(res))
+    logger.info("Fetched %d results", len(res))
 
     image_times = np.array([float(entry[1][0]) for entry in res])
-    _logger.info("Associating...")
-    _logger.info(
+    logger.info("Associating...")
+    logger.info(
         "%s %s %s %s",
         image_times.dtype,
         str(image_times.shape),
         str(image_times[0]) if len(image_times) else "n/A",
         str(type(image_times[0])) if len(image_times) else "n/A",
     )
-    _logger.info("%s %s %s %s", mrp_times.dtype, str(mrp_times.shape), str(mrp_times[0]), str(type(mrp_times[0])))
+    logger.info("%s %s %s %s", mrp_times.dtype, str(mrp_times.shape), str(mrp_times[0]), str(type(mrp_times[0])))
     assert np.all(mrp_times[1:] > mrp_times[:-1])
 
     utm_and_mrp_index = associate(image_times, mrp_times, max_delta_s=-1.0)
-    _logger.info("Associating complete.")
+    logger.info("Associating complete.")
     matched_timestamps_mrp = mrp_times[utm_and_mrp_index]
     deltas_mrp = np.abs(matched_timestamps_mrp - image_times)
 
-    _logger.info("Associating CP...")
+    logger.info("Associating CP...")
     cp_index = associate(image_times, cp_times, max_delta_s=-1.0)
-    _logger.info("Associating complete.")
+    logger.info("Associating complete.")
     matched_timestamps_cp = cp_times[cp_index]
     deltas_cp = np.abs(matched_timestamps_cp - image_times)
 
-    unindexed_frames = []
-    status = []
     raw_index = []
     for row_idx, ((img_fpath, img_data), pose_idx, cp_idx, delta_mrp_s, delta_cp_s) in enumerate(
         zip(res, utm_and_mrp_index, cp_index, deltas_mrp, deltas_cp)
     ):
         img_time, shutter_s, seq_counter, gain_db = img_data
         if delta_mrp_s > 0.10:
             mrp = None
             mrp_present = False
+            utm_present = False
             mrp_valid = False
             mrp_time_s, mrp_x, mrp_y, mrp_z, mrp_roll, mrp_pitch, mrp_yaw = 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0
             mrp_submap_id = b"\x00" * 16
             utm = None
             utm_x, utm_y, utm_z = 0.0, 0.0, 0.0
         else:
             mrp = mrp_poses[pose_idx, ...].tolist()
             utm = utm_poses[pose_idx, ...].tolist()
             mrp_present = True
+            utm_present = True
             mrp_time_s, mrp_valid, mrp_submap_id, mrp_x, mrp_y, mrp_z, mrp_roll, mrp_pitch, mrp_yaw = mrp
-            utm_x, utm_y = utm
-            # TODO(andrei): Update me
-            utm_z = 0
+            utm_x, utm_y, utm_z = utm
+            if math.isnan(utm_x):
+                utm_x = 0.0
+                utm_y = 0.0
+                utm_z = 0.0
+                utm_present = False
 
             # Handle submap IDs which were truncated upon encoded due to ending with a zero.
             mrp_submap_id = mrp_submap_id.ljust(16, b"\x00")
             assert type(mrp_submap_id) == bytes
             assert 16 == len(mrp_submap_id)
 
         if delta_cp_s > 0.10:
@@ -368,58 +554,70 @@
                 mrp_submap_id,
                 mrp_x,
                 mrp_y,
                 mrp_z,
                 mrp_roll,
                 mrp_pitch,
                 mrp_yaw,
-                # No MRP === No UTM
-                mrp_present,
-                mrp_present,
+                utm_present,
+                utm_present,
                 utm_x,
                 utm_y,
                 utm_z,
             )
         )
 
-    index = np.array(raw_index, dtype=CAM_INDEX_V0_0_DTYPE)
+    index = np.array(raw_index, dtype=camera_index_dtype)
+    index = np.sort(index, order="img_time")
 
     cp_p = index["cp_present"]
     print("CP total:", len(cp_p))
     print("CP valid:", sum(cp_p))
 
     mrp_p = index["mrp_present"]
     print("MRP total:", len(mrp_p))
     print("MRP valid:", sum(mrp_p))
     return index
 
 
-def build_lidar_index(in_root, log_reader, lidar_dir, _logger):
+def build_lidar_index(
+    in_root: str, log_reader: "LogReader", lidar_dir: str, _logger: logging.Logger, index_version: int
+) -> np.ndarray:
     """Internal function to build an index for a LiDAR in a log."""
     _logger.info("Reading continuous pose data")
     cp_dense = log_reader.continuous_pose_dense
     cp_times = np.array(cp_dense[:, 0])
     in_scheme = urlparse(in_root).scheme
     in_fs = fsspec.filesystem(in_scheme)
 
+    if index_version == 0:
+        lidar_dtype = LIDAR_INDEX_V0_0_DTYPE
+    elif index_version == 1:
+        lidar_dtype = LIDAR_INDEX_V1_0_DTYPE
+    elif index_version == 2:
+        lidar_dtype = LIDAR_INDEX_V2_0_DTYPE
+    else:
+        raise ValueError(f"Unknown index version {index_version}")
+
     _logger.info("Reading UTM and MRP")
     # Note that UTM is inferred from MRP via (very much imperfect) submap UTMs
-    utm_poses = log_reader.utm_poses_dense
+    _, utm_poses = log_reader.utm_poses_dense
     mrp_poses = log_reader.map_relative_poses_dense
-    assert len(mrp_poses) == len(utm_poses)
+    assert len(mrp_poses) == len(utm_poses), f"{len(mrp_poses) = } != {len(utm_poses) = }"
     mrp_times = np.array(mrp_poses["time"])
 
     _logger.info("Listing all LiDAR sweeps from %s", lidar_dir)
     lidar_sweep_uris = cached_glob_lidar_sweeps(lidar_dir, in_fs)
     _logger.info("There are %d LiDARs in %s", len(lidar_sweep_uris), lidar_dir)
 
     h = len(lidar_sweep_uris) / 10.0 / 3600.0
     print(f"{h:.2f} hours of driving")
 
-    pool = Parallel(n_jobs=mp.cpu_count() * 4, verbose=1, batch_size=8)
+    factor = 4
+    pool = Parallel(n_jobs=mp.cpu_count() * factor, verbose=1, batch_size=8)
     _logger.info("Fetching metadata...")
     all_lidar_meta_info = pool(delayed(fetch_metadata_for_lidar)(x) for x in lidar_sweep_uris)
     _logger.info("Fetched %d results", len(all_lidar_meta_info))
 
     errors = [x for x in all_lidar_meta_info if x[0] != "OK"]
 
     ts_path = os.path.join(lidar_dir, "timestamps.npz.lz4")
@@ -431,104 +629,113 @@
             # also be to some other predefined time which was hardcoded by the log reader. Either way, the information
             # is *there* (we have per-point times), it's just a matter of playing with projecting the LiDAR to the
             # cameras in order to identify the exact time whose pose the LiDAR data is wrt to.
             #
             # This estimate will however be enough for simple visual localization tasks for now. I have a more
             # overarching goal of sorting out LiDAR as the continuous-time sensor that it is once we get the first
             # version of the devkit out.
-            dumped_timestamps = np.load(ff)["data"]["timestamp"].ravel()
+            dumped_timestamps_gps = np.load(ff)["data"]["timestamp"].ravel()
 
     if len(errors) > 0:
         _logger.error("Found %d errors reading LiDAR for indexing purposes!!!", len(errors))
         print_list_with_limit(errors, 10, logger=_logger)
         log_id = log_reader.log_id
         raise RuntimeError(f"Could not index LIDAR for log ID {log_id} due to errors (see log)")
 
     _logger.info("No errors found reading %d LiDAR sweep files for indexing.", len(all_lidar_meta_info))
 
     # dmins = []
     # dmaxs = []
     lidar_info = []
     # Please read the above detailed comment for what we mean by "LiDAR time".
     lidar_times = []
-    for idx, (andrei_timestamp, (_, lidar_uri, min_time, max_time, mean_time, p50_time, shape)) in enumerate(
-        zip(dumped_timestamps, all_lidar_meta_info)
+    for idx, (andrei_timestamp_gps, (_, lidar_uri, min_time, max_time, mean_time, p50_time, shape)) in enumerate(
+        zip(dumped_timestamps_gps, all_lidar_meta_info)
     ):
         # NOTE(andrei): LIDAR is rolling shutter...
         # if idx % 200 == 0:
         #     print(f"{idx} / {len(lidar_sweep_uris)}")
         #     print(f"min_time: {min_time}")
         #     print(f"max_time: {max_time}")
         #     # print(f"mean_time: {mean_time}")
         #     print(f"{float(andrei_timestamp) = }")
         #     # print(f"dmin/dmax: {dmin}/{dmax}")
         num_points, pcd_dim = shape
         assert 3 == pcd_dim
+        # andrei_timestamp_unix = gps_seconds_to_utc(andrei_timestamp_gps).timestamp()
 
-        lidar_info.append((andrei_timestamp, lidar_uri, min_time, max_time, mean_time, p50_time, num_points))
-        lidar_times.append(andrei_timestamp)
+        # The 'dumped at' time should be within the LiDAR sweep time range.
+        assert abs(andrei_timestamp_gps - mean_time) < 1.0, f"{andrei_timestamp_gps = } too far from {mean_time = }"
 
-    lidar_times = np.array(lidar_times, dtype=np.float64)
+        lidar_info.append((andrei_timestamp_gps, lidar_uri, min_time, max_time, mean_time, p50_time, num_points))
+        lidar_times.append(andrei_timestamp_gps)
+
+    lidar_times_np = np.array(lidar_times, dtype=np.float64)
 
     #     dmin = andrei_timestamp - min_time
     #     dmax = max_time - andrei_timestamp
     #     dmins.append(dmin)
     #     dmaxs.append(dmax)
 
     # print(np.mean(dmins))
     # print(np.mean(dmaxs))
 
     _logger.info("Associating...")
     _logger.info(
         "%s %s %s %s",
-        type(lidar_times),
-        str(len(lidar_times)),
-        str(lidar_times[0]) if len(lidar_times) else "n/A",
-        str(type(lidar_times[0])) if len(lidar_times) else "n/A",
+        type(lidar_times_np),
+        str(len(lidar_times_np)),
+        str(lidar_times_np[0]) if len(lidar_times_np) else "n/A",
+        str(type(lidar_times_np[0])) if len(lidar_times_np) else "n/A",
     )
     _logger.info("%s %s %s %s", mrp_times.dtype, str(mrp_times.shape), str(mrp_times[0]), str(type(mrp_times[0])))
     assert np.all(mrp_times[1:] > mrp_times[:-1])
 
-    utm_and_mrp_index = associate(lidar_times, mrp_times, max_delta_s=-1.0)
+    utm_and_mrp_index = associate(lidar_times_np, mrp_times, max_delta_s=-1.0)
     _logger.info("Associating complete.")
 
     matched_timestamps_mrp = mrp_times[utm_and_mrp_index]
-    deltas_mrp = np.abs(matched_timestamps_mrp - lidar_times)
+    deltas_mrp = np.abs(matched_timestamps_mrp - lidar_times_np)
 
     _logger.info("Associating CP...")
-    cp_index = associate(lidar_times, cp_times, max_delta_s=-1.0)
+    cp_index = associate(lidar_times_np, cp_times, max_delta_s=-1.0)
     _logger.info("Associating complete.")
     matched_timestamps_cp = cp_times[cp_index]
-    deltas_cp = np.abs(matched_timestamps_cp - lidar_times)
+    deltas_cp = np.abs(matched_timestamps_cp - lidar_times_np)
 
     # TODO(andrei): Code duplication between this and the camera index builder.
     raw_index = []
     for (
         (lidar_time, lidar_fpath, min_time, max_time, mean_time, p50_time, npts),
         pose_idx,
         cp_idx,
         delta_mrp_s,
         delta_cp_s,
     ) in zip(lidar_info, utm_and_mrp_index, cp_index, deltas_mrp, deltas_cp):
         if delta_mrp_s > 0.10:
             mrp = None
             mrp_present = False
             mrp_valid = False
+            utm_present = False
             mrp_time_s, mrp_x, mrp_y, mrp_z, mrp_roll, mrp_pitch, mrp_yaw = 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0
             mrp_submap_id = b"\x00" * 16
             utm = None
             utm_x, utm_y, utm_z = 0.0, 0.0, 0.0
         else:
             mrp = mrp_poses[pose_idx, ...].tolist()
             utm = utm_poses[pose_idx, ...].tolist()
             mrp_present = True
+            utm_present = True
             mrp_time_s, mrp_valid, mrp_submap_id, mrp_x, mrp_y, mrp_z, mrp_roll, mrp_pitch, mrp_yaw = mrp
-            utm_x, utm_y = utm
-            # TODO(andrei): Update me
-            utm_z = 0
+            utm_x, utm_y, utm_z = utm
+            if math.isnan(utm_x):
+                utm_x = 0.0
+                utm_y = 0.0
+                utm_z = 0.0
+                utm_present = False
 
             # Handle submap IDs which were truncated upon encoded due to ending with a zero.
             mrp_submap_id = mrp_submap_id.ljust(16, b"\x00")
             assert type(mrp_submap_id) == bytes
             assert 16 == len(mrp_submap_id)
 
         if delta_cp_s > 0.10:
@@ -568,24 +775,25 @@
                 mrp_submap_id,
                 mrp_x,
                 mrp_y,
                 mrp_z,
                 mrp_roll,
                 mrp_pitch,
                 mrp_yaw,
-                # No MRP === No UTM
-                mrp_present,
-                mrp_present,
+                # No MRP => No UTM
+                utm_present,
+                utm_present,
                 utm_x,
                 utm_y,
                 utm_z,
             )
         )
 
-    index = np.array(raw_index, dtype=LIDAR_INDEX_V0_0_DTYPE)
+    index = np.array(raw_index, dtype=lidar_dtype)
+    index = np.sort(index, order="lidar_time")
 
     cp_p = index["cp_present"]
     print("CP total:", len(cp_p))
     print("CP valid:", sum(cp_p))
 
     mrp_p = index["mrp_present"]
     print("MRP total:", len(mrp_p))
```

### Comparing `pit30m-0.0.1/pit30m/monkeywrench.py` & `pit30m-0.0.2/pit30m/monkeywrench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Internal tooling for data management, validation, and indexing."""
 
 import csv
 import json
 import logging
 import multiprocessing as mp
 import os
+import random
 from collections import Counter
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from typing import List, Optional, Tuple, Union
 from urllib.parse import urlparse
 from uuid import UUID
@@ -60,24 +61,24 @@
 
 cache = Memory(location=os.path.expanduser("~/.cache/pit30m"), verbose=0)
 
 
 @dataclass
 class CamReportSummary:
     n_ok: int
-    warnings: List[str] = None
-    errors: List[str] = None
+    warnings: Optional[List[str]] = None
+    errors: Optional[List[str]] = None
 
     @property
     def n_warns(self) -> int:
-        return len(self.warnings)
+        return len(self.warnings) if self.warnings else 0
 
     @property
     def n_errs(self) -> int:
-        return len(self.errors)
+        return len(self.errors) if self.errors else 0
 
 
 class LogStatus(Enum):
     NOT_ATTEMPTED = "not_attempted"
     DONE_NOT_INDEXED = "done_not_indexed"
     CRASHED_OR_IN_PROGRESS = "crashed_or_in_progress"
     INDEXED = "INDEXED"
@@ -116,15 +117,15 @@
         elif non_img_ok:
             return LogStatus.ONLY_CPU_DONE
         else:
             # File exists but the dump did not finish (yet?)
             return LogStatus.CRASHED_OR_IN_PROGRESS
 
 
-def stat_sensors_for_log(root: str, log_id: str, index_version: int = 0):
+def stat_sensors_for_log(root: str, log_id: str, index_version: int):
     log_id = log_id.strip().strip("/")
     fs = fsspec.filesystem(urlparse(root).scheme)
     log_root = os.path.join(root, log_id)
     if not fs.exists(log_root):
         # n/A for a non-attempted log
         return None
     if not fs.exists(os.path.join(log_root, ETL_CANARY_FNAME)):
@@ -141,15 +142,15 @@
         cam_dir = os.path.join(log_root, "cameras", cam.value)
         # Load the 'npz' since we are OK with CPU overhead for saving network bandwidth.
         # As of 2023-02-04, stat_sensors 0..750
         #  - Before:                8.2 min
         #  - w/ npz:                2.8 min
         #  - w/ npz + 2x processes: 2.2 min (1Gbps net is saturated)
         #
-        index_fpath = os.path.join(cam_dir, "index", f"index_v{index_version}.npz")
+        index_fpath = os.path.join(cam_dir, "index", f"index_v{index_version:02d}.npz")
 
         if not fs.exists(index_fpath):
             # Camera not dumped
             cam_images[cam] = -1
             continue
 
         with fs.open(index_fpath, "rb") as f:
@@ -211,19 +212,15 @@
 
     @cached_property
     def all_logs(self) -> List[UUID]:
         """Return a list of all log IDs."""
         with open(self._log_list_fpath, "r") as f:
             return [UUID(line.strip()) for line in f]
 
-    @cached_property
-    def map(self) -> Map:
-        return Map.from_submap_utm_uri(self._submap_utm_fpath)
-
-    def index(self, log_id: str, out_index_fpath: Optional[str] = None, check: bool = True):
+    def index(self, log_id: str, out_index_dir: Optional[str] = None, check: bool = True, index_version: int = 2):
         """Create index files for the raw data in the dataset.
 
         At dump time, the dataset just contained numbered image files with small associated metadata files. This meant
         it was basically impossible to find images by GPS location or timestamp. This tool creates indexes that allow
         for fast lookups by GPS location or timestamp.
 
         Building large indexes from scratch can take a while, even on the order of hours on some machines. We are
@@ -233,76 +230,79 @@
             log_id:             The ID of the log to analyze and index.
             out_index_fpath:    Where to write indexes. If None (default) they will be written to the same directory as
                                 the respective sensor.
             check:              If True, run expensive integrity checks on the data, e.g., actually read each image,
                                 check its shape, load the metadata and ensure it's not corrupted, load the LiDAR and
                                 check its shape too, etc.
         """
-        # XXX(andrei): This function is deprecated.
-        self.index_all_cameras(log_id=log_id, out_index_fpath=out_index_fpath, check=check)
-        self.index_lidar(log_id=log_id, out_index_fpath=out_index_fpath, check=check)
-        res = self.diagnose_misc(log_id=log_id, out_index_fpath=out_index_fpath, check=check)
-        # XXX(andrei): Turn the misc diagnosis into a mini report too.
-        if len(res) > 0:
-            print("WARNING: misc non-sensor data had errors. See above for more information.")
+        self.index_all_cameras(log_id=log_id, out_index_dir=out_index_dir, index_version=index_version)
+        self.index_lidar(
+            log_id=log_id,
+            lidar_name=VELODYNE_NAME,
+            out_index_dir=out_index_dir,
+            reindex=False,
+            index_version=index_version,
+        )
+        self.diagnose_misc(log_id=log_id, out_index_fpath=out_index_dir, check=check)
+        # # TODO(andrei): Turn the misc diagnosis into a mini report too.
+        # if len(res) > 0:
+        #     print("WARNING: misc non-sensor data had errors. See above for more information.")
 
         print("Log indexing complete.")
 
     # def merge_indexes(self, log_ids: List[str]):
     #     """Given a list of log IDs with indexed data, merge the indexes into a single index."""
     #     # TODO(andrei): Implement this.
     #     ...
 
     def get_lidar_dir(self, log_root: str, lidar_name: str) -> str:
         return os.path.join(log_root, "lidars", lidar_name.lstrip("/"))
 
     def get_cam_dir(self, log_root: str, cam_name: str) -> str:
         return os.path.join(log_root, "cameras", cam_name.lstrip("/"))
 
-    # def next_to_validate(self, max: int = 10):
-    #     """Next logs to validate."""
-    #     pass
-
     def stat(self, max: int = 100, quiet: bool = False):
-        all_logs = self.all_logs[:max]
+        all_logs = [str(x) for x in self.all_logs[:max]]
 
         statuses = []
         for log, status in zip(all_logs, qls_it(self._root, all_logs, batch_size=250)):
             statuses.append(status)
             if not quiet:
                 print(log, status)
 
         counts = Counter(statuses)
         print(f"Stats for up to {max} dumped Pit30M logs:")
         for status, count in counts.items():
             print(f"{status.name}: {count}")
         print("=" * 80)
 
-    def stat_log(self, log_id: str) -> None:
+    def stat_log(self, log_id: str, index_version: int) -> None:
         log_id = log_id.strip().strip("/")
         print("=" * 80)
         print(f"Log ID: {log_id}")
         print(query_log_status(self._root, log_id))
         print("=" * 80)
-        for sensor, count in stat_sensors_for_log(self._root, log_id).items():
+        for sensor, count in stat_sensors_for_log(self._root, log_id, index_version=index_version).items():
             print(f"{sensor.value + ':':<40} {count: 6d}")
         print("=" * 80)
 
-    def stat_sensors(self, start: int = 0, max: int = 100, min_img: int = 10, out_root: str = "/tmp"):
+    def stat_sensors(
+        self, start: int = 0, max: int = 100, min_img: int = 10, out_root: str = "/tmp", index_version: int = 2
+    ):
         """Gets statistics over the sensors in the dataset.
 
         Args:
             start:      The index of the first log to analyze.
             max:        The index of the last log to analyze (exclusive).
             min_img:    The minimum number of images a sensor must have to count as "present".
             out_root:   Write detailed information to this directory.
         """
-        all_logs = self.all_logs[start:max]
-        pool = Parallel(n_jobs=mp.cpu_count() * 2, verbose=10)
-        results = pool(delayed(stat_sensors_for_log)(self._root, log) for log in all_logs)
+        all_logs = [str(x) for x in self.all_logs[start:max]]
+        pool = Parallel(n_jobs=mp.cpu_count() * 2, verbose=1)
+        results = pool(delayed(stat_sensors_for_log)(self._root, log, index_version) for log in all_logs)
 
         total = len(results)
         no_index = 0
         none_missing = 0
         just_one_missing = []
         two_plus_missing = []
         has_stereo_total = 0
@@ -393,15 +393,15 @@
         with open(all_missing_fpath, "w") as f:
             f.write("\n".join(map(str, all_missing)))
 
         print(f"Wrote statistic lists to {out_root}")
 
     def next_to_index(self, max: int = 10, input_limit: int = 300):
         """Prints internal index commands for indexing logs which need indexing."""
-        all_logs = self.all_logs[:input_limit]
+        all_logs = [str(x) for x in self.all_logs[:input_limit]]
         to_index = []
 
         for log_id, status in zip(all_logs, qls_it(self._root, all_logs, batch_size=50)):
             if status == LogStatus.DONE_NOT_INDEXED:
                 to_index.append(log_id)
 
             if len(to_index) >= max:
@@ -424,15 +424,15 @@
         """Computes internal dump commands for the next logs to process.
 
         Args:
             max:    Maximum number of logs to RETURN.
             ...
             input_limit: Maximum number of logs to CONSIDER. Useful for working our way through the dataset.
         """
-        all_logs = self.all_logs[:input_limit]
+        all_logs = [str(x) for x in self.all_logs[:input_limit]]
         not_attempted = []
         crashed_or_in_progress = []
 
         attempted_but_need_gpu_job = []
         attempted_but_need_cpu_job = []
         need_only_receipt = []
         effective_list = []
@@ -521,42 +521,37 @@
         if isinstance(files, str):
             files = files.split(",")
 
         print(f"Backing up files: {files}")
         for log_id in tqdm(self.all_logs):
             self.backup_specific_files(original_base_uri, log_id, out_root, files)
 
-    # def index_all_cameras(
-    #     self, log_id: str, out_index_fpath: Optional[str] = None, check: bool = True, parallel: bool = True
-    # ):
-    #     if parallel:
-    #         n_jobs = len(CamName)
-    #         print(f"Using exactly {n_jobs} jobs")
-    #         with mp.Pool(processes=n_jobs) as pool:
-    #             pool.starmap(
-    #                 self.index_camera,
-    #                 [(log_id, cam_name, out_index_fpath, check, index) for index, cam_name in enumerate(CamName)],
-    #             )
-    #     else:
-    #         for cam in CamName:
-    #             self.index_camera(log_id=log_id, cam_name=cam, out_index_fpath=out_index_fpath, check=check)
+    # def index_all_cameras_range(self, idx_start, idx_end, reindex=False, index_version: int = 2):
+    #     for idx in range(idx_start, idx_end):
+    #         self.index_all_cameras_debug(idx, reindex=reindex, index_version=index_version)
+
+    def gen_index_all_cameras(self, start_idx, end_idx, reindex=False, index_version: int = 2):
+        for idx in range(start_idx, end_idx):
+            print(
+                f"poetry run python -m pit30m.monkeywrench index_all_cameras_debug {idx} --reindex={str(reindex)} --index-version {index_version}"
+            )
 
-    def index_all_cameras_debug(self, idx, reindex=False, index_version: int = 0):
+    def index_all_cameras_debug(self, idx, reindex=False, index_version: int = 2):
         log_id = self.all_logs[idx]
         print("=" * 80)
         print(f"Indexing log {log_id} ({idx + 1} / {len(self.all_logs)})")
         print("=" * 80)
-        self.index_all_cameras(log_id, reindex=reindex, index_version=index_version)
+        self.index_all_cameras(str(log_id), reindex=reindex, index_version=index_version)
 
     def index_all_cameras(
         self,
         log_id: str,
         out_index_dir: Optional[str] = None,
         reindex: bool = False,
-        index_version: int = 0,
+        index_version: int = 2,
     ):
         """Create an index of the images in the given log.
 
         This is useful for quickly finding images in a given region, or for finding the closest image to a given GPS
         location.
 
         Building large indexes from scratch can take a while, even on the order of hours on some machines.
@@ -564,56 +559,55 @@
         Args:
             log_id:             ID of the log to process within the established root.
             out_index_fpath:    Path to the output index file. If not given, the index will be written relative to
                                 the respective camera roots (highly recommended).
             reindex:            If True, the index will be rebuilt even if it already exists.
             index_version:      The kind of indexing to use.
         """
+        assert isinstance(log_id, str), f"Expected log_id to be a string, got {type(log_id)}"
         for cam_name in CamName:
-            self._logger.info(f"\n==========\n{cam_name.name}\n==========")
+            self._logger.info(f"\n==========\n{cam_name.name} - index v{index_version:02d} generation - \n==========")
             self.index_camera_v2(
                 log_id=log_id,
-                # _root=_root,
+                cam_name=cam_name,
                 out_index_dir=out_index_dir,
-                # submap_utm_fpath=submap_utm_fpath,
                 reindex=reindex,
-                cam_name=cam_name,
                 index_version=index_version,
             )
 
     def index_camera_v2(
         self,
         log_id: str,
         cam_name: Union[CamName, str],
-        out_index_dir: Optional[str] = None,
-        reindex: bool = False,
-        index_version: int = 0,
+        out_index_dir: Optional[str],
+        reindex: bool,
+        index_version: int,
     ):
         """v2 indexer - parallel reading and no image loading. Please see `index_all_cameras` for info."""
-        assert index_version == 0, "v0 is the only currently supported DTYPE"
-        map = self.map
+        assert index_version == 2, "v2 is the only currently supported DTYPE"
+        map = Map()
 
         if isinstance(cam_name, str):
             cam_name = CamName(cam_name)
 
         self._logger.info("Setting up log reader to process camera %s", cam_name.value)
         log_root = os.path.join(self._root, log_id.lstrip("/"))
         log_reader = LogReader(log_root_uri=log_root, map=map)
         cam_dir = os.path.join(log_root, "cameras", cam_name.value.lstrip("/"))
 
         if out_index_dir is None:
             out_index_dir = os.path.join(cam_dir, "index")
 
-        in_scheme = urlparse(self._root).scheme
+        urlparse(self._root).scheme
         out_scheme = urlparse(out_index_dir).scheme
         # in_fs = fsspec.filesystem(in_scheme)
         out_fs = fsspec.filesystem(out_scheme)
         #     _logger.info("out fs scheme: %s", out_scheme)
 
-        out_index_fpath = os.path.join(out_index_dir, f"index_v{index_version}.npy")
+        out_index_fpath = os.path.join(out_index_dir, f"index_v{index_version:02d}.npy")
         out_index_fpath_npz = out_index_fpath.replace(".npy", ".npz")
 
         self._logger.info("Checking if index %s is there... (incl npz version)", out_index_fpath)
         exists_npy = out_fs.exists(out_index_fpath)
         exists_npz = out_fs.exists(out_index_fpath_npz)
         exists = exists_npy and exists_npz
         if exists and not reindex:
@@ -622,56 +616,69 @@
 
         self._logger.info(
             "Will build index... reindex = %s, exists_npy = %s, exists_npz = %s",
             str(reindex),
             str(exists_npy),
             str(exists_npz),
         )
-        index = build_camera_index(self._root, log_reader, cam_dir, self._logger)
+        index = build_camera_index(self._root, log_reader, cam_dir, self._logger, index_version=index_version)
 
         # For a rather hefty log (1h20) a v0 index would be ~17MiB uncompressed per camera.
         #
         # npz makes this 1/3 of the size, so I think it's worth it. I'll save both so users can pick.
         out_fs.makedirs(out_index_dir, exist_ok=True)
         with out_fs.open(out_index_fpath, "wb") as out_f:
             np.save(out_f, index)
         with out_fs.open(out_index_fpath_npz, "wb") as out_f:
             np.savez_compressed(out_f, index=index)
         print(f"Wrote index(es) to: {out_index_fpath}")
 
-    def index_lidar_debug(self, log_index, reindex=False, index_version: int = 0):
-        log_id = self.all_logs[log_index]
+    def gen_index_lidar(self, start_idx, end_idx, reindex=False, index_version: int = 2, shuffle_seed: int = 42):
+        for idx in range(start_idx, end_idx):
+            print(
+                f"poetry run python -m pit30m.monkeywrench index_lidar_debug {idx} "
+                f"--reindex={str(reindex)} --index-version {index_version} --shuffle-seed {shuffle_seed}"
+            )
+
+    def index_lidar_debug(self, log_index, reindex=False, index_version: int = 2, shuffle_seed: int = 42):
+        all_logs = list(self.all_logs)
+        random.seed(shuffle_seed)
+        random.shuffle(all_logs)
+        log_id = str(all_logs[log_index])
         print("=" * 80)
         print(f"Indexing log LiDAR {log_id} ({log_index + 1} / {len(self.all_logs)})")
+        print(f"Version: {index_version:03d} | Reindex: {reindex}")
         print("=" * 80)
-        return self.index_lidar(log_id, reindex=reindex, index_version=index_version, out_index_dir=None)
+        return self.index_lidar(
+            log_id, lidar_name=VELODYNE_NAME, reindex=reindex, index_version=index_version, out_index_dir=None
+        )
 
     def index_lidar(
         self,
         log_id: str,
-        lidar_name: str = VELODYNE_NAME,
-        out_index_dir: Optional[str] = None,
-        reindex: bool = False,
-        index_version: int = 0,
+        lidar_name: str,
+        out_index_dir: Optional[str],
+        reindex: bool,
+        index_version: int,
     ):
-        assert index_version == 0, "v0 is the only currently supported DTYPE"
-        map = self.map
+        assert index_version == 2, "v2 is the only currently supported DTYPE"
+        map = Map()
 
         self._logger.info("Setting up log reader to process LiDAR %s", lidar_name)
         log_root = os.path.join(self._root, log_id.lstrip("/"))
         log_reader = LogReader(log_root_uri=log_root, map=map)
         lidar_dir = self.get_lidar_dir(log_root, lidar_name)
 
         if out_index_dir is None:
             out_index_dir = os.path.join(lidar_dir, "index")
 
         out_scheme = urlparse(out_index_dir).scheme
         out_fs = fsspec.filesystem(out_scheme)
 
-        out_index_fpath = os.path.join(out_index_dir, f"index_v{index_version}.npy")
+        out_index_fpath = os.path.join(out_index_dir, f"index_v{index_version:02d}.npy")
         out_index_fpath_npz = out_index_fpath.replace(".npy", ".npz")
 
         self._logger.info("Checking if LiDAR index %s is there... (incl npz version)", out_index_fpath)
         exists_npy = out_fs.exists(out_index_fpath)
         exists_npz = out_fs.exists(out_index_fpath_npz)
         exists = exists_npy and exists_npz
         if exists and not reindex:
@@ -680,32 +687,39 @@
 
         self._logger.info(
             "Will build index... reindex = %s, exists_npy = %s, exists_npz = %s",
             str(reindex),
             str(exists_npy),
             str(exists_npz),
         )
-        index = build_lidar_index(self._root, log_reader, lidar_dir, self._logger)
+        index = build_lidar_index(self._root, log_reader, lidar_dir, self._logger, index_version=index_version)
 
         out_fs.makedirs(out_index_dir, exist_ok=True)
         with out_fs.open(out_index_fpath, "wb") as out_f:
             np.save(out_f, index)
         with out_fs.open(out_index_fpath_npz, "wb") as out_f:
             np.savez_compressed(out_f, index=index)
         print(f"Wrote LiDAR index(es) to: {out_index_fpath}")
 
+    def modernize_lidar(self):
+        # TODO(andrei): Implement simple LIDAR modernizer - it will speed up future indexing too!
+        pass
+
     def check_all_cameras_by_index(
         self,
         idx: int,
         sample_fraction: float = DEFAULT_CAM_CHECK_FRACTION,
         in_index_dir: Optional[str] = None,
         index_version: int = 0,
     ):
         return self.check_all_cameras(
-            self.all_logs[idx], sample_fraction=sample_fraction, in_index_dir=in_index_dir, index_version=index_version
+            str(self.all_logs[idx]),
+            sample_fraction=sample_fraction,
+            in_index_dir=in_index_dir,
+            index_version=index_version,
         )
 
     def check_all_cameras(
         self,
         log_id: str,
         sample_fraction: float = DEFAULT_CAM_CHECK_FRACTION,
         in_index_dir: Optional[str] = None,
@@ -722,15 +736,15 @@
 
     def check_camera(
         self,
         log_id: str,
         cam_name: Union[str, CamName],
         sample_fraction: float = DEFAULT_CAM_CHECK_FRACTION,
         in_index_dir: Optional[str] = None,
-        index_version: int = 0,
+        index_version: int = 2,
         min_num_samples: int = 500,
     ):
         """Samples camera data and checks its integrity. Camera needs to have been indexed first."""
         lr = LogReader(os.path.join(self._root, log_id.strip("/")))
 
         scheme = urlparse(self._root).scheme
         in_fs = fsspec.filesystem(scheme)
@@ -770,15 +784,15 @@
         # out_fs = fsspec.filesystem(out_scheme)
 
         # out_index_fpath = os.path.join(out_index_dir, f"index_v{index_version}.npy")
         # out_index_fpath_npz = out_index_fpath.replace(".npy", ".npz")
 
         if len(idx) < min_num_samples:
             self._logger.info("Will just check all images")
-            all_idx = range(len(idx))
+            all_idx = list(range(len(idx)))
         else:
             start_end = 60 * 10
             i_st = range(0, start_end)
             i_end = range(len(idx) - start_end, len(idx))
             step = int(1 / sample_fraction)
             mid = range(start_end, len(idx) - start_end, step)
 
@@ -831,15 +845,15 @@
         with in_fs.open(report_fpath, "w") as f:
             json.dump(problems, f)
         with in_fs.open(report_meta_fpath, "w") as f:
             json.dump(meta, f)
 
         return problems, meta
 
-    def validate_reports(self, logs: Optional[str] = None, check_receipt: bool = True, write_receipt: bool = True):
+    def validate_reports(self, logs: str, check_receipt: bool = True, write_receipt: bool = True):
         """
         Note that this will typically be the command you run locally, as reading a few CSVs for each log is more than
         doable locally.
 
         Args:
             logs:       Either a file path to a text file with a list of log IDs to validate, or a comma-separated list
                         of log IDs to validate.
@@ -959,16 +973,17 @@
                 with out_fs.open(receipt_fpath, "w") as f:
                     f.write("OK, 'other' not checked")
 
             return (True, "")
         else:
             return (False, lidar_status + camera_summary + other_summary)
 
-    def diagnose_misc(self, log_id: str, out_index_fpath: str, check: bool) -> List[Tuple[str, str]]:
+    def diagnose_misc(self, log_id: str, out_index_fpath: Optional[str], check: bool) -> List[Tuple[str, str]]:
         """Diagnoses non-sensor data, like poses, GPS, metadata, etc. Returns a list of errors, empty if all is well."""
+        del out_index_fpath  # unused for now
         fs = fsspec.filesystem(urlparse(self._root).scheme)
         log_root_uri = os.path.join(self._root, log_id)
         log_reader = LogReader(log_root_uri=log_root_uri)
 
         errors: List[Tuple[str, str]] = []
 
         # Active district information is not very important
@@ -985,15 +1000,15 @@
 
         # TODO(andrei): We probably want to provide poses as something uncompressed, since LZMA decoding is a few
         # seconds per log. For training we will cache this in some index files, but in general it's annoying to wait
         # 4-5 seconds on a modern PC to read 50MiB of data...
         try:
             mrp = log_reader.map_relative_poses_dense
             assert mrp["time"].min() > 0
-        except (RuntimeError, ValueError) as err:
+        except (RuntimeError, ValueError):
             errors.append(("map_relative_poses_dense", "invalid"))
 
         try:
             raw_wgs_dense = log_reader.raw_wgs84_poses_dense
             if raw_wgs_dense[:, 0].min() <= 0:
                 errors.append(("raw_wgs84_poses_dense", "negative or zero time"))
             min_lat = raw_wgs_dense[:, 2].min()
@@ -1122,21 +1137,21 @@
                         # print(vs.dtype)
                         # print(len(vs))
             except RuntimeError as err:
                 errors.append(("vehicle_state", "invalid" + str(err)))
         else:
             errors.append(("vehicle_state", "missing"))
 
-        # XXX(andrei): Write this as a report entry! Discriminate between WARNING and ERROR. The difference is about
+        # TODO(andrei): Write this as a report entry! Discriminate between WARNING and ERROR. The difference is about
         # which files are missing. E.g., tl states missing is a warning, but core metadata, poses, or calibration
         # missing is an error.
         if check and len(errors) > 0:
             print(f"{len(errors)} errors found in {log_id}!")
-            for err in errors:
-                print("\t- " + str(err))
+            for error in errors:
+                print("\t- " + str(error))
 
         return errors
 
     def validate_camera_report(
         self,
         log_id: str,
         cam_name: str,
@@ -1155,42 +1170,42 @@
             print("Skipping validation of", cam_dir, "since it has a receipt.")
             return (True, "canary_found")
 
         if not os.path.isfile(report_loc):
             return (False, "no_report")
 
         ok = 0
-        errors = []
+        errors: list[tuple[str, float, str, str]] = []
         warnings = []
         unmatched_frames = []
 
         with open(report_loc, "r") as csvfile:
             reader = csv.reader(csvfile, quotechar="|", quoting=csv.QUOTE_MINIMAL)
             header = next(reader)
             if len(header) != 4:
-                errors.append(("", -1, INVALID_REPORT, "Invalid header: " + str(header)))
+                errors.append(("", -1.0, INVALID_REPORT, "Invalid header: " + str(header)))
             else:
                 for sample_uri, timestamp, status, detail in reader:
                     if status == "OK":
                         ok += 1
                         continue
                     elif status == CAM_UNMATCHED_POSE:
                         delta_s = float(detail)
                         unmatched_frames.append((float(timestamp), delta_s, sample_uri))
                         warnings.append("unmatched frame at " + str(timestamp) + "s, delta_s=" + str(delta_s))
                     else:
                         # print(f"Problem with {sample_uri}: {status}")
-                        errors.append((sample_uri, timestamp, status, detail))
+                        errors.append((sample_uri, float(timestamp), status, detail))
 
         if len(unmatched_frames):
-            max_delta = -1
+            max_delta = -1.0
             clusters = []
-            cur_start = -1
+            cur_start = -1.0
             cur_start_idx = -1
-            prev_ts = -1
+            prev_ts = -1.0
             for idx, (ts, delta_s, sample_uri) in enumerate(unmatched_frames):
                 # print(f"{ts:.3f}", sample_uri.split("/")[-1], delta_s)
 
                 if cur_start == -1 or ts - prev_ts > 1.0:
                     # Add the previous cluster, if it exists
                     if cur_start != -1:
                         clusters.append((cur_start_idx, idx - 1))
@@ -1266,43 +1281,43 @@
         log_root = os.path.join(self._root, log_id.lstrip("/"))
         lidar_dir = self.get_lidar_dir(log_root, lidar_name)
         out_index_fpath = os.path.join(lidar_dir, "index")
         report_loc = os.path.join(out_index_fpath, "report.csv")
         canary_loc = os.path.join(out_index_fpath, VALIDATION_CANARY_FNAME)
 
         ok = 0
-        errors = []
-        warnings = []
+        errors: list[tuple[str, float, str, str]] = []
+        warnings: list[tuple[str, float, str, str]] = []
 
         fs = fsspec.filesystem(urlparse(self._root).scheme)
         if check_receipt and fs.isfile(canary_loc):
             print("Skipping validation of", lidar_dir, "since it has a receipt.")
             return (True, "canary_found")
 
         if not os.path.isfile(report_loc):
             return (False, "no_report")
 
         with open(report_loc, "r") as csvfile:
             reader = csv.reader(csvfile, quotechar="|", quoting=csv.QUOTE_MINIMAL)
             header = next(reader)
             if len(header) != 4:
-                errors.append(("", -1, INVALID_REPORT, "Invalid header: " + str(header)))
+                errors.append(("", -1.0, INVALID_REPORT, "Invalid header: " + str(header)))
             else:
                 for sample_uri, timestamp, status, detail in reader:
                     if status == "OK":
                         ok += 1
                         continue
                     elif status == "bad-raw-WGS84-offset":
                         offset_s = float(detail.rstrip("s"))
                         if offset_s > acceptable_wgs84_delay_s:
                             # Be a little lenient
-                            warnings.append((sample_uri, timestamp, status, detail))
+                            warnings.append((sample_uri, float(timestamp), status, detail))
                     else:
                         # print(f"Problem with {sample_uri}: {status}")
-                        errors.append((sample_uri, timestamp, status, detail))
+                        errors.append((sample_uri, float(timestamp), status, detail))
 
         if len(errors) > 0:
             print(f"Found {len(errors)} errors in {log_id}.")
             for err in errors[:10]:
                 print("\t", err)
             if len(errors) > 10:
                 print("...")
@@ -1344,12 +1359,12 @@
 # Trick to bypass !binary parts of YAML files before we can support them. (They are low priority and not
 # very important anyway.)
 class SafeLoaderIgnoreUnknown(yaml.SafeLoader):
     def ignore_unknown(self, node):
         return None
 
 
-SafeLoaderIgnoreUnknown.add_constructor(None, SafeLoaderIgnoreUnknown.ignore_unknown)
+SafeLoaderIgnoreUnknown.add_constructor("!binary", SafeLoaderIgnoreUnknown.ignore_unknown)
 
 
 if __name__ == "__main__":
     fire.Fire(MonkeyWrench)
```

### Comparing `pit30m-0.0.1/pit30m/time_utils.py` & `pit30m-0.0.2/pit30m/time_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,21 +39,21 @@
     # bisect.bisect returns the index `date` would have to be
     # inserted to keep `LEAP_DATES` sorted, so is the number of
     # values in `LEAP_DATES` that are less than `date`, or the
     # number of leap seconds.
     return bisect.bisect(LEAP_DATES, date)
 
 
-def gps_seconds_to_utc(gps_secs):
+def gps_seconds_to_utc(gps_secs) -> datetime:
     gps_epoch = datetime(1980, 1, 6, 0, 0, 0)
     date_before_leaps = gps_epoch + timedelta(seconds=gps_secs)
     return date_before_leaps - timedelta(seconds=leap(date_before_leaps))
 
 
-def gps2utc(week, secs):
+def gps2utc(week, secs) -> datetime:
     """
     :param week: GPS week number, i.e. 1866
     :param secs: number of seconds since the beginning of `week`
     :return: datetime instance with UTC time
     """
     secs_in_week = 604800
     gps_secs = week * secs_in_week + secs
```

### Comparing `pit30m-0.0.1/pit30m/torch/dataset.py` & `pit30m-0.0.2/pit30m/torch/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import os
 import time
 from functools import cached_property
 from typing import Sequence, Union
-from uuid import UUID
 
 import fire
 import numpy as np
-import torch.multiprocessing as mp
-from torch.utils.data import DataLoader, Dataset
+
+try:
+    import torch.multiprocessing as mp
+    from torch.utils.data import DataLoader, Dataset
+except ImportError as err:
+    raise ImportError(
+        "PyTorch is required to import PyTorch Pit30M functionality. Please install PyTorch and try again."
+    ) from err
+
 
 from pit30m.camera import CamName
-from pit30m.data.log_reader import CameraImage, LiDARFrame, LogReader
+from pit30m.data.log_reader import CameraImage, LogReader
 from pit30m.data.submap import Map
-from pit30m.indexing import CAM_INDEX_V0_0_DTYPE
+from pit30m.indexing import CAM_INDEX_V2_0_DTYPE
 
 
 class Pit30MLogDataset(Dataset):
     def __init__(
         self, log_ids: Sequence[str], cam_name: CamName = CamName.MIDDLE_FRONT_WIDE, root_uri: str = "s3://pit30m/"
     ) -> None:
         """A low-level interface dataset for Pit30M operating on a per-log single-sensor basis.
@@ -67,15 +73,15 @@
         # print(f"Getting item {index}...")
         log_idx = np.searchsorted(self._len_cdf, index, side="right")
         idx_in_log = index - self._len_cdf[log_idx] if log_idx > 0 else index
         cur_log_id, cur_index = self._indexes[log_idx]
 
         # Refer to the dtype definition for more information on what is available.
         cur_sample: np.ndarray = cur_index[idx_in_log]
-        assert cur_sample.dtype == CAM_INDEX_V0_0_DTYPE
+        assert cur_sample.dtype == CAM_INDEX_V2_0_DTYPE
 
         image: CameraImage = self._log_readers[cur_log_id].get_image(self._cam_name, idx_in_log)
 
         image_metadata = (
             cur_sample["mrp_present"],
             cur_sample["mrp_valid"],
             cur_sample["mrp_time"],
@@ -108,16 +114,14 @@
 ):
     # Failure to do this may cause fsspec to hang in workers
     mp.set_start_method("forkserver")
 
     if isinstance(logs, str):
         logs = [entry.strip() for entry in logs.split(",")]
 
-    logs = [UUID(log) for log in logs]
-
     print("root_uri", root_uri)
     print("logs:", logs)
     dataset = Pit30MLogDataset(logs, root_uri=root_uri)
     loader = DataLoader(
         # No shuffle for demo/benchmarking purposes.
         dataset=dataset,
         batch_size=batch_size,
```

### Comparing `pit30m-0.0.1/pit30m/util.py` & `pit30m-0.0.2/pit30m/util.py`

 * *Files identical despite different names*

### Comparing `pit30m-0.0.1/pyproject.toml` & `pit30m-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pit30m"
-version = "0.0.1"
+version = "0.0.2"
 description = "Development kit for the Pit30M large scale localization dataset"
 authors = ["Andrei Bârsan"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/pit30m/pit30m"
 classifiers = [
     "Framework :: Robot Framework :: Library",
     "Framework :: Robot Framework :: Tool",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
@@ -18,44 +19,44 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/pit30m/pit30m"
-
 [tool.poetry.dependencies]
 python = "^3.9"
-fsspec = ">=2022"
-s3fs = "*"
-geopandas = ">=0.10"
-pygeos = ">=0.12"
-numpy = ">=1.20"
-fire = ">=0.5"
-joblib = "*"
-pillow = ">=9"
-tqdm = ">=4"
-lz4 = ">=4"
-matplotlib = ">=3.4"
-pyyaml = ">=5"
-utm = ">=0.7.0"
+fsspec = ">=2022"     # seamlessly talk to local or remote (S3) filesystems
+s3fs = "*"            # provides S3 for fsspec
+geopandas = ">=0.10"  # handle geospatial data, e.g. for partitions
+pygeos = ">=0.12"     # backend for geopandas
+numpy = ">=1.20"      # numerical computation, array operations
+fire = ">=0.5"        # helper for command-line interface programs
+joblib = "*"          # parallelization
+pillow = ">=9"        # image processing
+tqdm = ">=4"          # progress bars
+lz4 = ">=4"           # LZ4 compression, similar to gzip but faster, great for loading lots of data
+matplotlib = ">=3.4"  # plotting, visualization, etc.
+pyyaml = ">=5"        # load YAML data, e.g., some of our calibration files
+utm = ">=0.7.0"       # additional geospatial computations concerning UTM projections
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7"
 pytest-mock = "*"
 ipdb = "^0.13"
 black = "^23.1"
 pytest-xdist = "^3.2"
 # TODO(andrei): Special group and special build for these optional deps.
 torch = "^1.13"
 torchdata = "^0.5"
 pylint = "^2.16"
 boto3 = "^1"
+ruff = "^0.0.270"
+mypy = "^1.3.0"
+types-pyyaml = "^6.0.12.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint]
 max-line-length = 120
@@ -80,7 +81,12 @@
   | dist
 )/
 '''
 
 [tool.isort]
 profile = "black"
 
+[tool.mypy]
+plugins = "numpy.typing.mypy_plugin"
+
+[tool.ruff]
+line-length = 120 # consistent witth black
```

