# Comparing `tmp/bert_squeeze-0.1.0.tar.gz` & `tmp/bert_squeeze-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_squeeze-0.1.0.tar", max compression
+gzip compressed data, was "bert_squeeze-0.1.1.tar", max compression
```

## Comparing `bert_squeeze-0.1.0.tar` & `bert_squeeze-0.1.1.tar`

### file list

```diff
@@ -1,83 +1,80 @@
--rw-r--r--   0        0        0        0 2023-05-12 11:31:28.487106 bert_squeeze-0.1.0/bert_squeeze/__init__.py
--rw-r--r--   0        0        0       90 2023-06-01 13:43:56.531792 bert_squeeze-0.1.0/bert_squeeze/assistants/__init__.py
--rw-r--r--   0        0        0     1990 2023-05-12 11:31:28.487723 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil.yaml
--rw-r--r--   0        0        0     2251 2023-05-12 11:31:28.487893 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil_hard.yaml
--rw-r--r--   0        0        0     1767 2023-05-12 11:31:28.488084 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil_parallel.yaml
--rw-r--r--   0        0        0     2094 2023-05-12 11:31:28.488282 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil_soft.yaml
--rw-r--r--   0        0        0      978 2023-05-12 11:31:28.488539 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_bert.yaml
--rw-r--r--   0        0        0     1061 2023-05-12 11:31:28.488860 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_deebert.yaml
--rw-r--r--   0        0        0     1085 2023-05-12 11:31:28.489029 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_fastbert.yaml
--rw-r--r--   0        0        0      852 2023-05-12 11:31:28.489257 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_lr.yaml
--rw-r--r--   0        0        0      774 2023-05-12 11:31:28.489533 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_lstm.yaml
--rw-r--r--   0        0        0     1084 2023-05-12 11:31:28.489769 bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_theseus_bert.yaml
--rw-r--r--   0        0        0     7570 2023-06-01 13:43:56.533272 bert_squeeze-0.1.0/bert_squeeze/assistants/distil_assistant.py
--rw-r--r--   0        0        0     5515 2023-06-01 13:43:56.534126 bert_squeeze-0.1.0/bert_squeeze/assistants/train_assistant.py
--rw-r--r--   0        0        0      145 2023-05-12 11:31:28.490778 bert_squeeze-0.1.0/bert_squeeze/data/__init__.py
--rw-r--r--   0        0        0       98 2023-05-12 11:31:28.490989 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/__init__.py
--rw-r--r--   0        0        0     2471 2023-06-01 13:43:56.534721 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/conference_dataset.py
--rw-r--r--   0        0        0    95109 2023-05-12 14:23:24.402902 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/parallel/test.json
--rw-r--r--   0        0        0   491830 2023-05-12 14:23:14.386217 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/parallel/train.json
--rw-r--r--   0        0        0   105192 2023-05-12 14:23:36.480283 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/parallel/validation.json
--rw-r--r--   0        0        0     2647 2023-06-01 13:43:56.535443 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/parallel_dataset.py
--rw-r--r--   0        0        0     1915 2023-06-01 13:43:56.536277 bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/unlabeled_dataset.py
--rw-r--r--   0        0        0      186 2023-05-12 11:31:28.491736 bert_squeeze-0.1.0/bert_squeeze/data/modules/__init__.py
--rw-r--r--   0        0        0     8382 2023-06-01 13:43:56.537049 bert_squeeze-0.1.0/bert_squeeze/data/modules/distillation_module.py
--rw-r--r--   0        0        0     4552 2023-06-01 13:43:56.537799 bert_squeeze-0.1.0/bert_squeeze/data/modules/lr_module.py
--rw-r--r--   0        0        0     6397 2023-06-01 13:43:56.538770 bert_squeeze-0.1.0/bert_squeeze/data/modules/lstm_module.py
--rw-r--r--   0        0        0     6148 2023-06-01 13:43:56.539512 bert_squeeze-0.1.0/bert_squeeze/data/modules/transformer_module.py
--rw-r--r--   0        0        0       33 2023-05-12 11:31:28.493188 bert_squeeze-0.1.0/bert_squeeze/distillation/__init__.py
--rw-r--r--   0        0        0    23337 2023-06-01 13:43:56.540645 bert_squeeze-0.1.0/bert_squeeze/distillation/distiller.py
--rw-r--r--   0        0        0        0 2023-05-12 11:31:28.494070 bert_squeeze-0.1.0/bert_squeeze/distillation/utils/__init__.py
--rw-r--r--   0        0        0     5418 2023-06-01 13:43:56.541341 bert_squeeze-0.1.0/bert_squeeze/distillation/utils/labeler.py
--rw-r--r--   0        0        0        0 2023-05-12 11:31:28.494797 bert_squeeze-0.1.0/bert_squeeze/inference/__init__.py
--rw-r--r--   0        0        0     1960 2023-06-01 13:43:56.542020 bert_squeeze-0.1.0/bert_squeeze/inference/model.py
--rw-r--r--   0        0        0      692 2023-06-01 13:43:56.542767 bert_squeeze-0.1.0/bert_squeeze/inference/processors.py
--rw-r--r--   0        0        0      256 2023-06-01 13:43:56.543443 bert_squeeze-0.1.0/bert_squeeze/models/__init__.py
--rw-r--r--   0        0        0    12841 2023-06-01 13:43:56.544310 bert_squeeze-0.1.0/bert_squeeze/models/base_lt_module.py
--rw-r--r--   0        0        0      113 2023-05-12 11:31:28.496681 bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/__init__.py
--rw-r--r--   0        0        0     8111 2023-06-01 13:43:56.545443 bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/bert.py
--rw-r--r--   0        0        0    13283 2023-06-01 13:43:56.546242 bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/deebert.py
--rw-r--r--   0        0        0     8452 2023-06-01 13:43:56.547083 bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/fastbert.py
--rw-r--r--   0        0        0    13974 2023-06-01 13:43:56.547721 bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/theseus_bert.py
--rw-r--r--   0        0        0        0 2023-05-12 11:31:28.498203 bert_squeeze-0.1.0/bert_squeeze/models/layers/__init__.py
--rw-r--r--   0        0        0     1387 2023-06-01 13:43:56.548514 bert_squeeze-0.1.0/bert_squeeze/models/layers/classifier.py
--rw-r--r--   0        0        0     1993 2023-06-01 13:43:56.549190 bert_squeeze-0.1.0/bert_squeeze/models/layers/mha.py
--rw-r--r--   0        0        0     7287 2023-06-01 13:43:56.549672 bert_squeeze-0.1.0/bert_squeeze/models/lr.py
--rw-r--r--   0        0        0     8457 2023-06-01 13:43:56.550277 bert_squeeze-0.1.0/bert_squeeze/models/lstm.py
--rw-r--r--   0        0        0     5391 2023-06-01 13:43:56.550956 bert_squeeze-0.1.0/bert_squeeze/models/lt_bert.py
--rw-r--r--   0        0        0    14340 2023-06-01 13:43:56.551615 bert_squeeze-0.1.0/bert_squeeze/models/lt_deebert.py
--rw-r--r--   0        0        0     4545 2023-06-01 13:43:56.552266 bert_squeeze-0.1.0/bert_squeeze/models/lt_distilbert.py
--rw-r--r--   0        0        0    11407 2023-06-01 13:43:56.552901 bert_squeeze-0.1.0/bert_squeeze/models/lt_fastbert.py
--rw-r--r--   0        0        0     6038 2023-06-01 13:43:56.553515 bert_squeeze-0.1.0/bert_squeeze/models/lt_theseus_bert.py
--rw-r--r--   0        0        0      182 2023-06-01 13:43:56.554285 bert_squeeze-0.1.0/bert_squeeze/utils/__init__.py
--rw-r--r--   0        0        0      172 2023-06-01 13:43:56.555080 bert_squeeze-0.1.0/bert_squeeze/utils/artifacts/__init__.py
--rw-r--r--   0        0        0     2356 2023-06-01 13:43:56.555754 bert_squeeze-0.1.0/bert_squeeze/utils/artifacts/distillation_artifacts.py
--rw-r--r--   0        0        0      759 2023-06-01 13:43:56.556407 bert_squeeze-0.1.0/bert_squeeze/utils/artifacts/transformer_artifacts.py
--rw-r--r--   0        0        0      111 2023-06-01 13:43:56.557265 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/__init__.py
--rw-r--r--   0        0        0     1651 2023-06-01 13:43:56.558263 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/checkpointing.py
--rw-r--r--   0        0        0     1659 2023-06-01 13:43:56.559420 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/fastbert_logic.py
--rw-r--r--   0        0        0    14219 2023-06-01 13:43:56.560747 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/lottery_ticket.py
--rw-r--r--   0        0        0     5728 2023-06-01 13:43:56.561427 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/pruning.py
--rw-r--r--   0        0        0     2952 2023-06-01 13:43:56.562102 bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/quantization.py
--rw-r--r--   0        0        0       92 2023-06-01 13:43:56.562981 bert_squeeze-0.1.0/bert_squeeze/utils/errors/__init__.py
--rw-r--r--   0        0        0      167 2023-05-12 11:31:28.504193 bert_squeeze-0.1.0/bert_squeeze/utils/errors/config_errors.py
--rw-r--r--   0        0        0      418 2023-05-12 11:31:28.504446 bert_squeeze-0.1.0/bert_squeeze/utils/errors/deebert_errors.py
--rw-r--r--   0        0        0      171 2023-06-01 13:43:56.563852 bert_squeeze-0.1.0/bert_squeeze/utils/losses/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-01 13:43:56.564585 bert_squeeze-0.1.0/bert_squeeze/utils/losses/distillation_losses.py
--rw-r--r--   0        0        0      923 2023-05-12 11:31:28.505424 bert_squeeze-0.1.0/bert_squeeze/utils/losses/losses.py
--rw-r--r--   0        0        0     1631 2023-06-01 13:43:56.565300 bert_squeeze-0.1.0/bert_squeeze/utils/losses/lsl.py
--rw-r--r--   0        0        0     3102 2023-06-01 13:43:56.565989 bert_squeeze-0.1.0/bert_squeeze/utils/losses/romebert_loss.py
--rw-r--r--   0        0        0       32 2023-05-12 11:31:28.506399 bert_squeeze-0.1.0/bert_squeeze/utils/optimizers/__init__.py
--rw-r--r--   0        0        0     7979 2023-06-01 13:43:56.566668 bert_squeeze-0.1.0/bert_squeeze/utils/optimizers/bert_adam.py
--rw-r--r--   0        0        0        0 2023-05-12 11:31:28.506990 bert_squeeze-0.1.0/bert_squeeze/utils/schedulers/__init__.py
--rw-r--r--   0        0        0     3387 2023-06-01 13:43:56.567257 bert_squeeze-0.1.0/bert_squeeze/utils/schedulers/theseus_schedulers.py
--rw-r--r--   0        0        0       80 2023-06-01 13:43:56.567999 bert_squeeze-0.1.0/bert_squeeze/utils/scorers/__init__.py
--rw-r--r--   0        0        0    10543 2023-06-01 13:43:56.568709 bert_squeeze-0.1.0/bert_squeeze/utils/scorers/scorer.py
--rw-r--r--   0        0        0     6765 2023-06-01 13:43:56.569334 bert_squeeze-0.1.0/bert_squeeze/utils/scorers/scorer_fast.py
--rw-r--r--   0        0        0     1296 2023-06-01 13:43:56.570071 bert_squeeze-0.1.0/bert_squeeze/utils/types.py
--rw-r--r--   0        0        0     2933 2023-06-01 13:43:56.570873 bert_squeeze-0.1.0/bert_squeeze/utils/utils_fct.py
--rw-r--r--   0        0        0     2493 2023-06-01 13:43:56.571470 bert_squeeze-0.1.0/bert_squeeze/utils/vocabulary.py
--rw-r--r--   0        0        0    15987 2023-05-12 11:31:28.510236 bert_squeeze-0.1.0/images/bert-squeeze.png
--rw-r--r--   0        0        0     1877 2023-06-01 13:44:18.611635 bert_squeeze-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 bert_squeeze-0.1.0/setup.py
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 bert_squeeze-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/__init__.py
+-rw-r--r--   0        0        0     1953 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil.yaml
+-rw-r--r--   0        0        0     2251 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_hard.yaml
+-rw-r--r--   0        0        0     1767 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_parallel.yaml
+-rw-r--r--   0        0        0     2094 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_soft.yaml
+-rw-r--r--   0        0        0      978 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_bert.yaml
+-rw-r--r--   0        0        0     1061 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_deebert.yaml
+-rw-r--r--   0        0        0     1085 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_fastbert.yaml
+-rw-r--r--   0        0        0      852 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_lr.yaml
+-rw-r--r--   0        0        0      774 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_lstm.yaml
+-rw-r--r--   0        0        0     1084 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_theseus_bert.yaml
+-rw-r--r--   0        0        0     7570 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/distil_assistant.py
+-rw-r--r--   0        0        0     5756 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/assistants/train_assistant.py
+-rw-r--r--   0        0        0      145 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/__init__.py
+-rw-r--r--   0        0        0       98 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/__init__.py
+-rw-r--r--   0        0        0     2471 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/conference_dataset.py
+-rw-r--r--   0        0        0     2647 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/parallel_dataset.py
+-rw-r--r--   0        0        0     1915 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/unlabeled_dataset.py
+-rw-r--r--   0        0        0      186 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/modules/__init__.py
+-rw-r--r--   0        0        0     8869 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/modules/distillation_module.py
+-rw-r--r--   0        0        0     4552 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/modules/lr_module.py
+-rw-r--r--   0        0        0     6397 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/modules/lstm_module.py
+-rw-r--r--   0        0        0     6073 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/data/modules/transformer_module.py
+-rw-r--r--   0        0        0       33 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/distillation/__init__.py
+-rw-r--r--   0        0        0    24364 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/distillation/distiller.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/distillation/utils/__init__.py
+-rw-r--r--   0        0        0     5418 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/distillation/utils/labeler.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/inference/__init__.py
+-rw-r--r--   0        0        0     1960 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/inference/model.py
+-rw-r--r--   0        0        0      692 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/inference/processors.py
+-rw-r--r--   0        0        0      256 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/models/__init__.py
+-rw-r--r--   0        0        0    13173 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/models/base_lt_module.py
+-rw-r--r--   0        0        0      113 2023-06-16 09:09:53.786079 bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/__init__.py
+-rw-r--r--   0        0        0     8111 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/bert.py
+-rw-r--r--   0        0        0    13283 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/deebert.py
+-rw-r--r--   0        0        0     8452 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/fastbert.py
+-rw-r--r--   0        0        0    13974 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/theseus_bert.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/layers/__init__.py
+-rw-r--r--   0        0        0     1387 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/layers/classifier.py
+-rw-r--r--   0        0        0     1993 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/layers/mha.py
+-rw-r--r--   0        0        0     7219 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lr.py
+-rw-r--r--   0        0        0     8435 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lstm.py
+-rw-r--r--   0        0        0     5422 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lt_bert.py
+-rw-r--r--   0        0        0    14299 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lt_deebert.py
+-rw-r--r--   0        0        0     4529 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lt_distilbert.py
+-rw-r--r--   0        0        0    11312 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lt_fastbert.py
+-rw-r--r--   0        0        0     6007 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/models/lt_theseus_bert.py
+-rw-r--r--   0        0        0      182 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/artifacts/__init__.py
+-rw-r--r--   0        0        0     2356 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/artifacts/distillation_artifacts.py
+-rw-r--r--   0        0        0      759 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/artifacts/transformer_artifacts.py
+-rw-r--r--   0        0        0       95 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     1651 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/checkpointing.py
+-rw-r--r--   0        0        0     1527 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/fastbert_logic.py
+-rw-r--r--   0        0        0    14219 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/lottery_ticket.py
+-rw-r--r--   0        0        0     5984 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/pruning.py
+-rw-r--r--   0        0        0     1420 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/quantization.py
+-rw-r--r--   0        0        0       92 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/errors/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/errors/config_errors.py
+-rw-r--r--   0        0        0      418 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/errors/deebert_errors.py
+-rw-r--r--   0        0        0      171 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/losses/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/losses/distillation_losses.py
+-rw-r--r--   0        0        0     1026 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/losses/losses.py
+-rw-r--r--   0        0        0     1631 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/losses/lsl.py
+-rw-r--r--   0        0        0     3102 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/losses/romebert_loss.py
+-rw-r--r--   0        0        0       32 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/optimizers/__init__.py
+-rw-r--r--   0        0        0     7979 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/optimizers/bert_adam.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/schedulers/__init__.py
+-rw-r--r--   0        0        0     3387 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/schedulers/theseus_schedulers.py
+-rw-r--r--   0        0        0       80 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/scorers/__init__.py
+-rw-r--r--   0        0        0    10543 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/scorers/scorer.py
+-rw-r--r--   0        0        0     6941 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/scorers/scorer_fast.py
+-rw-r--r--   0        0        0     1296 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/types.py
+-rw-r--r--   0        0        0     3053 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/utils_fct.py
+-rw-r--r--   0        0        0     2493 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/bert_squeeze/utils/vocabulary.py
+-rw-r--r--   0        0        0    15987 2023-06-16 09:09:53.790079 bert_squeeze-0.1.1/images/bert-squeeze.png
+-rw-r--r--   0        0        0     1897 2023-06-16 09:09:53.794079 bert_squeeze-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 bert_squeeze-0.1.1/setup.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 bert_squeeze-0.1.1/PKG-INFO
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_soft.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
   evaluate_during_training: true
   labels: [ 0, 1 ]
   num_labels: 2
   output_dir: outputs
   save_steps: 500
   validation_every_n_epoch: 1
 
