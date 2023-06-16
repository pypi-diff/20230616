# Comparing `tmp/GOcats-1.1.7.tar.gz` & `tmp/GOcats-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GOcats-1.1.7.tar", last modified: Tue Oct  6 14:30:11 2020, max compression
+gzip compressed data, was "GOcats-1.2.1.tar", last modified: Fri Jun 16 21:55:19 2023, max compression
```

## Comparing `GOcats-1.1.7.tar` & `GOcats-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2020-10-06 14:30:11.940108 GOcats-1.1.7/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1723 2020-09-26 23:33:12.000000 GOcats-1.1.7/CHANGELOG
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2123 2020-09-26 23:02:23.000000 GOcats-1.1.7/CITATION
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2020-10-06 14:30:11.932108 GOcats-1.1.7/GOcats.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     7335 2020-10-06 14:30:11.000000 GOcats-1.1.7/GOcats.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      443 2020-10-06 14:30:11.000000 GOcats-1.1.7/GOcats.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2020-10-06 14:30:11.000000 GOcats-1.1.7/GOcats.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       18 2020-10-06 14:30:11.000000 GOcats-1.1.7/GOcats.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       13 2020-10-06 14:30:11.000000 GOcats-1.1.7/GOcats.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1821 2020-09-26 23:02:23.000000 GOcats-1.1.7/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       70 2020-09-26 23:02:23.000000 GOcats-1.1.7/MANIFEST.in
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     7335 2020-10-06 14:30:11.940108 GOcats-1.1.7/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     5411 2020-10-06 14:29:04.000000 GOcats-1.1.7/README.rst
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2020-10-06 14:30:11.936108 GOcats-1.1.7/gocats/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      135 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2913 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/__main__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       44 2020-09-26 23:28:51.000000 GOcats-1.1.7/gocats/_version.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    27898 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/dag.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    19210 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/gocats.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1419 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/godag.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     8339 2020-09-26 23:26:04.000000 GOcats-1.1.7/gocats/ontologyparser.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    19206 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/subdag.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3969 2020-09-26 23:02:23.000000 GOcats-1.1.7/gocats/tools.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       67 2020-10-06 14:30:11.940108 GOcats-1.1.7/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3911 2020-09-26 23:36:24.000000 GOcats-1.1.7/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2020-10-06 14:30:11.940108 GOcats-1.1.7/tests/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2020-09-26 23:02:23.000000 GOcats-1.1.7/tests/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       94 2020-09-26 23:02:23.000000 GOcats-1.1.7/tests/test_dummy.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      730 2020-09-26 23:02:23.000000 GOcats-1.1.7/tests/test_manuscript3.py
+drwxrwxr-x   0 rmflight  (1000) rmflight  (1000)        0 2023-06-16 21:55:19.011892 GOcats-1.2.1/
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     2069 2023-06-15 17:57:35.000000 GOcats-1.2.1/CHANGELOG
+drwxrwxr-x   0 rmflight  (1000) rmflight  (1000)        0 2023-06-16 21:55:19.007892 GOcats-1.2.1/GOcats.egg-info/
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     6758 2023-06-16 21:55:18.000000 GOcats-1.2.1/GOcats.egg-info/PKG-INFO
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)      434 2023-06-16 21:55:19.000000 GOcats-1.2.1/GOcats.egg-info/SOURCES.txt
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)        1 2023-06-16 21:55:18.000000 GOcats-1.2.1/GOcats.egg-info/dependency_links.txt
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       18 2023-06-16 21:55:18.000000 GOcats-1.2.1/GOcats.egg-info/requires.txt
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       13 2023-06-16 21:55:18.000000 GOcats-1.2.1/GOcats.egg-info/top_level.txt
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     1821 2023-06-06 13:26:14.000000 GOcats-1.2.1/LICENSE
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       70 2023-06-06 13:26:14.000000 GOcats-1.2.1/MANIFEST.in
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     6758 2023-06-16 21:55:19.011892 GOcats-1.2.1/PKG-INFO
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     5979 2023-06-16 21:33:29.000000 GOcats-1.2.1/README.rst
+drwxrwxr-x   0 rmflight  (1000) rmflight  (1000)        0 2023-06-16 21:55:19.011892 GOcats-1.2.1/gocats/
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)      135 2023-06-06 13:26:14.000000 GOcats-1.2.1/gocats/__init__.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     7951 2023-06-16 21:04:12.000000 GOcats-1.2.1/gocats/__main__.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       44 2023-06-15 19:19:19.000000 GOcats-1.2.1/gocats/_version.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)    27898 2023-06-06 13:26:14.000000 GOcats-1.2.1/gocats/dag.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)    20794 2023-06-16 21:04:28.000000 GOcats-1.2.1/gocats/gocats.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     1419 2023-06-06 13:26:14.000000 GOcats-1.2.1/gocats/godag.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     8339 2023-06-06 13:26:14.000000 GOcats-1.2.1/gocats/ontologyparser.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)    19199 2023-06-15 14:36:01.000000 GOcats-1.2.1/gocats/subdag.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     3969 2023-06-06 13:26:14.000000 GOcats-1.2.1/gocats/tools.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       67 2023-06-16 21:55:19.011892 GOcats-1.2.1/setup.cfg
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)     3911 2023-06-15 19:19:27.000000 GOcats-1.2.1/setup.py
+drwxrwxr-x   0 rmflight  (1000) rmflight  (1000)        0 2023-06-16 21:55:19.011892 GOcats-1.2.1/tests/
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)        0 2023-06-06 13:26:14.000000 GOcats-1.2.1/tests/__init__.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)       94 2023-06-06 13:26:14.000000 GOcats-1.2.1/tests/test_dummy.py
+-rw-rw-r--   0 rmflight  (1000) rmflight  (1000)      730 2023-06-06 13:26:14.000000 GOcats-1.2.1/tests/test_manuscript3.py
```

### Comparing `GOcats-1.1.7/CITATION` & `GOcats-1.2.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,35 @@
-..
-    The Clear BSD License
+The Clear BSD License
 
