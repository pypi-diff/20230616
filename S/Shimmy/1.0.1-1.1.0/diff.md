# Comparing `tmp/Shimmy-1.0.1.tar.gz` & `tmp/Shimmy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-1.0.1.tar", last modified: Wed May 24 18:26:22 2023, max compression
+gzip compressed data, was "Shimmy-1.1.0.tar", last modified: Thu Jun 15 22:38:22 2023, max compression
```

## Comparing `Shimmy-1.0.1.tar` & `Shimmy-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.394135 Shimmy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-24 18:26:22.394135 Shimmy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-24 18:26:19.000000 Shimmy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/Shimmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-24 18:26:19.000000 Shimmy-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:26:22.394135 Shimmy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-24 18:26:19.000000 Shimmy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/shimmy/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/atari_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/bsuite_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_control_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/meltingpot_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/openspiel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/shimmy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_control_multiagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/envs_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/meltingpot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.394135 Shimmy-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_atari.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_bsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_control_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_meltingpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_openspiel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 22:38:22.037121 Shimmy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-15 22:38:18.000000 Shimmy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.033121 Shimmy-1.1.0/Shimmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 22:38:18.000000 Shimmy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:38:22.037121 Shimmy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-15 22:38:18.000000 Shimmy-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.033121 Shimmy-1.1.0/shimmy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/atari_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/shimmy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/envs_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_atari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_bsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_meltingpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_openspiel.py
```

### Comparing `Shimmy-1.0.1/PKG-INFO` & `Shimmy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.0.1
+Version: 1.1.0
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Shimmy-1.0.1/README.md` & `Shimmy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/Shimmy.egg-info/PKG-INFO` & `Shimmy-1.1.0/Shimmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.0.1
+Version: 1.1.0
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Shimmy-1.0.1/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.1.0/Shimmy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/Shimmy.egg-info/requires.txt` & `Shimmy-1.1.0/Shimmy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/pyproject.toml` & `Shimmy-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/setup.py` & `Shimmy-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/__init__.py` & `Shimmy-1.1.0/shimmy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
     "MeltingPotCompatibilityV0",
 ]
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `Shimmy-1.0.1/shimmy/atari_env.py` & `Shimmy-1.1.0/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/bsuite_compatibility.py` & `Shimmy-1.1.0/shimmy/bsuite_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/dm_control_compatibility.py` & `Shimmy-1.1.0/shimmy/dm_control_compatibility.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,74 +48,63 @@
     Note:
         dm-control uses `np.random.RandomState`, a legacy random number generator while gymnasium
         uses `np.random.Generator`, therefore the return type of `np_random` is different from expected.
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array", "depth_array", "multi_camera"],
-        "render_fps": 10,
+        "render_fps": 10,  # this value is updated to use the `env.control_timesteps() * 1000`
     }
 
     def __init__(
         self,
         env: composer.Environment | control.Environment | dm_env.Environment,
         render_mode: str | None = None,
-        render_height: int = 84,
-        render_width: int = 84,
-        camera_id: int | str = 0,
-        render_scene_callback: (Callable[[MujocoEnginePhysics, MjvScene], None])
-        | None = None,
         render_kwargs: dict[str, Any] | None = None,
     ):
         """Initialises the environment with a render mode along with render information.
 
         Note: this wrapper supports multi-camera rendering via the `render_mode` argument (render_mode = "multi_camera")
 
         For more information on DM Control rendering, see https://github.com/deepmind/dm_control/blob/main/dm_control/mujoco/engine.py#L178
 
         Args:
             env (Optional[composer.Environment | control.Environment | dm_env.Environment]): DM Control env to wrap
             render_mode (Optional[str]): rendering mode (options: "human", "rgb_array", "depth_array", "multi_camera")
-            render_height (Optional[int]): height for rendering frame in pixels
-            render_width (Optional[int]): width for rendering frame in pixels
-            camera_id (Optional[int | str]): Optional camera name or index. Defaults to -1, the free
-                camera, which is always defined. A nonnegative integer or string
-                corresponds to a fixed camera, which must be defined in the model XML.
-                If `camera_id` is a string then the camera must also be named.
-            render_scene_callback (Optional[(Callable[[MujocoEnginePhysics, mujoco.MjvScene], None])]): Called after
-                the scene has been created and before it is rendered. Can be used to add more geoms to the scene.
-            render_kwargs (Optional[dict[str, Any]]): Additional keyword arguments for rendering. Note: kwargs are not used
-                for human rendering, which uses simpler Gymnasium MuJoCo rendering.
+            render_kwargs (Optional[dict[str, Any]]): Additional keyword arguments for rendering.
+                For the width, height and camera id use "width", "height" and "camera_id" respectively.
+                See the dm_control implementation for the list of possible kwargs, https://github.com/deepmind/dm_control/blob/330c91f41a21eacadcf8316f0a071327e3f5c017/dm_control/mujoco/engine.py#L178
+                Note: kwargs are not used for human rendering, which uses simpler Gymnasium MuJoCo rendering.
         """
-        EzPickle.__init__(
-            self, env, render_mode, render_height, render_width, camera_id
-        )
+        EzPickle.__init__(self, env, render_mode, render_kwargs)
         self._env: Any = env
         self.env_type = self._find_env_type(env)
-        self.metadata["render_fps"] = self._env.control_timestep()
+        self.metadata["render_fps"] = self._env.control_timestep() * 1000
 
         self.observation_space = dm_spec2gym_space(env.observation_spec())
         self.action_space = dm_spec2gym_space(env.action_spec())
 
         assert render_mode is None or render_mode in self.metadata["render_modes"]
         self.render_mode = render_mode
-        self.render_height, self.render_width = render_height, render_width
-        self.camera_id = camera_id
-        self.render_scene_callback = render_scene_callback
 
         if render_kwargs is None:
             render_kwargs = {}
         self.render_kwargs = render_kwargs
 
         if self.render_mode == "human":
             # We use the gymnasium mujoco rendering, dm-control provides more complex rendering options.
             self.viewer = MujocoRenderer(
                 self._env.physics.model.ptr, self._env.physics.data.ptr
             )
 
+    @property
+    def dt(self):
+        """Returns the environment control timestep which is equivalent to the number of actions per second."""
+        return self._env.control_timestep()
+
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[ObsType, dict[str, Any]]:
         """Resets the dm-control environment."""
         super().reset(seed=seed)
         if seed is not None:
             self.np_random = np.random.RandomState(seed=seed)
@@ -144,53 +133,49 @@
             info,
         )
 
     def render(self) -> np.ndarray | None:
         """Renders the dm-control env."""
         if self.render_mode == "rgb_array":
             return self._env.physics.render(
-                height=self.render_height,
-                width=self.render_width,
-                camera_id=self.camera_id,
-                scene_callback=self.render_scene_callback,
                 **self.render_kwargs,
             )
         elif self.render_mode == "depth_array":
             return self._env.physics.render(
-                height=self.render_height,
-                width=self.render_width,
-                camera_id=self.camera_id,
                 depth=True,
-                scene_callback=self.render_scene_callback,
                 **self.render_kwargs,
             )
         elif self.render_mode == "multi_camera":
             physics = self._env.physics
             num_cameras = physics.model.ncam
             num_columns = int(math.ceil(math.sqrt(num_cameras)))
             num_rows = int(math.ceil(float(num_cameras) / num_columns))
+
+            # 240 and 320 are the default values in dm-control
+            height = self.render_kwargs.get("height", 240)
+            width = self.render_kwargs.get("width", 320)
             frame = np.zeros(
-                (num_rows * self.render_height, num_columns * self.render_width, 3),
+                (num_rows * height, num_columns * width, 3),
                 dtype=np.uint8,
             )
+            assert (
+                "camera_id" not in self.render_kwargs
+            ), "The camera_id is specified in `multi_camera` render so don't include it in the render_kwargs"
             for col in range(num_columns):
                 for row in range(num_rows):
                     camera_id = row * num_columns + col
                     if camera_id >= num_cameras:
                         break
                     subframe = physics.render(
-                        height=self.render_height,
-                        width=self.render_width,
                         camera_id=camera_id,
-                        scene_callback=self.render_scene_callback,
                         **self.render_kwargs,
                     )
                     frame[
-                        row * self.render_height : (row + 1) * self.render_height,
-                        col * self.render_width : (col + 1) * self.render_width,
+                        row * height : (row + 1) * height,
+                        col * width : (col + 1) * width,
                     ] = subframe
             return frame
 
     def close(self):
         """Closes the environment."""
         self._env.physics.free()
         self._env.close()
```