-
 train:
   adam_eps: 1e-8
   accumulation_steps: 1
   auto_lr: false
   discriminative_learning: true
   dropout: 0.2
   layer_lr_decay: 0.95
@@ -62,8 +61,14 @@
     dataset_config:
       is_local: ${data.teacher_module.dataset_config.is_local}
       path: ${data.teacher_module.dataset_config.path}
       split: ${data.teacher_module.dataset_config.split}
       text_col: ${data.teacher_module.dataset_config.text_col}
       label_col: ${data.teacher_module.dataset_config.label_col}
     tokenizer_name: ${model.student.pretrained_model_name_or_path}
-    max_length: 256
+    max_length: 256
+  soft_data_config:
+    is_local: false
+    path:
+    split:
+    text_col: "text"
+    max_samples: 10000
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil_hard.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_hard.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/distil_parallel.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/distil_parallel.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_bert.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_bert.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_deebert.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_deebert.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_fastbert.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_fastbert.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_lr.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_lr.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_lstm.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_lstm.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/configs/train_theseus_bert.yaml` & `bert_squeeze-0.1.1/bert_squeeze/assistants/configs/train_theseus_bert.yaml`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/distil_assistant.py` & `bert_squeeze-0.1.1/bert_squeeze/assistants/distil_assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 from typing import Any, Dict, List, Optional
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 import torch.nn
 from hydra.utils import instantiate
 from lightning.pytorch.callbacks import Callback
 from lightning.pytorch.loggers import Logger, TensorBoardLogger
 from omegaconf import DictConfig, OmegaConf
 from pkg_resources import resource_filename
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/assistants/train_assistant.py` & `bert_squeeze-0.1.1/bert_squeeze/assistants/train_assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 CONFIG_MAPPER = {
     "lr": "train_lr.yaml",
     "bert": "train_bert.yaml",
     "lstm": "train_lstm.yaml",
     "deebert": "train_deebert.yaml",
     "fastbert": "train_fastbert.yaml",
-    "theseus-bert": "train_theseus_bert.yaml",
+    "theseusbert": "train_theseus_bert.yaml",
 }
 
 
 class TrainAssistant(object):
     """
     Helper object that holds and instantiate the needed for training.
 
@@ -55,19 +55,25 @@
         general_kwargs: Dict[str, Any] = None,
         train_kwargs: Dict[str, Any] = None,
         model_kwargs: Dict[str, Any] = None,
         data_kwargs: Dict[str, Any] = None,
         logger_kwargs: Dict[str, Any] = None,
         callbacks: List[Callback] = None,
     ):
-        conf = OmegaConf.load(
-            resource_filename(
-                "bert_squeeze", os.path.join("assistants/configs", CONFIG_MAPPER[name])
+        try:
+            conf = OmegaConf.load(
+                resource_filename(
+                    "bert_squeeze",
+                    os.path.join("assistants/configs", CONFIG_MAPPER[name]),
+                )
+            )
+        except KeyError:
+            raise ValueError(
+                f"'{name}' is not a valid configuration name, please use one of the following: {CONFIG_MAPPER.keys()}"
             )
-        )
         if (
             data_kwargs is not None
             and data_kwargs.get("dataset_config", {}).get("path") is not None
         ):
             logging.warning(
                 "Found value for `dataset_config.path` which conflicts with parameter `dataset_path`, using"
                 "value from the later."
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/conference_dataset.py` & `bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/conference_dataset.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/parallel_dataset.py` & `bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/parallel_dataset.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/local_datasets/unlabeled_dataset.py` & `bert_squeeze-0.1.1/bert_squeeze/data/local_datasets/unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/modules/distillation_module.py` & `bert_squeeze-0.1.1/bert_squeeze/data/modules/distillation_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
 import datasets
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 from datasets import Features
 from omegaconf import DictConfig
 from torch.utils.data import DataLoader
 
 from ...distillation.utils.labeler import HardLabeler
 from .lr_module import LrDataModule
 from .lstm_module import LSTMDataModule
@@ -58,14 +58,33 @@
         self.labeler = hard_labeler
 
         self.dataset = None
         self.train = None
         self.test = None
         self.val = None
 
+    @staticmethod
+    def _concat_dataset(
+        a: Union[datasets.Dataset, datasets.DatasetDict],
+        b: Union[datasets.Dataset, datasets.DatasetDict],
+    ) -> Union[datasets.Dataset, datasets.DatasetDict]:
+        """"""
+        assert type(a) == type(b) and a.keys() == b.keys()
+
+        if isinstance(a, datasets.DatasetDict):
+            concat_dataset = datasets.DatasetDict(
+                {
+                    key: datasets.concatenate_datasets([a[key], b[key]], axis=1)
+                    for key in a.keys()
+                }
+            )
+        else:
+            concat_dataset = datasets.concatenate_datasets([a, b], axis=1)
+        return concat_dataset
+
     def create_hard_dataset(self) -> datasets.Dataset:
         """"""
         hard_dataset = self.labeler.label_dataset()
         return datasets.Dataset.from_dict(hard_dataset)
 
     def get_soft_dataset(self) -> datasets.Dataset:
         """
@@ -172,22 +191,15 @@
         for dataset_split, columns in student_data.column_names.items():
             for col in columns:
                 student_data[dataset_split] = student_data[dataset_split].rename_column(
                     col, "s_" + col
                 )
 
         # Merging the student and teacher datasets into a single one
-        concat_dataset = datasets.DatasetDict(
-            {
-                key: datasets.concatenate_datasets(
-                    [teacher_data[key], student_data[key]], axis=1
-                )
-                for key in ["train", "test", "validation"]
-            }
-        )
+        concat_dataset = self._concat_dataset(teacher_data, student_data)
         concat_dataset = concat_dataset.shuffle()
         concat_dataset.set_format(type="torch")
         return concat_dataset
 
     def prepare_data(self) -> None:
         """
         Load teacher and student datasets
@@ -196,36 +208,34 @@
         self.student_module.prepare_data()
 
     def setup(self, stage: Optional[str] = None) -> None:
         """"""
         featurized_dataset = self.featurize()
 
         self.train = featurized_dataset["train"]
-        self.val = featurized_dataset["validation"]
+        self.val = (
+            featurized_dataset["validation"]
+            if "validation" in featurized_dataset.keys()
+            else featurized_dataset["test"]
+        )
         self.test = featurized_dataset["test"]
 
     def train_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: Train dataloader
         """
-        return DataLoader(
-            self.train, batch_size=self.train_batch_size, drop_last=True, num_workers=0
-        )
+        return DataLoader(self.train, batch_size=self.train_batch_size, drop_last=True)
 
     def test_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: Test dataloader
         """
-        return DataLoader(
-            self.test, batch_size=self.eval_batch_size, drop_last=True, num_workers=0
-        )
+        return DataLoader(self.test, batch_size=self.eval_batch_size, drop_last=True)
 
     def val_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: Validation dataloader
         """
-        return DataLoader(
-            self.val, batch_size=self.eval_batch_size, drop_last=True, num_workers=0
-        )
+        return DataLoader(self.val, batch_size=self.eval_batch_size, drop_last=True)
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/modules/lr_module.py` & `bert_squeeze-0.1.1/bert_squeeze/data/modules/lr_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Optional
 
 import datasets
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 from datasets import Dataset, DatasetDict
 from hydra.core.hydra_config import HydraConfig
 from sklearn.feature_extraction.text import CountVectorizer
 from torch.utils.data import DataLoader
 
 
 class LrDataModule(pl.LightningDataModule):
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/modules/lstm_module.py` & `bert_squeeze-0.1.1/bert_squeeze/data/modules/lstm_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import re
 from typing import Any, Dict, List, Optional
 
 import datasets
+import lightning.pytorch as pl
 import numpy as np
-import pytorch_lightning as pl
 import torch
 from datasets import DatasetDict
 from hydra.core.hydra_config import HydraConfig
 from torch.utils.data import DataLoader
 
 from ...utils.vocabulary import Vocabulary
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/data/modules/transformer_module.py` & `bert_squeeze-0.1.1/bert_squeeze/data/modules/transformer_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Optional
 
 import datasets
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 from omegaconf import DictConfig
 from overrides import overrides
 from torch.utils.data import DataLoader
 from transformers import AutoTokenizer
 
 
 class TransformerDataModule(pl.LightningDataModule):
@@ -101,44 +101,41 @@
     def train_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: train dataloader
         """
         return DataLoader(
             self.train,
-            collate_fn=self._collate_fn(),
+            # collate_fn=self._collate_fn(),
             batch_size=self.train_batch_size,
             drop_last=True,
-            num_workers=0,
         )
 
     def test_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: test dataloader
         """
         return DataLoader(
             self.test,
-            collate_fn=self._collate_fn(),
+            # collate_fn=self._collate_fn(),
             batch_size=self.eval_batch_size,
             drop_last=True,
-            num_workers=0,
         )
 
     def val_dataloader(self) -> DataLoader:
         """
         Returns:
             DataLoader: Validation dataloader
         """
         return DataLoader(
             self.val,
-            collate_fn=self._collate_fn(),
+            # collate_fn=self._collate_fn(),
             batch_size=self.eval_batch_size,
             drop_last=True,
-            num_workers=0,
         )
 
 
 class TransformerParallelDataModule(TransformerDataModule):
     """
     DataModule for parallel dataset for Transformer-based models.
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/distillation/distiller.py` & `bert_squeeze-0.1.1/bert_squeeze/distillation/distiller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from typing import Any, Dict, List, Tuple, Union
 
+import lightning.pytorch as pl
 import matplotlib.pyplot as plt
 import numpy as np
-import pytorch_lightning as pl
 import seaborn as sns
 import torch
 import torch.nn.functional as F
 from omegaconf import DictConfig, ListConfig
 from overrides import overrides
 from torch.nn import CrossEntropyLoss
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from transformers import AdamW
+from transformers.modeling_outputs import SequenceClassifierOutput
 
 from ..utils.losses import LabelSmoothingLoss
 from ..utils.losses.distillation_losses import KLDivLoss
 from ..utils.optimizers import BertAdam
 from ..utils.scorers import Scorer
 from ..utils.types import DistillationLoss
 
@@ -45,14 +46,18 @@
     ):
         super().__init__()
         self.params = training_config
         self.teacher = teacher
         self.student = student
         self.teacher_checkpoint = teacher_checkpoint
 
+        self.training_step_outputs = []
+        self.test_step_outputs = []
+        self.validation_step_outputs = []
+
         self._set_objectives()
         self._set_scorers()
 
     def _set_objectives(self) -> None:
         """
         Sets the different objectives used for distillation:
         - a classical one to evaluate the student's predictions
@@ -221,35 +226,33 @@
         elif self.params.optimizer == "adamw":
             optimizer = AdamW(
                 optimizer_parameters,
                 lr=self.params.learning_rates[0],
                 eps=self.params.adam_eps,
             )
         elif self.params.optimizer == "bertadam":
-            num_training_steps = (
-                len(self.train_dataloader())
-                * self.params.num_epochs
-                // self.params.accumulation_steps
-            )
             optimizer = BertAdam(
                 optimizer_parameters,
                 lr=self.params.learning_rates[0],
                 warmup=self.params.warmup_ratio,
-                t_total=num_training_steps,
             )
         elif self.params.optimizer == "adam":
             optimizer = torch.optim.Adam(
                 optimizer_parameters, lr=self.params.learning_rates[0]
             )
         else:
             raise ValueError(f"Optimizer '{self.params.optimizer}' not supported.")
 
         if self.params.lr_scheduler:
             scheduler = ReduceLROnPlateau(optimizer)
-            lr_scheduler = {"scheduler": scheduler, "name": "NeptuneLogger"}
+            lr_scheduler = {
+                "scheduler": scheduler,
+                "name": "NeptuneLogger",
+                "monitor": "loss",
+            }
             return [optimizer], [lr_scheduler]
 
         return [optimizer], []
 
     def get_teacher_logits(self, batch: Dict[str, torch.Tensor]) -> Any:
         raise NotImplementedError()
 
@@ -261,22 +264,22 @@
 
     def test_step(self, batch, _) -> Dict:
         raise NotImplementedError()
 
     def validation_step(self, batch, _) -> Dict:
         raise NotImplementedError()
 
-    def training_epoch_end(self, _) -> None:
+    def on_train_epoch_end(self) -> None:
         """"""
         self.s_scorer.reset()
 
-    def validation_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_validation_epoch_end(self) -> None:
         raise NotImplementedError()
 
-    def test_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_test_epoch_end(self) -> None:
         raise NotImplementedError()
 
     def loss(
         self, teacher_logits: torch.Tensor, student_logits: torch.Tensor, *args, **kwargs
     ) -> DistillationLoss:
         raise NotImplementedError()
 
@@ -288,38 +291,37 @@
         the probability distribution of all labels.
 
         Args:
             probs (List[np.array]):
                 predicted probabilities
         """
         table = self.s_valid_scorer.get_table()
-        self.logger.experiment["eval/report"].log(table)
+        self.logger.experiment.add_text("eval/report", table)
 
         # logging losses to neptune
         logging_loss = {
             key: torch.stack(val).mean()
             for key, val in self.s_valid_scorer.losses.items()
         }
-        for key, value in logging_loss.items():
-            self.logger.experiment[f"eval/loss_{key}"].log(value)
+        self.log_dict({f"eval/loss_{key}": val for key, val in logging_loss.items()})
 
         # logging other metrics
         eval_report = self.s_valid_scorer.to_dict()
         for key, value in eval_report.items():
             if not isinstance(value, list) and not isinstance(value, np.ndarray):
-                self.logger.experiment["eval/{}".format(key)].log(
-                    value=value, step=self.global_step
+                self.log_dict(
+                    {f"eval/loss_{key}": val for key, val in logging_loss.items()}
                 )
 
         # logging probability distributions
         for i in range(len(probs)):
             fig = plt.figure(figsize=(15, 15))
             sns.distplot(probs[i], kde=False, bins=100)
             plt.title("Probability boxplot for label {}".format(i))
-            self.logger.experiment["eval/dist_label_{}".format(i)].log(fig)
+            self.logger.experiment.add_figure("eval/dist_label_{}".format(i), fig)
             plt.close("all")
 
 
 class Distiller(BaseDistiller):
     """
     Lightning module to distil a given teacher model into a given student one.
 
@@ -354,37 +356,49 @@
                 batched features
         Returns:
             torch.Tensor:
                 teacher logits
         """
         self.teacher.eval()
         teacher_inputs = {
-            key[2:]: val for key, val in batch.items() if key.startswith("t_")
+            key[2:]: val
+            for key, val in batch.items()
+            if key.startswith("t_") and "labels" not in key
         }
         with torch.no_grad():
-            logits = self.teacher.forward(**teacher_inputs)
-        return logits
+            outputs = self.teacher.forward(**teacher_inputs)
+
+        if isinstance(outputs, SequenceClassifierOutput):
+            return outputs.logits
+
+        return outputs
 
     @overrides
     def get_student_logits(self, batch: Dict[str, torch.Tensor]) -> torch.Tensor:
         """
         Get student's predictions.
 
         Args:
             batch (Dict[str, torch.Tensor]):
                 batched features
         Returns:
             torch.Tensor:
                 student logits
         """
         student_inputs = {
-            key[2:]: val for key, val in batch.items() if key.startswith("s_")
+            key[2:]: val
+            for key, val in batch.items()
+            if key.startswith("s_") and "labels" not in key
         }
-        logits = self.student.forward(**student_inputs)
-        return logits
+        outputs = self.student.forward(**student_inputs)
+
+        if isinstance(outputs, SequenceClassifierOutput):
+            return outputs.logits
+
+        return outputs
 
     @overrides
     def loss(
         self,
         teacher_logits: torch.Tensor,
         student_logits: torch.Tensor,
         labels: torch.Tensor = None,
@@ -406,15 +420,15 @@
                 labels to ignore during loss computation
         Returns:
 
         """
         # Ignore soft labeled indices (where label is `ignore_index`)
         active_idx = labels != ignore_index
         if active_idx.sum().item() > 0:
-            objective = self.loss_lce(student_logits[active_idx], labels[active_idx])
+            objective = self.loss_ce(student_logits[active_idx], labels[active_idx])
         else:
             objective = torch.tensor(0.0).to(labels.device)
 
         kd_loss = self.loss_distill(teacher_logits, student_logits)
         full_loss = (1 - self.params.alpha) * kd_loss + self.params.alpha * objective
         return DistillationLoss(kd_loss=kd_loss, objective=objective, full_loss=full_loss)
 
@@ -423,64 +437,71 @@
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits, batch["s_labels"])
 
         self.s_scorer.add(s_logits.detach().cpu(), batch["s_labels"].cpu(), loss)
-        if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
+        if self.global_step > 0 and self.global_step % self.params.logging_steps == 0:
             logging_loss = {
-                key: torch.stack(val).mean() for key, val in self.s_scorer.losses.items()
+                f"train/{key}": torch.stack(val).mean()
+                for key, val in self.s_scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"loss_{key}"].log(value)
+            self.log_dict(logging_loss)
 
-            self.logger.experiment["train/acc"].log(
-                self.s_scorer.acc, step=self.global_step
-            )
+            self.log("train/acc", self.scorer.acc)
         return loss.full_loss
 
     @overrides
     def test_step(self, batch, _) -> Dict:
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits, batch["s_labels"])
         self.s_test_scorer.add(
             s_logits.detach().cpu(), batch["labels"].detach().cpu(), loss
         )
-        return {"loss": loss.full_loss, "logits": s_logits.detach().cpu()}
+        self.test_step_outputs.append(
+            {"loss": loss.full_loss, "logits": s_logits.detach().cpu()}
+        )
+        return {"loss": loss.full_loss}
 
     @overrides
     def validation_step(self, batch, _) -> Dict:
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits, batch["s_labels"])
         self.s_valid_scorer.add(
             s_logits.detach().cpu(), batch["s_labels"].detach().cpu(), loss
         )
-        return {"loss": loss.full_loss, "logits": s_logits.detach().cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss.full_loss, "logits": s_logits.detach().cpu()}
+        )
+        return {"loss": loss.full_loss}
 
     @overrides
-    def validation_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_validation_epoch_end(self) -> None:
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
-        all_probs = F.softmax(all_logits, dim=-1)
-        labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
+        if not self.trainer.sanity_checking:
+            all_logits = torch.cat(
+                [pred["logits"] for pred in self.validation_step_outputs]
+            )
+            all_probs = F.softmax(all_logits, dim=-1)
+            labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
+            self.log_eval_report(labels_probs)
 
-        self.log_eval_report(labels_probs)
         self.s_valid_scorer.reset()
 
     @overrides
-    def test_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_test_epoch_end(self) -> None:
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
+        all_logits = torch.cat([pred["logits"] for pred in self.test_step_outputs])
         all_probs = F.softmax(all_logits, dim=-1)
         labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
 
         self.log_eval_report(labels_probs)
         self.s_test_scorer.reset()
 
 
@@ -519,19 +540,24 @@
                 batched features
         Returns:
             torch.Tensor:
                 teacher logits
         """
         self.teacher.eval()
         teacher_inputs = {
-            key[2:]: val for key, val in batch.items() if key.startswith("t_")
+            key[2:]: val
+            for key, val in batch.items()
+            if key.startswith("t_") and "labels" not in key
         }
         with torch.no_grad():
-            logits = self.teacher.forward(**teacher_inputs)
-        return logits
+            outputs = self.teacher.forward(**teacher_inputs)
+
+        if isinstance(outputs, SequenceClassifierOutput):
+            return outputs.logits
+        return outputs
 
     @overrides
     def get_student_logits(
         self, batch: Dict[str, torch.Tensor]
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Get student's predictions.
@@ -541,31 +567,39 @@
                 batched features
         Returns:
             Tuple[torch.Tensor, torch.Tensor]:
                 student logits predicted for the parallel data, resulting in one prediction for
                 the original text and one prediction for the translation.
         """
         student_inputs = {
-            key[2:]: val for key, val in batch.items() if key.startswith("s_")
+            key[2:]: val
+            for key, val in batch.items()
+            if key.startswith("s_") and "labels" not in key
         }
-        original_logits = self.student.forward(
+        original_outputs = self.student.forward(
             **{
                 key: val
                 for key, val in student_inputs.items()
                 if not key.startswith("translation")
             }
         )
-        translation_logits = self.student.forward(
+        if isinstance(original_outputs, SequenceClassifierOutput):
+            original_outputs = original_outputs.logits
+
+        translation_outputs = self.student.forward(
             **{
                 key: val
                 for key, val in student_inputs.items()
                 if key.startswith("translation")
             }
         )
-        return original_logits, translation_logits
+        if isinstance(translation_outputs, SequenceClassifierOutput):
+            translation_outputs = translation_outputs.logits
+
+        return original_outputs, translation_outputs
 
     @overrides
     def loss(
         self,
         teacher_logits: torch.Tensor,
         student_logits: torch.Tensor,
         student_logits_translation: torch.Tensor,
@@ -599,53 +633,61 @@
     @overrides
     def training_step(self, batch, _) -> torch.Tensor:
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits_original, s_logits_translated = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits_original, s_logits_translated)
-
         return loss.full_loss
 
     @overrides
     def test_step(self, batch, _) -> Dict:
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits_original, s_logits_translated = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits_original, s_logits_translated)
         self.s_test_scorer.add(
             s_logits_original.detach().cpu(), batch["labels"].detach().cpu(), loss
         )
-        return {"loss": loss.full_loss, "logits": s_logits_original.detach().cpu()}
+        self.test_step_outputs.append(
+            {"loss": loss.full_loss, "logits": s_logits_original.detach().cpu()}
+        )
+        return {"loss": loss.full_loss}
 
     @overrides
     def validation_step(self, batch, _) -> Dict:
         """"""
         t_logits = self.get_teacher_logits(batch)
         s_logits_original, s_logits_translated = self.get_student_logits(batch)
 
         loss = self.loss(t_logits, s_logits_original, s_logits_translated)
         self.s_valid_scorer.add(
             s_logits_original.detach().cpu(), batch["s_labels"].detach().cpu(), loss
         )
-        return {"loss": loss.full_loss, "logits": s_logits_original.detach().cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss.full_loss, "logits": s_logits_original.detach().cpu()}
+        )
+        return {"loss": loss.full_loss}
 
     @overrides
-    def validation_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_validation_epoch_end(self) -> None:
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
-        all_probs = F.softmax(all_logits, dim=-1)
-        labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
+        if not self.trainer.sanity_checking:
+            all_logits = torch.cat(
+                [pred["logits"] for pred in self.validation_step_outputs]
+            )
+            all_probs = F.softmax(all_logits, dim=-1)
+            labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
+            self.log_eval_report(labels_probs)
 
-        self.log_eval_report(labels_probs)
         self.s_valid_scorer.reset()
 
     @overrides
-    def test_epoch_end(self, test_step_outputs: List[Dict]) -> None:
+    def on_test_epoch_end(self) -> None:
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
+        all_logits = torch.cat([pred["logits"] for pred in self.test_step_outputs])
         all_probs = F.softmax(all_logits, dim=-1)
         labels_probs = [all_probs[:, i] for i in range(all_probs.shape[-1])]
 
         self.log_eval_report(labels_probs)
         self.s_test_scorer.reset()
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/distillation/utils/labeler.py` & `bert_squeeze-0.1.1/bert_squeeze/distillation/utils/labeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from collections import defaultdict
 from typing import Any, Dict, List, Tuple, Union
 
 import datasets
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 import torch
 import torch.nn.functional as F
 from datasets import Dataset, DatasetDict
 from omegaconf import DictConfig
 from pkg_resources import resource_filename
 from torch.utils.data import DataLoader
 from tqdm import tqdm
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/inference/model.py` & `bert_squeeze-0.1.1/bert_squeeze/inference/model.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/inference/processors.py` & `bert_squeeze-0.1.1/bert_squeeze/inference/processors.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/base_lt_module.py` & `bert_squeeze-0.1.1/bert_squeeze/models/base_lt_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from copy import deepcopy
 from typing import Dict, List, Tuple
 
+import lightning.pytorch as pl
 import matplotlib.pyplot as plt
 import numpy as np
-import pytorch_lightning as pl
 import seaborn as sns
 import torch
 import torch.nn.functional as F
 from omegaconf import DictConfig, ListConfig
 from torch.nn import CrossEntropyLoss
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from transformers import AdamW, AutoConfig
@@ -46,50 +46,60 @@
         self.num_labels = num_labels
 
         self.pretrained_model = pretrained_model
         self.model_config = AutoConfig.from_pretrained(
             pretrained_model, num_labels=num_labels
         )
 
-        self._set_scorers(training_config.get("scorer_type", "regular"))
+        self.training_step_outputs = []
+        self.test_step_outputs = []
+        self.validation_step_outputs = []
+
+        self._set_scorers(kwargs.get("scorer_type", "regular"))
         self._set_objective()
 
     def forward(self, **kwargs):
         """"""
         raise NotImplementedError()
 
     def training_step(self, batch, batch_idx, *args, **kwargs):
         """"""
         raise NotImplementedError()
 
-    def validation_step(self, batch, batch_idx, *args, **kwargs):
+    def on_train_epoch_end(self) -> None:
         """"""
-        raise NotImplementedError()
+        self.scorer.reset()
+        self.training_step_outputs.clear()
 
-    def test_step(self, batch, batch_idx, *args, **kwargs):
+    def validation_step(self, batch, batch_idx, *args, **kwargs):
         """"""
         raise NotImplementedError()
 
-    def training_epoch_end(self, _) -> None:
+    def on_validation_epoch_end(self):
         """"""
-        self.scorer.reset()
-
-    def validation_epoch_end(self, test_step_outputs: List[dict]):
-        """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
-        all_probs = F.softmax(all_logits, dim=-1)
-        labels_probs = all_probs.numpy()
+        if not self.trainer.sanity_checking:
+            all_logits = torch.cat(
+                [pred["logits"] for pred in self.validation_step_outputs]
+            )
+            all_probs = F.softmax(all_logits, dim=-1)
+            labels_probs = all_probs.numpy()
+            self.log_eval_report(labels_probs)
 
-        self.log_eval_report(labels_probs)
         self.valid_scorer.reset()
+        self.validation_step_outputs.clear()
 
-    def test_epoch_end(self, outputs) -> None:
+    def test_step(self, batch, batch_idx, *args, **kwargs):
+        """"""
+        raise NotImplementedError()
+
+    def on_test_epoch_end(self) -> None:
         """"""
         self.log("Test results", self.test_scorer.get_table())
         self.test_scorer.reset()
+        self.test_step_outputs.clear()
 
     def configure_optimizers(self) -> Tuple[List, List]:
         """
         Method to define optimizers and learning rate schedulers
 
         Returns:
             Tuple[List, List]: a tuple of containing a list of optimizers and
@@ -321,42 +331,41 @@
 
         Args:
             logits (torch.Tensor):
                 predicted logits
             labels (torch.Tensor):
                 ground truth labels
         """
-        return self.objective(logits.view(-1, self.num_labels), labels.view(-1))
+        return self.objective(logits.view(-1, self.num_labels), labels.view(-1).long())
 
     def log_eval_report(self, probs: np.array) -> None:
         """
         Method that logs an evaluation report.
 
         It uses the evaluation scorer to log all the available losses, metrics as well as
         the probability distribution of all labels.
 
         Args:
             probs (np.array):
                 predicted probabilities
         """
         table = self.valid_scorer.get_table()
-        self.logger.experiment["eval/report"].log(table)
+        self.logger.experiment.add_text("eval/report", table)
 
         logging_loss = {
             key: torch.stack(val).mean() for key, val in self.valid_scorer.losses.items()
         }
-        for key, value in logging_loss.items():
-            self.logger.experiment[f"eval/loss_{key}"].log(value)
+        self.log_dict({f"eval/loss_{key}": val for key, val in logging_loss.items()})
 
         eval_report = self.valid_scorer.to_dict()
-        for key, value in eval_report.items():
-            if not isinstance(value, list) and not isinstance(value, np.ndarray):
-                self.logger.experiment["eval/{}".format(key)].log(
-                    value=value, step=self.global_step
-                )
+        for metric, value in eval_report.items():
+            if isinstance(value, dict):
+                self.log_dict({f"eval/{metric}/{key}": v for key, v in value.items()})
+            elif not isinstance(value, list) and not isinstance(value, np.ndarray):
+                self.log("eval/{}".format(metric), value)
 
         for i in range(probs.shape[1]):
             fig = plt.figure(figsize=(15, 15))
-            sns.distplot(probs[:, i], kde=False, bins=100)
+            sns.histplot(probs[:, i], bins=100)
             plt.title("Probability boxplot for label {}".format(i))
-            self.logger.experiment["eval/dist_label_{}".format(i)].log(fig)
+            self.logger.experiment.add_figure("eval/dist_label_{}".format(i), fig)
             plt.close("all")
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/bert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/bert.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/deebert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/deebert.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/fastbert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/fastbert.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/custom_transformers/theseus_bert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/custom_transformers/theseus_bert.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/layers/classifier.py` & `bert_squeeze-0.1.1/bert_squeeze/models/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/layers/mha.py` & `bert_squeeze-0.1.1/bert_squeeze/models/layers/mha.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lr.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
-from typing import List
 
+import lightning.pytorch as pl
 import matplotlib.pyplot as plt
 import numpy as np
-import pytorch_lightning as pl
 import seaborn as sns
 import torch
 import torch.nn.functional as F
 from omegaconf import DictConfig
 from torch.nn import CrossEntropyLoss
 from torch.optim import Adam
 
@@ -33,72 +32,72 @@
     ):
         super().__init__()
         self._sanity_checks(training_config)
         self.config = training_config
         self.num_labels = num_labels
         self.vocab_size = vocab_size
 
+        self.training_step_outputs = []
+        self.test_step_outputs = []
+        self.validation_step_outputs = []
+
         self._build_model()
         self._set_objective()
         self._set_scorers()
 
     def forward(self, features: torch.Tensor = None, **kwargs) -> torch.Tensor:
         """
         Args:
             features (torch.Tensor):
                 Features tensor to feed to the Logistic Regression
         Returns:
             torch.Tensor: model's predictions
         """
         return self.classifier(features.float())
 
-    def training_step(self, batch, batch_idx, *args, **kwargs):
+    def training_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         logits = self.forward(**batch)
         loss = self.loss(logits, batch["labels"])
 
         self.scorer.add(logits, batch["labels"], loss.detach().cpu())
 
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
         return loss
 
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         logits = self.forward(**batch)
         loss = self.loss(logits, batch["labels"])
 
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu()}
+        self.validation_step_outputs.append({"loss": loss, "logits": logits.cpu()})
+        return loss
 
-    def validation_epoch_end(self, test_step_outputs: List[dict]):
+    def on_validation_epoch_end(self):
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
+        all_logits = torch.cat([pred["logits"] for pred in self.validation_step_outputs])
         all_probs = F.softmax(all_logits, dim=-1)
         labels_probs = all_probs.numpy()
 
         self.log_eval_report(labels_probs)
         self.valid_scorer.reset()
 
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         loss, logits = self.shared_step(batch)
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu()}
+        self.test_step_outputs.append({"loss": loss, "logits": logits.cpu()})
+        return loss
 
     def configure_optimizers(self) -> Adam:
         """
         Method to define optimizer to use for training
 
         Returns:
             Adam: optimizer used for training
@@ -181,28 +180,25 @@
         the probability distribution of all labels.
 
         Args:
             probs (np.array):
                 predicted probabilities by the model
         """
         table = self.valid_scorer.get_table()
-        self.logger.experiment["eval/report"].log(table)
+        self.logger.experiment.add_text("eval/report", table)
 
         logging_loss = {
             key: torch.stack(val).mean() for key, val in self.valid_scorer.losses.items()
         }
-        for key, value in logging_loss.items():
-            self.logger.experiment[f"eval/loss_{key}"].log(value)
+        self.log_dict({f"eval/loss_{key}": val for key, val in logging_loss.items()})
 
         eval_report = self.valid_scorer.to_dict()
         for key, value in eval_report.items():
             if not isinstance(value, list) and not isinstance(value, np.ndarray):
-                self.logger.experiment["eval/{}".format(key)].log(
-                    value=value, step=self.global_step
-                )
+                self.log("eval/{}".format(key), value)
 
         for i in range(probs.shape[1]):
             fig = plt.figure(figsize=(15, 15))
             sns.distplot(probs[:, i], kde=False, bins=100)
             plt.title("Probability boxplot for label {}".format(i))
-            self.logger.experiment["eval/dist_label_{}".format(i)].log(fig)
+            self.logger.experiment.add_figure("eval/dist_label_{}".format(i), fig)
             plt.close("all")
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lstm.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lstm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import List
 
+import lightning.pytorch as pl
 import matplotlib.pyplot as plt
 import numpy as np
-import pytorch_lightning as pl
 import seaborn as sns
 import torch
 import torch.nn.functional as F
 from omegaconf import DictConfig
 from torch.autograd import Variable
 from torch.nn import CrossEntropyLoss
 from torch.optim import Adam
@@ -44,14 +44,18 @@
         self._sanity_checks(training_config)
 
         self.config = training_config
         self.vocab_size = vocab_size
         self.hidden_dim = hidden_dim
         self.num_labels = num_labels
 
+        self.training_step_outputs = []
+        self.test_step_outputs = []
+        self.validation_step_outputs = []
+
         self._set_scorers()
         self._set_objective()
         self._build_model()
 
     def forward(self, tokens: torch.Tensor) -> torch.Tensor:
         """
         Args:
@@ -79,51 +83,51 @@
         loss = self.loss(logits, batch["labels"])
 
         self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
         return loss
 
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         logits = self.forward(tokens=batch["features"])
         loss = self.loss(logits, batch["labels"])
 
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
-
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
-        """"""
-        logits = self.forward(tokens=batch["features"])
-        loss = self.loss(logits, batch["labels"])
-
-        self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
-    def validation_epoch_end(self, test_step_outputs: List[dict]) -> None:
+    def on_validation_epoch_end(self) -> None:
         """"""
-        all_logits = torch.cat([pred["logits"] for pred in test_step_outputs])
+        all_logits = torch.cat([pred["logits"] for pred in self.validation_step_outputs])
         all_probs = F.softmax(all_logits, dim=-1)
         labels_probs = all_probs.numpy()
 
         self.log_eval_report(labels_probs)
         self.valid_scorer.reset()
 
-    def test_epoch_end(self, outputs) -> None:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
+        """"""
+        logits = self.forward(tokens=batch["features"])
+        loss = self.loss(logits, batch["labels"])
+
+        self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
+        self.test_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
+
+    def on_test_epoch_end(self) -> None:
         """"""
         print(self.test_scorer.get_table())
         self.test_scorer.reset()
 
     def configure_optimizers(self) -> Adam:
         """
         Method to define optimizer to use for training
@@ -214,28 +218,25 @@
         the probability distribution of all labels.
 
         Args:
             probs (np.array):
                 predicted probabilities
         """
         table = self.valid_scorer.get_table()
-        self.logger.experiment["eval/report"].log(table)
+        self.logger.experiment.add_text("eval/report", table)
 
         logging_loss = {
             key: torch.stack(val).mean() for key, val in self.valid_scorer.losses.items()
         }
-        for key, value in logging_loss.items():
-            self.logger.experiment[f"eval/loss_{key}"].log(value)
+        self.log_dict({f"eval/loss_{key}": val for key, val in logging_loss.items()})
 
         eval_report = self.valid_scorer.to_dict()
         for key, value in eval_report.items():
             if not isinstance(value, list) and not isinstance(value, np.ndarray):
-                self.logger.experiment["eval/{}".format(key)].log(
-                    value=value, step=self.global_step
-                )
+                self.log("eval/{}".format(key), value)
 
         for i in range(probs.shape[1]):
             fig = plt.figure(figsize=(15, 15))
             sns.distplot(probs[:, i], kde=False, bins=100)
             plt.title("Probability boxplot for label {}".format(i))
-            self.logger.experiment["eval/dist_label_{}".format(i)].log(fig)
+            self.logger.experiment.add_figure("eval/dist_label_{}".format(i), fig)
             plt.close("all")
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lt_bert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lt_bert.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,59 +80,58 @@
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"])
 
         self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"eval/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
-
         return loss
 
     @overrides
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"].float())
 
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
     @overrides
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"])
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.test_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
     @overrides
     def _build_model(self):
         """"""
         self.encoder = CustomBertModel.from_pretrained(self.pretrained_model)
         self.classifier = torch.nn.Sequential(
             torch.nn.Dropout(self.model_config.hidden_dropout_prob),
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lt_deebert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lt_deebert.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,68 @@
             ramps_exits = outputs[-1]
             exit_layer = e.exit_layer
             logits = outputs[0]
 
         return logits, ramps_exits, exit_layer
 
     @overrides
+    def training_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
+        """"""
+        inputs = {
+            "input_ids": batch["input_ids"],
+            "attention_mask": batch["attention_mask"],
+            "token_type_ids": batch["token_type_ids"],
+        }
+        logits, ramps_exits, exit_layer = self.forward(**inputs)
+        loss = self.loss(
+            logits=logits, labels=batch["labels"], train_ramps=self.train_highway
+        )
+
+        self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
+        if (
+            self.config.logging_steps > 0
+            and self.global_step % self.config.logging_steps == 0
+        ):
+            logging_loss = {
+                key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
+            }
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
+            self.scorer.reset()
+
+        return loss
+
+    @overrides
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
+        """"""
+        inputs = {
+            "input_ids": batch["input_ids"],
+            "attention_mask": batch["attention_mask"],
+            "token_type_ids": batch["token_type_ids"],
+        }
+        logits, ramps_exits, exit_layer = self.forward(**inputs)
+        loss = self.loss(
+            logits=logits, labels=batch["labels"], train_ramps=self.train_highway
+        )
+        self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
+        self.validation_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
+
+    def on_validation_epoch_end(self) -> None:
+        """"""
+        all_logits = torch.cat([pred["logits"] for pred in self.validation_step_outputs])
+        all_probs = F.softmax(all_logits, dim=-1)
+        labels_probs = all_probs.numpy()
+
+        self.log_eval_report(labels_probs)
+        self.valid_scorer.reset()
+
+    @overrides
     def _get_optimizer_parameters(self) -> List[Dict]:
         """
         Method that defines the parameter to optimize.
 
         Returns:
             List[Dict]: group of parameters to optimize
         """
@@ -275,87 +329,34 @@
             loss_fct = CrossEntropyLoss()
             loss = loss_fct(
                 logits.view(-1, self.model_config.num_labels), labels.view(-1)
             )
         return loss
 
     @overrides
-    def training_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
-        """"""
-        inputs = {
-            "input_ids": batch["input_ids"],
-            "attention_mask": batch["attention_mask"],
-            "token_type_ids": batch["token_type_ids"],
-        }
-        logits, ramps_exits, exit_layer = self.forward(**inputs)
-        loss = self.loss(
-            logits=logits, labels=batch["labels"], train_ramps=self.train_highway
-        )
-
-        self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
-        if (
-            self.config.logging_steps > 0
-            and self.global_step % self.config.logging_steps == 0
-        ):
-            logging_loss = {
-                key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
-            }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(value)
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
-            self.scorer.reset()
-
-        return loss
-
-    @overrides
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
-        """"""
-        inputs = {
-            "input_ids": batch["input_ids"],
-            "attention_mask": batch["attention_mask"],
-            "token_type_ids": batch["token_type_ids"],
-        }
-        logits, ramps_exits, exit_layer = self.forward(**inputs)
-        loss = self.loss(
-            logits=logits, labels=batch["labels"], train_ramps=self.train_highway
-        )
-        self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
-
-    @overrides
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> Dict[str, torch.Tensor]:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits, ramps_exits, exit_layer = self.forward(**inputs)
         loss = self.loss(
             logits=logits, labels=batch["labels"], train_ramps=self.train_highway
         )
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
-
-    def validation_epoch_end(self, outputs: List[dict]) -> torch.Tensor:
-        """"""
-        all_logits = torch.cat([pred["logits"] for pred in outputs])
-        all_probs = F.softmax(all_logits, dim=-1)
-        labels_probs = all_probs.numpy()
-
-        self.log_eval_report(labels_probs)
-        self.valid_scorer.reset()
-        return torch.stack([out["loss"] for out in outputs]).mean()
+        self.test_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
-    def test_epoch_end(self, _) -> None:
+    def on_test_epoch_end(self) -> None:
         """"""
-        logging.log(self.test_scorer.get_table())
+        logging.info(self.test_scorer.get_table())
         self.test_scorer.reset()
 
     @overrides
     def _build_model(self):
         """"""
         self.bert = DeeBertModel(self.model_config)
         self.num_layers = len(self.bert.encoder.layer)
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lt_distilbert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lt_distilbert.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,53 +74,54 @@
         loss = self.loss(logits, batch["labels"])
 
         self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
 
         return loss
 
     @overrides
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
         }
 
         logits = self.forward(**inputs)
         loss = self.loss(logits, batch["labels"])
 
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
     @overrides
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
         }
 
         logits = self.forward(**inputs)
         loss = self.loss(logits, batch["labels"])
 
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.test_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
+        return loss
 
     @overrides
     def _build_model(self):
         """"""
         self.encoder = AutoModel.from_pretrained(self.pretrained_model)
         self.classifier = torch.nn.Sequential(
             torch.nn.Dropout(self.model_config.seq_classif_dropout),
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lt_fastbert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lt_fastbert.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,25 +99,25 @@
         # effectively the same as removing these entirely.
         extended_attention_mask = extended_attention_mask.float()
         extended_attention_mask = (1.0 - extended_attention_mask) * -10000.0
 
         embedding_output = self.embeddings(input_ids, token_type_ids)
 
         output = self.encoder(
-            hidden_states=embedding_output,
+            embeddings=embedding_output,
             attention_mask=extended_attention_mask,
             device=self.device,
             inference=inference,
             inference_speed=inference_speed,
             training_stage=training_stage,
         )
         return output
 
     @overrides
-    def training_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def training_step(self, batch, batch_idx, *args, **kwargs) -> torch.Tensor:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
             "training_stage": self.training_stage,
         }
@@ -134,28 +134,22 @@
             logits = outputs[:-1]
 
         self.scorer.add(logits, batch["labels"], losses)
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
 
-        return {"loss": losses.full_loss}
+        return losses.full_loss
 
     @overrides
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> None:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
             "training_stage": self.training_stage,
         }
@@ -167,18 +161,20 @@
             # "outputs" is logits from the last classification layer
             logits = outputs
         else:
             # outputs[-1] is log prob from the last classification layer
             # outputs[:-1] is list of all the student classification layers logits
             logits = outputs[:-1]
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), losses)
-        return {"loss": losses.full_loss, "logits": logits.cpu()}
+        self.validation_step_outputs.append(
+            {"loss": losses.full_loss, "logits": logits.cpu()}
+        )
 
     @overrides
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> None:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
             "training_stage": self.training_stage,
         }
@@ -187,15 +183,15 @@
         losses = self.loss(outputs, batch["labels"])
 
         # outputs[-1] is log prob from the last classification layer
         # outputs[:-1] is list of all the student classification layers logits
         logits = outputs[:-1]
 
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), losses)
-        return {"loss": losses.full_loss, "logits": logits.cpu()}
+        self.test_step_outputs.append({"loss": losses.full_loss, "logits": logits.cpu()})
 
     @overrides
     def _build_model(self):
         """"""
         self.embeddings = BertEmbeddings(self.model_config)
         self.encoder = FastBertGraph(self.model_config)
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/models/lt_theseus_bert.py` & `bert_squeeze-0.1.1/bert_squeeze/models/lt_theseus_bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,58 +95,56 @@
 
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"])
 
         self.scorer.add(logits.detach().cpu(), batch["labels"], loss.detach().cpu())
         if self.global_step > 0 and self.global_step % self.config.logging_steps == 0:
             logging_loss = {
                 key: torch.stack(val).mean() for key, val in self.scorer.losses.items()
             }
-            for key, value in logging_loss.items():
-                self.logger.experiment[f"train/loss_{key}"].log(
-                    value=value, step=self.global_step
-                )
-
-            self.logger.experiment["train/acc"].log(
-                self.scorer.acc, step=self.global_step
-            )
+            self.log_dict({f"train/loss_{key}": val for key, val in logging_loss.items()})
+            self.log("train/acc", self.scorer.acc)
             self.scorer.reset()
 
         return loss
 
     @overrides
-    def validation_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def validation_step(self, batch, batch_idx, *args, **kwargs) -> None:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"])
         self.valid_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.validation_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
 
     @overrides
-    def test_step(self, batch, batch_idx, *args, **kwargs) -> dict:
+    def test_step(self, batch, batch_idx, *args, **kwargs) -> None:
         """"""
         inputs = {
             "input_ids": batch["input_ids"],
             "attention_mask": batch["attention_mask"],
             "token_type_ids": batch["token_type_ids"],
         }
         logits = self.forward(**inputs)
-        loss = self.loss(logits, batch["labels"])
+        loss = self.loss(logits=logits, labels=batch["labels"])
         self.test_scorer.add(logits.cpu(), batch["labels"].cpu(), loss.cpu())
-        return {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        self.test_step_outputs.append(
+            {"loss": loss, "logits": logits.cpu(), "labels": batch["labels"].cpu()}
+        )
 
     @overrides
     def _build_model(self):
         """"""
         encoder = TheseusBertModel(AutoConfig.from_pretrained(self.pretrained_model))
         encoder.from_pretrained(self.pretrained_model)
         encoder.encoder.init_successor_layers()
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/artifacts/distillation_artifacts.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/artifacts/distillation_artifacts.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/artifacts/transformer_artifacts.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/artifacts/transformer_artifacts.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/checkpointing.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/checkpointing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ##########################################
 ########## Code from andrewjong ##########
 ##########################################
 import os
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 
 
 class CheckpointEveryNSteps(pl.Callback):
     """
     Save a checkpoint every N steps, instead of Lightning's default that checkpoints
     based on validation loss.
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/fastbert_logic.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/fastbert_logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import pytorch_lightning as pl
-from pytorch_lightning.callbacks import BaseFinetuning
+import lightning.pytorch as pl
+from lightning.pytorch.callbacks import BaseFinetuning
 from torch.optim.optimizer import Optimizer
 
 
 class FastBertLogic(BaseFinetuning):
     """
     Callback freezing the model backbone after 'freeze_at_epoch' epochs.
 
@@ -27,28 +27,22 @@
             pl_module:
         """
         assert (
             pl_module.training_stage == 0
         ), "The 'training_stage' should be 0 when starting to finetune FastBert."
 
     def finetune_function(
-        self,
-        pl_module: pl.LightningModule,
-        current_epoch: int,
-        optimizer: Optimizer,
-        optimizer_idx: int,
+        self, pl_module: pl.LightningModule, current_epoch: int, optimizer: Optimizer
     ) -> None:
         """
         Called when the epoch begins
 
         Args:
             pl_module (pl.LightningModule):
             current_epoch (int):
                 current epoch we are in
             optimizer (Optimizer):
                 optimizer used for training
-            optimizer_idx (int):
-                index of the optimizer to use
         """
         if current_epoch >= self.freeze_at_epoch:
             pl_module.training_stage = 1
             pl_module.freeze_encoder()
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/lottery_ticket.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/lottery_ticket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This code is heavily based on:
 # https://github.com/huggingface/transformers/blob/master/examples/research_projects/bertology/run_bertology.py
 
 import logging
 from datetime import datetime
 from typing import Tuple
 
+import lightning.pytorch as pl
 import numpy as np
-import pytorch_lightning as pl
 import torch
 from pytorch_lightning.callbacks.base import Callback
 from sklearn.metrics import accuracy_score, f1_score, precision_score, recall_score
 from torch.utils.data import DataLoader
 from tqdm import tqdm
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/callbacks/pruning.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/callbacks/pruning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, List, Union
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 import torch
-from pytorch_lightning.callbacks.base import Callback
+from lightning.pytorch.callbacks import Callback
 from torch.optim import Optimizer
 
 STEP_OUTPUT = Union[torch.Tensor, Dict[str, Any]]
 
 
 class ThresholdBasedPruning(Callback):
     """
@@ -21,37 +21,31 @@
         start_pruning_epoch (int):
             epoch from which to apply the pruning strategy
     """
 
     def __init__(
         self, threshold: float, start_pruning_epoch: int = 10, *args: Any, **kwargs: Any
     ):
-        super().__init__(*args, **kwargs)
+        super().__init__()
         self.threshold = threshold
         self.start_pruning_epoch = start_pruning_epoch
 
     def on_before_optimizer_step(
-        self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        optimizer: Optimizer,
-        optimizer_idx: int,
+        self, trainer: pl.Trainer, pl_module: pl.LightningModule, optimizer: Optimizer
     ) -> None:
         """
         Method called before `optimizer.step()` to zero prune gradients
 
         Args:
             trainer (pl.Trainer):
                 Lightning trainer
             pl_module (pl.LightningModule):
                 Lightning module
             optimizer (Optimizer):
                 optimizer used for training
-            optimizer_idx (int):
-                index of the optimizer to use
 
         """
         if pl_module.current_epoch >= self.start_pruning_epoch != -1:
             self._zero_pruned_gradients(pl_module)
 
     def on_train_epoch_end(
         self, trainer: pl.Trainer, pl_module: pl.LightningModule
@@ -77,25 +71,32 @@
 
         Args:
             trainer (pl.Trainer):
                 Lightning trainer
             pl_module (pl.LightningModule):
                 Lightning module
         """
+        print("Pruning model...")
         if self.start_pruning_epoch == -1:
             self._prune_model(pl_module)
 
     def _prune_model(self, pl_module: pl.LightningModule) -> None:
         """
         Method used to zero parameters which magnitude are below `self.threshold`.
 
         Args:
             pl_module (pl.LightningModule):
                 Lightning module
         """
+        try:
+            # Only prune the student when performing distillation
+            pl_module = pl_module.get_submodule("student")
+        except AttributeError:
+            pass
+
         for name, param in pl_module.named_parameters():
             if "weight" in name:
                 param_mask = torch.abs(param) < self.threshold
                 param.data[param_mask] = 0.0
 
     @staticmethod
     def _zero_pruned_gradients(pl_module: pl.LightningModule) -> None:
@@ -169,11 +170,17 @@
 
         Args:
             threshold (float):
                 value below which weights will be pruned
             pl_module (pl.LightningModule):
                 Lightning module
         """
+        try:
+            # Only prune the student when performing distillation
+            pl_module = pl_module.get_submodule("student")
+        except AttributeError:
+            pass
+
         with torch.no_grad():
             for param in pl_module.parameters():
                 mask = torch.lt(torch.abs(param), threshold)
                 param.data[mask] = 0.0
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/losses/distillation_losses.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/losses/distillation_losses.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/losses/losses.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/losses/losses.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,8 +28,11 @@
     Args:
         p (torch.Tensor):
             tensor of predicted probabilities
     Returns:
         torch.Tensor:
             entropy of the predicted probabilities
     """
-    return torch.distributions.Categorical(probs=p).entropy()
+    try:
+        return torch.distributions.Categorical(probs=p).entropy()
+    except ValueError:
+        return torch.distributions.Categorical(logits=p).entropy()
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/losses/lsl.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/losses/lsl.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/losses/romebert_loss.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/losses/romebert_loss.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/optimizers/bert_adam.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/optimizers/bert_adam.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/schedulers/theseus_schedulers.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/schedulers/theseus_schedulers.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/scorers/scorer.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/scorers/scorer_fast.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/scorers/scorer_fast.py`

 * *Files 8% similar despite different names*

