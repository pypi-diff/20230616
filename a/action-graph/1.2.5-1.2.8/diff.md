# Comparing `tmp/action-graph-1.2.5.tar.gz` & `tmp/action-graph-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.2.5.tar", last modified: Fri Mar 10 21:06:16 2023, max compression
+gzip compressed data, was "action-graph-1.2.8.tar", last modified: Fri Jun 16 14:47:09 2023, max compression
```

## Comparing `action-graph-1.2.5.tar` & `action-graph-1.2.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.5/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.5/README.md
--rw-r--r--   0        0        0      684 2023-03-10 21:00:00.232971 action-graph-1.2.5/action_graph/__init__.py
--rw-r--r--   0        0        0     3181 2022-12-14 19:29:21.720928 action-graph-1.2.5/action_graph/action.py
--rw-r--r--   0        0        0     9491 2022-12-14 18:55:20.840750 action-graph-1.2.5/action_graph/agent.py
--rw-r--r--   0        0        0     4630 2022-12-14 19:25:01.486788 action-graph-1.2.5/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-03-10 21:00:53.340695 action-graph-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     1182 2022-12-14 18:55:45.420838 action-graph-1.2.5/tests/01-redundant_precon.py
--rw-r--r--   0        0        0     1180 2022-12-14 18:55:48.488849 action-graph-1.2.5/tests/02-multi_feasible.py
--rwxr-xr-x   0        0        0     1371 2022-10-27 19:31:38.000000 action-graph-1.2.5/tests/03-references.py
--rwxr-xr-x   0        0        0      917 2022-12-14 19:54:19.695451 action-graph-1.2.5/tests/04-loop_test.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.2.8/README.md
+-rw-r--r--   0        0        0      684 2023-06-16 14:46:27.786532 action-graph-1.2.8/action_graph/__init__.py
+-rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.2.8/action_graph/action.py
+-rw-r--r--   0        0        0     9491 2023-06-16 02:52:33.411377 action-graph-1.2.8/action_graph/agent.py
+-rw-r--r--   0        0        0     4689 2023-06-16 03:39:34.857713 action-graph-1.2.8/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-16 14:46:33.286410 action-graph-1.2.8/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.2.8/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1096 2023-06-16 14:35:32.753006 action-graph-1.2.8/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.2.8/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      917 2023-06-16 14:31:44.398052 action-graph-1.2.8/tests/04-loop_test.py
+-rw-r--r--   0        0        0        0 2023-06-16 14:40:25.834530 action-graph-1.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.2.8/PKG-INFO
```

### Comparing `action-graph-1.2.5/LICENSE` & `action-graph-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.5/README.md` & `action-graph-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.5/action_graph/__init__.py` & `action-graph-1.2.8/action_graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.2.5'
+__version__ = '1.2.8'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.2.5/action_graph/action.py` & `action-graph-1.2.8/action_graph/action.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.5/action_graph/agent.py` & `action-graph-1.2.8/action_graph/agent.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.5/action_graph/planner.py` & `action-graph-1.2.8/action_graph/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         :return:List[Action]: List of actions updated with their expected outcomes (effects)
         """
 
         if len(target_state.items()) > 1:
             raise PlanningFailedException('target_state should have a single state variable')
         tk, tv = list(target_state.items())[0]
         # in case target state value is a reference to another state variable
-        tv = self.__parse_references(tv, start_state)
+        if isinstance(tv, str) and tv[0] == '@':
+            tv = self.__parse_references(tv, start_state)
         # check if the target state is already satisfied
         if (tk, tv) in list(start_state.items()):
             return []   # goal already met, move on
         #
         # find action(s) that satisfy the state current effect-item
         probable_actions: List[Action] = self._action_lookup[(tk, tv)]
         if not probable_actions:  # if no actions are found, try with templated actions
@@ -59,15 +60,16 @@
             action = p_action.__copy__()
             if action.effects[tk] is Ellipsis:
                 action.effects[tk] = tv  # apply variable effects
             #
             action_path: List[Action] = []
             for pk, pv in action.preconditions.items():  # for each pre-condition ...
                 try:  # choose the shortest feasible path
-                    pv = self.__parse_references(pv, action.effects)
+                    if isinstance(pv, str) and pv[0] == '$':
+                        pv = self.__parse_references(pv, action.effects)
                     action_path += self.generate_plan({pk: pv}, start_state, avoid_actions)  # merge the actions
                 except RecursionError:  # watch out for cyclic references
                     raise PlanningFailedException(f'Found cyclic references!')
             # include the current action;  remove duplicates; keep the order intact
             action_path = self.__make_unique(action_path + [action])
             #
             if not chosen_path:  # if no other path is available...
@@ -87,15 +89,14 @@
         action_lookup: Dict[Tuple[Any, Any], List[Action]] = defaultdict(list)
         for action in actions:
             for k, v in action.effects.items():
                 action_lookup[(k, v)].append(action)
         return action_lookup
 
     def __parse_references(self, ref: Any, state: State) -> Any:
-        if isinstance(ref, str) and ref[0] == '$':
-            if ref[1:] in state:
-                return state[ref[1:]]
+        if ref[1:] in state:
+            return state[ref[1:]]
         return ref
 
     def __make_unique(self, path):
         unique = set()
         return [x for x in path if x not in unique and not unique.add(x)]
```

### Comparing `action-graph-1.2.5/pyproject.toml` & `action-graph-1.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.2.5"
+version = "1.2.8"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.2.5/tests/01-redundant_precon.py` & `action-graph-1.2.8/tests/01-redundant_precon_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,16 @@
     world_state = {} # unknown
     goal_state = {"FOURTH": True}
 
     ai = Agent()
 
     actions = [a(ai) for a in Action.__subclasses__()]
     ai.load_actions(actions)
-
-    print("Initial State:", world_state)
     ai.update_state(world_state)
-
-    print("Goal State:   ", goal_state)
     plan = ai.get_plan(goal_state)
-
+    
     expected_actions = ["Action1", "Action2", "Action3", "Action4"]
     expected_outcome = [{'FIRST': True}, {'SECOND': True}, {'THIRD': True}, {'FOURTH': True}]
 
     for ax, eax, eoc in zip(plan, expected_actions, expected_outcome):
         assert ax.__class__.__name__ == eax, f'Incorrect Action!'
         assert ax.effects == eoc, f'Incorrect Action Outcome!'
```

### Comparing `action-graph-1.2.5/tests/02-multi_feasible.py` & `action-graph-1.2.8/tests/03-references_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action
 from action_graph.agent import Agent
 
 
+class Action5(Action):
+    effects = {"FINAL": True}
+    preconditions = {"FIRST": True, "FOURTH": "TESTSTATE"}
+
+
 class Action1(Action):
     effects = {"FIRST": True}
-    preconditions = {}
+    preconditions = {"FIRST": False}
 
 
-class Action2A(Action):
-    effects = {"SECOND": True}
-    preconditions = {"FIRST": True}
+class Action4(Action):
+    effects = {"FOURTH": ...}
+    preconditions = {
+        "SECOND": "$FOURTH",
+        "THIRD": "$FOURTH",
+    }
 
 
-class Action2B(Action):
-    effects = {"SECOND": True}
+class Action2(Action):
+    effects = {"SECOND": ...}
     preconditions = {}
-    cost = 1.5
 
 
 class Action3(Action):
-    effects = {"THIRD": True}
-    preconditions = {"FIRST": True, "SECOND": True}
+    effects = {"THIRD": ...}
+    preconditions = {}
 
 
 def test():
-    world_state = {"FIRST": False, "SECOND": False, "THIRD": False}
-    goal_state = {"THIRD": True}
+    world_state = {"FINAL": False, "FIRST": False}
+    goal_state = {"FINAL": True}
 
     ai = Agent()
 
     actions = [a(ai) for a in Action.__subclasses__()]
     ai.load_actions(actions)
-
-    print("Initial State:", world_state)
     ai.update_state(world_state)
-
-    print("Goal State:   ", goal_state)
     plan = ai.get_plan(goal_state)
 
-    expected_actions = ["Action1", "Action2B", "Action3"]
-    expected_outcome = [{'FIRST': True}, {'SECOND': True}, {'THIRD': True}]
+    expected_actions = ["Action1", "Action2", "Action3", "Action4", "Action5"]
+    expected_outcome = [{'FIRST': True}, {'SECOND': 'TESTSTATE'}, {'THIRD': 'TESTSTATE'}, {'FOURTH': 'TESTSTATE'}, {'FINAL': True}]
 
     for ax, eax, eoc in zip(plan, expected_actions, expected_outcome):
         assert ax.__class__.__name__ == eax, f'Incorrect Action!'
         assert ax.effects == eoc, f'Incorrect Action Outcome!'
-
```

### Comparing `action-graph-1.2.5/tests/04-loop_test.py` & `action-graph-1.2.8/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.2.5/PKG-INFO` & `action-graph-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.2.5
+Version: 1.2.8
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

