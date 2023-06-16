# Comparing `tmp/text2story-1.3.3.tar.gz` & `tmp/text2story-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.3.3.tar", last modified: Tue Jun 13 08:51:36 2023, max compression
+gzip compressed data, was "text2story-1.3.4.tar", last modified: Fri Jun 16 13:04:49 2023, max compression
```

## Comparing `text2story-1.3.3.tar` & `text2story-1.3.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.3.3/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.3.3/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-13 08:51:36.299235 text2story-1.3.3/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7752 2023-05-30 12:31:10.000000 text2story-1.3.3/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2023-06-13 08:51:26.000000 text2story-1.3.3/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      989 2023-06-13 08:51:36.299235 text2story-1.3.3/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-26 15:16:02.000000 text2story-1.3.3/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.291232 text2story-1.3.3/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.291232 text2story-1.3.3/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.291232 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/ALLENNLP/cache/
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)     4090 2021-03-09 07:42:06.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/cache/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1553 2023-05-29 13:21:32.000000 text2story-1.3.3/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4406 2023-05-25 14:12:26.000000 text2story-1.3.3/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.3.3/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.3.3/text2story/annotators/SRLWeakLabeling/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.3.3/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-05-30 10:06:48.000000 text2story-1.3.3/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.3.3/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9846 2023-06-12 14:58:33.000000 text2story-1.3.3/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.295234 text2story-1.3.3/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.3.3/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.3.3/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2917 2023-06-12 15:28:35.000000 text2story-1.3.3/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      709 2023-06-09 13:29:38.000000 text2story-1.3.3/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2621 2023-06-09 14:35:24.000000 text2story-1.3.3/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23443 2023-06-13 08:51:06.000000 text2story-1.3.3/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6935 2023-06-09 15:00:43.000000 text2story-1.3.3/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.3.3/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/exp.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/exp_en_fn.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/exp_en_pb.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2870 2023-05-29 11:37:16.000000 text2story-1.3.3/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.3.3/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22827 2023-06-07 13:53:21.000000 text2story-1.3.3/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.3.3/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.3.3/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.3.3/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.3.3/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.3.3/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.3.3/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.3.3/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.3.3/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.299235 text2story-1.3.3/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.3.3/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-06-01 12:14:40.000000 text2story-1.3.3/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-13 08:51:36.291232 text2story-1.3.3/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-13 08:51:36.000000 text2story-1.3.3/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2885 2023-06-13 08:51:36.000000 text2story-1.3.3/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-06-13 08:51:36.000000 text2story-1.3.3/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      454 2023-06-13 08:51:36.000000 text2story-1.3.3/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-06-13 08:51:36.000000 text2story-1.3.3/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.3.3/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.344429 text2story-1.3.4/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.3.4/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.3.4/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9576 2023-06-16 13:04:49.344429 text2story-1.3.4/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9395 2023-06-16 13:04:37.000000 text2story-1.3.4/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2023-06-16 13:04:37.000000 text2story-1.3.4/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      989 2023-06-16 13:04:49.344429 text2story-1.3.4/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-26 15:16:02.000000 text2story-1.3.4/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.316429 text2story-1.3.4/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.320429 text2story-1.3.4/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.320429 text2story-1.3.4/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.312429 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.320429 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.324429 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.324429 text2story-1.3.4/text2story/annotators/ALLENNLP/cache/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)     4090 2021-03-09 07:42:06.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/cache/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1553 2023-05-29 13:21:32.000000 text2story-1.3.4/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4406 2023-05-25 14:12:26.000000 text2story-1.3.4/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.3.4/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.3.4/text2story/annotators/SRLWeakLabeling/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2424 2023-06-14 15:02:41.000000 text2story-1.3.4/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.328429 text2story-1.3.4/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-05-30 10:06:48.000000 text2story-1.3.4/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.332429 text2story-1.3.4/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.3.4/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9846 2023-06-12 14:58:33.000000 text2story-1.3.4/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.336429 text2story-1.3.4/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.3.4/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.3.4/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2917 2023-06-12 15:28:35.000000 text2story-1.3.4/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      709 2023-06-09 13:29:38.000000 text2story-1.3.4/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2621 2023-06-09 14:35:24.000000 text2story-1.3.4/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23459 2023-06-13 10:26:18.000000 text2story-1.3.4/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6935 2023-06-09 15:00:43.000000 text2story-1.3.4/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.336429 text2story-1.3.4/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.3.4/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16496 2023-06-14 09:45:23.000000 text2story-1.3.4/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14456 2023-06-14 11:43:28.000000 text2story-1.3.4/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1278 2023-06-13 09:44:33.000000 text2story-1.3.4/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3506 2023-06-15 11:08:35.000000 text2story-1.3.4/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.340429 text2story-1.3.4/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.3.4/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23394 2023-06-15 10:56:57.000000 text2story-1.3.4/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.3.4/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.344429 text2story-1.3.4/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.3.4/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.3.4/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.3.4/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.3.4/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.344429 text2story-1.3.4/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.3.4/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.344429 text2story-1.3.4/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.3.4/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.3.4/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.344429 text2story-1.3.4/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.3.4/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-06-01 12:14:40.000000 text2story-1.3.4/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-16 13:04:49.320429 text2story-1.3.4/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9576 2023-06-16 13:04:49.000000 text2story-1.3.4/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2885 2023-06-16 13:04:49.000000 text2story-1.3.4/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-06-16 13:04:49.000000 text2story-1.3.4/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      454 2023-06-16 13:04:49.000000 text2story-1.3.4/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-06-16 13:04:49.000000 text2story-1.3.4/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.3.4/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.3.3/LICENSE` & `text2story-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/setup.cfg` & `text2story-1.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = text2story
-version = 1.3.3
+version = 1.3.4
 project_urls = 
 	Source =  https://github.com/LIAAD/Text2StoryPackage
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
```

### Comparing `text2story-1.3.3/text2story/__init__.py` & `text2story-1.3.4/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.3.4/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.3.4/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.3.4/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/cache/config.json` & `text2story-1.3.4/text2story/annotators/ALLENNLP/cache/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.3.4/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.3.4/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.3.4/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.3.4/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.3.4/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.3.4/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.3.4/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/NLTK/__init__.py` & `text2story-1.3.4/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.3.4/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/SPACY/__init__.py` & `text2story-1.3.4/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.3.4/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.3.4/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/annotators/__init__.py` & `text2story-1.3.4/text2story/annotators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,24 @@
 def get_srlink_tools():
     return SEMANTIC_ROLE_LABELLING_TOOLS
 
 def extract_actors(tool, lang, text):
 
     if tool == 'spacy':
         return SPACY.extract_actors(lang, text)