```diff
@@ -155,18 +155,18 @@
                 self.losses[attr].append(getattr(loss, attr).detach())
         else:
             raise TypeError(f"Got 'loss' with type: {type(loss)}")
 
     def to_dict(self) -> Dict[str, Dict[str, float]]:
         """"""
         return {
-            "acc": self.acc,
-            "prec": self.precision,
-            "rec": self.recall,
-            "f1": self.f1,
+            "acc": {key: np.mean(val) for key, val in self.acc.items()},
+            "prec": {key: np.mean(val) for key, val in self.precision.items()},
+            "rec": {key: np.mean(val) for key, val in self.recall.items()},
+            "f1": {key: np.mean(val) for key, val in self.f1.items()},
         }
 
     def reset(self) -> None:
         """
         Resets the confusion matrix, batch counter and losses.
         This method should be called after logging metrics.
         """
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/types.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/types.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/utils_fct.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/utils_fct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections.abc
 import logging
 import os
 import sys
 from typing import List
 
-import pytorch_lightning as pl
+import lightning.pytorch as pl
 from omegaconf import DictConfig, OmegaConf
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 
 
 def load_model_from_exp(
     path_to_folder: str, module: pl.LightningModule
@@ -83,13 +83,20 @@
     if args.train.get("objective", None):
         tags.append(args.train.objective)
     tags.append(args.train.optimizer)
     return tags
 
 
 def deep_update(d, u):
+    """"""
+    if isinstance(u, list):
+        if d is None:
+            return u
+        d.extend(u)
+        return d
+
     for k, v in u.items():
         if isinstance(v, collections.abc.Mapping):
             d[k] = deep_update(d.get(k, {}), v)
         else:
             d[k] = v
     return d
```