### Comparing `Shimmy-1.0.1/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.1.0/shimmy/dm_control_multiagent_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/dm_lab_compatibility.py` & `Shimmy-1.1.0/shimmy/dm_lab_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/meltingpot_compatibility.py` & `Shimmy-1.1.0/shimmy/meltingpot_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/openai_gym_compatibility.py` & `Shimmy-1.1.0/shimmy/openai_gym_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/openspiel_compatibility.py` & `Shimmy-1.1.0/shimmy/openspiel_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/registration.py` & `Shimmy-1.1.0/shimmy/registration.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/utils/dm_control_multiagent.py` & `Shimmy-1.1.0/shimmy/utils/dm_control_multiagent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/utils/dm_env.py` & `Shimmy-1.1.0/shimmy/utils/dm_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/utils/dm_lab.py` & `Shimmy-1.1.0/shimmy/utils/dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/utils/envs_configs.py` & `Shimmy-1.1.0/shimmy/utils/envs_configs.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/shimmy/utils/meltingpot.py` & `Shimmy-1.1.0/shimmy/utils/meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_atari.py` & `Shimmy-1.1.0/tests/test_atari.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_bsuite.py` & `Shimmy-1.1.0/tests/test_bsuite.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_dm_control.py` & `Shimmy-1.1.0/tests/test_dm_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,21 @@
         assert term_1 == term_2 and trunc_1 == trunc_2
         assert data_equivalence(info_1, info_2)
 
     env_1.close()
     env_2.close()
 
 