-    Copyright (c) 2017, Eugene W. Hinderer III, Hunter N.B. Moseley
-    All rights reserved.
+Copyright (c) 2017, Eugene W. Hinderer III, Hunter N.B. Moseley
+All rights reserved.
 
-    Redistribution and use in source and binary forms, with or without
-    modification, are permitted (subject to the limitations in the disclaimer
-    below) provided that the following conditions are met:
-
-    * Redistributions of source code must retain the above copyright notice, this
-      list of conditions and the following disclaimer.
-
-    * Redistributions in binary form must reproduce the above copyright notice,
-      this list of conditions and the following disclaimer in the documentation
-      and/or other materials provided with the distribution.
-
-    * Neither the name of the copyright holder nor the names of its contributors may be used
-      to endorse or promote products derived from this software without specific
-      prior written permission.
-
-    * If the source code is used in a published work, then proper citation of the source
-      code must be included with the published work.
-
-    NO EXPRESS OR IMPLIED LICENSES TO ANY PARTY'S PATENT RIGHTS ARE GRANTED BY THIS
-    LICENSE. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-    "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-    THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-    ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-    LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-    CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-    GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-    HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-    LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-    OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
-    DAMAGE.
-..
-
-*********
-Citations
-*********
-
-Software Citation
-=================
-
-If you use the GOcats software, you must cite:
-    GOcats Software URL https://figshare.com/s/26b336a06946a9248e08
+Redistribution and use in source and binary forms, with or without
+modification, are permitted (subject to the limitations in the disclaimer
+below) provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its contributors may be used
+  to endorse or promote products derived from this software without specific
+  prior written permission.
+
+* If the source code is used in a published work, then proper citation of the source
+  code must be included with the published work.
+
+NO EXPRESS OR IMPLIED LICENSES TO ANY PARTY'S PATENT RIGHTS ARE GRANTED BY THIS
+LICENSE. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGE.
```

### Comparing `GOcats-1.1.7/README.rst` & `GOcats-1.2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 specific annotations into customizable, biologically-relevant concept categories. Concept subgraphs are defined by lists
 of keywords created by the user.
 
 Currently, the `GOcats` package can be used to:
    * Create subgraphs of GO which each represent a user-specified concept.
    * Map specific, or fine-grained, GO terms in a Gene Annotation File (GAF) to an arbitrary number of concept
      categories.
