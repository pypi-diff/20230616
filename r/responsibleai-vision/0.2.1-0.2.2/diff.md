# Comparing `tmp/responsibleai_vision-0.2.1.tar.gz` & `tmp/responsibleai_vision-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.2.1.tar", last modified: Wed May 31 18:48:38 2023, max compression
+gzip compressed data, was "responsibleai_vision-0.2.2.tar", last modified: Fri Jun 16 18:59:55 2023, max compression
```

## Comparing `responsibleai_vision-0.2.1.tar` & `responsibleai_vision-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:38.051345 responsibleai_vision-0.2.1/
--rw-rw-rw-   0        0        0     1403 2023-05-31 18:48:38.050342 responsibleai_vision-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.797791 responsibleai_vision-0.2.1/responsibleai_vision/
--rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.871887 responsibleai_vision-0.2.1/responsibleai_vision/common/
--rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/constants.py
--rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/interfaces.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.908697 responsibleai_vision-0.2.1/responsibleai_vision/managers/
--rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/__init__.py
--rw-rw-rw-   0        0        0    13897 2023-05-05 19:17:38.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/error_analysis_manager.py
--rw-rw-rw-   0        0        0    26315 2023-05-04 17:50:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/explainer_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.932563 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/
--rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/__init__.py
--rw-rw-rw-   0        0        0    46805 2023-05-31 14:23:26.000000 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.981601 responsibleai_vision-0.2.1/responsibleai_vision/utils/
--rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/__init__.py
--rw-rw-rw-   0        0        0     2443 2023-05-12 20:02:09.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/feature_extractors.py
--rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/image_reader.py
--rw-rw-rw-   0        0        0     2880 2023-05-30 17:49:11.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/image_utils.py
--rw-rw-rw-   0        0        0      194 2023-05-31 18:43:36.000000 responsibleai_vision-0.2.1/responsibleai_vision/version.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.839844 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/
--rw-rw-rw-   0        0        0     1403 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 18:48:38.052494 responsibleai_vision-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:48:38.046193 responsibleai_vision-0.2.1/tests/
--rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_automl_images_insights.py
--rw-rw-rw-   0        0        0     8318 2023-05-30 17:49:11.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_insights.py
--rw-rw-rw-   0        0        0     3401 2023-05-31 14:23:26.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.839594 responsibleai_vision-0.2.2/
+-rw-rw-rw-   0        0        0     1403 2023-06-16 18:59:55.836377 responsibleai_vision-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.332246 responsibleai_vision-0.2.2/responsibleai_vision/
+-rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.459308 responsibleai_vision-0.2.2/responsibleai_vision/common/
+-rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/__init__.py
+-rw-rw-rw-   0        0        0     2634 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/constants.py
+-rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.2/responsibleai_vision/common/interfaces.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.551491 responsibleai_vision-0.2.2/responsibleai_vision/managers/
+-rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/__init__.py
+-rw-rw-rw-   0        0        0    13897 2023-05-05 19:17:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/error_analysis_manager.py
+-rw-rw-rw-   0        0        0    26875 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/managers/explainer_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.607855 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/
+-rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-rw-rw-   0        0        0    50360 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.718725 responsibleai_vision-0.2.2/responsibleai_vision/utils/
+-rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/__init__.py
+-rw-rw-rw-   0        0        0     2443 2023-05-12 20:02:09.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/feature_extractors.py
+-rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/image_reader.py
+-rw-rw-rw-   0        0        0     4907 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/responsibleai_vision/utils/image_utils.py
+-rw-rw-rw-   0        0        0      194 2023-06-16 18:59:00.000000 responsibleai_vision-0.2.2/responsibleai_vision/version.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.396288 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/
+-rw-rw-rw-   0        0        0     1403 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-16 18:59:54.000000 responsibleai_vision-0.2.2/responsibleai_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:59:55.840618 responsibleai_vision-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:59:55.827954 responsibleai_vision-0.2.2/tests/
+-rw-rw-rw-   0        0        0     2067 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/tests/test_image_utils.py
+-rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_automl_images_insights.py
+-rw-rw-rw-   0        0        0    12099 2023-06-16 18:35:38.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_insights.py
+-rw-rw-rw-   0        0        0     3088 2023-06-08 15:48:16.000000 responsibleai_vision-0.2.2/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.2.1/PKG-INFO` & `responsibleai_vision-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.1/README.md` & `responsibleai_vision-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.2.2/responsibleai_vision/common/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     Can be 'image_url', 'image' or 'label'.
     """
 
     IMAGE_URL = 'image_url'
     IMAGE = 'image'
     LABEL = 'label'
+    IMAGE_DETAILS = 'image_details'
 
 
 class ExplainabilityLiterals:
     """Parameters for explainability method names."""
 
     MODEL_EXPLAINABILITY = 'model_explainability'
     XAI_PARAMETERS = 'xai_parameters'
@@ -58,14 +59,17 @@
     """DEFAULT values for explainability parameters."""
 
     MODEL_EXPLAINABILITY = False
     XAI_ALGORITHM = ExplainabilityLiterals.GUIDEDGRADCAM_METHOD_NAME
     OUTPUT_VISUALIZATIONS = True
     OUTPUT_ATTRIBUTIONS = False
     CONFIDENCE_SCORE_THRESHOLD_MULTILABEL = 0.5
+    DEFAULT_MAX_EVALS = 100
+    DEFAULT_MASK_RES = 4
+    DEFAULT_NUM_MASKS = 50
 
 
 class XAIPredictionLiterals:
     """Strings that will be keys in the output json during prediction."""
 
     VISUALIZATIONS_KEY_NAME = 'visualizations'
     ATTRIBUTIONS_KEY_NAME = 'attributions'
```

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.2.2/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.2.2/responsibleai_vision/managers/explainer_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,26 +45,35 @@
 CLASSES = 'classes'
 U_EVALUATION_EXAMPLES = '_evaluation_examples'
 FEATURES = 'features'
 META_JSON = Metadata.META_JSON
 MODEL = Metadata.MODEL
 EXPLANATION = '_explanation'
 TASK_TYPE = 'task_type'
+_MAX_EVALS = '_max_evals'
+_NUM_MASKS = '_num_masks'
+_MASK_RES = '_mask_res'
+DEFAULT_MAX_EVALS = ExplainabilityDefaults.DEFAULT_MAX_EVALS
+DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
+DEFAULT_NUM_MASKS = ExplainabilityDefaults.DEFAULT_NUM_MASKS
 
 
 class ExplainerManager(BaseManager):
 
     """Defines the ExplainerManager for explaining an image-based model."""
 
     def __init__(self, model: Any,
                  evaluation_examples: pd.DataFrame,
                  target_column: str,
                  task_type: str,
                  classes: Optional[List] = None,
-                 image_mode: str = None):
+                 image_mode: str = None,
+                 max_evals: Optional[int] = DEFAULT_MAX_EVALS,
+                 num_masks: Optional[int] = DEFAULT_NUM_MASKS,
+                 mask_res: Optional[int] = DEFAULT_MASK_RES):
         """Creates an ExplainerManager object.
 
         :param model: The model to explain.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param evaluation_examples: A matrix of feature vector
