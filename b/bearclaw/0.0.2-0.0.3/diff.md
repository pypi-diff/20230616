# Comparing `tmp/bearclaw-0.0.2.tar.gz` & `tmp/bearclaw-0.0.3.tar.gz`

## Comparing `bearclaw-0.0.2.tar` & `bearclaw-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,34 @@
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.dockerignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 bearclaw-0.0.2/Dockerfile
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 bearclaw-0.0.2/Dockerfile.GRCh37
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bearclaw-0.0.2/requirements.txt
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.vscode/tasks.json
--rw-r--r--   0        0        0    13902 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/feature_extraction.html
--rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/index.html
--rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/preprocessing.html
--rw-r--r--   0        0        0    16873 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/transforms.html
--rw-r--r--   0        0        0    16271 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/io/index.html
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/io/tso.html
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 bearclaw-0.0.2/public/bearclaw/io/vcf.html
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/_version.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/feature_extraction.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/preprocessing.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/transforms.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/io/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/io/tso.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/io/vcf.py
--rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt
--rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt
--rw-r--r--   0        0        0   149327 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/__init__.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/test_feature_extraction.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/test_io.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/test_transforms.py
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/test_vcf.py
--rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/GRCh37/sample1.vcf
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/GRCh37/sample1.vcf.gz
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/GRCh37/sample2.vcf
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/GRCh37/tso500.example.vcf
--rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/GRCh38/sample1.vcf
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bearclaw-0.0.2/src/test/resources/tso500/example_TMB_Trace.tsv
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 bearclaw-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bearclaw-0.0.2/LICENSE
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bearclaw-0.0.2/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bearclaw-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 bearclaw-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.dockerignore
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 bearclaw-0.0.3/Dockerfile
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 bearclaw-0.0.3/Dockerfile.GRCh37
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bearclaw-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/_version.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/feature_extraction.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/preprocessing.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/transforms.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/tso.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/vcf.py
+-rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt
+-rw-r--r--   0        0        0   149327 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/__init__.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_feature_extraction.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_io.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_transforms.py
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_vcf.py
+-rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf.gz
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample2.vcf
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/tso500.example.vcf
+-rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh38/sample1.vcf
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/tso500/example_TMB_Trace.tsv
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bearclaw-0.0.3/LICENSE
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bearclaw-0.0.3/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 bearclaw-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 bearclaw-0.0.3/PKG-INFO
```

### Comparing `bearclaw-0.0.2/.gitlab-ci.yml` & `bearclaw-0.0.3/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -22,29 +22,39 @@
         coverage_format: cobertura
         path: src/coverage.xml
 
 build:
   image: arm64v8/docker
   stage: build
   services:
-    - arm64v8/docker:dind
+    - name: arm64v8/docker:dind
+      alias: docker
+  variables:
+    DOCKER_HOST: tcp://docker:2375
   tags:
     - deployment
   script:
     - docker login -u gitlab-ci-token -p $CI_BUILD_TOKEN $CI_REGISTRY
     # Install dependencies to build multi-architecture Dockerfile.
     - docker run --privileged --rm tonistiigi/binfmt --install all
     - docker buildx create --use
     - docker buildx build
       --push
       --platform linux/amd64,linux/arm64,linux/arm/v7
       -f Dockerfile.GRCh37
       -t registry.gitlab.com/hylkedonker/bearclaw/grch37:${CI_COMMIT_SHORT_SHA}
       -t registry.gitlab.com/hylkedonker/bearclaw/grch37:latest
       .
+    - docker buildx build
+      --push
+      --platform linux/amd64,linux/arm64,linux/arm/v7
+      -f Dockerfile
+      -t registry.gitlab.com/hylkedonker/bearclaw:${CI_COMMIT_SHORT_SHA}
+      -t registry.gitlab.com/hylkedonker/bearclaw:latest
+      .
   only:
   - main
 
 pages:
   image: python:3.10
   stage: deploy
   tags:
```

### Comparing `bearclaw-0.0.2/Dockerfile.GRCh37` & `bearclaw-0.0.3/Dockerfile.GRCh37`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/feature_extraction.py` & `bearclaw-0.0.3/src/bearclaw/feature_extraction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
-from typing import Literal
+from typing import Literal, Optional
 
 from pandas import DataFrame, read_csv
 from sklearn.decomposition import NMF
 
 
 RESOURCE_DIR = Path(__file__).parent.resolve() / "resources"
 
 _COSMIC_MUTATIONAL_SIGNATURES = {
     "single_base_substitutions": RESOURCE_DIR / "COSMIC_v3.3_SBS_GRCh37.txt",
     "doublet_base_substitutions": RESOURCE_DIR / "COSMIC_v3.3_DBS_GRCh37.txt",
     "indel": RESOURCE_DIR / "COSMIC_v3.3_ID_GRCh37.txt",
     "cnv": RESOURCE_DIR / "COSMIC_v3.3_CN_GRCh37.txt",
 }
 
-_POSSIBLE_SBS_SEQUENCING_ARTEFACTS = [
+POSSIBLE_SBS_SEQUENCING_ARTEFACTS = [
     # Extracted from https://cancer.sanger.ac.uk/signatures/sbs/.
     "SBS27",
     "SBS43",
     "SBS45",
     "SBS46",
     "SBS47",
     "SBS48",
@@ -32,15 +32,15 @@
     "SBS56",
     "SBS57",
     "SBS58",
     "SBS59",
     "SBS60",
 ]
 
-_POSSIBLE_CN_SEQUENCING_ARTEFACTS = ["CN22", "CN23", "CN24"]
+POSSIBLE_CN_SEQUENCING_ARTEFACTS = ["CN22", "CN23", "CN24"]
 
 
 def _get_cosmic_feature_names(
     representation: Literal[
         "single_base_substitutions",
         "doublet_base_substitutions",
         "indel",
@@ -72,16 +72,18 @@
     """
 
     def __init__(
         self,
         cosmic_signature: Literal[
             "single_base_substitutions", "doublet_base_substitutions", "indel", "cnv"
         ],
+        init: Optional[str] = "nndsvda",
         tol: float = 1e-6,
         max_iter: int = 10000,
+        random_state=None,
     ):
         """
         Load NMF COSMIC GRCh37 mutational signature checkpoint.
 
         Args:
             cosmic_signature: Input features correspond to 96 single base
                 substution (SBS), 78 double base substitutions (DBS), 83
@@ -93,16 +95,17 @@
         ).T
         self.n_components_, self.n_features_in_ = H.shape
 
         super().__init__(
             n_components=self.n_components_,
             max_iter=max_iter,
             solver="cd",
-            init="nndsvda",
+            init=init,
             tol=tol,
+            random_state=random_state,
         )
         self.components_ = H.to_numpy()
         self.feature_names_in_ = H.columns
         self.feature_names_out_ = H.index
 
     def transform(self, X):
         """Transform back to pandas dataframe."""
```

### Comparing `bearclaw-0.0.2/src/bearclaw/preprocessing.py` & `bearclaw-0.0.3/src/bearclaw/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/transforms.py` & `bearclaw-0.0.3/src/bearclaw/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from pandas import DataFrame, concat
 
-from bearclaw.feature_extraction import CosmicNMF, _POSSIBLE_SBS_SEQUENCING_ARTEFACTS
+from bearclaw.feature_extraction import CosmicNMF, POSSIBLE_SBS_SEQUENCING_ARTEFACTS
 from bearclaw.io import extract_mutation_spectra, from_tso500_trace, vcf
 
 
 def spectrum(vcf_file: Path, exome: bool = False) -> DataFrame:
     """Extract single + doublet base substitutions and indel spectra from VCF file."""
     mutation_matrices = extract_mutation_spectra(vcf_file, exome=exome)
     spectra = list(mutation_matrices.values())
@@ -52,15 +52,15 @@
         "indel",
     ]:
         decomposer = CosmicNMF(cosmic_signature=spectrum)  # type: ignore
         signatures.append(decomposer.transform(mutation_matrices[spectrum]))
 
     result = concat(signatures, axis="columns")
     if filter_seq_artefact_signatures:
-        return result.drop(columns=_POSSIBLE_SBS_SEQUENCING_ARTEFACTS)
+        return result.drop(columns=POSSIBLE_SBS_SEQUENCING_ARTEFACTS)
     return result
 
 
 @from_tso500_trace
 def mutational_signature_from_trace(
     trace_file: Path, filter_seq_artefact_signatures: bool = True
 ) -> DataFrame:
```

### Comparing `bearclaw-0.0.2/src/bearclaw/io/__init__.py` & `bearclaw-0.0.3/src/bearclaw/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/io/tso.py` & `bearclaw-0.0.3/src/bearclaw/io/tso.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/io/vcf.py` & `bearclaw-0.0.3/src/bearclaw/io/vcf.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt` & `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt` & `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt` & `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt` & `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/test_feature_extraction.py` & `bearclaw-0.0.3/src/test/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/test_io.py` & `bearclaw-0.0.3/src/test/test_io.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/test_transforms.py` & `bearclaw-0.0.3/src/test/test_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from numpy.linalg import norm
 from numpy.testing import assert_almost_equal, assert_array_almost_equal
 from pandas import DataFrame, read_csv
 
 from bearclaw.feature_extraction import (
     _get_cosmic_feature_names,
-    _POSSIBLE_SBS_SEQUENCING_ARTEFACTS,
+    POSSIBLE_SBS_SEQUENCING_ARTEFACTS,
     _COSMIC_MUTATIONAL_SIGNATURES,
     CosmicNMF,
 )
 from bearclaw.preprocessing import VariantDataGenerator
 from bearclaw.transforms import mutational_signature, non_synonymous_spectrum, spectrum
 
 TEST_RESOURCES = Path(__file__).parent.resolve() / "resources"