+   * Remap ancestor Gene Ontology term relationships and the gene annotations with a set of user defined relationships.
    * Explore the Gene Ontology graph within a Python interpreter.
 
 Citation
 ~~~~~~~~
 Please cite the following papers when using GOcats:
 
 Hinderer EW, Moseley NHB. GOcats: A tool for categorizing Gene Ontology into subgraphs of user-defined concepts. PLoS One. 2020;15(6):1-29.
@@ -85,14 +86,21 @@
 
 GAF mappings can also be made from the command line:
 
 .. code:: bash
 
    python3 -m gocats categorize_dataset YOUR_GAF.goa YOUR_OUTPUT_DIRECTORY/GC_id_mapping.json_pickle YOUR_OUTPUT_DIRECTORY MAPPED_DATASET_NAME.goa
 
+Gene to GO Term remappings with consideration of ``has_part`` relationships can created from the command line:
+
+.. code:: bash
+
+   python3 -m gocats remap_goterms /path_to_ontology_file.obo /path_to_gaf.goa ancestors_output.json namespace_output.json --allowed_relationships=is_a,part_of,has_part --identifier_column=1
+
+Gene to GO terms will be in JSON format in ``ancestor_output.json``, and new GO term to namespace in ``namespace_output.json``.
 
 License
 ~~~~~~~
 
 Made available under the terms of The Clear BSD License. See full license in LICENSE.
 
 The Clear BSD License
```

### Comparing `GOcats-1.1.7/gocats/dag.py` & `GOcats-1.2.1/gocats/dag.py`

 * *Files identical despite different names*

### Comparing `GOcats-1.1.7/gocats/gocats.py` & `GOcats-1.2.1/gocats/gocats.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 for evaluating those subgraphs.
 """
 import os
 import sys
 import re
 import csv
 import jsonpickle
+import json
+from collections import defaultdict
 from . import ontologyparser
 from . import godag
 from . import subdag
 from . import tools
 from . import _version
 
 jsonpickle.set_encoder_options('json', sort_keys=True, indent=2)
@@ -71,97 +73,77 @@
     graph = godag.GoGraph(supergraph_namespace, allowed_relationships)
     go_parser = ontologyparser.GoParser(database, graph, relationship_directionality=relationship_directionality)
     go_parser.parse()
     database.close()
     return graph
 
 
-def create_subgraphs(args):
+def create_subgraphs(database_file, keyword_file, output_directory, supergraph_namespace=None, subgraph_namespace=None, supergraph_relationships=['is_a', 'part_of', 'has_part'], subgraph_relationships=['is_a', 'part_of', 'has_part'], map_supersets=False, output_termlist=False, go_basic_scoping=False, network_table_name=None, test=False):
     """Creates a graph object of an ontology, processed into :class:`gocats.dag.OboGraph` or to an object that
     inherits from :class:`gocats.dag.OboGraph`, and then extracts subgraphs which represent concepts that are defined
     by a list of provided keywords. Each subgraph is processed into :class:`gocats.subdag.SubGraph`.
 
     :param database_file: Ontology database file.
     :param keyword_file: A CSV file with two columns: column 1 naming categories, and column 2 listing search strings (no quotation marks, separated by semicolons).
     :param output_directory: The directory where results are stored.
