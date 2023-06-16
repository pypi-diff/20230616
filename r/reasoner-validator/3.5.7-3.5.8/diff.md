# Comparing `tmp/reasoner_validator-3.5.7.tar.gz` & `tmp/reasoner_validator-3.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.7.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.8.tar", max compression
```

## Comparing `reasoner_validator-3.5.7.tar` & `reasoner_validator-3.5.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/LICENSE
--rw-r--r--   0        0        0    12606 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/README.md
--rw-r--r--   0        0        0      131 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/conf.py
--rw-r--r--   0        0        0    19034 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/pyproject.toml
--rw-r--r--   0        0        0    20545 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    61511 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26862 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9718 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9922 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/conftest.py
--rw-r--r--   0        0        0   112361 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    42178 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_data/sample_trapi_schema.yaml
--rw-r--r--   0        0        0    31899 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_response_validator.py
--rw-r--r--   0        0        0     4533 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_semver.py
--rw-r--r--   0        0        0     1746 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_workflows.py
--rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/LICENSE
+-rw-r--r--   0        0        0    12606 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/README.md
+-rw-r--r--   0        0        0      131 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/conf.py
+-rw-r--r--   0        0        0    19034 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-16 04:51:42.743725 reasoner_validator-3.5.8/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/pyproject.toml
+-rw-r--r--   0        0        0    34621 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    63110 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26862 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9718 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9922 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/conftest.py
+-rw-r--r--   0        0        0   113749 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    31899 2023-06-16 04:51:42.747725 reasoner_validator-3.5.8/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4533 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-16 04:51:42.751725 reasoner_validator-3.5.8/tests/test_workflows.py
+-rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.8/PKG-INFO
```

### Comparing `reasoner_validator-3.5.7/LICENSE` & `reasoner_validator-3.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/README.md` & `reasoner_validator-3.5.8/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/docs/Makefile` & `reasoner_validator-3.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/docs/conf.py` & `reasoner_validator-3.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/docs/index.rst` & `reasoner_validator-3.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/docs/make.bat` & `reasoner_validator-3.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.8/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/pyproject.toml` & `reasoner_validator-3.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.7"
+version = "3.5.8"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.7/reasoner_validator/__init__.py` & `reasoner_validator-3.5.8/reasoner_validator/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Optional, List, Dict
+
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.biolink import (
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph,
-    BiolinkValidator
+    BiolinkValidator,
+    get_biolink_model_toolkit,
+    BiolinkValidator, TRAPIGraphType
 )
 
 # Maximum number of data points to scrutinize
 # in various parts TRAPI Query Response.Message
 from reasoner_validator.trapi import check_trapi_validity, TRAPISchemaValidator
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
 from reasoner_validator.versioning import SemVer, SemVerError
@@ -157,15 +160,15 @@
     def sample_graph(graph: Dict, edges_limit: int = 100) -> Dict:
         """
         Only process a strict subsample of the TRAPI Response Message knowledge graph.
 
         :param graph: original knowledge graph
         :type graph: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (could take awhile! Default: 100)
+                            triggers validation of all edges in the knowledge graph (could take a while! Default: 100)
         :type edges_limit: int
 
         :return: Dict, 'edges_limit' sized subset of knowledge graph
         """
         # We don't check for non-empty graphs here simply because the sole caller of this
         # method is the 'has_valid_knowledge_graph' method, which filters out empty graphs
         if edges_limit > 0:
@@ -173,15 +176,15 @@
                 "nodes": dict(),
                 "edges": dict()
             }
             # 'sample_size' will always be a positive number here.
             # The kg_sample size will always be the 'sample_size'
             # or less, the latter situation arising if the number
             # of graph edges is smaller or some subject or
-            # object id's are missing in the nodes list.
+            # object ids are missing in the nodes list.
             sample_size = min(edges_limit, len(graph["edges"]))
             n = 0
             for key, edge in graph['edges'].items():
 
                 kg_sample['edges'][key] = edge
 
                 if 'subject' in edge and \
@@ -254,15 +257,15 @@
     def has_valid_knowledge_graph(self, message: Dict, edges_limit: int = 100) -> bool:
         """
         Validate a TRAPI Knowledge Graph.
 
         :param message: input message expected to contain the 'knowledge_graph'
         :type message: Dict
         :param edges_limit: integer maximum number of edges to be validated in the knowledge graph. A value of zero
-                            triggers validation of all edges in the knowledge graph (could take awhile! Default: 100)
+                            triggers validation of all edges in the knowledge graph (could take a while! Default: 100)
         :type edges_limit: int
 
         :return: bool, False, if validation errors
         """
         # This integrity constraint may not really be necessary
         # since negative numbers are functionally inequivalent to zero
         assert edges_limit >= 0, "The 'edges_limit' must be zero or a positive integer!"
