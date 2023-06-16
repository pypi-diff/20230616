# Comparing `tmp/llm_client-0.5.0.tar.gz` & `tmp/llm_client-0.6.0.tar.gz`

## Comparing `llm_client-0.5.0.tar` & `llm_client-0.6.0.tar`

### file list

```diff
@@ -1,289 +1,309 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.5.0/.DS_Store
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 llm_client-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/anthropic_client.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/google_client.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/sync/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 llm_client-0.5.0/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate.fish
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/convert-caffe2-to-onnx
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/convert-onnx-to-caffe2
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/docutils
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/f2py
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/f2py3
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/f2py3.11
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/httpx
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/huggingface-cli
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/isympy
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/keyring
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/normalizer
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/openai
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pip3.11
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pkginfo
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/publish.py
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/py.test
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyproject-build
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-decrypt
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-encrypt
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-keygen
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-priv2pub
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-sign
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pyrsa-verify
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2html.py
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2man.py
--rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2odt.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/torchrun
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/tqdm
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/transformers-cli
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/twine
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/wheel-3.11
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/bin/wheel3.11
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/etc/jupyter/nbconfig/notebook.d/jupyterlab-plotly.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/LICENSE.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/README.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
--rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
--rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
--rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/package.json
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-r--r--   0        0        0  3578814 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-r--r--   0        0        0    70520 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/style.js
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/extension.js
--rw-r--r--   0        0        0  3666905 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.5.0/new_venv/share/man/man1/isympy.1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/conftest.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/anthropic_client/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/anthropic_client/conftest.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/google_client/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/google_client/conftest.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/google_client/test_google_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/google/chat_completion.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/google/embedding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/google/text_completion.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/google/tokens_count.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/sync/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/sync/test_sync_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.5.0/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/Activate.ps1
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/activate
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/activate.csh
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/activate.fish
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/docutils
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/keyring
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/normalizer
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pip
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pip3
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pip3.10
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pip3.9
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pkginfo
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pygmentize
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/python -> python3.9
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/python3 -> python3.9
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/python3.9 -> /opt/miniconda3/bin/python3.9
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2html.py
--rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1107 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2html5.py
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2latex.py
--rwxr-xr-x   0        0        0      672 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2man.py
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2odt.py
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2s5.py
--rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rst2xml.py
--rwxr-xr-x   0        0        0      726 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_3_9/bin/twine
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/pyvenv.cfg
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate.csh
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate.fish
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/deactivate.nu
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/normalizer
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/pip
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/pip3
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/pip3.11
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/py.test
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/wheel
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/wheel-3.11
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/wheel3
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_ai21/bin/wheel3.11
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/.gitignore
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/pyvenv.cfg
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate.csh
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate.fish
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/activate_this.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/deactivate.nu
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/f2py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/f2py3
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/f2py3.11
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/huggingface-cli
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/normalizer
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/pip3
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/pip3.11
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/py.test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/tqdm
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/transformers-cli
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/wheel
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/wheel-3.11
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/wheel3
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.5.0/venv_local/bin/wheel3.11
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.5.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.5.0/LICENSE
--rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 llm_client-0.5.0/README.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 llm_client-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 llm_client-0.6.0/.DS_Store
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 llm_client-0.6.0/preformnce_banchmark.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/anthropic_client.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/google_client.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 llm_client-0.6.0/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate.csh
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate.fish
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/convert-caffe2-to-onnx
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/convert-onnx-to-caffe2
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/docutils
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/f2py
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/f2py3
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/f2py3.11
+-rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/get_objgraph
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/httpx
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/isympy
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/keyring
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/langchain
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/langchain-server
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/markdown-it
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/normalizer
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/openai
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pip
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pip3
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pip3.11
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pkginfo
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/publish.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/py.test
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pygmentize
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyproject-build
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-decrypt
+-rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-encrypt
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-keygen
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-priv2pub
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-sign
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pyrsa-verify
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      835 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      654 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      723 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/torchrun
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/tqdm
+-rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/transformers-cli
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/twine
+-rwxr-xr-x   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/undill
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/wheel
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/wheel3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/bin/wheel3.11
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/etc/jupyter/nbconfig/notebook.d/jupyterlab-plotly.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/LICENSE.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/README.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/README.txt
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/README.txt
+-rw-r--r--   0        0        0  1346746 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/README.txt
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/README.txt
+-rw-r--r--   0        0        0   100224 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
+-rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/README.txt
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
+-rw-r--r--   0        0        0    33695 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/subclass/README.txt
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/package.json
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-r--r--   0        0        0     8368 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-r--r--   0        0        0  3578814 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-r--r--   0        0        0    70520 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-r--r--   0        0        0    14737 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/style.js
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/extension.js
+-rw-r--r--   0        0        0  3666905 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 llm_client-0.6.0/new_venv/share/man/man1/isympy.1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/conftest.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/anthropic_client/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/anthropic_client/conftest.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/google_client/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/google_client/conftest.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/google_client/test_google_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/google/chat_completion.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/google/embedding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/google/text_completion.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/google/tokens_count.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.0/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/Activate.ps1
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/activate
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/activate.csh
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/activate.fish
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/docutils
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/f2py
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/f2py3
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/f2py3.9
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/httpx
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/keyring
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/normalizer
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/openai
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pip
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pip3
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pip3.10
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pip3.9
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pkginfo
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/publish.py
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/py.test
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pygmentize
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyproject-build
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-decrypt
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-encrypt
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-keygen
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-priv2pub
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-sign
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pyrsa-verify
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/python -> python3.9
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/python3 -> python3.9
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/python3.9 -> /opt/miniconda3/bin/python3.9
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2html.py
+-rwxr-xr-x   0        0        0      772 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1107 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      672 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2man.py
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      726 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/tqdm
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/transformers-cli
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_3_9/bin/twine
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/pyvenv.cfg
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate.csh
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate.fish
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/normalizer
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/pip
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/pip3
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/pip3.11
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/py.test
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/wheel
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/wheel3
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_ai21/bin/wheel3.11
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/.gitignore
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/pyvenv.cfg
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate.csh
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate.fish
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/activate_this.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/f2py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/f2py3
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/f2py3.11
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/huggingface-cli
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/normalizer
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/pip
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/pip3
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/pip3.11
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/py.test
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/python -> /Library/Frameworks/Python.framework/Versions/3.11/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/tqdm
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/transformers-cli
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/wheel
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/wheel3
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 llm_client-0.6.0/venv_local/bin/wheel3.11
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 llm_client-0.6.0/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 llm_client-0.6.0/PKG-INFO
```