-    :param --supergraph_namespace=<None>: OPTIONAL-Specify a supergraph sub-ontology to filter e.g. cellular_component.
-    :param --subgraph_namespace=<None>: OPTIONAL-Specify a subgraph sub-ontology to filter e.g. cellular_component.
-    :param --supergraph_relationships=[]: OPTIONAL-Specify a list of relationships to limit in the supergraph e.g. [is_a, part_of].
-    :param --subgraph_relationships=[]: OPTIONAL-Specify a list of relationships to limit in subgraphs e.g. [is_a, part_of].
-    :param --map_supersets: OPTIONAL-Allow subgraphs to subsume other subgraphs.
-    :param --output_termlist: OPTIONAL-Create a translation of ontology terms to their names to improve interpretability of dev test results.
-    :param --go-basic-scoping: OPTIONAL-Creates a GO graph similar to go-basic with only scoping-type relationships (is_a and part_of).
-    :param --network_table_name=<None>: OPTIONAL-Make a specific name for the network table produced from the subgraphs (defaults to NetworkTable.csv)
+    :param supergraph_namespace: a supergraph sub-ontology to filter e.g. cellular_component, optional
+    :param subgraph_namespace: a subgraph sub-ontology to filter e.g. cellular_component, optional
+    :param supergraph_relationships: a list of relationships to limit in the supergraph e.g. ['is_a', 'part_of'], optional
+    :param subgraph_relationships: a list of relationships to limit in subgraphs e.g. ['is_a', 'part_of'], optional
+    :param map_supersets: whether to allow subgraphs to subsume other subgraphs, logical, optional
+    :param output_termlist: whether to create a translation of ontology terms to their names to improve interpretability of dev test results, logical, optional
+    :param go-basic-scoping: whether to create a GO graph similar to go-basic with only scoping-type relationships (is_a and part_of), logical, optional
+    :param network_table_name: whether to make a specific name for the network table produced from the subgraphs (defaults to NetworkTable.csv)
     :return: None
     :rtype: :py:obj:`None`
     """
 
-    if args['--supergraph_namespace']:
-        supergraph_namespace = args['--supergraph_namespace']
-    else:
-        supergraph_namespace = None
-    if args['--subgraph_namespace']:
-        subgraph_namespace = args['--subgraph_namespace']
-    else:
-        subgraph_namespace = None
-    if args['--supergraph_relationships']:
-        supergraph_relationships = args['--supergraph_relationships']
-    else:
-        supergraph_relationships = None
-    if args['--subgraph_relationships']:
-        subgraph_relationships = args['--subgraph_relationships']
-    else:
-        subgraph_relationships = None
-    if args['--go-basic-scoping']:
+    if go_basic_scoping:
         supergraph_relationships = ['is_a', 'part_of']
         subgraph_relationships = ['is_a', 'part_of']
-    if args['--test']:
-        test = True
-    else:
-        test = False
 
     # Building the supergraph
-    database = open(args['<database_file>'], 'r')
-    output_directory = args['<output_directory>']
+    database = open(database_file, 'r')
+    output_directory = output_directory
     if not os.path.exists(output_directory):
         os.makedirs(output_directory)
-    database_name = os.path.basename(args['<database_file>'])
+    database_name = os.path.basename(database_file)
     graph_class = {'go.obo': godag.GoGraph(supergraph_namespace, supergraph_relationships)}
     try:
         supergraph = graph_class[database_name]
     except KeyError:
         print("The provided ontology filename was not recognized. Please do not rename ontology files. The accepted list of file names are as follows: \n", graph_class.keys())
         sys.exit()
     parsing_class = {'go.obo': ontologyparser.GoParser(database, supergraph)}
     try:
         parsing_class[database_name].parse()
     except KeyError:
         print("The provided ontology filename was not recognized. Please do not rename ontology files. The accepted list of file names are as follows: \n", graph_class.keys())
         sys.exit()
-    if args['--output_termlist']:
-        tools.jsonpickle_save(list(supergraph.id_index.keys()), os.path.join(args['<output_directory>'], "termlist"))
+    if output_termlist:
+        tools.jsonpickle_save(list(supergraph.id_index.keys()), os.path.join(output_directory, "termlist"))
 
     id_translation = dict()
     for id, node in supergraph.id_index.items():
         id_translation[id] = node.name
-    tools.jsonpickle_save(id_translation, os.path.join(args['<output_directory>'], "id_translation"))
+    tools.jsonpickle_save(id_translation, os.path.join(output_directory, "id_translation"))
 
     database.close()
 
     # Building and collecting subgraphs
     subgraph_collection = dict()
-    with open(args['<keyword_file>'], newline='') as file:
+    with open(keyword_file, newline='') as file:
         reader = csv.reader(file, delimiter=',', quoting=csv.QUOTE_MINIMAL)
         for row in reader:
             subgraph_name = row[0]
             keyword_list = [keyword for keyword in re.split(';', row[1])]
             subgraph_collection[subgraph_name] = subdag.SubGraph.from_filtered_graph(supergraph, subgraph_name, keyword_list, subgraph_namespace, subgraph_relationships)
 
     # Handling superset mapping
-    if not args['--map_supersets']:
+    if not map_supersets:
         category_subsets = find_category_subsets(subgraph_collection)
     else:
         print("NOTE: supersets were mapped.")
         category_subsets = None
 
     collection_id_mapping = dict()
     collection_node_mapping = dict()
@@ -185,18 +167,18 @@
         for node_id, root_id_list in collection_id_mapping.items():
             for subset_id, superset_ids in category_subsets.items():
                 if subset_id in root_id_list:
                     [root_id_list.remove(node) for node in superset_ids if node in root_id_list]
     # TODO: do the same for node_object_mapping
 
     # Save mapping files and create report
-    tools.jsonpickle_save(collection_id_mapping, os.path.join(args['<output_directory>'], "GC_id_mapping"))
-    tools.json_save(collection_id_mapping, os.path.join(args['<output_directory>'], "GC_id_mapping"))
-    tools.jsonpickle_save(collection_content_mapping, os.path.join(args['<output_directory>'], "GC_content_mapping"))
-    tools.json_save(collection_content_mapping, os.path.join(args['<output_directory>'], "GC_content_mapping"))
+    tools.jsonpickle_save(collection_id_mapping, os.path.join(output_directory, "GC_id_mapping"))
+    tools.json_save(collection_id_mapping, os.path.join(output_directory, "GC_id_mapping"))
+    tools.jsonpickle_save(collection_content_mapping, os.path.join(output_directory, "GC_content_mapping"))
+    tools.json_save(collection_content_mapping, os.path.join(output_directory, "GC_content_mapping"))
     with open(os.path.join(output_directory, 'subgraph_report.txt'), 'w') as report_file:
         report_file.write(
             'Subgraph data\nSupergraph filter: {}\nSubgraph filter: {}\nGO terms in the supergraph: {}\nGO terms in subgraphs: {}\nRelationship prevalence: {}'.format(
                 supergraph_namespace, subgraph_namespace, len(set(supergraph.node_list)),
                 len(set(collection_id_mapping.keys())), supergraph.relationship_count))
         for subgraph_name, subgraph in subgraph_collection.items():
             out_string = """