@@ -98,15 +98,15 @@
     def test_sbs_filter_sequencing_artefacts(self):
         """Verify that all SBS sequencing artefacts are removed."""
         dg = VariantDataGenerator(transform=mutational_signature)
         X, _ = dg.flow_from_dataframe(self.dataframe, keep_columns=False, x_col="vcf")
 
         self.assertEqual(
             len(X.columns),
-            11 + 78 + 18 - len(_POSSIBLE_SBS_SEQUENCING_ARTEFACTS),
+            11 + 78 + 18 - len(POSSIBLE_SBS_SEQUENCING_ARTEFACTS),
         )
 
     def test_sbs_mutational_signature(self):
         """Test non-synonymous single base substitution mutational signature."""
         dg = VariantDataGenerator(
             transform=lambda x: mutational_signature(
                 x, filter_seq_artefact_signatures=False
@@ -154,15 +154,15 @@
     def test_commutation_normalisation_operation(self):
         """Test that deconvolution<->normalisation commutes."""
 
         all_sbs_signatures = _get_cosmic_feature_names(
             representation="single_base_substitutions", signatures=True
         )
         sbs_signatures = [
-            c for c in all_sbs_signatures if c not in _POSSIBLE_SBS_SEQUENCING_ARTEFACTS
+            c for c in all_sbs_signatures if c not in POSSIBLE_SBS_SEQUENCING_ARTEFACTS
         ]
         sbs_spectrum = _get_cosmic_feature_names(
             representation="single_base_substitutions", signatures=False
         )
         # 1)
         # First deconvolution, then normalisation.
         deconv = VariantDataGenerator(transform=mutational_signature)
@@ -180,15 +180,15 @@
             self.dataframe,
             coverage_size="coverage",
             x_col="vcf",
         )
 
         decomposer = CosmicNMF(cosmic_signature="single_base_substitutions")
         X_sbs96_deconv = decomposer.transform(X_spectrum[sbs_spectrum]).drop(
-            columns=_POSSIBLE_SBS_SEQUENCING_ARTEFACTS
+            columns=POSSIBLE_SBS_SEQUENCING_ARTEFACTS
         )
 
         # Compare results.
         assert_array_almost_equal(
             X_sbs96_deconv, X_normalised[sbs_signatures], decimal=5
         )
```

### Comparing `bearclaw-0.0.2/src/test/test_vcf.py` & `bearclaw-0.0.3/src/test/test_vcf.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/GRCh37/sample1.vcf` & `bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/GRCh37/sample1.vcf.gz` & `bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf.gz`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/GRCh37/sample2.vcf` & `bearclaw-0.0.3/src/test/resources/GRCh37/sample2.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/GRCh37/tso500.example.vcf` & `bearclaw-0.0.3/src/test/resources/GRCh37/tso500.example.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/GRCh38/sample1.vcf` & `bearclaw-0.0.3/src/test/resources/GRCh38/sample1.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/src/test/resources/tso500/example_TMB_Trace.tsv` & `bearclaw-0.0.3/src/test/resources/tso500/example_TMB_Trace.tsv`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/.gitignore` & `bearclaw-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/LICENSE` & `bearclaw-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/README.md` & `bearclaw-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.2/pyproject.toml` & `bearclaw-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bearclaw"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hylke C. Donker", email="h.c.donker@umcg.nl" },
 ]
 description = "Pipeline components to extract features from variants."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/hylkedonker/bearclaw"
-"Bug Tracker" = "https://gitlab.com/hylkedonker/bearclaw/-/issues"
+"Bug Tracker" = "https://gitlab.com/hylkedonker/bearclaw/-/issues"
```

### Comparing `bearclaw-0.0.2/PKG-INFO` & `bearclaw-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bearclaw
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pipeline components to extract features from variants.
 Project-URL: Homepage, https://gitlab.com/hylkedonker/bearclaw
 Project-URL: Bug Tracker, https://gitlab.com/hylkedonker/bearclaw/-/issues
 Author-email: "Hylke C. Donker" <h.c.donker@umcg.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