### Comparing `llm_client-0.5.0/.DS_Store` & `llm_client-0.6.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/.github/workflows/test.yml` & `llm_client-0.6.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   test:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9", "3.10", "3.11"]
-        flavor: [all, api, base-api, openai, huggingface, anthropic, local, sync]
+        flavor: [all, api, base-api, openai, huggingface, anthropic, local]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
@@ -39,14 +39,11 @@
             ;;
           base-api)
             pytest tests/llm_api_client/ai21_client tests/llm_api_client/google_client
             ;;
           local)
             pytest tests/llm_client/local_client
             ;;
-          sync)
-            pytest tests/sync
-            ;;
           *)
             pytest tests/llm_api_client/${{ matrix.flavor }}_client
             ;;
         esac
```

### Comparing `llm_client-0.5.0/llm_client/__init__.py` & `llm_client-0.6.0/llm_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
     from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
@@ -31,14 +31,10 @@
 # load local clients
 try:
     from llm_client.llm_client.local_client import LocalClient, LocalClientConfig
 except ImportError:
     pass
 # load sync support
 try:
-    from llm_client.sync.get_sync_llm_client import get_sync_llm_client
-    try:
-        from llm_client.sync.sync_llm_api_client_factory import SyncLLMAPIClientFactory
-    except ImportError:
-        pass
+    from llm_client.sync.sync_llm_api_client_factory import init_sync_llm_api_client
 except ImportError:
     pass