@@ -213,41 +195,39 @@
                            len(subgraph.node_list) - len(subgraph.root_id_mapping.keys()),
                            len(subgraph.root_id_mapping.keys()))
             report_file.write(out_string)
 
     # FIXME: cannot json save due to recursion of objects within objects...
     # tools.jsonpickle_save(collection_node_mapping, os.path.join(args['<output_directory>'], "GC_node_mapping"))
 
-    if args['--network_table_name']:
-        network_table_name = args['--network_table_name']
-    else:
+    if network_table_name is None:
         network_table_name = "Network_table.csv"
 
     # Making a file for network visualization via Cytoscape 3.0
-    with open(os.path.join(args['<output_directory>'], network_table_name), 'w', newline='') as network_table:
+    with open(os.path.join(output_directory, network_table_name), 'w', newline='') as network_table:
         edgewriter = csv.writer(network_table, delimiter=',', quotechar='|', quoting=csv.QUOTE_MINIMAL)
         for term_id, root_id_list in collection_id_mapping.items():
             for root_id in root_id_list:
                 edgewriter.writerow([term_id, root_id])
 
     if test:
-        json_graph_destination_file = os.path.join(args['<output_directory>'], str(__version__)+'_graph_output.json')
+        json_graph_destination_file = os.path.join(output_directory, str(__version__)+'_graph_output.json')
         with open(json_graph_destination_file, 'w') as destfile:
             destfile.write(jsonpickle.encode(json_format_graph(supergraph, 'supergraph')))
             for subgraph_name, subgraph in subgraph_collection.items():
                 destfile.write(jsonpickle.encode(json_format_graph(subgraph, subgraph_name)))
 