@@ -79,14 +88,26 @@
             The order of the class names should match that of the model
             output. Only required if explaining classifier.
         :type classes: list
         :param image_mode: The mode to open the image in.
             See pillow documentation for all modes:
             https://pillow.readthedocs.io/en/stable/handbook/concepts.html
         :type image_mode: str
+        :param max_evals: The maximum number of evaluations to run.
+            Used by shap hierarchical image explainer.
+            If not specified defaults to 100.
+        :type max_evals: int
+        :param num_masks: The number of masks to use for the
+            DRISE image explainer for object detection.
+            If not specified defaults to 50.
+        :type num_masks: int
+        :param mask_res: The resolution of the masks to use for the
+            DRISE image explainer for object detection.
+            If not specified defaults to 4.
+        :type mask_res: int
         """
         self._image_mode = image_mode
         if task_type == ModelTask.OBJECT_DETECTION:
             if is_automl_image_model(model):
                 self._model = MLflowDRiseWrapper(model._model, classes)
             else:
                 self._model = PytorchDRiseWrapper(model._model, len(classes))
@@ -99,14 +120,17 @@
             evaluation_examples.drop(columns=target_column)
         self._is_run = False
         self._is_added = False
         self._features = list(self._evaluation_examples.columns)
         self._classes = classes
         self._explanation = None
         self._task_type = task_type
+        self._max_evals = max_evals
+        self._num_masks = num_masks
+        self._mask_res = mask_res
 
     def add(self):
         """Add an explainer to be computed later."""
         if self._model is None:
             raise UserConfigValidationException(
                 'Model is required for model explanations')
 
@@ -124,78 +148,52 @@
             return
         if self._is_run:
             return
         self._explanation = []
         if self._is_classification_task:
             for i in range(len(self._evaluation_examples)):
                 self._explanation.append(
-                    self.compute_single_explanation(i, max_evals=100, **kwargs)
+                    self.compute_single_explanation(i, **kwargs)
                 )
         elif self._is_object_detection_task:
             for i in range(len(self._evaluation_examples)):
                 self._explanation.append(
-                    self.compute_batch_explanation(i)
+                    self.compute_single_explanation(i, object_index=None)
                 )
         else:
             raise ValueError('Unknown task type: {}'.format(self._task_type))
 
         self._is_run = True
 
-    def compute_batch_explanation(self,
-                                  index):
-        """
-        This function is a subroutine of the compute method.
-        It computes explanations using batching to optimize performance.
-
-        Currently only supported for object detection, in which all
-        explanations per image are computed in parallel (each image
-        may have multiple detections).
-
-        :param index: The index of the image to create the explanation for
-        :type index: int
-
-        :return: The computed explanations on the image level
-        :rtype: list of strings
-        """
-        if self._is_object_detection_task:
-            ex = self._evaluation_examples
-            img = ex.iloc[index:index+1, 0].values[0]
-            try:
-                # calling DRISE to generate saliency maps for all objects
-                fl, _, _, = get_drise_saliency_map(img,
-                                                   self._model,
-                                                   len(self._classes),
-                                                   savename=str(index),
-                                                   nummasks=50,
-                                                   max_figures=5000)
-            except BaseException:
-                fl = [self._get_fail_str()]
-            return fl
-        else:
-            raise ValueError('Unknown task type: {}'.format(self._task_type))
-
     def compute_single_explanation(self,
                                    index,
-                                   max_evals=100,
+                                   max_evals=None,
                                    object_index=0,
                                    **kwargs):
         """Creates an explanation for a single image in the dataset
 
         :param index: The index of the image to create the explanation for
         :type index: int
         :param max_evals: the maximum number of evalutions
         :type max_evals: int
         :param object_index: The index of the object within the image we are
         looking to create the explanation for. Note that saliency maps are
         created one object per image. The default value for this is 0 to
         ensure a modular development process (so this function won't fail
         without an updated frontend). This parameter is only for the object
         detection scenario using the DRISE functionality.