```

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/ai21_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/anthropic_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/anthropic_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/base_llm_api_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/base_llm_api_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/google_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/huggingface_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/huggingface_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.6.0/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,40 +13,45 @@
     ALEPH_ALPHA = "AlephAlpha"
     ANTHROPIC = "ANTHROPIC"
     GOOGLE = "GOOGLE"
 
 
 class LLMAPIClientFactory:
     def __init__(self):
-        self._client_session: Optional[ClientSession] = None
+        self._session: Optional[ClientSession] = None
 
     async def __aenter__(self):
-        self._client_session = ClientSession()
+        self._session = ClientSession()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self._client_session.close()
+        await self._session.close()
 
     def get_llm_api_client(self, llm_api_client_type: LLMAPIClientType, **config_kwargs) -> BaseLLMAPIClient:
-        if self._client_session is None:
+        if self._session is None:
             raise ValueError("Must be used as an context manager")
-        config = LLMAPIClientConfig(session=self._client_session, **config_kwargs)
-        if llm_api_client_type == LLMAPIClientType.OPEN_AI:
-            from llm_client import OpenAIClient
-            return OpenAIClient(config)
-        elif llm_api_client_type == LLMAPIClientType.AI21:
-            from llm_client import AI21Client
-            return AI21Client(config)
-        elif llm_api_client_type == LLMAPIClientType.HUGGING_FACE:
-            from llm_client import HuggingFaceClient
-            return HuggingFaceClient(config)
-        elif llm_api_client_type == LLMAPIClientType.ALEPH_ALPHA:
-            from llm_client import AlephAlphaClient
-            return AlephAlphaClient(config)
-        elif llm_api_client_type == LLMAPIClientType.ANTHROPIC:
-            from llm_client import AnthropicClient
-            return AnthropicClient(config)
-        elif llm_api_client_type == LLMAPIClientType.GOOGLE:
-            from llm_client import GoogleClient
-            return GoogleClient(config)
-        else:
-            raise ValueError("Unknown LLM client type")
+        config = LLMAPIClientConfig(session=self._session, **config_kwargs)
+        llm_api_client_class = get_llm_api_client_class(llm_api_client_type)
+        return llm_api_client_class(config)
+
+
+def get_llm_api_client_class(llm_api_client_type: LLMAPIClientType):
+    if llm_api_client_type == LLMAPIClientType.OPEN_AI:
+        from llm_client import OpenAIClient
+        return OpenAIClient
+    elif llm_api_client_type == LLMAPIClientType.AI21:
+        from llm_client import AI21Client
+        return AI21Client
+    elif llm_api_client_type == LLMAPIClientType.HUGGING_FACE:
+        from llm_client import HuggingFaceClient
+        return HuggingFaceClient
+    elif llm_api_client_type == LLMAPIClientType.ALEPH_ALPHA:
+        from llm_client import AlephAlphaClient
+        return AlephAlphaClient
+    elif llm_api_client_type == LLMAPIClientType.ANTHROPIC:
+        from llm_client import AnthropicClient
+        return AnthropicClient
+    elif llm_api_client_type == LLMAPIClientType.GOOGLE:
+        from llm_client import GoogleClient
+        return GoogleClient
+    else:
+        raise ValueError("Unknown LLM client type")
```

### Comparing `llm_client-0.5.0/llm_client/llm_api_client/openai_client.py` & `llm_client-0.6.0/llm_client/llm_api_client/openai_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/llm_client/llm_client/local_client.py` & `llm_client-0.6.0/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate` & `llm_client-0.6.0/new_venv/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate.csh` & `llm_client-0.6.0/new_venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate.fish` & `llm_client-0.6.0/new_venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate.nu` & `llm_client-0.6.0/new_venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate.ps1` & `llm_client-0.6.0/new_venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/activate_this.py` & `llm_client-0.6.0/new_venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/deactivate.nu` & `llm_client-0.6.0/new_venv/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/publish.py` & `llm_client-0.6.0/new_venv/bin/publish.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2html.py` & `llm_client-0.6.0/new_venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2html4.py` & `llm_client-0.6.0/new_venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2html5.py` & `llm_client-0.6.0/new_venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2latex.py` & `llm_client-0.6.0/new_venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2man.py` & `llm_client-0.6.0/new_venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2odt.py` & `llm_client-0.6.0/new_venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2odt_prepstyles.py` & `llm_client-0.6.0/new_venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2pseudoxml.py` & `llm_client-0.6.0/new_venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2s5.py` & `llm_client-0.6.0/new_venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2xetex.py` & `llm_client-0.6.0/new_venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rst2xml.py` & `llm_client-0.6.0/new_venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/bin/rstpep2html.py` & `llm_client-0.6.0/new_venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/LICENSE.txt` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_snap.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_properties.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_read_write.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_center_node.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_degree.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_directed.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_sampson.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_tsp.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/drawing/unix_email.mbox`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_football.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_mst.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_roget.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_triad_types.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/plot_words.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py` & `llm_client-0.6.0/new_venv/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/package.json` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json` & `llm_client-0.6.0/new_venv/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js` & `llm_client-0.6.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt` & `llm_client-0.6.0/new_venv/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/new_venv/share/man/man1/isympy.1` & `llm_client-0.6.0/new_venv/share/man/man1/isympy.1`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.6.0/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest.mock import patch
 
 import pytest
 
 from llm_client import LLMAPIClientType, LLMAPIClientFactory, LLMAPIClientConfig