-        jsonpickle_supergraph_destination_file = os.path.join(args['<output_directory>'], str(__version__)+'_supergraph_output.jsonpickle')
+        jsonpickle_supergraph_destination_file = os.path.join(output_directory, str(__version__)+'_supergraph_output.jsonpickle')
         jsonpickle_clean_graph(supergraph)
         with open(jsonpickle_supergraph_destination_file, 'w') as destfile:
             destfile.write(jsonpickle.encode(supergraph))
 
         for subgraph_name, subgraph in subgraph_collection.items():
             jsonpickle_clean_graph(subgraph)
-            jsonpickle_subgraph_destination_file = os.path.join(args['<output_directory>'], str(__version__)+'_'+subgraph_name+'_output.jsonpickle')
+            jsonpickle_subgraph_destination_file = os.path.join(output_directory, str(__version__)+'_'+subgraph_name+'_output.jsonpickle')
             with open(jsonpickle_subgraph_destination_file, 'w') as destfile:
                 destfile.write(jsonpickle.encode(subgraph))
 
 
 def jsonpickle_clean_graph(graph):
     # remove circular references from the nodes
     for node in graph.node_list:
@@ -290,51 +270,39 @@
                     try:
                         is_subset_of[next(iter(subgraph.category_node.child_node_set)).id].add(next(iter(next_subgraph.category_node.child_node_set)).id)
                     except KeyError:
                         is_subset_of[next(iter(subgraph.category_node.child_node_set)).id] = {next(iter(next_subgraph.category_node.child_node_set)).id}
     return is_subset_of
 
 
-def categorize_dataset(args):
+def categorize_dataset(dataset_file, term_mapping, output_directory, mapped_dataset_filename, dataset_type="GAF", entity_col=0, go_col=1, retain_unmapped_annotations=False):
     """Reads in a Gene Annotation File (GAF) and maps the annotations contained therein to the categories organized by
     GOcats or other methods. Outputs a mapped GAF and a list of unmapped genes in the specified output directory.
 
     :param dataset_file: A file containing gene annotations.
     :param term_mapping: A dictionary mapping category-defining ontology terms to their subgraph children terms. May be produced by GOcats or another method.
-    :param output_directory: Specify the directory where the output file will be stored.
-    :param mapped_dataset_filename: Specify the desired name of the mapped GAF.
-    :param --dataset_type: Enter file type for dataset [GAF|TSV|CSV]. Defaults to GAF.
-    :param --entity_col=<0>: If CSV or TSV file type, indicate which column the entity IDs are listed. Defaults to 0.
-    :param --go_col: If CSV or TSV file type, indicate which column the GO IDs are listed. Defaults to 1.
-    :param --retain_unmapped_annotations: If specified, annotations that are not mapped to a concept are copied into the mapped dataset output file with its original annotation.
+    :param output_directory: The directory where the output file will be stored.
+    :param mapped_dataset_filename: The desired name of the mapped GAF.
+    :param dataset_type: Enter file type for dataset [GAF|TSV|CSV]. Defaults to "GAF".
+    :param entity_col: If CSV or TSV file type, indicate which column the entity IDs are listed. Defaults to 0.
+    :param go_col: If CSV or TSV file type, indicate which column the GO IDs are listed. Defaults to 1.
+    :param retain_unmapped_annotations: If specified, annotations that are not mapped to a concept are copied into the mapped dataset output file with its original annotation.
     :return: None
     :rtype: :py:obj:`None`
     """