-        :type object_index: int
-        """
+        :type object_index: Optional[int]
+        :return: The explanation for the image, which is a saliency map.
+            For object detection, this can be a list of saliency maps if
+            object index is not specified.
+        :rtype: str or list[str]
+        """
+        if max_evals is None:
+            # if not specified use global max_evals value
+            max_evals = self._max_evals
         self.automl_image_model = is_automl_image_model(self._model)
         if self.automl_image_model:
             # get xai algorithm name
             xai_algo_name = kwargs.get(
                 ExplainabilityLiterals.XAI_ALGORITHM,
                 ExplainabilityDefaults.XAI_ALGORITHM
             )
@@ -249,22 +247,28 @@
                         self._model = MLflowDRiseWrapper(self._model._model,
                                                          self._classes)
                     else:
                         self._model = PytorchDRiseWrapper(self._model._model,
                                                           len(self._classes))
 
                 # calling DRISE to generate saliency maps for all objects
+                mask_res_tuple = (self._mask_res, self._mask_res)
                 fl, _, _, = get_drise_saliency_map(img,
                                                    self._model,
                                                    len(self._classes),
                                                    savename=str(index),
-                                                   nummasks=50,
+                                                   nummasks=self._num_masks,
+                                                   maskres=mask_res_tuple,
                                                    max_figures=5000)
+                if object_index is None:
+                    return fl
                 b64_string = fl[object_index]
             except BaseException:
+                if object_index is None:
+                    return [self._get_fail_str()]
                 b64_string = self._get_fail_str()
             return b64_string
         else:
             raise ValueError('Unknown task type: {}'.format(self._task_type))
 
     def get_shap_explanations(self, image, max_evals):
         """Generates an explanation using shap method.
@@ -634,14 +638,17 @@
             inst.__dict__[EXPLANATION] = None
 
         wrapped_model = wrap_model(rai_insights.model, rai_insights.test,
                                    rai_insights.task_type,
                                    classes=rai_insights._classes)
         inst.__dict__['_' + MODEL] = wrapped_model
         inst.__dict__['_' + CLASSES] = rai_insights._classes
+        inst.__dict__[_MAX_EVALS] = rai_insights.max_evals
+        inst.__dict__[_NUM_MASKS] = rai_insights.num_masks
+        inst.__dict__[_MASK_RES] = rai_insights.mask_res
         target_column = rai_insights.target_column
         if not isinstance(target_column, list):
             target_column = [target_column]
         test = rai_insights.test.drop(columns=target_column)
         inst.__dict__[U_EVALUATION_EXAMPLES] = test
         inst.__dict__['_' + FEATURES] = list(test.columns)
         inst.__dict__['_' + TASK_TYPE] = rai_insights.task_type
```

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.2.2/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,27 +31,36 @@
 from responsibleai.exceptions import UserConfigValidationException
 from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai.rai_insights.rai_base_insights import RAIBaseInsights
 from responsibleai.serialization_utilities import serialize_json_safe
 
 from responsibleai_vision.common.constants import (CommonTags, ImageColumns,
                                                    MLFlowSchemaLiterals,
-                                                   ModelTask)
+                                                   ModelTask,
+                                                   ExplainabilityDefaults)
 from responsibleai_vision.managers.explainer_manager import ExplainerManager
 from responsibleai_vision.managers.error_analysis_manager import (
     ErrorAnalysisManager)
 from responsibleai_vision.utils.feature_extractors import extract_features
 from responsibleai_vision.utils.image_reader import (
     get_base64_string_from_path, get_image_from_path, is_automl_image_model)
-from responsibleai_vision.utils.image_utils import convert_images, get_images
+from responsibleai_vision.utils.image_utils import (
+    convert_images, get_images, transform_object_detection_labels)
 
 IMAGE = ImageColumns.IMAGE.value
 IMAGE_URL = ImageColumns.IMAGE_URL.value
+DEFAULT_MAX_EVALS = ExplainabilityDefaults.DEFAULT_MAX_EVALS
+DEFAULT_NUM_MASKS = ExplainabilityDefaults.DEFAULT_NUM_MASKS
+DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
 _IMAGE_MODE = 'image_mode'
 _IMAGE_DOWNLOADER = 'image_downloader'
+_IMAGE_WIDTH = 'image_width'
+_MAX_EVALS = 'max_evals'
+_NUM_MASKS = 'num_masks'
+_MASK_RES = 'mask_res'
 _PREDICTIONS = 'predictions'
 _TEST = 'test'
 _TARGET_COLUMN = 'target_column'
 _TASK_TYPE = 'task_type'
 _CLASSES = 'classes'
 _META_JSON = Metadata.META_JSON
 _JSON_EXTENSION = '.json'
@@ -101,15 +110,19 @@
                  classes: Optional[np.ndarray] = None,
                  serializer: Optional[Any] = None,
                  maximum_rows_for_test: int = 5000,
                  image_mode: str = "RGB",
                  test_data_path: Optional[str] = None,
                  transformations: Optional[Any] = None,
                  image_downloader: Optional[Any] = None,
-                 feature_metadata: Optional[FeatureMetadata] = None):
+                 feature_metadata: Optional[FeatureMetadata] = None,
+                 image_width: Optional[float] = None,
+                 max_evals: Optional[int] = DEFAULT_MAX_EVALS,
+                 num_masks: Optional[int] = DEFAULT_NUM_MASKS,
+                 mask_res: Optional[int] = DEFAULT_MASK_RES):
         """Creates an RAIVisionInsights object.
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param test: The test dataframe including the label column.
@@ -142,23 +155,56 @@
         :type transformations: object
         :param image_downloader: The image downloader to use to download
             images from a URL.
         :type image_downloader: object
         :param feature_metadata: Feature metadata for the dataset
             to identify different kinds of features.
         :type feature_metadata: Optional[FeatureMetadata]
