# Comparing `tmp/datamaestro_text-2023.6.16.tar.gz` & `tmp/datamaestro_text-2023.6.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaestro_text-2023.6.16.tar", last modified: Fri Jun 16 06:29:04 2023, max compression
+gzip compressed data, was "datamaestro_text-2023.6.16.1.tar", last modified: Fri Jun 16 11:12:53 2023, max compression
```

## Comparing `datamaestro_text-2023.6.16.tar` & `datamaestro_text-2023.6.16.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.938529 datamaestro_text-2023.6.16/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.930529 datamaestro_text-2023.6.16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.938529 datamaestro_text-2023.6.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.938529 datamaestro_text-2023.6.16/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.938529 datamaestro_text-2023.6.16/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.938529 datamaestro_text-2023.6.16/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/api/conversation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/api/ir.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/api/text.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/docs/source/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/conversation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/embeddings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/ir.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/recommendation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/datasets/text.rst
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.930529 datamaestro_text-2023.6.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/ai/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/ai/quac.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/fastml/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/fastml/goodbooks-10k.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.930529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/aagohary/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/aagohary/canard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/soskek/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/soskek/bookcorpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/msmarco/
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/msmarco/passage.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/wikiqa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/oscar-corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/sentiment140.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/smashwords/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/com/smashwords/bookcorpus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/cornell/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/cornell/nlvr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/aclimdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/glove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/im2p.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/ldc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/ldc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/ldc/aquaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/ir/
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/ir/covid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/clueweb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/deeplearning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/tipster.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/web.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/rajpurkar/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/rajpurkar/squad.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/thunlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/thunlp/fewrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/metamind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/metamind/research/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/metamind/research/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/io/metamind/research/wikitext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/net/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/net/mattmahoney/
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/net/mattmahoney/enwiki.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/acm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/acm/recsys/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/acm/recsys/cb2014.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/cocodataset/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/cocodataset/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/grouplens/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/grouplens/movielens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/universaldependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/org/universaldependencies/french.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/ac/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.934529 datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/ac/ucl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/ac/ucl/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/ac/ucl/cs/qangaroo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.946529 datamaestro_text-2023.6.16/src/datamaestro_text/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/cord19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/trec.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/data/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/download/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/download/tmdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/interfaces/plaintext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/interfaces/trec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/test/test_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/transforms/ir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.950529 datamaestro_text-2023.6.16/src/datamaestro_text/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/utils/randomstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/src/datamaestro_text/utils/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:29:04.942529 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:29:04.000000 datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 06:28:46.000000 datamaestro_text-2023.6.16/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/api/conversation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/api/ir.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/api/text.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/docs/source/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/conversation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/embeddings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/ir.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/recommendation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/datasets/text.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/ai/quac.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/fastml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/fastml/goodbooks-10k.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/aagohary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/aagohary/canard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/soskek/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/soskek/bookcorpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/msmarco/passage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/wikiqa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/oscar-corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/sentiment140.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/smashwords/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/smashwords/bookcorpus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/cornell/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/cornell/nlvr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/aclimdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/glove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/im2p.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/ldc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/ldc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/ldc/aquaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/ir/covid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/clueweb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/deeplearning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/tipster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/web.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/rajpurkar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/rajpurkar/squad.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/thunlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/thunlp/fewrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/metamind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/metamind/research/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/metamind/research/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/metamind/research/wikitext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/net/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/net/mattmahoney/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/net/mattmahoney/enwiki.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/acm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/acm/recsys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/acm/recsys/cb2014.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/cocodataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/cocodataset/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/grouplens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/grouplens/movielens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/universaldependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/universaldependencies/french.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/ac/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.905226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/ac/ucl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/ac/ucl/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/ac/ucl/cs/qangaroo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/cord19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/trec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/data/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/download/tmdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/interfaces/plaintext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/interfaces/trec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/test/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/transforms/ir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.913226 datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/randomstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:12:53.909226 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:12:53.000000 datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 11:12:42.000000 datamaestro_text-2023.6.16.1/tox.ini
```

### Comparing `datamaestro_text-2023.6.16/.circleci/config.yml` & `datamaestro_text-2023.6.16.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/.github/workflows/pytest.yml` & `datamaestro_text-2023.6.16.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/.github/workflows/python-publish.yml` & `datamaestro_text-2023.6.16.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/LICENSE` & `datamaestro_text-2023.6.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/Makefile` & `datamaestro_text-2023.6.16.1/Makefile`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/PKG-INFO` & `datamaestro_text-2023.6.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaestro_text
-Version: 2023.6.16
+Version: 2023.6.16.1
 Summary: "Text related datasets"
 Home-page: https://github.com/experimaestro/datamaestro_text
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: dataset manager
 Platform: any
```