+from llm_client.llm_api_client.llm_api_client_factory import get_llm_api_client_class
 
 
 def test_get_llm_api_client__without_context_manager():
     llm_api_client_factory = LLMAPIClientFactory()
     with pytest.raises(ValueError):
         llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI, api_key="super secret key")
 
@@ -23,17 +24,38 @@
 
     llm_api_client_factory = LLMAPIClientFactory()
     async with llm_api_client_factory:
         with patch(f"llm_client.{client_patch}") as mock_client:
             actual = llm_api_client_factory.get_llm_api_client(client_type, api_key="super secret key")
 
             assert actual is mock_client.return_value
-            mock_client.assert_called_once_with(LLMAPIClientConfig(session=llm_api_client_factory._client_session,
+            mock_client.assert_called_once_with(LLMAPIClientConfig(session=llm_api_client_factory._session,
                                                                    api_key="super secret key"))
 
 
 @pytest.mark.asyncio
 async def test_get_llm_api_client__with_unknown_client_type():
     llm_api_client_factory = LLMAPIClientFactory()
     async with llm_api_client_factory:
         with pytest.raises(ValueError):
             llm_api_client_factory.get_llm_api_client("unknown-client-type", api_key="super secret key")
+
+
+@pytest.mark.parametrize("client_type,client_patch",
+                         [(LLMAPIClientType.OPEN_AI, "OpenAIClient"), (LLMAPIClientType.AI21, "AI21Client"),
+                          (LLMAPIClientType.HUGGING_FACE, "HuggingFaceClient"),
+                          (LLMAPIClientType.ALEPH_ALPHA, "AlephAlphaClient"),
+                          (LLMAPIClientType.ANTHROPIC, "AnthropicClient"),
+                          (LLMAPIClientType.GOOGLE, "GoogleClient")])
+def test_get_llm_api_client_class(client_type, client_patch):
+    assert len(LLMAPIClientType) == 6
+
+    with patch(f"llm_client.{client_patch}") as mock_client:
+        actual = get_llm_api_client_class(client_type)
+
+        assert actual is mock_client
+        mock_client.assert_not_called()
+
+
+def test_get_llm_api_client_class__with_unknown_client_type():
+    with pytest.raises(ValueError):
+        get_llm_api_client_class("unknown-client-type")
```

### Comparing `llm_client-0.5.0/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.6.0/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.6.0/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/anthropic_client/conftest.py` & `llm_client-0.6.0/tests/llm_api_client/anthropic_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py` & `llm_client-0.6.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/google_client/conftest.py` & `llm_client-0.6.0/tests/llm_api_client/google_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/google_client/test_google_client.py` & `llm_client-0.6.0/tests/llm_api_client/google_client/test_google_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.6.0/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.6.0/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/openai_client/conftest.py` & `llm_client-0.6.0/tests/llm_api_client/openai_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.6.0/tests/llm_api_client/openai_client/test_openai.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_client/local_client/conftest.py` & `llm_client-0.6.0/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.6.0/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/tests/resources/ai21/text_completion.json` & `llm_client-0.6.0/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/Activate.ps1` & `llm_client-0.6.0/venv_3_9/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/activate` & `llm_client-0.6.0/venv_3_9/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/activate.csh` & `llm_client-0.6.0/venv_3_9/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/activate.fish` & `llm_client-0.6.0/venv_3_9/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2html.py` & `llm_client-0.6.0/venv_3_9/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2html4.py` & `llm_client-0.6.0/venv_3_9/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2html5.py` & `llm_client-0.6.0/venv_3_9/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2latex.py` & `llm_client-0.6.0/venv_3_9/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2man.py` & `llm_client-0.6.0/venv_3_9/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2odt.py` & `llm_client-0.6.0/venv_3_9/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2odt_prepstyles.py` & `llm_client-0.6.0/venv_3_9/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2pseudoxml.py` & `llm_client-0.6.0/venv_3_9/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2s5.py` & `llm_client-0.6.0/venv_3_9/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2xetex.py` & `llm_client-0.6.0/venv_3_9/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rst2xml.py` & `llm_client-0.6.0/venv_3_9/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_3_9/bin/rstpep2html.py` & `llm_client-0.6.0/venv_3_9/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate` & `llm_client-0.6.0/venv_ai21/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate.csh` & `llm_client-0.6.0/venv_ai21/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate.fish` & `llm_client-0.6.0/venv_ai21/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate.nu` & `llm_client-0.6.0/venv_ai21/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate.ps1` & `llm_client-0.6.0/venv_ai21/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/activate_this.py` & `llm_client-0.6.0/venv_ai21/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_ai21/bin/deactivate.nu` & `llm_client-0.6.0/venv_ai21/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate` & `llm_client-0.6.0/venv_local/bin/activate`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate.csh` & `llm_client-0.6.0/venv_local/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate.fish` & `llm_client-0.6.0/venv_local/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate.nu` & `llm_client-0.6.0/venv_local/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate.ps1` & `llm_client-0.6.0/venv_local/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/activate_this.py` & `llm_client-0.6.0/venv_local/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/venv_local/bin/deactivate.nu` & `llm_client-0.6.0/venv_local/bin/deactivate.nu`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/.gitignore` & `llm_client-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/LICENSE` & `llm_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/README.md` & `llm_client-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -124,29 +124,29 @@
 
 OPENAI_API_KEY = os.environ["API_KEY"]
 
 
 async def main():
     async with LLMAPIClientFactory() as llm_api_client_factory:
         llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
-                                                               api_key=OPENAI_API_KEY)
+                                                               api_key=OPENAI_API_KEY,
+                                                               default_model="text-davinci-003")
 
         await llm_client.text_completion(prompt="This is indeed a test")
         await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
         
 # Or if you don't want to use async
