# Comparing `tmp/openrlbenchmark-0.2.1a2.tar.gz` & `tmp/openrlbenchmark-0.2.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.2.1a2.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.1a3.tar", max compression
```

## Comparing `openrlbenchmark-0.2.1a2.tar` & `openrlbenchmark-0.2.1a3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a2/LICENSE
--rw-r--r--   0        0        0    20353 2023-06-07 20:05:43.595075 openrlbenchmark-0.2.1a2/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a2/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a2/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a2/openrlbenchmark/cache_legacy.py
--rw-r--r--   0        0        0     6147 2023-06-07 19:47:32.024056 openrlbenchmark-0.2.1a2/openrlbenchmark/capped_hns.py
--rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a2/openrlbenchmark/hns.py
--rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a2/openrlbenchmark/offline_db.py
--rw-r--r--   0        0        0    36776 2023-06-07 20:11:32.988139 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    30367 2023-06-07 20:11:32.994334 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0    24942 2023-06-07 20:11:32.989025 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_multi_metrics.py
--rw-r--r--   0        0        0    36919 2023-06-07 20:07:01.541242 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl.py
--rw-r--r--   0        0        0    25177 2023-06-07 20:11:32.986812 openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl_multi_metrics.py
--rw-r--r--   0        0        0      748 2023-06-07 20:26:31.890615 openrlbenchmark-0.2.1a2/pyproject.toml
--rw-r--r--   0        0        0    21316 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.1a3/LICENSE
+-rw-r--r--   0        0        0    20353 2023-06-07 20:05:43.595075 openrlbenchmark-0.2.1a3/README.md
+-rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.1a3/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340069 openrlbenchmark-0.2.1a3/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:34:08.340155 openrlbenchmark-0.2.1a3/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     6147 2023-06-07 19:47:32.024056 openrlbenchmark-0.2.1a3/openrlbenchmark/capped_hns.py
+-rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.1a3/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-05-23 20:34:08.340377 openrlbenchmark-0.2.1a3/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    37404 2023-06-16 13:19:06.422225 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    30367 2023-06-07 20:11:32.994334 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0    24994 2023-06-16 13:11:33.831627 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics.py
+-rw-r--r--   0        0        0    25030 2023-06-12 14:59:30.792810 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics_oai.py
+-rw-r--r--   0        0        0    36919 2023-06-07 20:07:01.541242 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl.py
+-rw-r--r--   0        0        0    25177 2023-06-07 20:11:32.986812 openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl_multi_metrics.py
+-rw-r--r--   0        0        0      748 2023-06-16 13:19:35.534932 openrlbenchmark-0.2.1a3/pyproject.toml
+-rw-r--r--   0        0        0    21316 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.1a3/PKG-INFO
```

### Comparing `openrlbenchmark-0.2.1a2/LICENSE` & `openrlbenchmark-0.2.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/README.md` & `openrlbenchmark-0.2.1a3/README.md`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/cache.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/cache.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/cache_legacy.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/cache_legacy.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/capped_hns.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/capped_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/hns.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/offline_db.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/offline_db.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 @dataclass
 class Args:
     filters: tyro.conf.UseAppendAction[List[List[str]]]
     """the filters of the experiments; see docs"""
     env_ids: tyro.conf.UseAppendAction[List[List[str]]]
     """the ids of the environment to compare"""
-    output_filename: str = "compare"
+    output_filename: str = "static/0compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
     check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
@@ -141,18 +141,18 @@
         self.offline_db = offline_db
         self.offline = offline
 
         user = [{"username": self.username}] if self.username else []
         include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
         self.wandb_filters = {
             "$and": [
-                {f"config.{self.custom_env_id_key}.value": self.env_id},
+                {f"config.trl_ppo_trainer_config.value.{self.custom_env_id_key}": self.env_id},
                 *include_tag_groups,
                 *user,
-                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
+                {f"config.trl_ppo_trainer_config.value.{self.custom_exp_name_key}": self.exp_name},
             ]
         }
 
     @property
     def runs(self):
         if not self.offline:
             return wandb.Api().runs(
@@ -236,14 +236,16 @@
             run_df = run.run_df
         else:
             run_df = run.history(samples=1500)
         if "videos" in run_df:
             run_df = run_df.drop(columns=["videos"], axis=1)
         if len(runset.metric) > 0:
             run_df["charts/episodic_return"] = run_df[runset.metric]
+        if "global_step" not in run_df:
+            run_df["global_step"] = run_df["_step"]
         cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
         runs += [Run(f"seed{idx}", cleaned_df)]
     return Hypothesis(runset.name, runs)
 
 
 def compare(
     console: Console,
@@ -386,15 +388,15 @@
         ax_time.set_xlabel("")
         ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    if len(os.path.dirname(output_filename)) > 0:
+    if os.path.dirname(output_filename) != "":
         os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
```

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_hns.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_multi_metrics.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_multi_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,14 +567,15 @@
                         offline=args.offline,
                     )
                 )
                 if args.check_empty_runs:
                     console.print(f"{exp_name} [green]({query})[/] in [purple]{env_id}[/] has {len(runsets[-1].runs)} runs")
                     for run in runsets[-1].runs:
                         console.print(f"┣━━ [link={run.url}]{run.name}[/link] with tags = {run.tags}")