### Comparing `datamaestro_text-2023.6.16/README.md` & `datamaestro_text-2023.6.16.1/README.md`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/docs/Makefile` & `datamaestro_text-2023.6.16.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/docs/make.bat` & `datamaestro_text-2023.6.16.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/docs/source/api/ir.rst` & `datamaestro_text-2023.6.16.1/docs/source/api/ir.rst`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/docs/source/conf.py` & `datamaestro_text-2023.6.16.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/docs/source/index.rst` & `datamaestro_text-2023.6.16.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/mkdocs.yml` & `datamaestro_text-2023.6.16.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/setup.cfg` & `datamaestro_text-2023.6.16.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/ai/quac.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/ai/quac.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/fastml/goodbooks-10k.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/fastml/goodbooks-10k.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/aagohary/canard.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/aagohary/canard.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     co-reference and ellipsis resolution.
 
     Each dataset is an instance of :class:`datamaestro_text.data.conversation.CanardDataset`
     """
     return {
         "train": CanardDataset(path=archive / "train.json"),
         "validation": CanardDataset(path=archive / "dev.json"),
-        "test": CanardDataset(path=archive / "dev.json"),
+        "test": CanardDataset(path=archive / "test.json"),
     }
```

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/github/soskek/bookcorpus.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/github/soskek/bookcorpus.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/msmarco/passage.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/msmarco/passage.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/microsoft/wikiqa.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/microsoft/wikiqa.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/oscar-corpus.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/oscar-corpus.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/sentiment140.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/sentiment140.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/com/smashwords/bookcorpus.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/com/smashwords/bookcorpus.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/cornell/nlvr.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/cornell/nlvr.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/aclimdb.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/aclimdb.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/glove.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/glove.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/stanford/im2p.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/stanford/im2p.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/edu/upenn/ldc/aquaint.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/edu/upenn/ldc/aquaint.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/ir/covid.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/ir/covid.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/adhoc.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/adhoc.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/clueweb.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/clueweb.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/deeplearning.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/deeplearning.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/index.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/index.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/tipster.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/tipster.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/gov/nist/trec/web.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/gov/nist/trec/web.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/rajpurkar/squad.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/rajpurkar/squad.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/io/github/thunlp/fewrel.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/github/thunlp/fewrel.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/io/metamind/research/wikitext.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/io/metamind/research/wikitext.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/net/mattmahoney/enwiki.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/net/mattmahoney/enwiki.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/org/acm/recsys/cb2014.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/acm/recsys/cb2014.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/org/grouplens/movielens.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/grouplens/movielens.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/org/universaldependencies/french.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/org/universaldependencies/french.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/config/uk/ac/ucl/cs/qangaroo.yaml` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/config/uk/ac/ucl/cs/qangaroo.yaml`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/conversation.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/conversation.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/embeddings.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/__init__.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/cord19.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/cord19.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/csv.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/csv.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/huggingface.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/huggingface.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/ir/trec.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/ir/trec.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/data/tagging.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/data/tagging.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/download/tmdb.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/download/tmdb.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/interfaces/plaintext.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/interfaces/plaintext.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/interfaces/trec.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/interfaces/trec.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/transforms/ir.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/transforms/ir.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/utils/__init__.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/utils/randomstream.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/randomstream.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text/utils/shuffle.py` & `datamaestro_text-2023.6.16.1/src/datamaestro_text/utils/shuffle.py`

 * *Files identical despite different names*

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/PKG-INFO` & `datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaestro-text
-Version: 2023.6.16
+Version: 2023.6.16.1
 Summary: "Text related datasets"
 Home-page: https://github.com/experimaestro/datamaestro_text
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: dataset manager
 Platform: any
```

### Comparing `datamaestro_text-2023.6.16/src/datamaestro_text.egg-info/SOURCES.txt` & `datamaestro_text-2023.6.16.1/src/datamaestro_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