### Comparing `bert_squeeze-0.1.0/bert_squeeze/utils/vocabulary.py` & `bert_squeeze-0.1.1/bert_squeeze/utils/vocabulary.py`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/images/bert-squeeze.png` & `bert_squeeze-0.1.1/images/bert-squeeze.png`

 * *Files identical despite different names*

### Comparing `bert_squeeze-0.1.0/pyproject.toml` & `bert_squeeze-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bert-squeeze"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tools for Transformers compression using PyTorch Lightning"
 authors = ["JulesBelveze <jules.belveze@hotmail.fr>"]
 keywords = ["nlp", "transformers", "bert"]
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Text Processing"
 ]
@@ -15,39 +15,40 @@
     "images/"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 transformers = "^4.20.0"
 torch = "^2.0.1"
-numpy = "^1.20.3"
+numpy = "<1.20.0"
 tabulate = "^0.8.9"
 overrides = "^6.1.0"
 python-dotenv = "^0.18.0"
 datasets = "^1.8.0"
 neptune-client = { extras = ["pytorch-lightning"], version = "^0.14.0" }
 omegaconf = "^2.1.0"
 lightning = "^2.0.0"
 psutil = "^5.8.0"
 hydra-core = "^1.1.1"
-matplotlib = "^3.7.1"
+matplotlib = "<3.7.1"
 seaborn = "^0.12.2"
 scikit-learn = "^1.2.2"
 huggingface-hub = "0.13.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "<7.0"
 furo = "^2023.3.27"
 autodoc-pydantic = "^1.8.0"
 sphinxext-opengraph = "^0.8.2"
 sphinx-copybutton = "^0.5.2"
 myst-parser = "^1.0.0"