@@ -408,7 +411,340 @@
                     #             output_node_binding=output_node_binding
                     #         )
                     #         # data_dump=f"Resolved aliases:\n{','.join(output_aliases)}\n" +
                     #         #           f"Result object IDs:\n{_output(object_ids,flat=True)}"
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
+
+    @staticmethod
+    def case_node_found(target: str, identifier: str, case: Dict, nodes: Dict) -> bool:
+        """
+        Check for presence of the target identifier,
+        with expected categories, in the "nodes" catalog.
+
+        :param target: 'subject' or 'object'
+        :param identifier: (CURIE) identifier of the node
+        :param case: Dict, full test case (to access the target node 'category')
+        :param nodes: Dict, nodes category indexed by node identifiers.
+        :return:
+        """
+        #
+        #     "nodes": {
+        #         "MONDO:0005148": {"name": "type-2 diabetes"},
+        #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
+        #     }
+        #
+
+        # Sanity check
+        assert target in ["subject", "object"]
+
+        if identifier in nodes.keys():
+            # Found the target node identifier,
+            # but is the expected category present?
+            node_details = nodes[identifier]
+            if "categories" in node_details:
+                category = case[f"{target}_category"]
+                if category in node_details["categories"]:
+                    return True
+
+        # Target node identifier or categories is missing,
+        # or not annotated with the expected category?
+        return False
+
+    @staticmethod
+    def case_edge_bindings(target_edge_id: str, data: Dict) -> bool:
+        """
+        Check if target query edge id and knowledge graph edge id are in specified edge_bindings.
+        :param target_edge_id:  str, expected knowledge edge identifier in a matching result
+        :param data: TRAPI version-specific Response context from which the 'edge_bindings' may be retrieved
+        :return: True, if found
+        """
+        edge_bindings: Dict = data["edge_bindings"]
+        for bound_query_id, edge in edge_bindings.items():
+            # The expected query identifier in this context is
+            # hard coded as 'ab' in the 'one_hop.util.py' model
+            if bound_query_id == "ab":
+                for binding_details in edge:
+                    # TRAPI schema validation actually
+                    # catches missing id's, but sanity check...
+                    if "id" in binding_details:
+                        if target_edge_id == binding_details["id"]:
+                            return True
+        return False
+
+    def case_result_found(
+            self,
+            subject_id: str,
+            object_id: str,
+            edge_id: str,
+            results: List,
+            trapi_version: str
+    ) -> bool:
+        """
+        Validate that test case S--P->O edge is found bound to the Results?
+        :param subject_id: str, subject node (CURIE) identifier
+        :param object_id:  str, subject node (CURIE) identifier
+        :param edge_id:  str, subject node (CURIE) identifier
+        :param results: List of (TRAPI-version specific) Result objects
+        :param trapi_version: str, target TRAPI version of the Response being validated
+        :return: bool, True if case S-P-O edge was found in the results
+        """
+        trapi_1_4_0: bool
+        try:    # try block ... Sanity check: in case the trapi_version is somehow invalid?
+            target_version: SemVer = SemVer.from_string(trapi_version)
+            trapi_1_4_0 = target_version >= SemVer.from_string("1.4.0")
+        except SemVerError as sve:
+            logger.warning(f"case_result_found() 'trapi_version' seems invalid: {str(sve)}. Default to latest?")
+            trapi_1_4_0 = True
+
+        result_found: bool = False
+        result: Dict
+
+        for result in results:
+
+            # Node binding validation still currently same for recent TRAPI versions
+            node_bindings: Dict = result["node_bindings"]
+            subject_id_found: bool = False
+            object_id_found: bool = False
+            edge_id_found: bool = False
+            for node in node_bindings.values():
+                for details in node:
+                    if "id" in details:
+                        if subject_id == details["id"]:
+                            subject_id_found = True
+                        elif object_id == details["id"]:
+                            object_id_found = True
+
+            # However, TRAPI 1.4.0 Message 'Results' 'edge_bindings' are reported differently
+            #          from 1.3.0, rather, embedded in 'Analysis' objects (and 'Auxiliary Graphs')
+            if trapi_1_4_0:
+                #
+                #     "auxiliary_graphs": {
+                #         "a0": {
+                #             "edges": [
+                #                 "e02",
+                #                 "e12"
+                #             ]
+                #         },
+                #         "a1": {
+                #             "edges": [
+                #                 "extra_edge0"
+                #             ]
+                #         },
+                #         "a2": {
+                #             "edges" [
+                #                 "extra_edge1"
+                #             ]
+                #         }
+                #     },
+                #     "results": [
+                #         {
+                #             "node_bindings": {
+                #                 "n0": [
+                #                     "id": "diabetes"
+                #                 ],
+                #                 "n1": [
+                #                     "id": "metformin"
+                #                 ]
+                #             },
+                #             "analyses":[
+                #                 {
+                #                     "reasoner_id": "ara0",
+                #                     "edge_bindings": {
+                #                         "e0": [
+                #                             {
+                #                                 "id": "e01"
+                #                             },
+                #                             {
+                #                                 "id": "creative_edge"
+                #                             }
+                #                         ]
+                #                     },
+                #                     "support_graphs": [
+                #                         "a1",
+                #                         "a2"
+                #                     ]
+                #                     "score": ".7"
+                #                 },
+                #             ]
+                #         }
+                #     ]
+
+                # result["analyses"] may be empty but prior TRAPI 1.4.0 schema validation ensures that
+                # the "analysis" key is at least present plus the objects themselves are 'well-formed'
+                analyses: List = result["analyses"]
+                for analysis in analyses:
+                    edge_id_found = self.case_edge_bindings(edge_id, analysis)
+                    if edge_id_found:
+                        break
+
+            else:
+                # TRAPI 1.3.0 or earlier?
+                #
+                # Then, the TRAPI 1.3.0 Message Results (referencing the
+                # Response Knowledge Graph) could be something like this:
+                #
+                #     "results": [
+                #         {
+                #             "node_bindings": {
+                #                # node "id"'s in knowledge graph, in edge "id"
+                #                 "type-2 diabetes": [{"id": "MONDO:0005148"}],
+                #                 "drug": [{"id": "CHEBI:6801"}]
+                #             },
+                #             "edge_bindings": {
+                #                 # the edge binding key should be the query edge id
+                #                 # bounded edge "id" is from knowledge graph
+                #                 "treats": [{"id": "df87ff82"}]
+                #             }
+                #         }
+                #     ]
+                #
+                edge_id_found = self.case_edge_bindings(edge_id, result)
+
+            if subject_id_found and object_id_found and edge_id_found:
+                result_found = True
+                break
+
+        return result_found
+
+    def case_input_found_in_response(
+            self,
+            case: Dict,
+            response: Dict,
+            trapi_version: str
+    ) -> bool:
+        """
+        Predicate to validate if test data test case specified edge is returned
+        in the Knowledge Graph of the TRAPI Response Message. This method assumes
+        that the TRAPI response is already generally validated as well-formed.
+
+        :param case: Dict, input data test case
+        :param response: Dict, TRAPI Response whose message ought to contain the test case edge
+        :param trapi_version: str, TRAPI version of response being tested
+        :return: True if test case edge found; False otherwise
+        """
+        # sanity checks
+        assert case, "case_input_found_in_response(): Empty or missing test case data!"
+        assert response, "case_input_found_in_response(): Empty or missing TRAPI Response!"
+        assert "message" in response, "case_input_found_in_response(): TRAPI Response missing its Message component!"
+        assert trapi_version
+
+        #
+        # case: Dict parameter contains something like:
+        #
+        #     idx: 0,
+        #     subject_category: 'biolink:SmallMolecule',
+        #     object_category: 'biolink:Disease',
+        #     predicate: 'biolink:treats',
+        #     subject_id: 'CHEBI:3002',  # may have the deprecated key 'subject' here
+        #     object_id: 'MESH:D001249', # may have the deprecated key 'object' here
+        #
+        # the contents for which ought to be returned in
+        # the TRAPI Knowledge Graph, as a Result mapping?
+        #
+
+        message: Dict = response["message"]
+        if not (
+            "knowledge_graph" in message and message["knowledge_graph"] and
+            "results" in message and message["results"]
+        ):
+            # empty knowledge graph is syntactically ok, but in
+            # this, input test data edge is automatically deemed missing
+            return False
+
+        # TODO: We need to check **here*** whether or not the
+        #       TRAPI response returned the original test case edge!!?!!
+        #       Not totally sure if we should first search the Results then
+        #       the Knowledge Graph, or go directly to the Knowledge Graph...
+
+        # The Message Query Graph could be something like:
+        # "query_graph": {
+        #     "nodes": {
+        #         "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+        #         "drug": {"categories": ["biolink:Drug"]}
+        #     },
+        #     "edges": {
+        #         "treats": {
+        #             "subject": "drug",
+        #             "predicates": ["biolink:treats"],
+        #             "object": "type-2 diabetes"
+        #         }
+        #     }
+        # }
+        #
+        # with a Response Message Knowledge Graph
+        # dictionary with 'nodes' and 'edges':
+        #
+        # "knowledge_graph": {
+        #     "nodes": ...,
+        #     "edges": ...
+        # }
+        knowledge_graph: Dict = message["knowledge_graph"]
+
+        # In the Knowledge Graph:
+        #
+        #     "nodes": {
+        #         "MONDO:0005148": {"name": "type-2 diabetes"},
+        #         "CHEBI:6801": {"name": "metformin", "categories": ["biolink:Drug"]}
+        #     }
+        #
+        # Check for case 'subject_id' and 'object_id',
+        # with expected categories, in nodes catalog
+        nodes: Dict = knowledge_graph["nodes"]
+        subject_id = case["subject_id"] if "subject_id" in case else case["subject"]
+        if not self.case_node_found("subject", subject_id, case, nodes):
+            # 'subject' node not found?
+            return False
+
+        object_id = case["object_id"] if "object_id" in case else case["object"]
+        if not self.case_node_found("object", object_id, case, nodes):
+            # 'object' node not found?
+            return False
+
+        # In the Knowledge Graph:
+        #
+        #     "edges": {
+        #         "df87ff82": {
+        #             "subject": "CHEBI:6801",
+        #             "predicate": "biolink:treats",
+        #             "object": "MONDO:0005148"
+        #         }
+        #     }
+        #
+        # Check in the edges catalog for an edge containing
+        # the case 'subject_id', 'predicate' and 'object_id'
+        edges: Dict = knowledge_graph["edges"]
+
+        predicate = case["predicate"]
+
+        validator = BiolinkValidator(TRAPIGraphType.Knowledge_Graph, biolink_version=self.biolink_version)
+        inverse_predicate = validator.get_inverse_predicate(predicate)
+
+        edge_id_found: Optional[str] = None
+        for edge_id, edge in edges.items():
+            # Note: this edge search could be arduous on a big knowledge graph?
+            if edge["subject"] == subject_id and \
+                    edge["predicate"] == predicate and \
+                    edge["object"] == object_id:
+                edge_id_found = edge_id
+                break
+            elif edge["subject"] == object_id and \
+                    edge["predicate"] == inverse_predicate and \
+                    edge["object"] == subject_id:
+                # observation of the inverse edge is also counted as a match?
+                edge_id_found = edge_id
+                break
+
+        if edge_id_found is None:
+            # Test case S--P->O edge not found?
+            return False
+
+        results: List = message["results"]
+        if not self.case_result_found(subject_id, object_id, edge_id_found, results, trapi_version):
+            # Some components of test case S--P->O edge
+            # NOT bound within any Results?
+            return False
+
+        # By this point, the case data assumed to be
+        # successfully validated in the TRAPI Response?
+        return True
```

### Comparing `reasoner_validator-3.5.7/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.8/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Any, Dict, List, Tuple, Set
 from enum import Enum
 from functools import lru_cache
 from urllib.error import HTTPError
 from pprint import PrettyPrinter
 
 
