# Comparing `tmp/dreamsim-0.1.0.tar.gz` & `tmp/dreamsim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamsim-0.1.0.tar", last modified: Fri Jun 16 00:09:33 2023, max compression
+gzip compressed data, was "dreamsim-0.1.1.tar", last modified: Fri Jun 16 01:07:53 2023, max compression
```

## Comparing `dreamsim-0.1.0.tar` & `dreamsim-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 00:09:33.716123 dreamsim-0.1.0/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-06-15 23:35:43.000000 dreamsim-0.1.0/LICENSE
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1370 2023-06-16 00:09:33.711558 dreamsim-0.1.0/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7549 2023-06-15 23:37:39.000000 dreamsim-0.1.0/README.md
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 00:09:33.530210 dreamsim-0.1.0/dreamsim/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      563 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/config.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 00:09:33.698386 dreamsim-0.1.0/dreamsim/feature_extraction/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/extractor.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/load_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/load_mae_as_vit.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/load_open_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/vision_transformer.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/feature_extraction/vit_wrapper.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11462 2023-06-15 23:37:26.000000 dreamsim-0.1.0/dreamsim/model.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 00:09:33.606636 dreamsim-0.1.0/dreamsim.egg-info/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1370 2023-06-16 00:09:33.000000 dreamsim-0.1.0/dreamsim.egg-info/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-06-16 00:09:33.000000 dreamsim-0.1.0/dreamsim.egg-info/SOURCES.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-06-16 00:09:33.000000 dreamsim-0.1.0/dreamsim.egg-info/dependency_links.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-06-16 00:09:33.000000 dreamsim-0.1.0/dreamsim.egg-info/requires.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-06-16 00:09:33.000000 dreamsim-0.1.0/dreamsim.egg-info/top_level.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-06-16 00:09:33.718304 dreamsim-0.1.0/setup.cfg
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      945 2023-06-16 00:08:44.000000 dreamsim-0.1.0/setup.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.784095 dreamsim-0.1.1/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-06-15 23:35:43.000000 dreamsim-0.1.1/LICENSE
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7472 2023-06-16 01:07:53.779476 dreamsim-0.1.1/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     8642 2023-06-16 01:01:52.000000 dreamsim-0.1.1/README.md
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.608144 dreamsim-0.1.1/dreamsim/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      563 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/config.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.766266 dreamsim-0.1.1/dreamsim/feature_extraction/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/extractor.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_mae_as_vit.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/load_open_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/vision_transformer.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/feature_extraction/vit_wrapper.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11462 2023-06-16 01:06:22.000000 dreamsim-0.1.1/dreamsim/model.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:07:53.675546 dreamsim-0.1.1/dreamsim.egg-info/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7472 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/SOURCES.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/dependency_links.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/requires.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-06-16 01:07:53.000000 dreamsim-0.1.1/dreamsim.egg-info/top_level.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-06-16 01:07:53.786290 dreamsim-0.1.1/setup.cfg
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      980 2023-06-16 01:07:04.000000 dreamsim-0.1.1/setup.py
```

### Comparing `dreamsim-0.1.0/LICENSE` & `dreamsim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/README.md` & `dreamsim-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- # ![icon](images/figs/icon.png)  DreamSim Perceptual Metric -->
 <!-- # DreamSim Perceptual Metric <img src="images/figs/icon.png" align="left" width="50px"/>  -->
 # DreamSim: Learning New Dimensions of Human Visual Similarity using Synthetic Data