+nbsphinx = "^0.9.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 ipdb = "^0.13.13"
@@ -55,15 +56,15 @@
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 
 
 [tool.poetry.group.inference.dependencies]
-onnxruntime = "^1.15.0"
+onnxruntime = "<1.15.0"
 
 [tool.black]
 line-length = 90
 skip-string-normalization = true
 target-version = ["py38"]
 
 [tool.isort]
```

### Comparing `bert_squeeze-0.1.0/setup.py` & `bert_squeeze-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,39 +19,37 @@
  'bert_squeeze.utils.errors',
  'bert_squeeze.utils.losses',
  'bert_squeeze.utils.optimizers',
  'bert_squeeze.utils.schedulers',
  'bert_squeeze.utils.scorers']
 
 package_data = \
-{'': ['*'],
- 'bert_squeeze.assistants': ['configs/*'],
- 'bert_squeeze.data.local_datasets': ['parallel/*']}
+{'': ['*'], 'bert_squeeze.assistants': ['configs/*']}
 
 install_requires = \
 ['datasets>=1.8.0,<2.0.0',
  'huggingface-hub==0.13.4',
  'hydra-core>=1.1.1,<2.0.0',
  'lightning>=2.0.0,<3.0.0',
- 'matplotlib>=3.7.1,<4.0.0',
+ 'matplotlib<3.7.1',
  'neptune-client[pytorch-lightning]>=0.14.0,<0.15.0',
- 'numpy>=1.20.3,<2.0.0',
+ 'numpy<1.20.0',
  'omegaconf>=2.1.0,<3.0.0',
  'overrides>=6.1.0,<7.0.0',
  'psutil>=5.8.0,<6.0.0',
  'python-dotenv>=0.18.0,<0.19.0',
  'scikit-learn>=1.2.2,<2.0.0',
  'seaborn>=0.12.2,<0.13.0',
  'tabulate>=0.8.9,<0.9.0',
  'torch>=2.0.1,<3.0.0',
  'transformers>=4.20.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'bert-squeeze',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Tools for Transformers compression using PyTorch Lightning',
     'long_description': 'None',
     'author': 'JulesBelveze',
     'author_email': 'jules.belveze@hotmail.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bert_squeeze-0.1.0/PKG-INFO` & `bert_squeeze-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-squeeze
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for Transformers compression using PyTorch Lightning
 Keywords: nlp,transformers,bert
 Author: JulesBelveze
 Author-email: jules.belveze@hotmail.fr
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Requires-Dist: datasets (>=1.8.0,<2.0.0)
 Requires-Dist: huggingface-hub (==0.13.4)
 Requires-Dist: hydra-core (>=1.1.1,<2.0.0)
 Requires-Dist: lightning (>=2.0.0,<3.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: matplotlib (<3.7.1)
 Requires-Dist: neptune-client[pytorch-lightning] (>=0.14.0,<0.15.0)
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: numpy (<1.20.0)
 Requires-Dist: omegaconf (>=2.1.0,<3.0.0)
 Requires-Dist: overrides (>=6.1.0,<7.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: python-dotenv (>=0.18.0,<0.19.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
```