-from bmt import Toolkit
+from bmt import Toolkit, utils
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
 from reasoner_validator.sri.util import is_curie
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.versioning import SemVer, SemVerError
 
 import logging
@@ -134,14 +134,50 @@
             current: SemVer = SemVer.from_string(self.biolink_version)
             target: SemVer = SemVer.from_string(version)
             return current >= target
         except SemVerError as sve:
             logger.error(f"minimum_required_biolink_version() error: {str(sve)}")
             return False
 
+    def is_symmetric(self, name: str) -> bool:
+        """
+        Checks if a given element identified by name, is a symmetric (predicate) slot.
+        :param name: name of the element
+        :return: True if element is a symmetric (predicate) slot.
+        """
+        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
+        if not name:
+            return False
+        element: Optional[Element] = self.bmt.get_element(name)
+        if element['symmetric']:
+            return True
+        else:
+            return False
+
+    def get_inverse_predicate(self, predicate: Optional[str]) -> Optional[str]:
+        """
+        Utility wrapper of logic to robustly test if a predicate exists and has an inverse.
+        :param predicate: CURIE or string name of predicate for which the inverse is sought.
+        :return: CURIE string of inverse predicate, if it exists; None otherwise
+        """
+        # TODO: perhaps this method ought to be in the Biolink Model Toolkit?
+        if predicate and self.bmt.is_predicate(predicate):
+            predicate_name = utils.parse_name(predicate)
+            inverse_predicate_name = self.bmt.get_inverse(predicate_name)
+            if not inverse_predicate_name:
+                if self.is_symmetric(predicate_name):
+                    inverse_predicate_name = predicate_name
+                else:
+                    inverse_predicate_name = None
+
+            if inverse_predicate_name:
+                ip = self.bmt.get_element(inverse_predicate_name)
+                return utils.format_element(ip)
+        return None
+
     def get_result(self) -> Tuple[str, Optional[Dict[str, Dict[str, Optional[List[Dict[str, str]]]]]]]:
         """
         Get result of validation.
 
         :return: model version of the validation and dictionary of reported validation messages.
         :rtype Tuple[str, Optional[Dict[str, Set[str]]]]
         """
