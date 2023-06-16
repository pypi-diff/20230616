# Comparing `tmp/autogluon.tabular-0.8.0.tar.gz` & `tmp/autogluon.tabular-0.8.0b20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.8.0.tar", last modified: Fri Jun 16 02:01:14 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.8.0b20230615.tar", last modified: Thu Jun 15 09:04:19 2023, max compression
```

## Comparing `autogluon.tabular-0.8.0.tar` & `autogluon.tabular-0.8.0b20230615.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.299255 autogluon.tabular-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.299255 autogluon.tabular-0.8.0/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.311255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.315255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.319254 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35982 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.323255 autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.327255 autogluon.tabular-0.8.0/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-16 02:00:41.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:01:14.307255 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:01:14.000000 autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.185677 autogluon.tabular-0.8.0b20230615/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.185677 autogluon.tabular-0.8.0b20230615/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.193677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.197677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.197677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.205677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.209677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.213677 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-15 09:03:44.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 09:04:18.000000 autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:04:19.189677 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:04:19.000000 autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.8.0/PKG-INFO` & `autogluon.tabular-0.8.0b20230615/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.0
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.8.0/setup.py` & `autogluon.tabular-0.8.0b20230615/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files 20% similar despite different names*

```diff
@@ -116,61 +116,14 @@
         'CAT': [
             {'depth': 5, 'l2_leaf_reg': 4.774992314058497, 'learning_rate': 0.038551267822920274, 'ag_args': {'name_suffix': '_r16', 'priority': 6}},
             {'depth': 4, 'l2_leaf_reg': 1.9950125740798321, 'learning_rate': 0.028091050379971633, 'ag_args': {'name_suffix': '_r42', 'priority': 5}},
             {'depth': 6, 'l2_leaf_reg': 1.8298803017644376, 'learning_rate': 0.017844259810823604, 'ag_args': {'name_suffix': '_r93', 'priority': 4}},
             {'depth': 7, 'l2_leaf_reg': 4.81099604606794, 'learning_rate': 0.019085060180573103, 'ag_args': {'name_suffix': '_r44', 'priority': 3}}
         ],
     },
-    zeroshot_hpo_hybrid={
-        'NN_TORCH': {},
-        'XT': [
-            {'criterion': 'gini', 'ag_args': {'name_suffix': 'Gini', 'problem_types': ['binary', 'multiclass']}},
-            {'criterion': 'entropy', 'ag_args': {'name_suffix': 'Entr', 'problem_types': ['binary', 'multiclass']}},
-            {'criterion': 'squared_error', 'ag_args': {'name_suffix': 'MSE', 'problem_types': ['regression', 'quantile']}},
-            {'min_samples_leaf': 1, 'max_leaf_nodes': 15000, 'max_features': 0.5, 'ag_args': {'name_suffix': '_r19', 'priority': 20}},
-        ],
-        'RF': [
-            {'criterion': 'gini', 'ag_args': {'name_suffix': 'Gini', 'problem_types': ['binary', 'multiclass']}},
-            {'criterion': 'entropy', 'ag_args': {'name_suffix': 'Entr', 'problem_types': ['binary', 'multiclass']}},
-            {'criterion': 'squared_error', 'ag_args': {'name_suffix': 'MSE', 'problem_types': ['regression', 'quantile']}},
-            {'min_samples_leaf': 5, 'max_leaf_nodes': 50000, 'max_features': 0.5, 'ag_args': {'name_suffix': '_r5', 'priority': 19}},
-        ],
-        'GBM': [
-            {'extra_trees': True, 'ag_args': {'name_suffix': 'XT'}},
-            {},
-            'GBMLarge',
-            {'extra_trees': False, 'feature_fraction': 0.7248284762542815, 'learning_rate': 0.07947286942946127, 'min_data_in_leaf': 50, 'num_leaves': 89, 'ag_args': {'name_suffix': '_r158', 'priority': 18}},
-            {'extra_trees': True, 'feature_fraction': 0.7832570544199176, 'learning_rate': 0.021720607471727896, 'min_data_in_leaf': 3, 'num_leaves': 21, 'ag_args': {'name_suffix': '_r118', 'priority': 17}},
-            {'extra_trees': True, 'feature_fraction': 0.7113010892989156, 'learning_rate': 0.012535427424259274, 'min_data_in_leaf': 16, 'num_leaves': 48, 'ag_args': {'name_suffix': '_r97', 'priority': 16}},
-            {'extra_trees': True, 'feature_fraction': 0.45555769907110816, 'learning_rate': 0.009591347321206594, 'min_data_in_leaf': 50, 'num_leaves': 110, 'ag_args': {'name_suffix': '_r71', 'priority': 15}},
-            {'extra_trees': False, 'feature_fraction': 0.40979710161022476, 'learning_rate': 0.008708890211023034, 'min_data_in_leaf': 3, 'num_leaves': 80, 'ag_args': {'name_suffix': '_r111', 'priority': 14}}
-        ],
-        'XGB': {},
-        'FASTAI': [
-            {},
-            {'bs': 1024, 'emb_drop': 0.6167722379778131, 'epochs': 44, 'layers': [200, 100, 50], 'lr': 0.053440377855629266, 'ps': 0.48477211305443607, 'ag_args': {'name_suffix': '_r25', 'priority': 13}},
-            {'bs': 1024, 'emb_drop': 0.6046989241462619, 'epochs': 48, 'layers': [200, 100, 50], 'lr': 0.00775309042164966, 'ps': 0.09244767444160731, 'ag_args': {'name_suffix': '_r51', 'priority': 12}},
-            {'bs': 512, 'emb_drop': 0.6557225316526186, 'epochs': 49, 'layers': [200, 100], 'lr': 0.023627682025564638, 'ps': 0.519566584552178, 'ag_args': {'name_suffix': '_r82', 'priority': 11}},
-            {'bs': 2048, 'emb_drop': 0.4066210919034579, 'epochs': 43, 'layers': [400, 200], 'lr': 0.0029598312717673434, 'ps': 0.4378695797438974, 'ag_args': {'name_suffix': '_r121', 'priority': 10}},
-            {'bs': 128, 'emb_drop': 0.44339037504795686, 'epochs': 31, 'layers': [400, 200, 100], 'lr': 0.008615195908919904, 'ps': 0.19220253419114286, 'ag_args': {'name_suffix': '_r145', 'priority': 9}},
-            {'bs': 128, 'emb_drop': 0.12106594798980945, 'epochs': 38, 'layers': [200, 100, 50], 'lr': 0.037991970245029975, 'ps': 0.33120008492595093, 'ag_args': {'name_suffix': '_r173', 'priority': 8}},
-            {'bs': 128, 'emb_drop': 0.4599138419358, 'epochs': 47, 'layers': [200, 100], 'lr': 0.03888383281136287, 'ps': 0.28193673177122863, 'ag_args': {'name_suffix': '_r128', 'priority': 7}}
-        ],
-        'CAT': [
-            {},
-            {'depth': 5, 'l2_leaf_reg': 4.774992314058497, 'learning_rate': 0.038551267822920274, 'ag_args': {'name_suffix': '_r16', 'priority': 6}},
-            {'depth': 4, 'l2_leaf_reg': 1.9950125740798321, 'learning_rate': 0.028091050379971633, 'ag_args': {'name_suffix': '_r42', 'priority': 5}},
-            {'depth': 6, 'l2_leaf_reg': 1.8298803017644376, 'learning_rate': 0.017844259810823604, 'ag_args': {'name_suffix': '_r93', 'priority': 4}},
-            {'depth': 7, 'l2_leaf_reg': 4.81099604606794, 'learning_rate': 0.019085060180573103, 'ag_args': {'name_suffix': '_r44', 'priority': 3}}
-        ],
-        'KNN': [
-            {'weights': 'uniform', 'ag_args': {'name_suffix': 'Unif'}},
-            {'weights': 'distance', 'ag_args': {'name_suffix': 'Dist'}},
-        ],
-    },
 )
 
 # default_FTT is experimental
 hyperparameter_config_dict['default_FTT'] = {'FT_TRANSFORMER': {}}
 hyperparameter_config_dict['default_FTT'].update(hyperparameter_config_dict['default'])
 
 # extreme is experimental
```

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/configs/presets_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     #  May have **extremely** slow inference speed, to a potentially unusable degree.
     experimental_extreme_quality={'auto_stack': True, 'hyperparameters': 'extreme'},
 
     # Experimental simulated model portfolio.
     # Shown to achieve superior results compared to best_quality on OpenML datasets <5000 rows.
     # Note that runtimes might be much longer than usual with this config.
     experimental_zeroshot_hpo={'auto_stack': True, 'hyperparameters': 'zeroshot_hpo'},