-@pytest.mark.parametrize("camera_id", [0, 1])
+@pytest.mark.parametrize("camera_id", [-1, 0, 1])
 def test_rendering_camera_id(camera_id):
     """Test that dm-control rendering works."""
     env = gym.make(
         DM_CONTROL_ENV_IDS[0],
         render_mode="rgb_array",
-        camera_id=camera_id,
+        render_kwargs=dict(camera_id=camera_id),
     )
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
@@ -153,16 +153,18 @@
 
 @pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
 def test_rendering_multiple_cameras(height, width):
     """Test that multi_camera rendering mode works for dm-control environments."""
     env = gym.make(
         DM_CONTROL_ENV_IDS[0],
         render_mode="multi_camera",
-        render_height=height,
-        render_width=width,
+        render_kwargs=dict(
+            height=height,
+            width=width,
+        ),
     )
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
@@ -171,16 +173,18 @@
 
 @pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
 def test_rendering_depth(height, width):
     """Test that depth rendering mode works for dm-control environments."""
     env = gym.make(
         DM_CONTROL_ENV_IDS[0],
         render_mode="depth_array",
-        render_height=height,
-        render_width=width,
+        render_kwargs=dict(
+            height=height,
+            width=width,
+        ),
     )
     env.reset()
     frames = []
     for _ in range(10):
         frames.append(env.render())
         env.step(env.action_space.sample())
 
@@ -189,16 +193,18 @@
 
 @pytest.mark.parametrize("height,width", [(84, 84), (48, 48), (128, 128), (100, 200)])
 def test_render_height_widths(height, width):
     """Tests that dm-control rendering heights and widths works."""
     env = gym.make(
         DM_CONTROL_ENV_IDS[0],
         render_mode="rgb_array",
-        render_height=height,
-        render_width=width,
+        render_kwargs=dict(
+            height=height,
+            width=width,
+        ),
     )
     env.reset()
     frame = env.render()
     assert isinstance(frame, np.ndarray)
     assert frame.shape == (height, width, 3), frame.shape
 
     env.close()
```

### Comparing `Shimmy-1.0.1/tests/test_dm_control_multi_agent.py` & `Shimmy-1.1.0/tests/test_dm_control_multi_agent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_dm_lab.py` & `Shimmy-1.1.0/tests/test_dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_gym.py` & `Shimmy-1.1.0/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_meltingpot.py` & `Shimmy-1.1.0/tests/test_meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.1/tests/test_openspiel.py` & `Shimmy-1.1.0/tests/test_openspiel.py`

 * *Files identical despite different names*