-    if args['--dataset_type']:
-        dataset_type = args['--dataset_type']
-    else:
-        dataset_type = None
-    if args['--entity_col']:
-        entity_id_index = int(args['--entity_col'])
-    else:
-        entity_id_index = 0
-    if args['--go_col']:
-        go_id_index = int(args['--go_col'])
-    else:
-        go_id_index = 1
+    
 
-    mapping_dict = tools.jsonpickle_load(args['<term_mapping>'])
-    output_directory = os.path.realpath(args['<output_directory>'])
-    mapped_dataset_filename = args['<mapped_dataset_filename>']
+    mapping_dict = tools.jsonpickle_load(term_mapping)
+    output_directory = os.path.realpath(output_directory)
     unmapped_entities = set()
     if not os.path.exists(output_directory):
         os.makedirs(output_directory)
 
     if dataset_type == "GAF" or not dataset_type:
-        loaded_gaf_array = tools.parse_gaf(args['<dataset_file>'])
+        loaded_gaf_array = tools.parse_gaf(dataset_file)
         mapped_gaf_array = list()
         for line in loaded_gaf_array:
             if line[4] in mapping_dict.keys():
                 mapped_terms = mapping_dict[line[4]]
                 for term in mapped_terms:
                     mapped_gaf_array.append(line[0:4] + [term] + line[5:-1])
             else:
@@ -343,26 +311,70 @@
                 else:
                     unmapped_entities.add(line[2])
         tools.write_out_gaf(mapped_gaf_array, os.path.join(output_directory, mapped_dataset_filename))
         tools.list_to_file(os.path.join(output_directory, mapped_dataset_filename + '_unmappedEntities'), unmapped_entities)
 
     elif dataset_type == "CSV":
         mapped_rows = []
-        with open(os.path.realpath(args['<dataset_file>']), 'r') as csv_file:
+        with open(os.path.realpath(dataset_file), 'r') as csv_file:
             csv_reader = csv.reader(csv_file, delimiter=',')
             header = next(csv_reader)
             for row in csv_reader:
                 mapped_row = row
                 if mapped_row[go_id_index] in mapping_dict.keys():
                     for concept_term in mapping_dict[mapped_row[go_id_index]]:
                         mapped_row[go_id_index] = concept_term
                         mapped_rows.append(mapped_row)
                 else:
                     unmapped_entities.add(mapped_row[entity_id_index])
-                    if args['--retain_unmapped_annotations']:
+                    if retain_unmapped_annotations:
                         mapped_rows.append(mapped_row)
             mapped_rows.insert(0, header)
         with open(os.path.join(output_directory, mapped_dataset_filename), 'w') as output_csv:
             csv_writer = csv.writer(output_csv, delimiter=',')
             for row in mapped_rows:
                 csv_writer.writerow([item for item in row])
         tools.list_to_file(os.path.join(output_directory, 'unmappedEntities'), unmapped_entities)