+        :param image_width: The width to resize the image to.
+            The size is in inches. Note larger resolutions in
+            dashboard can cause slowness and memory errors.
+            If not specified does not resize images.
+        :type image_width: float
+        :param max_evals: The maximum number of evaluations to run.
+            Used by shap hierarchical image explainer.
+            If not specified defaults to 100.
+        :type max_evals: int
+        :param num_masks: The number of masks to use for the
+            DRISE image explainer for object detection.
+            If not specified defaults to 50.
+        :type num_masks: int
+        :param mask_res: The resolution of the masks to use for the
+            DRISE image explainer for object detection.
+            If not specified defaults to 4.
+        :type mask_res: int
         """
         # drop index as this can cause issues later like when copying
         # target column below from test dataset to _ext_test_df
         test = test.reset_index(drop=True)
         if feature_metadata is None:
             # initialize to avoid having to keep checking if it is None
             feature_metadata = FeatureMetadata()
         self._feature_metadata = feature_metadata
         self.image_mode = image_mode
+        self.image_width = image_width
+        if max_evals is None:
+            max_evals = DEFAULT_MAX_EVALS
+        elif max_evals < 1:
+            raise ValueError('max_evals must be greater than 0')
+        if num_masks is None:
+            num_masks = DEFAULT_NUM_MASKS
+        elif num_masks < 1:
+            raise ValueError('num_masks must be greater than 0')
+        if mask_res is None:
+            mask_res = DEFAULT_MASK_RES
+        elif mask_res < 1:
+            raise ValueError('mask_res must be greater than 0')
+        self.max_evals = max_evals
+        self.num_masks = num_masks
+        self.mask_res = mask_res
         self.test_mltable_path = test_data_path
         self._transformations = transformations
         self._image_downloader = image_downloader
         sample = test.iloc[0:2]
         sample = get_images(sample, self.image_mode, self._transformations)
         self._wrapped_model = wrap_model(
             model, sample, task_type, classes=classes)
@@ -177,14 +223,17 @@
         self._classes = RAIVisionInsights._get_classes(
             task_type=task_type,
             test=test,
             target_column=target_column,
             classes=classes
         )
         self.predict_output = None
+        if task_type == ModelTask.OBJECT_DETECTION:
+            test = transform_object_detection_labels(
+                test, target_column, self._classes)
         super(RAIVisionInsights, self).__init__(
             model, None, test, target_column, task_type,
             serializer)
 
         ext_test, ext_features = extract_features(
             self.test, self.target_column, self.task_type,
             self.image_mode,
@@ -202,15 +251,18 @@
         Initializes the explainer manager.
         """
         self._explainer_manager = ExplainerManager(
             self._wrapped_model, self.test,
             self.target_column,
             self.task_type,
             self._classes,
-            self.image_mode)
+            self.image_mode,
+            self.max_evals,
+            self.num_masks,
+            self.mask_res)
         self._error_analysis_manager = ErrorAnalysisManager(
             self._wrapped_model, self.test, self._ext_test_df,
             self.target_column,
             self.task_type,
             self.image_mode,
             self._transformations,
             self._classes,
@@ -560,14 +612,15 @@
         if IMAGE in column_names:
             images = self.test[:].image
         elif IMAGE_URL in column_names:
             images = self.test[:].image_url
         else:
             raise ValueError('No image column found in test data')
         encoded_images = []
+        image_dimensions = []
 
         for i, image in enumerate(images):
             if isinstance(image, str):
                 image = get_image_from_path(image, self.image_mode)
             s = io.BytesIO()
             # IMshow only accepts floats in range [0, 1]
             try:
@@ -575,33 +628,45 @@
             except Exception:
                 # In-place divide can fail for certain types
                 image = image / 255
             axes = pl.gca()
             axes.get_xaxis().set_visible(False)
             axes.get_yaxis().set_visible(False)
 
+            # TODO: remove condition after drawing bboxes in the frontend
             if tasktype == ModelTask.OBJECT_DETECTION:
                 num_classes = len(dashboard_dataset.class_names)
-                # TODO: switch to Fluent UI
                 colors = np.random.uniform(0, 255, size=(num_classes, 3))
                 image = self._draw_bounding_boxes(
                     image=image,
                     image_gt=dashboard_dataset.true_y[i],
                     image_prediction=dashboard_dataset.predicted_y[i],
                     class_names=dashboard_dataset.class_names,
                     colors=colors
                 )
             pl.imshow(image)
+            # resize image as optimization
+            size = pl.gcf().get_size_inches()
+            curr_width = size[0]
+            curr_height = size[1]
+            image_dimensions.append([image.shape[1], image.shape[0]])
+            new_width = self.image_width
+            if new_width is not None:
+                factor = new_width / curr_width
+                pl.gcf().set_size_inches((new_width, curr_height * factor))
             pl.savefig(s, format='jpg', bbox_inches='tight', pad_inches=0.)
             pl.clf()
             s.seek(0)
             b64_encoded = base64.b64encode(s.read())
             b64 = b64_encoded.decode(CommonTags.IMAGE_DECODE_UTF_FORMAT)
             encoded_images.append(b64)
 
+        # passing to frontend to draw bounding boxes with the correct scale
+        dashboard_dataset.imageDimensions = image_dimensions
+
         if len(encoded_images) > 0:
             dashboard_dataset.images = encoded_images
 
         if tasktype == ModelTask.OBJECT_DETECTION:
             d = dashboard_dataset
             dashboard_dataset.object_detection_predicted_y = d.predicted_y
             dashboard_dataset.object_detection_true_y = d.true_y
@@ -689,24 +754,19 @@
             color = tuple(colors[pred_labels[k]-1])
             cv2.rectangle(
                 image,
                 (int(pred_box[0]), int(pred_box[1])),
                 (int(pred_box[2]), int(pred_box[3])),
                 color, thickness=3
             )
-            label_text = label_classes[k] + ' (' \
+            label_text = str(k) + ". " + label_classes[k] + ' (' \
                 + str(round(pred_scores[k] * 100)) + '%)'
-            cv2.putText(image,
-                        str(k) + ". ",
-                        (int(pred_box[0]),
-                         int(pred_box[1]-30)),
-                        cv2.FONT_HERSHEY_SIMPLEX,
-                        0.8,
-                        color,
-                        2,
+            cv2.putText(image, label_text, (int(pred_box[0]),
+                                            int(pred_box[1]-5)),
+                        cv2.FONT_HERSHEY_SIMPLEX, 0.8, (0, 0, 0), 4,
                         lineType=cv2.LINE_AA)
             cv2.putText(image, label_text, (int(pred_box[0]),
                                             int(pred_box[1]-5)),
                         cv2.FONT_HERSHEY_SIMPLEX, 0.8, color, 2,
                         lineType=cv2.LINE_AA)
 
         return image
@@ -918,14 +978,18 @@
         feature_metadata_dict = self._feature_metadata.to_dict()
         meta = {
             _TARGET_COLUMN: self.target_column,
             _TASK_TYPE: self.task_type,
             _CLASSES: classes,
             _IMAGE_MODE: self.image_mode,
             _FEATURE_METADATA: feature_metadata_dict,
+            _IMAGE_WIDTH: self.image_width,
+            _MAX_EVALS: self.max_evals,
+            _NUM_MASKS: self.num_masks,
+            _MASK_RES: self.mask_res
         }
         with open(top_dir / _META_JSON, 'w') as file:
             json.dump(meta, file)
 
     @staticmethod
     def _load_metadata(inst, path):
         """Load the metadata.
@@ -938,14 +1002,25 @@
         top_dir = Path(path)
         with open(top_dir / _META_JSON, 'r') as meta_file:
             meta = meta_file.read()
         meta = json.loads(meta)
         inst.__dict__[_TARGET_COLUMN] = meta[_TARGET_COLUMN]
         inst.__dict__[_TASK_TYPE] = meta[_TASK_TYPE]
         inst.__dict__[_IMAGE_MODE] = meta[_IMAGE_MODE]
+        if _IMAGE_WIDTH in meta:
+            inst.__dict__[_IMAGE_WIDTH] = meta[_IMAGE_WIDTH]
+        else:
+            inst.__dict__[_IMAGE_WIDTH] = None
+        params = [_MAX_EVALS, _NUM_MASKS, _MASK_RES]
+        defaults = [DEFAULT_MAX_EVALS, DEFAULT_NUM_MASKS, DEFAULT_MASK_RES]
+        for param, default in zip(params, defaults):
+            if param in meta:
+                inst.__dict__[param] = meta[param]
+            else:
+                inst.__dict__[param] = default
         classes = meta[_CLASSES]
 
         inst.__dict__['_' + _CLASSES] = RAIVisionInsights._get_classes(
             task_type=meta[_TASK_TYPE],
             test=inst.__dict__[_TEST],
             target_column=meta[_TARGET_COLUMN],
             classes=classes
```

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.2.2/responsibleai_vision/utils/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.2.2/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.2.2/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-vision
-Version: 0.2.1
+Version: 0.2.2
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.1/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.2.2/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 responsibleai_vision/managers/explainer_manager.py
 responsibleai_vision/rai_vision_insights/__init__.py
 responsibleai_vision/rai_vision_insights/rai_vision_insights.py
 responsibleai_vision/utils/__init__.py
 responsibleai_vision/utils/feature_extractors.py
 responsibleai_vision/utils/image_reader.py
 responsibleai_vision/utils/image_utils.py
+tests/test_image_utils.py
 tests/test_rai_vision_automl_images_insights.py
 tests/test_rai_vision_insights.py
 tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.2.1/setup.py` & `responsibleai_vision-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.2.2/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.1/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.2.2/tests/test_rai_vision_insights.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft Corporation
 # Licensed under the MIT License.
 
 import numpy as np
 import pytest
 import sys
+import PIL
 
 from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai_vision import RAIVisionInsights, ModelTask
 from common_vision_utils import (
     create_pytorch_vision_model,
     gridify_fridge_multilabel_labels,
     load_multilabel_fridge_dataset,
@@ -18,28 +19,57 @@
     load_imagenet_labels, retrieve_or_train_fridge_model,
     retrieve_fridge_object_detection_model,
     FRIDGE_MULTILABEL_TARGETS,
     ImageTransforms,
     ImageTransformEnum,
     load_flowers_dataset,
     create_dummy_model)
-from responsibleai_vision.common.constants import ImageColumns
+from responsibleai_vision.common.constants import (
+    ImageColumns, ExplainabilityDefaults)
 from rai_vision_insights_validator import validate_rai_vision_insights
 
+DEFAULT_MAX_EVALS = ExplainabilityDefaults.DEFAULT_MAX_EVALS
+DEFAULT_NUM_MASKS = ExplainabilityDefaults.DEFAULT_NUM_MASKS
+DEFAULT_MASK_RES = ExplainabilityDefaults.DEFAULT_MASK_RES
+
 
 class TestRAIVisionInsights(object):
 
     def test_rai_insights_image_classification_imagenet(self):
         data = load_imagenet_dataset()
         pred = create_image_classification_pipeline()
         task_type = ModelTask.IMAGE_CLASSIFICATION
         class_names = load_imagenet_labels()
         run_rai_insights(pred, data[:3], ImageColumns.LABEL,
                          task_type, class_names, image_mode='RGB')
 
+    @pytest.mark.parametrize('max_evals', [None, 10, 200])
+    def test_rai_insights_image_classification_max_evals(self, max_evals):
+        data = load_imagenet_dataset()
+        pred = create_image_classification_pipeline()
+        task_type = ModelTask.IMAGE_CLASSIFICATION
+        class_names = load_imagenet_labels()
+        # run on a single image to avoid running out of memory on
+        # test machines
+        run_rai_insights(pred, data[:1], ImageColumns.LABEL,
+                         task_type, class_names, image_mode='RGB',
+                         test_explainer=True, max_evals=max_evals)
+
+    @pytest.mark.parametrize('max_evals', [-100, -1, 0])
+    def test_rai_insights_invalid_max_evals(self, max_evals):
+        data = load_imagenet_dataset()
+        pred = create_image_classification_pipeline()
+        task_type = ModelTask.IMAGE_CLASSIFICATION
+        class_names = load_imagenet_labels()
+        with pytest.raises(ValueError,
+                           match="max_evals must be greater than 0"):
+            run_rai_insights(pred, data[:1], ImageColumns.LABEL,
+                             task_type, class_names, image_mode='RGB',
+                             test_explainer=True, max_evals=max_evals)
+
     def test_rai_insights_image_classification_fridge(self):
         data = load_fridge_dataset()
         try:
             model = retrieve_or_train_fridge_model(data)
         except Exception as e:
             print("Failed to retrieve or load Fastai model, force training")
             print("Inner exception message on retrieving model: {}".format(e))
@@ -70,22 +100,49 @@
         data = gridify_fridge_multilabel_labels(data)
         task_type = ModelTask.MULTILABEL_IMAGE_CLASSIFICATION
         run_rai_insights(model, data[:3], FRIDGE_MULTILABEL_TARGETS,
                          task_type, test_error_analysis=True)
 
     @pytest.mark.skip("This test seems to fail due to issues in the \
                       MacOS/Linux versions of the build/PR gate.")
-    def test_rai_insights_object_detection_fridge(self):
+    @pytest.mark.parametrize('num_masks', [None, 25, DEFAULT_NUM_MASKS])
+    @pytest.mark.parametrize('mask_res', [None, DEFAULT_MASK_RES, 8])
+    def test_rai_insights_object_detection_fridge(self, num_masks, mask_res):
         data = load_fridge_object_detection_dataset()
         model = retrieve_fridge_object_detection_model()
         task_type = ModelTask.OBJECT_DETECTION
         class_names = np.array(['can', 'carton',
                                 'milk_bottle', 'water_bottle'])
-        run_rai_insights(model, data[:3], ImageColumns.LABEL,
-                         task_type, class_names)
+        run_rai_insights(model, data[:2], ImageColumns.LABEL,
+                         task_type, class_names,
+                         num_masks=num_masks, mask_res=mask_res)
+
+    @pytest.mark.parametrize('num_masks', [-100, -1, 0])
+    def test_rai_insights_invalid_num_masks(self, num_masks):
+        data = load_fridge_object_detection_dataset()
+        model = retrieve_fridge_object_detection_model()
+        task_type = ModelTask.OBJECT_DETECTION
+        class_names = np.array(['can', 'carton',
+                                'milk_bottle', 'water_bottle'])
+        with pytest.raises(ValueError,
+                           match="num_masks must be greater than 0"):
+            run_rai_insights(model, data[:1], ImageColumns.LABEL,
+                             task_type, class_names, num_masks=num_masks)
+
+    @pytest.mark.parametrize('mask_res', [-100, -1, 0])
+    def test_rai_insights_invalid_mask_res(self, mask_res):
+        data = load_fridge_object_detection_dataset()
+        model = retrieve_fridge_object_detection_model()
+        task_type = ModelTask.OBJECT_DETECTION
+        class_names = np.array(['can', 'carton',
+                                'milk_bottle', 'water_bottle'])
+        with pytest.raises(ValueError,
+                           match="mask_res must be greater than 0"):
+            run_rai_insights(model, data[:1], ImageColumns.LABEL,
+                             task_type, class_names, mask_res=mask_res)
 
     @pytest.mark.skip("This test fails in the build due to \
                       incompatibility between fastai and pytorch \
                       2.0.0. TODO: fix may be to ping pytorch <2.0.0 \
                       in the build until fastai updates.")
     def test_rai_insights_object_detection_fridge_label_format(self):
         data = load_fridge_object_detection_dataset()
@@ -147,37 +204,58 @@
         class_names = np.array(['can', 'carton',
                                 'milk_bottle', 'water_bottle'])
         dropped_features = [i for i in range(0, 10)]
         run_rai_insights(model, data[:3], ImageColumns.LABEL,
                          task_type, class_names,
                          dropped_features=dropped_features)
 
-    def test_jagged_image_sizes(self):
-        data = load_flowers_dataset()
+    @pytest.mark.parametrize(
+        'upscale',
+        [
+            pytest.param(
+                True,
+                marks=pytest.mark.skip(
+                    'Insufficient memory on test machines to load images')),
+            False
+        ])
+    def test_jagged_image_sizes(self, upscale):
+        if upscale:
+            PIL.Image.MAX_IMAGE_PIXELS = None
+        data = load_flowers_dataset(upscale=upscale)
         model = create_dummy_model(data)
         test_data = data
         class_names = data[ImageColumns.LABEL.value].unique()
         task_type = ModelTask.IMAGE_CLASSIFICATION
         run_rai_insights(model, test_data, ImageColumns.LABEL,
-                         task_type, class_names)
+                         task_type, class_names, upscale=upscale)
 
 
 def run_rai_insights(model, test_data, target_column,
                      task_type, classes=None, test_explainer=False,
                      test_error_analysis=False,
-                     image_mode=None, dropped_features=None):
+                     image_mode=None, dropped_features=None,
+                     upscale=False, max_evals=DEFAULT_MAX_EVALS,
+                     num_masks=DEFAULT_NUM_MASKS,
+                     mask_res=DEFAULT_MASK_RES):
     feature_metadata = None
     if dropped_features:
         feature_metadata = FeatureMetadata(dropped_features=dropped_features)
+    image_width = None
+    if upscale:
+        image_width = 2
     rai_insights = RAIVisionInsights(model, test_data,
                                      target_column,
                                      task_type=task_type,
                                      classes=classes,
                                      image_mode=image_mode,
-                                     feature_metadata=feature_metadata)
+                                     feature_metadata=feature_metadata,
+                                     image_width=image_width,
+                                     max_evals=max_evals,
+                                     num_masks=num_masks,
+                                     mask_res=mask_res)
     # Note: this seems too resource-intensive
     # TODO: re-add when we get beefier test machines
     if test_explainer:
         rai_insights.explainer.add()
     if test_error_analysis:
         rai_insights.error_analysis.add()
     if test_explainer or test_error_analysis:
```