-from llm_client import SyncLLMAPIClientFactory
+from llm_client import init_sync_llm_api_client
 
-with SyncLLMAPIClientFactory() as llm_api_client_factory:
-    llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
-                                                           api_key=OPENAI_API_KEY)
+llm_client = init_sync_llm_api_client(LLMAPIClientType.OPEN_AI, api_key=OPENAI_API_KEY,
+                                      default_model="text-davinci-003")
 
-    llm_client.text_completion(prompt="This is indeed a test")
-    llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
+llm_client.text_completion(prompt="This is indeed a test")
+llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 Local model
 ```python
 import os
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 from llm_client import LocalClientConfig, LocalClient
```

### Comparing `llm_client-0.5.0/pyproject.toml` & `llm_client-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_client-0.5.0/PKG-INFO` & `llm_client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -167,29 +167,29 @@
 
 OPENAI_API_KEY = os.environ["API_KEY"]
 
 
 async def main():
     async with LLMAPIClientFactory() as llm_api_client_factory:
         llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
-                                                               api_key=OPENAI_API_KEY)
+                                                               api_key=OPENAI_API_KEY,
+                                                               default_model="text-davinci-003")
 
         await llm_client.text_completion(prompt="This is indeed a test")
         await llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 
         
 # Or if you don't want to use async
-from llm_client import SyncLLMAPIClientFactory
+from llm_client import init_sync_llm_api_client
 
-with SyncLLMAPIClientFactory() as llm_api_client_factory:
-    llm_client = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.OPEN_AI,
-                                                           api_key=OPENAI_API_KEY)
+llm_client = init_sync_llm_api_client(LLMAPIClientType.OPEN_AI, api_key=OPENAI_API_KEY,
+                                      default_model="text-davinci-003")
 
-    llm_client.text_completion(prompt="This is indeed a test")
-    llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
+llm_client.text_completion(prompt="This is indeed a test")
+llm_client.text_completion(prompt="This is indeed a test", max_tokens=50)
 ```
 Local model
 ```python
 import os
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 from llm_client import LocalClientConfig, LocalClient
```