+
+
+def remap_goterms(go_database, goa_gaf, ancestor_filename, namespace_filename, allowed_relationships, identifier_column):
+    """Reads in a Gene Ontology relationship file, and a Gene Annotation File (GAF), and
+    follows the GOcats rules for allowed term-to-term relationships. Generates as output
+    a new GAF, and a new term to ontology namespace mapping.
+    
+    :param go_database: the gene ontology dataset
+    :param goa_gaf: the gene annotation file
+    :param ancestor_filename: the output file containing new gene to ontology mappings
+    :param namespace_filename: the output file containing the term to ontology mappings
+    :param allowed_relationships: what term to term relationships will be considered (is_a,part_of,has_part) 
+    :param identifier_column: which column is being used for the gene identifiers (1)
+    :return: None
+    :rtype: :py:obj:`None`
+    """
+    
+    graph = build_graph_interpreter(go_database, allowed_relationships=allowed_relationships)
+    gaf_array = tools.parse_gaf(goa_gaf)
+    goa_gene_annotation_dict = defaultdict(set)
+    # Building the annotation dictionary
+    for line in gaf_array:
+        goa_gene_annotation_dict[line[identifier_column]].add(line[4]) # the dictionary has DB object symbol  keys and a set of go terms as values
+    ancestor_dict = defaultdict(set)
+    missing_go_terms = set()
+    # Adding ancestors to the annotation dictionary.
+    for gene_symbol, go_term_set in goa_gene_annotation_dict.items():
+        ancestor_dict[gene_symbol].update(go_term_set)
+        for go_term in go_term_set:
+            if go_term in graph.id_index.keys():
+                ancestor_dict[gene_symbol].update([node.id for node in graph.id_index[go_term].ancestors])
+            else:
+                missing_go_terms.add(go_term)  # NOTE: These are missing because they are depreciated IDs that are now ALT IDs of another term. Need to incorporate alt ids in GOcats.
+    # Need to convert dict sets into lists for json
+    ancestor_dict = {gene_symbol: list(go_term_set) for gene_symbol, go_term_set in ancestor_dict.items()}
+    # Writeout output json file.
+    with open(ancestor_filename, "w") as output_file:
+        json.dump(ancestor_dict, output_file)
+    with open(namespace_filename, "w") as output_file:
+        namespace_translation = {}
+        for node in graph.node_list:
+            namespace_translation[node.id] = node.namespace
+        json.dump(namespace_translation, output_file)
+    return None
```

### Comparing `GOcats-1.1.7/gocats/godag.py` & `GOcats-1.2.1/gocats/godag.py`

 * *Files identical despite different names*

### Comparing `GOcats-1.1.7/gocats/ontologyparser.py` & `GOcats-1.2.1/gocats/ontologyparser.py`

 * *Files identical despite different names*

### Comparing `GOcats-1.1.7/gocats/subdag.py` & `GOcats-1.2.1/gocats/subdag.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         elif not self.category_node:
             raise Exception("Mapping failed: category node not identified.")
         return self._root_id_mapping
 
     @property
     def root_node_mapping(self):
         """Property describing a mapping :py:obj:`dict` that relates every ontology :class:`gocats.subdag.SubGraphNode`
-        object of subgraphs in :class:`gocats.subdag.SubGraph` to a :py:obj:`list` of root
-       :class:`gocats.subdag.CategoryNode` objects.
+        object of subgraphs in :class:`gocats.subdag.SubGraph` to a :py:obj:`list` of root :class:`gocats.subdag.CategoryNode` objects.
 
         :return: :py:obj:`dict` of :class:`gocats.subdag.SubGraphNode` objects mapped to a :py:obj:`list` of root :class:`gocats.subdag.CategoryNode` objects.
         :rtype: :py:obj:`dict`
         """
         if (self._modified and self.category_node) or self._root_node_mapping == None:
             self._root_node_mapping = {node: self.category_node for node in self.category_node.descendants}
             self._root_node_mapping[self.category_node] = self.category_node
```

### Comparing `GOcats-1.1.7/gocats/tools.py` & `GOcats-1.2.1/gocats/tools.py`

 * *Files identical despite different names*

### Comparing `GOcats-1.1.7/setup.py` & `GOcats-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 setup(
     name='GOcats',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
 
-    version='1.1.7',
+    version='1.2.1',
 
     description='A tool for categorizing Gene Ontology into subgraphs of user-defined emergent concepts',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/MoseleyBioinformaticsLab/GOcats',
```

### Comparing `GOcats-1.1.7/tests/test_manuscript3.py` & `GOcats-1.2.1/tests/test_manuscript3.py`

 * *Files identical despite different names*

