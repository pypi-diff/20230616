# Comparing `tmp/ssg-sea-1.5.3.tar.gz` & `tmp/ssg-sea-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssg-sea-1.5.3.tar", last modified: Thu Feb  2 17:07:29 2023, max compression
+gzip compressed data, was "ssg-sea-1.6.0.tar", last modified: Fri Jun 16 07:37:33 2023, max compression
```

## Comparing `ssg-sea-1.5.3.tar` & `ssg-sea-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.413694 ssg-sea-1.5.3/
--rw-r--r--   0 loisji     (501) staff       (20)      281 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/MANIFEST.in
--rw-r--r--   0 loisji     (501) staff       (20)      921 2023-02-02 17:07:29.413522 ssg-sea-1.5.3/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)     2197 2023-02-02 16:59:29.000000 ssg-sea-1.5.3/README.md
--rw-r--r--   0 loisji     (501) staff       (20)     1941 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/pyproject.toml
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.408320 ssg-sea-1.5.3/requirements/
--rw-r--r--   0 loisji     (501) staff       (20)       71 2023-02-02 17:07:11.000000 ssg-sea-1.5.3/requirements/requirements.txt
--rw-r--r--   0 loisji     (501) staff       (20)       38 2023-02-02 17:07:29.413745 ssg-sea-1.5.3/setup.cfg
--rw-r--r--   0 loisji     (501) staff       (20)     2248 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/setup.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.409651 ssg-sea-1.5.3/ssg_sea/
--rw-r--r--   0 loisji     (501) staff       (20)        5 2023-02-02 16:42:48.000000 ssg-sea-1.5.3/ssg_sea/VERSION
--rw-r--r--   0 loisji     (501) staff       (20)      144 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/ssg_sea/__init__.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.411255 ssg-sea-1.5.3/ssg_sea/config/
--rw-r--r--   0 loisji     (501) staff       (20)        0 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/ssg_sea/config/__init__.py
--rw-r--r--   0 loisji     (501) staff       (20)      488 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/ssg_sea/config/core.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.411561 ssg-sea-1.5.3/ssg_sea/data/
--rw-r--r--   0 loisji     (501) staff       (20)   964604 2023-02-02 16:57:32.000000 ssg-sea-1.5.3/ssg_sea/data/pickle.pkl
--rw-r--r--   0 loisji     (501) staff       (20)     6928 2023-01-09 04:46:54.000000 ssg-sea-1.5.3/ssg_sea/extract_skills.py
--rw-r--r--   0 loisji     (501) staff       (20)      164 2023-02-02 17:00:23.000000 ssg-sea-1.5.3/ssg_sea/params.yaml
--rw-r--r--   0 loisji     (501) staff       (20)     6710 2022-11-07 02:29:25.000000 ssg-sea-1.5.3/ssg_sea/utils.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-02-02 17:07:29.410847 ssg-sea-1.5.3/ssg_sea.egg-info/
--rw-r--r--   0 loisji     (501) staff       (20)      921 2023-02-02 17:07:29.000000 ssg-sea-1.5.3/ssg_sea.egg-info/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      404 2023-02-02 17:07:29.000000 ssg-sea-1.5.3/ssg_sea.egg-info/SOURCES.txt
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-02-02 17:07:29.000000 ssg-sea-1.5.3/ssg_sea.egg-info/dependency_links.txt
--rw-r--r--   0 loisji     (501) staff       (20)       71 2023-02-02 17:07:29.000000 ssg-sea-1.5.3/ssg_sea.egg-info/requires.txt
--rw-r--r--   0 loisji     (501) staff       (20)        8 2023-02-02 17:07:29.000000 ssg-sea-1.5.3/ssg_sea.egg-info/top_level.txt
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.633572 ssg-sea-1.6.0/
+-rw-r--r--   0 loisji     (501) staff       (20)      281 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/MANIFEST.in
+-rw-r--r--   0 loisji     (501) staff       (20)      921 2023-06-16 07:37:33.633363 ssg-sea-1.6.0/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)     2197 2023-02-02 16:59:29.000000 ssg-sea-1.6.0/README.md
+-rw-r--r--   0 loisji     (501) staff       (20)     1941 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/pyproject.toml
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.628001 ssg-sea-1.6.0/requirements/
+-rw-r--r--   0 loisji     (501) staff       (20)       66 2023-06-16 07:36:36.000000 ssg-sea-1.6.0/requirements/requirements.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       38 2023-06-16 07:37:33.633633 ssg-sea-1.6.0/setup.cfg
+-rw-r--r--   0 loisji     (501) staff       (20)     2248 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/setup.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.629222 ssg-sea-1.6.0/ssg_sea/
+-rw-r--r--   0 loisji     (501) staff       (20)        5 2023-06-16 07:17:20.000000 ssg-sea-1.6.0/ssg_sea/VERSION
+-rw-r--r--   0 loisji     (501) staff       (20)      144 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/ssg_sea/__init__.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.630882 ssg-sea-1.6.0/ssg_sea/config/
+-rw-r--r--   0 loisji     (501) staff       (20)        0 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/ssg_sea/config/__init__.py
+-rw-r--r--   0 loisji     (501) staff       (20)      488 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/ssg_sea/config/core.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.631108 ssg-sea-1.6.0/ssg_sea/data/
+-rw-r--r--   0 loisji     (501) staff       (20)   964604 2023-02-02 16:57:32.000000 ssg-sea-1.6.0/ssg_sea/data/pickle.pkl
+-rw-r--r--   0 loisji     (501) staff       (20)     8029 2023-06-16 07:12:36.000000 ssg-sea-1.6.0/ssg_sea/extract_skills.py
+-rw-r--r--   0 loisji     (501) staff       (20)      164 2023-06-16 07:17:12.000000 ssg-sea-1.6.0/ssg_sea/params.yaml
+-rw-r--r--   0 loisji     (501) staff       (20)     6952 2023-06-16 06:55:44.000000 ssg-sea-1.6.0/ssg_sea/utils.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.630480 ssg-sea-1.6.0/ssg_sea.egg-info/
+-rw-r--r--   0 loisji     (501) staff       (20)      921 2023-06-16 07:37:33.000000 ssg-sea-1.6.0/ssg_sea.egg-info/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      468 2023-06-16 07:37:33.000000 ssg-sea-1.6.0/ssg_sea.egg-info/SOURCES.txt
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-06-16 07:37:33.000000 ssg-sea-1.6.0/ssg_sea.egg-info/dependency_links.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       66 2023-06-16 07:37:33.000000 ssg-sea-1.6.0/ssg_sea.egg-info/requires.txt
+-rw-r--r--   0 loisji     (501) staff       (20)        8 2023-06-16 07:37:33.000000 ssg-sea-1.6.0/ssg_sea.egg-info/top_level.txt
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-06-16 07:37:33.632294 ssg-sea-1.6.0/tests/
+-rw-r--r--   0 loisji     (501) staff       (20)      649 2023-06-16 07:12:18.000000 ssg-sea-1.6.0/tests/test_batch_extract_skills.py
+-rw-r--r--   0 loisji     (501) staff       (20)      656 2022-11-07 02:29:25.000000 ssg-sea-1.6.0/tests/test_extract_skills.py
```

### Comparing `ssg-sea-1.5.3/PKG-INFO` & `ssg-sea-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-sea
-Version: 1.5.3
+Version: 1.6.0
 Summary: Skills Extraction Algorithm to extract skills from free text based on Singapore Skills Taxonomy (SST)
 Home-page: https://github.com/ssg-leo/SSG-SEA/
 Author: LeoLi
 Author-email: leo_li@ssg.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-sea-1.5.3/README.md` & `ssg-sea-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ssg-sea-1.5.3/pyproject.toml` & `ssg-sea-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ssg-sea-1.5.3/setup.py` & `ssg-sea-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `ssg-sea-1.5.3/ssg_sea/data/pickle.pkl` & `ssg-sea-1.6.0/ssg_sea/data/pickle.pkl`

 * *Files identical despite different names*