+                    print(runsets[0].wandb_filters)
                     assert len(runsets[0].runs) > 0, f"{exp_name} ({query}) in {env_id} has no runs"
             runsetss.append(runsets)
 
     blocks, runtimes, global_steps, exs = compare(
         console,
         runsetss,
         args.env_ids[0],
```

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 @dataclass
 class Args:
     filters: tyro.conf.UseAppendAction[List[List[str]]]
     """the filters of the experiments; see docs"""
     env_ids: tyro.conf.UseAppendAction[List[List[str]]]
     """the ids of the environment to compare"""
-    output_filename: str = "static/0compare"
+    output_filename: str = "compare"
     """the output filename of the plot, without extension"""
     metric_last_n_average_window: int = 100
     """the last n number of episodes to average metric over in the result table"""
     scan_history: bool = False
     """if toggled, we will pull the complete metrics from wandb instead of sampling 500 data points (recommended for generating tables)"""
     check_empty_runs: bool = True
     """if toggled, we will check for empty wandb runs"""
@@ -113,14 +113,15 @@
         self,
         name: str,
         entity: str,
         project: str,
         metric: str = "charts/episodic_return",
         groupby: str = "",
         custom_exp_name_key: str = "exp_name",
+        custom_xaxis_key: str = "global_step",
         exp_name: str = "",
         custom_env_id_key: str = "env_id",
         env_id: str = "",
         tags: List[str] = [],
         username: str = "",
         color: str = "#000000",
         offline_db: pw.Database = None,
@@ -128,31 +129,32 @@
     ):
         self.name = name
         self.entity = entity
         self.project = project
         self.metric = metric
         self.groupby = groupby
         self.custom_exp_name_key = custom_exp_name_key
+        self.custom_xaxis_key = custom_xaxis_key
         self.exp_name = exp_name
         self.custom_env_id_key = custom_env_id_key
         self.env_id = env_id
         self.color = color
         self.tags = tags
         self.username = username
         self.offline_db = offline_db
         self.offline = offline
 
         user = [{"username": self.username}] if self.username else []
         include_tag_groups = [{"tags": {"$in": [tag]}} for tag in self.tags] if len(self.tags) > 0 else []
         self.wandb_filters = {
             "$and": [
-                {f"config.trl_ppo_trainer_config.value.{self.custom_env_id_key}": self.env_id},
+                {f"config.{self.custom_env_id_key}.value": self.env_id},
                 *include_tag_groups,
                 *user,
-                {f"config.trl_ppo_trainer_config.value.{self.custom_exp_name_key}": self.exp_name},
+                {f"config.{self.custom_exp_name_key}.value": self.exp_name},
             ]
         }
 
     @property
     def runs(self):
         if not self.offline:
             return wandb.Api().runs(
@@ -200,15 +202,15 @@
     console.print(table)
 
 
 def create_hypothesis(runset: Runset, scan_history: bool = False) -> Hypothesis:
     runs = []
     for idx, run in enumerate(runset.runs):
         print("loading", run, run.url)
-        if run.state == "running":
+        if run.state == "running" or run.state == "crashed":
             print(f"Skipping running run: {run}")
             continue
         if scan_history:
             run = openrlbenchmark.cache.CachedRun(run, cache_dir=os.path.join(openrlbenchmark.__path__[0], "dataset"))
             with runset.offline_db.bind_ctx([OfflineRun, OfflineRunTag, Tag]):
                 tags = []
                 for tag_str in run.run.tags:
@@ -234,18 +236,21 @@
                 )
                 offline_run.save()
             run_df = run.run_df
         else:
             run_df = run.history(samples=1500)
         if "videos" in run_df:
             run_df = run_df.drop(columns=["videos"], axis=1)
+        if runset.custom_xaxis_key in run_df:
+            run_df["global_step"] = run_df[runset.custom_xaxis_key]
+        if runset.metric not in run_df:
+            print(f"Skipping run {run} because metric {runset.metric} not found")
+            continue
         if len(runset.metric) > 0:
             run_df["charts/episodic_return"] = run_df[runset.metric]
-        if "global_step" not in run_df:
-            run_df["global_step"] = run_df["_step"]
         cleaned_df = run_df[["global_step", "_runtime", "charts/episodic_return"]].dropna()
         runs += [Run(f"seed{idx}", cleaned_df)]
     return Hypothesis(runset.name, runs)
 
 
 def compare(
     console: Console,
@@ -388,15 +393,15 @@
         ax_time.set_xlabel("")
         ax_time.set_ylabel("")
     runtimes = pd.DataFrame(np.array(runtimes), index=env_ids, columns=list(ex.summary()["name"]))
     global_steps = pd.DataFrame(np.array(global_steps), index=env_ids, columns=list(ex.summary()["name"]))
     print_rich_table(f"Runtime ({pc.time_unit}) (mean ± std)", runtimes.rename_axis("Environment").reset_index(), console)
 
     # create the required directory for `output_filename`
-    if os.path.dirname(output_filename) != "":
+    if len(os.path.dirname(output_filename)) > 0:
         os.makedirs(os.path.dirname(output_filename), exist_ok=True)
     print_rich_table(f"{pc.ylabel} (mean ± std)", result_table.rename_axis("Environment").reset_index(), console)
     result_table.to_markdown(open(f"{output_filename}.md", "w"))
     result_table.to_csv(open(f"{output_filename}.csv", "w"))
     runtimes.to_markdown(open(f"{output_filename}_runtimes.md", "w"))
     runtimes.to_csv(open(f"{output_filename}_runtimes.csv", "w"))
     average_runtime = pd.DataFrame(runtimes.mean(axis=0)).reset_index()
@@ -491,20 +496,22 @@
         parse_result = urlparse(filters[0])
         query = parse_qs(parse_result.query)
         metric = query["metric"][0] if "metric" in query else "charts/episodic_return"
         wandb_project_name = query["wpn"][0] if "wpn" in query else args.wandb_project_name
         wandb_entity = query["we"][0] if "we" in query else args.wandb_entity
         custom_env_id_key = query["ceik"][0] if "ceik" in query else "env_id"
         custom_exp_name_key = query["cen"][0] if "cen" in query else "exp_name"
+        custom_xaxis_key = query["xaxis"][0] if "xaxis" in query else "global_step"
         pprint(
             {
                 "wandb_project_name": wandb_project_name,
                 "wandb_entity": wandb_entity,
                 "custom_env_id_key": custom_env_id_key,
                 "custom_exp_name_key": custom_exp_name_key,
+                "custom_xaxis_key": custom_xaxis_key,
                 "metric": metric,
             },
             expand_all=True,
         )
         if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
             offline_db_folder = os.path.join(openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}")
             offline_db_path = os.path.join(offline_db_folder, "offline.sqlite")
@@ -536,28 +543,30 @@
                         if custom_legend == ""
                         else custom_legend,
                         entity=wandb_entity,
                         project=wandb_project_name,
                         metric=metric,
                         groupby=custom_exp_name_key,
                         custom_exp_name_key=custom_exp_name_key,
+                        custom_xaxis_key=custom_xaxis_key,
                         exp_name=exp_name,
                         custom_env_id_key=custom_env_id_key,
                         env_id=env_id,
                         tags=tags,
                         username=username,
                         color=color,
                         offline_db=offline_dbs[f"{wandb_entity}/{wandb_project_name}"],
                         offline=args.offline,
                     )
                 )
                 if args.check_empty_runs:
                     console.print(f"{exp_name} [green]({query})[/] in [purple]{env_id}[/] has {len(runsets[-1].runs)} runs")
                     for run in runsets[-1].runs:
                         console.print(f"┣━━ [link={run.url}]{run.name}[/link] with tags = {run.tags}")
+                    print(runsets[0].wandb_filters)
                     assert len(runsets[0].runs) > 0, f"{exp_name} ({query}) in {env_id} has no runs"
             runsetss.append(runsets)
 
     blocks, runtimes, global_steps, exs = compare(
         console,
         runsetss,
         args.env_ids[0],
```

### Comparing `openrlbenchmark-0.2.1a2/openrlbenchmark/rlops_trl_multi_metrics.py` & `openrlbenchmark-0.2.1a3/openrlbenchmark/rlops_trl_multi_metrics.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.1a2/pyproject.toml` & `openrlbenchmark-0.2.1a3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.2.1a2"
+version = "0.2.1a3"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "openrlbenchmark" },
 ]
```

### Comparing `openrlbenchmark-0.2.1a2/PKG-INFO` & `openrlbenchmark-0.2.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrlbenchmark
-Version: 0.2.1a2
+Version: 0.2.1a3
 Summary: 
 Author: Costa Huang
 Author-email: costa.huang@outlook.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