-    elif tool == 'nltk':
+    elif tool == 'nltk' and lang == "en":
         return NLTK.extract_actors(lang, text)
     elif tool == 'allennlp':
         return ALLENNLP.extract_actors(lang, text)
     elif tool == 'srlweaklabeling':
         return SRLWeakLabeling.extract_actors(lang, text)
     #elif tool == 'sparknlp':
     #    return SPARKNLP.extract_actors(lang, text)
-
-    raise InvalidTool
+    else:
+        raise InvalidTool
 
 
 def extract_times(tool, lang, text, publication_time):
     if tool == 'py_heideltime':
         return PY_HEIDELTIME.extract_times(lang, text, publication_time)
 
     raise InvalidTool
```

### Comparing `text2story-1.3.3/text2story/brat2viz/README.md` & `text2story-1.3.4/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.3.4/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.3.4/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/brat2viz/drs2viz/app.py` & `text2story-1.3.4/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.3.4/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.3.4/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/core/annotator.py` & `text2story-1.3.4/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/core/entity_structures.py` & `text2story-1.3.4/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/core/exceptions.py` & `text2story-1.3.4/text2story/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/core/link_structures.py` & `text2story-1.3.4/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/core/narrative.py` & `text2story-1.3.4/text2story/core/narrative.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.actors = {}
         self.times = {}
         self.events = {}
         self.spatial_relations = {}
 
         self.links = {}
 
-        self.sem_role_map = {"participant":"agent"}
+        self.sem_role_map = {"participant":"agent","event":"cause"}
         #self.obj_links = {}
         #self.sem_links = {}
 
         #self.temp_links = {}
         #self.subordination_links = {}
         #self.qualitative_spatial_links = {}
         #self.movement_links = {}
```

### Comparing `text2story-1.3.3/text2story/core/utils.py` & `text2story-1.3.4/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/experiments/evaluation.py` & `text2story-1.3.4/text2story/experiments/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     ann_target = reader.read_annotation_file(target_file)
 
     # compute accuracy of the exacttly same span
     event_pred = ann_pred["Event"]
     event_target = ann_target["Event"]
 
     scores_relax = compute_relax_scores("event",event_pred, event_target)