-    experimental_zeroshot_hpo_hybrid={'auto_stack': True, 'hyperparameters': 'zeroshot_hpo_hybrid'},
 
     # ------------------------------------------
     # ------------------------------------------
     # ------------------------------------------
 
     # TODO: Consider HPO-enabled configs if training time doesn't matter but inference latency does.
 )
```

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """ 
 Variant of the sklearn OneHotEncoder and OrdinalEncoder that can handle unknown classes at test-time 
 as well as binning of infrequent categories to limit the overall number of categories considered.
 Unknown categories are returned as None in inverse transforms. Always converts input list X to list of the same type elements first (string typically)
 """
-import copy
 from numbers import Integral
 
 import numpy as np
 from scipy import sparse
 
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
-from autogluon.features.generators import LabelEncoderFeatureGenerator
-
 
 __all__ = [
     'OneHotMergeRaresHandleUnknownEncoder',
     'OrdinalMergeRaresHandleUnknownEncoder'
 ]
 
 
@@ -399,16 +396,14 @@
                  dtype=np.float64, max_levels=None):
         self.categories = categories
         self.sparse = sparse
         self.dtype = dtype
         self.handle_unknown = 'ignore'
         self.drop = drop
         self.max_levels = max_levels
-        self._label_encoder = None
-        self._cat_cols = None
     
     def _validate_keywords(self):
         if self.handle_unknown not in ('error', 'ignore'):
             msg = ("handle_unknown should be either 'error' or 'ignore', "
                    "got {0}.".format(self.handle_unknown))
             raise ValueError(msg)
         # If we have both dropped columns and ignored unknown
@@ -452,38 +447,27 @@
             return np.array([np.where(cat_list == val)[0][0]
                              for (val, cat_list) in
                              zip(self.drop, self.categories_)], dtype=np.int_)
         else:
             msg = ("Wrong input for parameter `drop`. Expected "
                    "'first', None or array of objects, got {}")
             raise ValueError(msg.format(type(self.drop)))
-
-    def _convert_cat_to_int(self, X):
-        if self._cat_cols:
-            X = copy.deepcopy(X)
-            X[self._cat_cols] = self._label_encoder.transform(X[self._cat_cols])
-        return X
-
+    
     def fit(self, X, y=None):
         """Fit OneHotEncoder to X.
     
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to determine the categories of each feature.
     
         Returns
         -------
         self
         """
-        self._label_encoder = LabelEncoderFeatureGenerator(verbosity=0)
-        self._cat_cols = list(X.select_dtypes(include='category').columns)
-        if self._cat_cols:
-            self._label_encoder.fit(X=X[self._cat_cols])
-        X = self._convert_cat_to_int(X=X)
         X = np.array(X).tolist() # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
         self._validate_keywords()
         self._fit(X, handle_unknown=self.handle_unknown)
         self.drop_idx_ = self._compute_drop_idx()
         # check if user wants to manually drop a feature that is
         # infrequent: this is not allowed
         if self.drop is not None and not isinstance(self.drop, str):
@@ -495,29 +479,47 @@
                         "cannot be dropped. Use drop='infrequent' "
                         "instead.".format(
                             self.categories_[feature_idx][drop_idx],
                             feature_idx
                         )
                     )
         return self
+    
+    def fit_transform(self, X, y=None):
+        """Fit OneHotEncoder to X, then transform X.
 
+        Equivalent to fit(X).transform(X) but more convenient.
+
+        Parameters
+        ----------
+        X : array-like, shape [n_samples, n_features]
+            The data to encode.
+
+        Returns
+        -------
+        X_out : sparse matrix if sparse=True else a 2-d array
+            Transformed input.
+        """
+        X = np.array(X).tolist() # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
+        self._validate_keywords()
+        return super().fit_transform(X, y)
+    
     def transform(self, X):
         """Transform X using one-hot encoding.
         
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to encode.
         
         Returns
         -------
         X_out : sparse matrix if sparse=True else a 2-d array
             Transformed input.
         """
-        X = self._convert_cat_to_int(X=X)
         X = np.array(X).tolist() # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
         check_is_fitted(self, 'categories_')
         # validation of X happens in _check_X called by _transform
         X_int, X_mask = self._transform(X, handle_unknown=self.handle_unknown)
         n_samples, n_features = X_int.shape
         
         # n_columns indicates, for each feature, how many columns are used in
@@ -745,32 +747,28 @@
     
     """
     
     def __init__(self, categories='auto', dtype=np.float64, max_levels=None):
         self.categories = categories
         self.dtype = dtype
         self.max_levels = max_levels
-        self._label_encoder = None
     
     def fit(self, X, y=None):
         """Fit the OrdinalEncoder to X.
         
         Parameters
         ----------
         X : array-like, shape [n_samples, n_features]
             The data to determine the categories of each feature.
         
         Returns
         -------
         self
         
         """
-        self._label_encoder = LabelEncoderFeatureGenerator(verbosity=0)
-        self._label_encoder.fit(X=X)
-        X = self._label_encoder.transform(X)
         X = np.array(X).tolist()  # converts all elements in X to the same type (i.e. cannot mix floats, ints, and str)
         self._fit(X, handle_unknown='ignore')
 
         self.categories_as_sets_ = [np.array(list(set(categories))) for categories in self.categories_]
         # new level introduced to account for unknown categories, always = 1 + total number of categories seen during training
         self.categories_unknown_level_ = [min(len(categories), self.max_levels) for categories in self.categories_]
         self.categories_len_ = [len(categories) for categories in self.categories_]
@@ -786,15 +784,14 @@
         
         Returns
         -------
         X_out : sparse matrix or a 2-d array
             Transformed input.
         
         """
-        X = self._label_encoder.transform(X)
         X_og_array = np.array(X)  # original X array before transform
         X_int, _ = self._transform(X, handle_unknown='ignore')  # will contain zeros for 0th category as well as unknown values.
 
         for i in range(X_int.shape[1]):
             X_col_data = X_og_array[:, i]
             cat_set = self.categories_as_sets_[i]
             unknown_elements = np.isin(X_col_data, cat_set, invert=True)
```

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,20 @@
     if skewed_features:
         power_transformer = Pipeline(steps=[
             ('imputer', SimpleImputer(strategy=impute_strategy)),
             ('quantile', QuantileTransformer(output_distribution='normal')) ])  # Or output_distribution = 'uniform'
         transformers.append( ('skewed', power_transformer, skewed_features) )
     if onehot_features:
         onehot_transformer = Pipeline(steps=[
+            ('imputer', SimpleImputer(strategy='constant', fill_value=unique_category_str)),
             ('onehot', OneHotMergeRaresHandleUnknownEncoder(max_levels=max_category_levels, sparse=False))])  # test-time unknown values will be encoded as all zeros vector
         transformers.append( ('onehot', onehot_transformer, onehot_features) )
     if embed_features:  # Ordinal transformer applied to convert to-be-embedded categorical features to integer levels
         ordinal_transformer = Pipeline(steps=[
+            ('imputer', SimpleImputer(strategy='constant', fill_value=unique_category_str)),
             ('ordinal', OrdinalMergeRaresHandleUnknownEncoder(max_levels=max_category_levels))])  # returns 0-n when max_category_levels = n-1. category n is reserved for unknown test-time categories.
         transformers.append( ('ordinal', ordinal_transformer, embed_features) )
     return ColumnTransformer(transformers=transformers, remainder='passthrough')  # numeric features are processed in the same order as in numeric_features vector, so feature-names remain the same.
 
 def convert_df_dtype_to_str(df):
     return df.astype(str)
```

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.8.0b20230615/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.8.0
+Version: 0.8.0b20230615
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.8.0/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.8.0b20230615/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