```

### Comparing `reasoner_validator-3.5.7/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.8/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/report.py` & `reasoner_validator-3.5.8/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.8/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.8/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.8/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.8/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/reasoner_validator/versioning.py` & `reasoner_validator-3.5.8/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.8/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1617,15 +1617,14 @@
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
         query=query,
         biolink_version="suppress"
     )
 
 
-
 QC_QS_NOT_A_CURIE = {
     'qualifier_constraints': [
         {
             "qualifier_set": [
                 {
                     'qualifier_type_id': "not-a-curie",
                     'qualifier_value': "fake-qualifier-value"
@@ -2939,7 +2938,46 @@
         edge["sources"] = sources
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=sample_message,
         # trapi_version="latest",  # 1.4.0++
         biolink_version=LATEST_BIOLINK_MODEL_VERSION
     )
     check_messages(validator, validation_code)
+
+
+@pytest.mark.parametrize(
+    "predicate,result",
+    [
+        (None, False),
+        ("biolink:related_to", True),
+        ("related_to", True),
+        ("related to", True),
+        ("biolink:active_in", False),
+        ("active_in", False),
+        ("active in", False),
+        ("biolink:has_active_component", False)
+    ]
+)
+def test_is_symmetric(predicate, result):
+    # we assume the default is a late version which has proper inverse
+    validator: BiolinkValidator = BiolinkValidator(TRAPIGraphType.Knowledge_Graph, biolink_version=None)
+    assert validator.is_symmetric(predicate) == result
+
+
+@pytest.mark.parametrize(
+    "predicate,inverse",
+    [
+        (None, None),
+        ("", None),
+        ("biolink:related_to", "biolink:related_to"),
+        ("related_to", "biolink:related_to"),
+        ("related to", "biolink:related_to"),
+        ("biolink:active_in", "biolink:has_active_component"),
+        ("active_in", "biolink:has_active_component"),
+        ("active in", "biolink:has_active_component"),
+        ("biolink:has_active_component", "biolink:active_in")
+    ]
+)
+def test_get_inverse_predicate(predicate, inverse):
+    # we assume the default is a late version which has proper inverse
+    validator: BiolinkValidator = BiolinkValidator(TRAPIGraphType.Knowledge_Graph, biolink_version=None)
+    assert validator.get_inverse_predicate(predicate) == inverse
```

### Comparing `reasoner_validator-3.5.7/tests/test_data/sample_trapi_schema.yaml` & `reasoner_validator-3.5.8/tests/test_data/sample_trapi_schema.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_response_validator.py` & `reasoner_validator-3.5.8/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_semver.py` & `reasoner_validator-3.5.8/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_trapi_versioning.py` & `reasoner_validator-3.5.8/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_validate.py` & `reasoner_validator-3.5.8/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_validation_report.py` & `reasoner_validator-3.5.8/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/tests/test_workflows.py` & `reasoner_validator-3.5.8/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.7/PKG-INFO` & `reasoner_validator-3.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.7
+Version: 3.5.8
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