-    scores = compute_strict_scores(event_pred, event_target)
+    scores = compute_strict_scores("event",event_pred, event_target)
     return scores_relax, scores
 
 
 def evaluate_actor(pred_file, target_file):
     """
     Implements token actor precision/recall/f1 and span actor precision/recall/f1
 
@@ -231,15 +231,15 @@
     # compute accuracy of the exacttly same span
     time_pred = ann_pred["Time"]
     if len(time_pred) == 0:
         time_pred = ann_pred["TIME_X3"]
     time_target = ann_target["Time"]
 
     scores_relax = compute_relax_scores("time",time_pred, time_target)
-    scores = compute_strict_scores(time_pred, time_target)
+    scores = compute_strict_scores("time",time_pred, time_target)
     return scores_relax, scores
 
 def evaluate_srlink(pred_file, target_file):
     """
     Implements token srlink precision/recall/f1 and span time precision/recall/f1
 
     @param string: predict file in the brat .ann format
@@ -257,30 +257,29 @@
     pred, target = get_element("srlink",ann_pred, ann_target)
 
 
     scores_relax = compute_relax_scores("srlink", pred, target)
     scores = compute_strict_scores("srlink", pred, target)
     return scores_relax, scores
 
-def prediction(input_dir, results_dir, narrative_elements, language):
+def prediction(input_dir, results_dir, narrative_elements, language, split=None):
     """
     Read brat data (.ann and .txt files) in the input directory,
     and write the results (columns files: token, pred_label, target_label)
     in the results dir
 
     @param string: input directory with ann and txt files
     @param string: directory with results file for each document file in
     the input_dir
 
     @return [(string,string)]: a tuple file list to compare
     """
 
     reader = read_brat.ReadBrat()
-
-    doc_lst = reader.process(input_dir)
+    doc_lst = reader.process(input_dir, split)
 
     doc_pred_target = []  #
 
     for idx_doc, doc in enumerate(doc_lst):
         text_ = ""
         with open(reader.file_lst[idx_doc], "r") as fd:
             text_ = fd.read()
@@ -304,15 +303,15 @@
         target_file = os.path.join(input_dir, target_file)
 
         doc_pred_target.append((ann_filename, target_file))
 
     return doc_pred_target
 
 