### Comparing `ssg-sea-1.5.3/ssg_sea/extract_skills.py` & `ssg-sea-1.6.0/ssg_sea/extract_skills.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,36 +64,34 @@
 
     tsc_list = extractTSC(context_list=context_list, stem_list=stem_list,
                           skill_to_context_dict=skillToContextDict, stem_to_skill_dict=stemToSkillDict,
                           skill_indpt_context_set=skillSetIndptContext)
     app_list = extractAPP(app_word_list)
     ccs_list = extractCCS(ccs_word_list)
 
-    tsc_output = getSkillWeight(skillExtractionList=tsc_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillForm="TSC")
-    app_output = getSkillWeight(skillExtractionList=app_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillForm="App/Tools")
-    ccs_output = getSkillWeight(skillExtractionList=ccs_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillForm="CCS")
+    tsc_output = getSkillWeight(skillExtractionList=tsc_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillType="TSC")
+    app_output = getSkillWeight(skillExtractionList=app_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillType="App/Tools")
+    ccs_output = getSkillWeight(skillExtractionList=ccs_list, id_mapping_dict=skill_to_id_mapping_dict, sfs_mapping_dict=skill_to_sfs_mapping_dict, skillType="CCS")
 
     output_list = tsc_output + ccs_output + app_output
 
     results = {}
     _list = []
     keys = range(len(output_list))
 
     for tuple in output_list:
-        extractDict = {
-            "skill_sea_id": tuple[0],
+        results[tuple[0]] = {
             "skill_title": tuple[1],
-            "skill_weight": tuple[2],
             "skill_type": tuple[3],
-            "skill_label": tuple[4]
+            "skill_source": "sfw", # Default to "sfw" for SEA v1
+            "proficiency_lvl": "Not Applicable",
+            "confidence_score": 1.0, # Default value of 1.0 for rule-based version
+            "skill_occurrence": tuple[2], # Change to reflect absolute skills count
+            "skill_tags": tuple[4], # Change to skill_tag as a list
         }
-        _list.append(extractDict)
-
-    for i in keys:
-        results[i] = _list[i]
 
     if len(results) == 0:
         output = {}
     else:
         output = {
             "extractions": results
         }
@@ -117,46 +115,66 @@
         df['text_id'] = df[id_col]
     
     text_id_ls = []
     input_text_ls = []
     skill_id_ls = []
     skill_title_ls = []
     skill_type_ls = []
-    skill_weight_ls = []
+    skill_source_ls = []
+    skill_proficiency_lvl_ls = []
+    confidence_score_ls = []
+    skill_occurrence_ls = []
+    skill_tags_ls = []
     for j in tqdm(range(df.shape[0])):
         text = df.input_text[j]
         _id = df.text_id[j]
         skill_json = extract_skills(text=text)
         if len(skill_json) > 0:
-            for i in range(len(skill_json['extractions'])):
-                skill_id = skill_json['extractions'][i]['skill_sea_id']
-                skill_title = skill_json['extractions'][i]['skill_title']
-                skill_type = skill_json['extractions'][i]['skill_type']
-                skill_weight = skill_json['extractions'][i]['skill_weight']
+            for key, val in skill_json['extractions'].items():
+                skill_id = key
+                skill_title = val['skill_title']
+                skill_type = val['skill_type']
+                skill_source = val['skill_source']
+                skill_proficiency_lvl = val['proficiency_lvl']
+                skill_confidence_score = val['confidence_score']
+                skill_occurrence = val['skill_occurrence']
+                skill_tags = val['skill_tags']
                 text_id_ls.append(_id)
                 input_text_ls.append(text)
                 skill_id_ls.append(skill_id)
                 skill_title_ls.append(skill_title)
                 skill_type_ls.append(skill_type)
-                skill_weight_ls.append(skill_weight)
+                skill_source_ls.append(skill_source)
+                skill_proficiency_lvl_ls.append(skill_proficiency_lvl)
+                confidence_score_ls.append(skill_confidence_score)
+                skill_occurrence_ls.append(skill_occurrence)
+                skill_tags_ls.append(skill_tags)
         else:
             text_id_ls.append(_id)
             input_text_ls.append(text)
             skill_id_ls.append("no skill extracted")
             skill_title_ls.append("no skill extracted")
             skill_type_ls.append("no skill extracted")
-            skill_weight_ls.append("no skill extracted")
+            skill_source_ls.append("no skill extracted")
+            skill_proficiency_lvl_ls.append("no skill extracted")
+            confidence_score_ls.append("no skill extracted")
+            skill_occurrence_ls.append("no skill extracted")
+            skill_tags_ls.append("no skill extracted")
     
     output_df = pd.DataFrame(None)
     output_df['text_id'] = text_id_ls
     output_df['skill_id'] = skill_id_ls
     output_df['input_text'] = input_text_ls
     output_df['skill_title'] = skill_title_ls
     output_df['skill_type'] = skill_type_ls
-    output_df['skill_weight'] = skill_weight_ls
+    output_df['skill_source'] = skill_source_ls
+    output_df['skill_prof_lvl'] = skill_proficiency_lvl_ls
+    output_df['confidence_score'] = confidence_score_ls
+    output_df['skill_occurrence'] = skill_occurrence_ls
+    output_df['skill_tags'] = skill_tags_ls
 
     return output_df
 
     # # JSON output format for skills grouped by skill types
     # output = {}
     # for _id, text in zip(df.text_id, df.input_text):
     #     skill_json = extract_skills(text=text)
```

### Comparing `ssg-sea-1.5.3/ssg_sea/utils.py` & `ssg-sea-1.6.0/ssg_sea/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,21 @@
         for askill in flashRes:
             skillFreq = flashRes.count(askill)
             extracts += [askill] * skillFreq
 
     return extracts
 
 
-def getSkillWeight(skillExtractionList, id_mapping_dict, sfs_mapping_dict, skillForm):
+def getSkillWeight(skillExtractionList, id_mapping_dict, sfs_mapping_dict, skillType):
     """
     output skills weight and skills form from the extracted skills list
     :param skillExtractionList: list of the skills from the skills extraction process
-    :param skillForm: type of skills; TSC or Apps and Tools or CCS
+    :param id_mapping_dict: dictionary of skills to skill_id mapping
+    :param sfs_mapping_dict: dictionary of skills labels; SFS Emerging or Green etc.
+    :param skillType: type of skills; TSC or Apps and Tools or CCS
     :return:
         output_list: list of skills output with weight and skills form
     """
     skillIdList = []
     skillList = []
     skillWeightList = []
     skillLabelList = []
@@ -90,27 +92,28 @@
     for askill in skillExtractionList:
         freq = askill.count(askill)
         if askill not in skillFreqDict:
             skillFreqDict[askill] = int()
         skillFreqDict[askill] += freq
     odict = dict(sorted(skillFreqDict.items(), key=lambda item: item[1], reverse=True))
     for askill, afreq in odict.items():
-        wtAvg = sum(odict.values()) / len(odict)
-        aWeight = np.round(((odict[askill]) / wtAvg), 3)
+        # wtAvg = sum(odict.values()) / len(odict)
+        # aWeight = np.round(((odict[askill]) / wtAvg), 3) # Using absolute skill count instead
+        aWeight = int(afreq)
         aSkillId = id_mapping_dict.get(askill.lower().strip())[0]
-        aSkillLabel = sfs_mapping_dict.get(askill.lower().strip())[0]
+        aSkillLabel = sfs_mapping_dict.get(askill.lower().strip()) #[0], will be a list
 
         skillIdList += [aSkillId]
         skillList += [askill]
         skillWeightList += [aWeight]
         skillLabelList += [aSkillLabel]
 
     output_list = []
     for i in range(len(skillList)):
-        output_with_weight = (skillIdList[i], skillList[i], skillWeightList[i], skillForm, skillLabelList[i])
+        output_with_weight = (skillIdList[i], skillList[i], skillWeightList[i], skillType, skillLabelList[i])
         output_list.append(output_with_weight)
 
     return output_list
 
 
 def extractTSC(context_list, stem_list, skill_to_context_dict, stem_to_skill_dict, skill_indpt_context_set):
     """
```

### Comparing `ssg-sea-1.5.3/ssg_sea.egg-info/PKG-INFO` & `ssg-sea-1.6.0/ssg_sea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-sea
-Version: 1.5.3
+Version: 1.6.0
 Summary: Skills Extraction Algorithm to extract skills from free text based on Singapore Skills Taxonomy (SST)
 Home-page: https://github.com/ssg-leo/SSG-SEA/
 Author: LeoLi
 Author-email: leo_li@ssg.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