-### [Project Page](https://dreamsim-nights.github.io/) | [Paper](https://google.com) | [Bibtex](https://google.com)
+### [Project Page](https://dreamsim-nights.github.io/) | [Paper](https://arxiv.org/abs/2306.09344) | [Bibtex](#bibtex)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1taEOMzFE9g81D9AwH27Uhy2U82tQGAVI?usp=sharing)
 
 [Stephanie Fu](https://stephanie-fu.github.io)\* $^{1}$, [Netanel Tamir](https://netanel-tamir.github.io)\* $^{2}$, [Shobhita Sundaram](https://ssundaram21.github.io)\* $^{1}$, [Lucy Chai](https://people.csail.mit.edu/lrchai/) $^1$, [Richard Zhang](http://richzhang.github.io) $^3$, [Tali Dekel](https://www.weizmann.ac.il/math/dekel/) $^2$, [Phillip Isola](https://web.mit.edu/phillipi/) $^1$. (*equal contribution)<br>
 $^1$ MIT, $^2$ Weizmann Institute of Science, $^3$ Adobe Research.
 
 ![teaser](images/figs/teaser.png)
 
@@ -24,27 +24,35 @@
 
 **Option 1:** Install using pip: 
 
 ```pip install dreamsim```
 
 The package is used for importing and using the DreamSim model.
 
-**Option 2:** Clone our repo and install dependencies:
+**Option 2:** Clone our repo and install dependencies.
+This is necessary for running our training/evaluation scripts.
 <!--  ```
 git clone https://github.com/ssundaram21/DreamSim.git
 conda env create -f environment.yml
 export PYTHONPATH="$PYTHONPATH:$(realpath ./DreamSim)"
 ``` -->
 ```
 python3 -m venv ds
 source ds/bin/activate
 pip install -r requirements.txt
-export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsim-dev)"
+export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsimv)"
+```
+To install with conda:
+```
+conda create -n ds
+conda activate ds
+conda install pip # verify with the `which pip` command
+pip install -r requirements.txt
+export PYTHONPATH="$PYTHONPATH:$(realpath ./dreamsim)"
 ```
-This is necessary for running our training/evaluation scripts.
 
 ## Usage
 **For walk-through examples of the below use-cases, check out our [Colab demo](https://colab.research.google.com/drive/1taEOMzFE9g81D9AwH27Uhy2U82tQGAVI?usp=sharing).**
 
 ### Quickstart: Perceptual similarity metric
 The basic use case is to measure the perceptual distance between two images. **A higher score means more different, lower means more similar**. 
 
@@ -130,21 +138,30 @@
 
 ```
 python ./training/evaluate.py --config ./configs/eval_baseline.yaml
 ```
 
 For an example of evaluating using a trained checkpoint, refer to `./configs/eval_checkpoint.yaml`. See `./training/evaluate.py` for a full list and description of evaluation options.
 <!--Experiments-->
+
+<a name="bibtex"></a>
 # Citation
 
 If you find our work or any of our materials useful, please cite our paper:
 ```
- @article{fu2023learning,
-  title={Learning New Dimensions of Human Visual Similarity using Synthetic Data},
-  author={Stephanie Fu* and Netanel Tamir* and Shobhita Sundaram* and Lucy Chai and Richard Zhang and Tali Dekel and Phillip Isola},
-  journal={arXiv:ID},
-  year={2023}
+@misc{fu2023dreamsim,
+      title={DreamSim: Learning New Dimensions of Human Visual Similarity using Synthetic Data}, 
+      author={Stephanie Fu and Netanel Tamir and Shobhita Sundaram and Lucy Chai and Richard Zhang and Tali Dekel and Phillip Isola},
+      year={2023},
+      eprint={2306.09344},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
 }
 ```
 
 ## Acknowledgements
+We thank Jim DiCarlo, Liad Mudrik, Nitzan Censor for fruitful discussions throughout the project. Additionally, we thank Narek Tumanyan for his insightful comments over the course of the project. Finally, we thank Michelle Li for proofreading sections of this paper and offering helpful comments. 
+
+This work was supported by the NSF GRFP Fellowship to Shobhita Sundaram, the Meta PhD Fellowship to Lucy Chai, the Israeli Science Foundation (grant 2303/20) to Tali Dekel, and the Packard Fellowship to Phillip Isola.
+
+Our code borrows from the ["Deep ViT Features as Dense Visual Descriptors"](https://dino-vit-features.github.io/) repository for ViT feature extraction, and takes inspiration from the [UniverSeg](https://github.com/JJGO/UniverSeg) respository for code structure.
```

### Comparing `dreamsim-0.1.0/dreamsim/config.py` & `dreamsim-0.1.1/dreamsim/config.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/feature_extraction/extractor.py` & `dreamsim-0.1.1/dreamsim/feature_extraction/extractor.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/feature_extraction/load_clip_as_dino.py` & `dreamsim-0.1.1/dreamsim/feature_extraction/load_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/feature_extraction/load_mae_as_vit.py` & `dreamsim-0.1.1/dreamsim/feature_extraction/load_mae_as_vit.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/feature_extraction/load_open_clip_as_dino.py` & `dreamsim-0.1.1/dreamsim/feature_extraction/load_open_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/feature_extraction/vision_transformer.py` & `dreamsim-0.1.1/dreamsim/feature_extraction/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim/model.py` & `dreamsim-0.1.1/dreamsim/model.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/dreamsim.egg-info/SOURCES.txt` & `dreamsim-0.1.1/dreamsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.0/setup.py` & `dreamsim-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 long_description = "".join(long_description.split("<!--Experiments-->")[::2])
-long_description = "".join(long_description.split("![teaser](images/figs/teaser.png)")[::2])
+long_description = "".join(long_description.split("![teaser](images/figs/teaser.png)"))
 
 setuptools.setup(
     name="dreamsim",
-    version="0.1.0",
+    version="0.1.1",
     description="DreamSim similarity metric",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ssundaram21/dreamsim",
+    url="https://github.com/ssundaram21/dreamsim-dev",
     packages=['dreamsim', 'dreamsim/feature_extraction'],
     install_requires=[
         "numpy",
         "open-clip-torch",
         "peft==0.1.0",
         "Pillow",
         "torch",
@@ -26,7 +26,10 @@
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
+
+# "scipy==1.9.2",
+# "timm==0.6.12",
```