-def process_evaluation(narrative_elements, doc_lst, merge_entities=True):
+def process_evaluation(narrative_elements, doc_lst):
     """
     Process evaluation for a given element (time, actors or event), in a
     given tool (spacy, spacy, py_heideltime, custompt, etc).
 
     You should set DATA_DIR and RESULTS_DIR in your PATH enviroment
     vari
 
@@ -330,16 +329,16 @@
         for m in metrics:
             res[m + "_" + elem] = []
 
     for pred_file, target_file in doc_lst:
         print("Evaluating %s and %s" % (pred_file, target_file))
         reader = read_brat.ReadBrat()
 
-        ann_pred = reader.read_annotation_file(pred_file, merge_entities)
-        ann_target = reader.read_annotation_file(target_file, merge_entities)
+        ann_pred = reader.read_annotation_file(pred_file, merge_entities=True)
+        ann_target = reader.read_annotation_file(target_file, merge_entities=False)
 
         for elem in narrative_elements:
             pred, target = get_element(elem, ann_pred, ann_target)
 
             # TODO: esse e so para o srlink. Depois posso querer
             # fazer a divisao por tipos
             #if len(pred) > 0 and len(target) > 0 and \
@@ -367,28 +366,28 @@
                     time_str = now.strftime("%m/%d/%Y, %H:%M:%S")
                     fd_log.write( "[%s] <p>Error: %s</p>\n" % (time_str, e))
                 print("Warning: Some error computing score of %s file" % pred_file)
 
     return res
 
 
-def build_evaluation(narrative_elements, language, data_dir: str, results_dir: str):
+def build_evaluation(narrative_elements, language, data_dir: str, results_dir: str, split=None):
     """
     Process the evaluation of DATA_DIR (enviroment variable) and put
     the extracted elements in the RESULTS_DIR (enviroment variable)
 
     @param dict: A dictionary with the elements (actor, time, event) with the
     the tool list to be employed
     @param string: the language to be evaluated (pt or en)
     @param: The System Path where data is stored
     @parm: The System Path where results will be output
     @return None
     """
 
-    doc_pred_lst = prediction(data_dir, results_dir, narrative_elements, language)
+    doc_pred_lst = prediction(data_dir, results_dir, narrative_elements, language, split)
     return process_evaluation(narrative_elements, doc_pred_lst)
 
 
 
 def print_metrics_result(res: dict):
     print(f"\n-------Metrics Results-------")
```

### Comparing `text2story-1.3.3/text2story/experiments/exp_en_pb.json` & `text2story-1.3.4/text2story/experiments/exp_en_pb.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/experiments/metrics.py` & `text2story-1.3.4/text2story/experiments/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
 
     fn = 0  # false negative
     search_target = {}
     for target in ann_target:
         ans, id_ans = partial_search_annotation(target, interval_pred_lst)
         if ans == -1:
-            search_target[target["id"]] = id_ans
+            search_target[target["id"]] = None
         else:
             search_target[target["id"]] = id_ans
 
     return search_pred, search_target
 
 
 def compute_relax_scores_srlink(ann_pred, ann_target):
```

### Comparing `text2story-1.3.3/text2story/experiments/run_experiments.py` & `text2story-1.3.4/text2story/experiments/run_experiments.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 
         narrative_elements = {"participant":tools["participant"],\
                           "time":tools["time"],\
                           "event":tools["event"],\
                           "srlink":tools["srlink"]}
 
         data_dir = config_exp[name_experiment]["data"]
+        split_info = config_exp[name_experiment].get("split", None)
+
         res = build_evaluation(narrative_elements=narrative_elements, language=language, data_dir=data_dir,
-                           results_dir=name_experiment)
+                           results_dir=name_experiment,split=split_info)
 
         with open("%s_metrics.txt" % name_experiment, "w") as fd:
             write_metrics_result(res, fd)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `text2story-1.3.3/text2story/experiments/stats.py` & `text2story-1.3.4/text2story/experiments/stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,14 +37,36 @@
                         else:
                             attr_count[attr][attr_map[attr]] = 1
                     else:
                         attr_count[attr] = {attr_map[attr]:1}
 
     return attr_count, nelements
 
+def build_stats_byrelation(doc):
+    rel_stats = {}
+    rel_set = set()
+
+    for tok in doc:
+        for rel in tok.relations:
+            if rel.rel_id not in rel_set:
+
+                rel_type = rel.rel_type.split("_")
+                maintype = rel_type[0]
+                subtype = rel_type[1]
+
+                if maintype in rel_stats:
+                    if subtype in rel_stats[maintype]:
+                        rel_stats[maintype][subtype] += 1
+                    else:
+                        rel_stats[maintype][subtype] = 1
+                else:
+                    rel_stats[maintype] = {subtype:1}
+
+    return rel_stats
+
 def build_stats_byelement_batch(data_dir, element_type="event", dataset_type="BRAT"):
     """
 
     Count a given type element
 
     @param data_dir: A string of data directory
     @param dataset_type: default type assumes the BRAT standoff format
```

### Comparing `text2story-1.3.3/text2story/readers/pb-vn2.json` & `text2story-1.3.4/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/read.py` & `text2story-1.3.4/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/read_brat.py` & `text2story-1.3.4/text2story/readers/read_brat.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     def _is_adjacent(self, el1, el2):
         """
         Check if two annotation elements (dictionaries) are adjacent to each other
         1, if el1 < el2, -1, if el1 > el2, and 0 if el1 is not adjacent to el2
         """
 
-        if "offset2_start" in el1 and "offset2_start" in el2:
+        if "offset2" in el1 and "offset2" in el2:
             return 0
 
         (left1_start, left1_end) = self._get_left_span(el1)
         (left2_start, left2_end) = self._get_left_span(el2)
 
         (right1_start, right1_end) = self._get_right_span(el1)
         (right2_start, right2_end) = self._get_right_span(el2)
@@ -158,26 +158,26 @@
         if ans != 0: return ans
 
         return 0
 
     def _build_merged_element(self, el1, el2):
 
         new_el = {}
-        if "offset2_start" in el1:
+        if "offset2" in el1:
 
             new_el["offset1"] = (el1["offset1"][0], el1["offset1"][1])
 
             # the union if make in the second offset
             new_el["offset2"] = (el1["offset2"][0], el2["offset2"][1])
 
         else:
             # the union if make in the first offset
             new_el["offset1"] = (el1["offset1"][0], el2["offset1"][1])
             if "offset2" in el2:
-                new_el["offset2"] = (el2["offset2"][0], el2["offset2_end"][1])
+                new_el["offset2"] = (el2["offset2"][0], el2["offset2"][1])
 
         new_el["value"] = el1["value"] + " " + el2["value"]
         new_el["id"] = el1["id"]
         return new_el
 
     def merge_span(self, ann_entity):
         """
@@ -233,21 +233,22 @@
         """
 
         new_ann = {}
         for ent_type in ann:
             if ent_type in LINK_TYPES:
                 new_ann[ent_type] = ann[ent_type]
                 continue # if it is a link, just ignore it
-
+            #if "offset2_end" not in ann[ent_type]:
+            #    print("-->", ann[ent_type])
             new_ann_ent = self.merge_span(ann[ent_type])
             new_ann[ent_type] = new_ann_ent
 
         return new_ann
 
-    def read_annotation_file(self, file_ann, merge_entities=True):
+    def read_annotation_file(self, file_ann, merge_entities=False):
         """
         It reads only the annotation file, then returns
         the processed tokens as TokenCorpus type
 
         @param string: path of data to gather and process
 
         @return dictionary: a dictionary of annotations
@@ -270,19 +271,19 @@
                         if ann_type not in ann:
                             ann[ann_type] = []
 
                         if ';' in line_toks[3]:
                             # this situation is when the annotation of th event
                             # is two segments not adjacents
                             offset1_start = int(line_toks[2])
-                            offset1_end = int(line_toks[4])
+                            offset2_end = int(line_toks[4])
 
-                            offset2 = line_toks[3].split(';')
-                            offset2_start = int(offset2[0])
-                            offset2_end = int(offset2[1])
+                            offset_toks = line_toks[3].split(';')
+                            offset1_end = int(offset_toks[0])
+                            offset2_start = int(offset_toks[1])
 
                             value = " ".join(line_toks[5:])
 
                             ann[ann_type].append({"id":line_toks[0],"offset1": (offset1_start, offset1_end), \
                                               "offset2": (offset2_start, offset2_end), \
                                               "value": value})
 
@@ -315,33 +316,43 @@
                         else:
                             self.ann_ref[ann_type] = {ref:{attr_name:attr_value}}
         if merge_entities:
             return self.merge_entity_span(ann)
         else:
             return ann
 
-    def process(self, data_dir):
+    def process(self, data_dir, split=None):
         """
         It reads a set of files of annotations and text, then returns
         the processed tokens as TokenCorpus type
 
         @param string: path of data to gather and process
+        @param string: a file name that contains a list of the files in data dir that
+        should be processed by this reader
 
         @return [[TokenCorpus]]: a list of lists of tokens
         """
         # process the data corpus
         # and return a list of tokens
+        split_lst = []
+        if split is not None:
+            with open(split, "r") as fd:
+                split_lst = fd.readlines()
+                split_lst = [line.replace("\n","") for line in split_lst]
 
         data_tokens = []
 
         for dirpath, dirnames, filenames in os.walk(data_dir):
             for f in filenames:
                 if f.endswith(".ann"):
 
                     p = Path(f)
+                    if split_lst != [] and not(p.stem + ".txt" in split_lst):
+                        continue
+                 
                     fullname = os.path.join(data_dir, p.stem)
                     token_lst = self.process_file(fullname)
                     self.file_lst.append(fullname + ".txt")
 
                     if len(token_lst) > 0:
                         data_tokens.append(token_lst)
 
@@ -554,15 +565,14 @@
                     if ref in ann_rel: # if the current token has any relation, then...
 
                         # the relation for the reference ref
                         for rel_id, rel_type, ref_arg,argn in ann_rel[ref]:
                             rel_obj = token_corpus.TokenRelation(rel_id, ref2tok[ref_arg], rel_type, argn, ref_arg)
                             mytok.relations.append(rel_obj)
 
-
         return token_lst
 
     def search_all_idx(self, idx, idx_lst):
         """
         Since a token can be annotated with multiple id's, it is necessary 
         to perform multiple search for each one of these id's.
         """
```

### Comparing `text2story-1.3.3/text2story/readers/read_ecb.py` & `text2story-1.3.4/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/read_framenet.py` & `text2story-1.3.4/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/read_propbank.py` & `text2story-1.3.4/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/token_corpus.py` & `text2story-1.3.4/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/readers/utils.py` & `text2story-1.3.4/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/select/bubble.py` & `text2story-1.3.4/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/select/event.py` & `text2story-1.3.4/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/text2viz/Text2Viz.py` & `text2story-1.3.4/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/text2viz/visualization.py` & `text2story-1.3.4/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/training/participant_concept.py` & `text2story-1.3.4/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story/viz/bubble_tikz.py` & `text2story-1.3.4/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.3/text2story.egg-info/SOURCES.txt` & `text2story-1.3.4/text2story.egg-info/SOURCES.txt`

 * *Files identical despite different names*

