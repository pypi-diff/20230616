# Comparing `tmp/bas_geoplot-0.0.19.tar.gz` & `tmp/bas_geoplot-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bas_geoplot-0.0.19.tar", last modified: Tue Jun  6 12:54:58 2023, max compression
+gzip compressed data, was "bas_geoplot-0.0.20.tar", last modified: Fri Jun 16 08:38:34 2023, max compression
```

## Comparing `bas_geoplot-0.0.19.tar` & `bas_geoplot-0.0.20.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.19/LICENSE
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/MANIFEST.in
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/README.md
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.411331 bas_geoplot-0.0.19/bas_geoplot/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-06-06 12:52:13.000000 bas_geoplot-0.0.19/bas_geoplot/__init__.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5358 2023-06-06 12:53:52.000000 bas_geoplot-0.0.19/bas_geoplot/cli.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/bas_geoplot/config/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7342 2023-04-20 13:24:57.000000 bas_geoplot-0.0.19/bas_geoplot/config/interactive.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.19/bas_geoplot/config/static.json
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    34748 2023-06-06 12:52:13.000000 bas_geoplot-0.0.19/bas_geoplot/interactive.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/bas_geoplot/static.py
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2201 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/bas_geoplot/utils.py
-drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/bas_geoplot.egg-info/
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/PKG-INFO
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/entry_points.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/not-zip-safe
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/requires.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-06-06 12:54:58.000000 bas_geoplot-0.0.19/bas_geoplot.egg-info/top_level.txt
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-06-06 12:54:58.415331 bas_geoplot-0.0.19/setup.cfg
--rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.19/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-16 08:38:34.627796 bas_geoplot-0.0.20/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-10-25 08:33:04.000000 bas_geoplot-0.0.20/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       92 2022-10-21 13:21:48.000000 bas_geoplot-0.0.20/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-16 08:38:34.627796 bas_geoplot-0.0.20/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2004 2022-10-21 13:21:48.000000 bas_geoplot-0.0.20/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-16 08:38:34.623796 bas_geoplot-0.0.20/bas_geoplot/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      194 2023-06-16 08:38:06.000000 bas_geoplot-0.0.20/bas_geoplot/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7280 2023-06-16 08:38:06.000000 bas_geoplot-0.0.20/bas_geoplot/cli.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-16 08:38:34.627796 bas_geoplot-0.0.20/bas_geoplot/config/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     8687 2023-06-16 08:38:06.000000 bas_geoplot-0.0.20/bas_geoplot/config/interactive.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4536 2023-01-24 13:37:08.000000 bas_geoplot-0.0.20/bas_geoplot/config/static.json
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    37081 2023-06-16 08:38:06.000000 bas_geoplot-0.0.20/bas_geoplot/interactive.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9658 2022-10-21 13:21:48.000000 bas_geoplot-0.0.20/bas_geoplot/static.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3435 2023-06-16 08:38:06.000000 bas_geoplot-0.0.20/bas_geoplot/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-06-16 08:38:34.627796 bas_geoplot-0.0.20/bas_geoplot.egg-info/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2905 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      474 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       61 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-10-21 13:36:47.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       71 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-06-16 08:38:34.000000 bas_geoplot-0.0.20/bas_geoplot.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      107 2023-06-16 08:38:34.627796 bas_geoplot-0.0.20/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1540 2022-10-21 13:21:48.000000 bas_geoplot-0.0.20/setup.py
```

### Comparing `bas_geoplot-0.0.19/LICENSE` & `bas_geoplot-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.19/PKG-INFO` & `bas_geoplot-0.0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas_geoplot
-Version: 0.0.19
+Version: 0.0.20
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.19/README.md` & `bas_geoplot-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.19/bas_geoplot/config/interactive.json` & `bas_geoplot-0.0.20/bas_geoplot/config/interactive.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9649621212121212%*

 * *Differences: {"'Maps'": "{'dummy_data': OrderedDict([('data_name', 'dummy_data')]), 'Battery Usage': "*

 * *           "OrderedDict([('line_color', 'gray'), ('line_width', 0.05), ('fill_color', "*

 * *           "OrderedDict([('colormap', 'YlOrRd_04')])), ('fill_opacity', 0.6), ('data_name', "*

 * *           "'battery'), ('units', 'Ah/Day')]), 'Shallows': OrderedDict([('fill_opacity', 0.6), "*

 * *           "('data_name', 'shallow'), ('fill_color', 'blue'), ('line_width', 0.05)])}",*

 * * "'Paths'": "{'Fuel': {'unit': 'Tonnes'}, 'tCO2e': {'un […]*

```diff
@@ -3,14 +3,24 @@
         "offline_coastlines": null,
         "offline_filepath": null,
         "plot_title": true,
         "title": null,
         "zoom_start": 2.6
     },
     "Maps": {
+        "Battery Usage": {
+            "data_name": "battery",
+            "fill_color": {
+                "colormap": "YlOrRd_04"
+            },
+            "fill_opacity": 0.6,
+            "line_color": "gray",
+            "line_width": 0.05,
+            "units": "Ah/Day"
+        },
         "Elev": {
             "data_name": "elevation",
             "fill_color": {
                 "colormap": "BuPu_09"
             },
             "fill_opacity": 0.6,
             "line_color": "gray",
@@ -70,14 +80,20 @@
                 "colormap": "BuPu_09"
             },
             "fill_opacity": 0.6,
             "line_color": "gray",
             "line_width": 0.05,
             "units": "%"
         },
+        "Shallows": {
+            "data_name": "shallow",
+            "fill_color": "blue",
+            "fill_opacity": 0.6,
+            "line_width": 0.05
+        },
         "Total Resistance": {
             "data_name": "resistance",
             "fill_color": {
                 "colormap": "YlOrRd_04"
             },
             "fill_opacity": 0.6,
             "line_color": "gray",
@@ -93,14 +109,17 @@
             "fill_opacity": 0.6,
             "line_color": "gray",
             "line_width": 0.01,
             "scaling_factor": 0.001,
             "units": "kN"
         },
         "data_name": null,
+        "dummy_data": {
+            "data_name": "dummy_data"
+        },
         "fill_color": "black",
         "fill_opacity": 0.0,
         "line_color": "black",
         "line_width": 0.6,
         "tCO2e": {
             "data_name": "fuel",
             "fill_color": {
@@ -190,14 +209,21 @@
                     "Name": "Cell ID",
                     "data": "id"
                 }
             ]
         }
     },
     "Paths": {
+        "Battery": {
+            "data_name": "battery",
+            "line_color": {
+                "color": "Dark2_03"
+            },
+            "unit": "Ah"
+        },
         "Distance (Nautical miles)": {
             "data_name": "distance",
             "line_color": {
                 "color": "viridis"
             },
             "scaling_factor": 0.000539957,
             "unit": "Nautical miles"
@@ -211,15 +237,15 @@
             "unit": "km"
         },
         "Fuel": {
             "data_name": "fuel",
             "line_color": {
                 "color": "Dark2_03"
             },
-            "unit": "Tonnes/Day"
+            "unit": "Tonnes"
         },
         "Max Speed (km/hr)": {
             "data_name": "speed",
             "line_color": {
                 "color": "viridis"
             },
             "unit": "km/hr"
@@ -243,29 +269,57 @@
             "data_name": "traveltime",
             "line_color": {
                 "color": "viridis"
             },
             "scaling_factor": 24.0,
             "unit": "Hrs"
         },
+        "black": {
+            "data_name": "traveltime",
+            "line_color": "black"
+        },
+        "blue": {
+            "data_name": "traveltime",
+            "line_color": "blue"
+        },
         "data_name": null,
+        "green": {
+            "data_name": "traveltime",
+            "line_color": "green"
+        },
         "line_color": "black",
         "line_opacity": 1.0,
         "line_width": 3.0,
+        "orange": {
+            "data_name": "traveltime",
+            "line_color": "orange"
+        },
         "path_points": false,
+        "purple": {
+            "data_name": "traveltime",
+            "line_color": "purple"
+        },
+        "red": {
+            "data_name": "traveltime",
+            "line_color": "red"
+        },
         "scaling_factor": 1.0,
         "tCO2e": {
             "data_name": "fuel",
             "line_color": {
                 "color": "Dark2_03"
             },
             "scaling_factor": 3.25,
-            "unit": "tCO2e/Day"
+            "unit": "tCO2e"
         },
-        "unit": ""
+        "unit": "",
+        "yellow": {
+            "data_name": "traveltime",
+            "line_color": "yellow"
+        }
     },
     "Points": {
         "Waypoints": {
             "icon": "circle",
             "names": {
                 "font_size": 10.0
             }
```

### Comparing `bas_geoplot-0.0.19/bas_geoplot/config/static.json` & `bas_geoplot-0.0.20/bas_geoplot/config/static.json`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.19/bas_geoplot/interactive.py` & `bas_geoplot-0.0.20/bas_geoplot/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import folium
 import os
 import json
 import copy
+import logging
 import pandas as pd
-
 import numpy as np
+import geopandas as gpd
+
 from folium import plugins
 from folium.plugins import TimestampedGeoJson
-
 from branca.colormap import linear
 from branca.element import MacroElement
 from shapely import wkt
 from shapely.geometry import Polygon
-import geopandas as gpd
 from jinja2 import Template
 from pyproj import Geod
-import logging
 
+from bas_geoplot.utils import convert_decimal_days
 
 
-
-def paramsObject(layer,predefined=None,**kwargs):
+def params_object(layer, predefined=None, **kwargs):
     # Loading config of standards
     p_file = os.path.join(os.path.dirname(__file__),'config','interactive.json')
     with open(p_file, 'r') as f:
         p = json.load(f)[layer]
 
     # If a standard type for the specific layer is used replace the global standard values
     if not (predefined is None):
@@ -35,14 +34,17 @@
     for key, value in kwargs.items():
         p[key] = value
 
     return p
 
 
 def build_sectors(cell_poly, dcx, dcy, cx, cy):
+    """
+        Split a rectangular polygon into 8 triangular sectors corresponding to the 8 angular ranges used for array data
+    """
 
     coords = list(cell_poly.exterior.coords)
     x_gap = dcx - (np.sqrt(2) - 1) * dcy
     y_gap = dcy - (np.sqrt(2) - 1) * dcx
     centre = (cx, cy)
 
     # Find coordinates of sector vertices on the cell edge
@@ -69,14 +71,18 @@
     sec_polys[6] = Polygon([centre, edge_coords[1], coords[1], edge_coords[2]])
     sec_polys[7] = Polygon([centre, edge_coords[2], edge_coords[3]])
 
     return sec_polys
 
 
 def sectorise_df(df,dn):
+    """
+        Split all cells in mesh into 8 sectors corresponding to the 8 angular ranges used for array data and assign the
+        correct values to each sector
+    """
 
     sec_df = pd.DataFrame(columns=[dn,'geometry'])
 
     for i, row in df.iterrows():
         sec_polys = build_sectors(row['geometry'], row['dcx'], row['dcy'], row['cx'], row['cy'])
         for j, poly in enumerate(sec_polys):
             idx = i*8 + j
@@ -135,44 +141,39 @@
             ---
 
         """
 
         # === Initialising layer info
         self._layer_info = {}
 
-
         # ==== Loading standard configs
-        p = paramsObject('Basemap',predefined=predefined,**kwargs)
+        p = params_object('Basemap', predefined=predefined, **kwargs)
 
         if p['title']:
             title='{} &ensp;|&ensp;'.format(p['title'])
         else:
             title=''
 
-
         title_html = '''
             <h1 style="color:#003b5c;font-size:16px">
             &ensp;<img src="https://i.ibb.co/XtZdzDt/BAS-colour-eps.png" alt="BAS-colour-eps" border="0" style="width:179px;height:40px;"> 
             &ensp; |&ensp; {}
             </h1>
             </body>
-            '''.format(title)   
-
+            '''.format(title)
 
         if 'map_centre' in p.keys():
             map_centre = p['map_centre']
         else:
             map_centre = None
 
         if 'size' in p.keys():
             self.map = folium.Map(location=map_centre,zoom_start=p['zoom_start'],tiles=None,width=p['size'][0],height=p['size'][1])
         else:
             self.map = folium.Map(location=map_centre,zoom_start=p['zoom_start'],tiles=None)
-        
-        
 
         if p['offline_filepath']:
             self._offline_mode = True
             self._offline_mode_path = p['offline_filepath']
         else:
             self._offline_mode = False
 
@@ -189,15 +190,14 @@
                         'weight': 0.5,
                     }, name="geojson").add_to(bsmap)
             bsmap.add_to(self.map)
 
         if (p['plot_title']) and (p['title'] is not None):
             self.map.get_root().html.add_child(folium.Element(title_html))
 
-
     def _layer(self,name,show=False):
         if name not in self._layer_info:
             lyr = folium.FeatureGroup(name='{}'.format(name),show=show)
             self._layer_info[name] = lyr
         return self._layer_info[name]
 
     def _add_plots_map(self):
@@ -218,15 +218,14 @@
             Saving the interactive plot to file
 
             Attributes:
                 file (str): File path for output
         """
         map = self.show()
 
-
         html = map.get_root().render()
         if self._offline_mode:
             html = html.replace('https://cdn.jsdelivr.net/npm/leaflet@1.6.0/dist/leaflet.js',f'{os.path.join(self._offline_mode_path, "leaflet.js")}')
             html = html.replace('https://code.jquery.com/jquery-1.12.4.min.js',f'{os.path.join(self._offline_mode_path, "jquery-1.12.4.min.js")}')
             html = html.replace('https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/js/bootstrap.min.js',f'{os.path.join(self._offline_mode_path, "bootstrap.min.js")}')
             html = html.replace('https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.js',f'{os.path.join(self._offline_mode_path, "leaflet.awesome-markers.js")}')
 
@@ -240,16 +239,14 @@
             html = html.replace('https://cdnjs.cloudflare.com/ajax/libs/d3/3.5.5/d3.min.js',f'{os.path.join(self._offline_mode_path, "d3.min.js")}')
             html = html.replace('https://cdnjs.cloudflare.com/ajax/libs/leaflet-dvf/0.3.0/leaflet-dvf.markers.min.js',f'{os.path.join(self._offline_mode_path, "leaflet-dvf.markers.min.js")}')
             html = html.replace('https://i.ibb.co/XtZdzDt/BAS-colour-eps.png',f'{os.path.join(self._offline_mode_path, "BAS-colour-eps.png")}')
 
             html = html.replace('https://cdn.jsdelivr.net/gh/marslan390/BeautifyMarker/leaflet-beautify-marker-icon.min.js',f'{os.path.join(self._offline_mode_path, "leaflet-beautify-marker-icon.min.js")}')
             html = html.replace("https://cdn.jsdelivr.net/gh/marslan390/BeautifyMarker/leaflet-beautify-marker-icon.min.css",f'{os.path.join(self._offline_mode_path, "leaflet-beautify-marker-icon.min.css")}')
 
-            
-            
         with open(file,'w') as fp:
             fp.write(html)
             fp.close()
 
     def fit_to_bounds(self, bounds=None):
         """
             Change zoom level to match plotted data
@@ -261,41 +258,40 @@
         else:
             bounds = self.map.get_bounds()
             if bounds == [[None, None], [None, None]]:
                 logging.info("No bounds returned, can't fit to layers")
             else:
                 self.map.fit_bounds(bounds)
 
-    def Paths(self,geojson,name,show=True,predefined=None,**kwargs):
+    def Paths(self,geojson,name,show=True,predefined=None,arrows=False,**kwargs):
         """
             Overlays paths on the interactive plot with layer defined by `name`
 
             Attributes:
                 geojson (dict): A geojson file with several features representing all
                     the separate paths
                 name (string): Layer name to add to the interactive plot
                 show (opt=True, boolean) - Show the layer on loading of plot
                 predefined (opt=None, string) - Predefined plotting formats given in
                     config/interactive.json of the package files
         """
-        p = paramsObject('Paths',predefined=predefined,**kwargs)
+
+        p = params_object('Paths', predefined=predefined, **kwargs)
 
         # Defining the feature groups to add
         pths = self._layer(name,show=show)
         paths = geojson['features']
 
-
         no_path_name = True
         for path in copy.deepcopy(paths):
             if p['data_name'] in path['properties'].keys():
                 no_path_name = False
         if no_path_name:
             return
 
-
         # Determining min-max values of all paths if colormap being used
         if type(p['line_color']) is dict:
             max_val = -np.inf
             min_val = np.inf
             for path in copy.deepcopy(paths):
                     if (np.array(path['properties'][p['data_name']])*p['scaling_factor']).max() > max_val:
                         max_val = (np.array(path['properties'][p['data_name']])*p['scaling_factor']).max()
@@ -326,26 +322,56 @@
             if type(p['line_color']) is dict:
                 if "cmin" in p["line_color"].keys():
                     min_val = p["line_color"]['cmin']
                 if "cmax" in p["line_color"].keys():
                     max_val = p["line_color"]['cmax']
 
                 colormap = linear._colormaps[p["line_color"]['color']].scale(min_val,max_val)
-                colormap.caption = '{} ({},Max Value={:.3f})'.format(name,p['unit'],max_val)
+                if p['unit'] == 'Days':
+                    colormap.caption = '{} ({}, Max Value: {})'.format(name, p['unit'], convert_decimal_days(max_val))
+                else:
+                    colormap.caption = '{} ({}, Max Value: {:.3f})'.format(name,p['unit'],max_val)
                 folium.ColorLine(points,data_val, colormap=colormap,nb_steps=50, weight=p['line_width'],
                                  opacity=p['line_opacity']).add_to(pths)
 
-                folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
-                                popup = "Path - {} to {}\n{} = {:.3f} {}".format(start_wpt,end_wpt,p['data_name'],
-                                                                                 path_max,p['unit'])).add_to(pths)
+                if p['unit'] == 'Days':
+                    folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
+                                    popup = "Path - {} to {}\n{} = {}".format(start_wpt, end_wpt, p['data_name'],
+                                                                              convert_decimal_days(path_max))
+                                    ).add_to(pths)
+                else:
+                    folium.PolyLine(points, color='black', weight=p['line_width'], opacity=0.0,
+                                    popup="Path - {} to {}\n{} = {:.3f} {}".format(start_wpt, end_wpt, p['data_name'],
+                                                                                   path_max, p['unit'])).add_to(pths)
+
+                if arrows:
+                    # Every 10 segments, draw a triangle as an arrow head
+                    for idx in range(1, len(points), 10):
+                        lon_diff = points[idx, 0] - points[idx-1, 0]
+                        lat_diff = points[idx, 1] - points[idx-1, 1]
+                        loc = [points[idx,0],points[idx,1]]
+                        heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
+                        folium.RegularPolygonMarker(location=loc, rotation=heading,
+                                                    color=colormap(data_val[idx]), fill=True,
+                                                    number_of_sides=3, radius=10).add_to(pths)
 
             else:
                 folium.PolyLine(points, color=p['line_color'], weight=p['line_width'], opacity=p['line_opacity'],
                                 popup = "Path - {} to {}".format(start_wpt,end_wpt)).add_to(pths)
 
+                if arrows:
+                    # Every 10 segments, draw a triangle as an arrow head
+                    for idx in range(1, len(points), 10):
+                        lon_diff = points[idx, 0] - points[idx-1, 0]
+                        lat_diff = points[idx, 1] - points[idx-1, 1]
+                        loc = [points[idx,0],points[idx,1]]
+                        heading = -np.degrees(np.arctan2(lon_diff, lat_diff))
+                        folium.RegularPolygonMarker(location=loc, rotation=heading,
+                                                    color=p['line_color'], fill=True,
+                                                    number_of_sides=3, radius=10).add_to(pths)
 
             if p['path_points']:
                 for idx in range(len(points)):
                     loc = [points[idx,0],points[idx,1]]
                     folium.Marker(
                         location=loc,
                         icon=folium.plugins.BeautifyIcon(icon='circle',
@@ -356,28 +382,27 @@
                                                     inner_icon_style='margin:0px;font-size:0.8em')
                     ).add_to(pths)
         
         if type(p['line_color']) is dict:
             self.map.add_child(colormap)
             self.map.add_child(BindColormap(pths,colormap))
 
-
     def Points(self,dataframe_points,name,show=True,predefined=None,**kwargs):
         """
             Overlays small collection of Points, such as waypoints and sites of interest.
 
             Attributes:
                 dataframe_points (Pandas DataFrame): A Dataframe requiring at least columns of Latitude ('Lat') Longitude ('Long'), Name ('Name').
                 name (string): Layer name to add to the interactive plot
                 show (opt=True, boolean) - Show the layer on loading of plot
                 predefined (opt=None, string) - Predefined plotting formats given in
                     config/interactive.json of the package files
         """
 
-        p = paramsObject('Points',predefined=predefined,**kwargs)
+        p = params_object('Points', predefined=predefined, **kwargs)
 
         wpts      = self._layer(name,show=show)
  
         for id,wpt in dataframe_points.iterrows():
             loc = [wpt['Lat'], wpt['Long']]
             folium.Marker(
                 location=loc,
@@ -396,32 +421,30 @@
                                 icon=folium.features.DivIcon(
                                     icon_size=(250,36),
                                     icon_anchor=(0,0),
                                     html='<div style="font-size: {}pt">{}</div>'.format(p['names']['font_size'],wpt['Name']),
                                     ),
                 ).add_to(wpts)
 
-
         wpts.add_to(self.map)
 
-
     def Maps(self,dataframe_pandas,name,show=True,predefined=None,plot_sectors=False,**kwargs):
         """
             Overlays a layer of scalars or booleans such as sea ice concentration or land.
 
             Attributes:
                 dataframe_pandas (GeoPandas DataFrame): A Dataframe in Geopandas format. This requires at least a column
                     with 'geometry'. Additional plotting of specific columns is done in the configuration files.
                 name (string): Layer name to add to the interactive plot
                 show (opt=True, boolean): Show the layer on loading of plot
                 predefined (opt=None, string): Predefined plotting formats given in config/interactive.json of the
                     package files
                 plot_sectors (boolean): Display sectorised list values as eight individual polygons
         """
-        p = paramsObject('Maps',predefined=predefined,**kwargs)
+        p = params_object('Maps', predefined=predefined, **kwargs)
 
         dataframe_pandas = copy.copy(dataframe_pandas)
         dataframe_pandas['geometry'] = dataframe_pandas['geometry'].apply(wkt.loads)
 
         # Don't plot anything in the land cells unless, of course, we are plotting the land mask
         if 'land' in dataframe_pandas.keys() and p['data_name'] != 'land':
             dataframe_pandas = dataframe_pandas[dataframe_pandas['land']==False].reset_index(drop=True)
@@ -432,32 +455,27 @@
                 dataframe_pandas = sectorise_df(dataframe_pandas, p['data_name'])
             else:
                 dataframe_pandas[p['data_name']] = [np.mean(dn) for dn in dataframe_pandas[p['data_name']]]
         dataframe_geo = gpd.GeoDataFrame(dataframe_pandas,crs='EPSG:4326', geometry='geometry')
 
         feature_info = self._layer(name,show=show)
 
-
         if p['data_name']:
             try:
                 if 'scaling_factor' in p.keys():
                     dataframe_geo[p['data_name']] = dataframe_geo[p['data_name']]*p['scaling_factor']
                 else:
                     dataframe_geo[p['data_name']] = dataframe_geo[p['data_name']]
             except:
                 raise print('Data name not in variables')
 
-
-
         if p['data_name'] and p['trim_min']:
             dataframe_geo = dataframe_geo[dataframe_geo[p['data_name']] > p['trim_min']]
         if p['data_name'] and p['trim_max']:
             dataframe_geo = dataframe_geo[dataframe_geo[p['data_name']] < p['trim_max']]
-            
-
 
         if (type(p['fill_color']) is dict) and (p['data_name']):
             dataframe_geo = dataframe_geo[dataframe_geo[p['data_name']].notna() & ~np.isinf(abs(dataframe_geo[p['data_name']]))]
             if 'cmin' in p['fill_color'].keys():
                 cmin = p['fill_color']['cmin']
             else:
                 cmin = dataframe_geo[p['data_name']].min()
@@ -493,38 +511,35 @@
                         'fillColor': p['fill_color'],
                         'color': p['line_color'],
                         'weight': p['line_width'],
                         'fillOpacity': p['fill_opacity']
                         }
                 ).add_to(feature_info)
 
-
-
     def Vectors(self,mesh,name,show=True,predefined=None,**kwargs):
         """
             Overlays a layer of vectors such as currents.
 
             Attributes:
                 dataframe_points (Pandas DataFrame): A Dataframe requiring at least columns of Longitude ('cx') Latitude ('cy'), Displacement in X ('uC') and Displacement in Y ('vC').
                 name (string): Layer name to add to the interactive plot
                 show (opt=True, boolean) - Show the layer on loading of plot
                 predefined (opt=None, string) - Predefined plotting formats given in
                     config/interactive.json of the package files
         """
 
-
-        p = paramsObject('Vectors',predefined=predefined,**kwargs)
+        p = params_object('Vectors', predefined=predefined, **kwargs)
 
         Vectors = mesh
         # Filter out empty vectors but allow single component vectors
         Vectors = Vectors[(Vectors[p['V']]!=0.0)|(Vectors[p['U']]!=0.0)].reset_index(drop=True)
         Vectors = Vectors.dropna(subset=[p['U'], p['V']]).reset_index(drop=True)
 
-        if 'land' in Vectors.keys():
-            Vectors = Vectors[Vectors['land']==False].reset_index(drop=True)
+        if 'inaccessible' in Vectors.keys():
+            Vectors = Vectors[Vectors['inaccessible']==False].reset_index(drop=True)
 
         vcts = self._layer(name,show=show)
         for idx,vec in Vectors.iterrows():
             loc =[[vec[p['Lat']],vec[p['Long']]],[vec[p['Lat']]+vec[p['V']]*p['scale'],vec[p['Long']]+vec[p['U']]*p['scale']]]
             mag = np.sqrt(vec[p['V']]**2 + vec[p['U']]**2)
             folium.PolyLine(loc, color=p['color'],weight=1.4, popup='{} (m/s)'.format(mag)).add_to(vcts)
             # get pieces of the line
@@ -533,40 +548,35 @@
             geodesic = Geod(ellps='WGS84')
             rotations = [geodesic.inv(pair[0][1], pair[0][0], pair[1][1], pair[1][0])[0]+90 for pair in pairs]
             # create your arrow
             for pair, rot in zip(pairs, rotations):
                 folium.RegularPolygonMarker(location=pair[0], color=p['color'], fill=True, fill_color=p['color'], fill_opacity=1,
                                             number_of_sides=3, rotation=rot,radius=4,weight=p['line_width']).add_to(vcts)
 
-
-
     def MeshInfo(self,mesh,name,predefined='PolarRoute',show=True,**kwargs):
         """
             Overlays a layer that gives information on all polygon boxes.
 
             Attributes:
                 cellboxes (GeodataFrame): A Dataframe in Geopandas format. This requires at least a column with 'geometry'.
                 name (string): Layer name to add to the interactive plot
                 show (opt=True, boolean) - Show the layer on loading of plot
                 predefined (opt=None, string) - Predefined plotting formats given in
                     config/interactive.json of the package files
         """
 
-        p = paramsObject('MeshInfo',predefined=predefined,**kwargs)
-
-
+        p = params_object('MeshInfo', predefined=predefined, **kwargs)
 
         dataframe_pandas = copy.copy(pd.DataFrame(mesh))
         dataframe_pandas['geometry'] = dataframe_pandas['geometry'].apply(wkt.loads)
         dataframe_geo = gpd.GeoDataFrame(dataframe_pandas,crs='EPSG:4326', geometry='geometry')
 
         p = p['fields']
 
-        column_names = []
-        column_names.append('geometry')
+        column_names = ['geometry']
         for col_info in p:
             try:
                 column_name = col_info['Name']
                 data = col_info['data']
                 dataframe_geo[column_name] = dataframe_geo[data]
                 if 'scaling_factor' in col_info.keys():
                     dataframe_geo[column_name] = dataframe_geo[column_name]*col_info['scaling_factor']
@@ -609,17 +619,14 @@
             bounds=bounds,
             mercator_project=True,
             opacity=0.6
         ).add_to(feature_info)
         self.map.add_child(colormap)
         self.map.add_child(BindColormap(feature_info,colormap))
 
-
-
-
     def _Geotiff(self,path,name,show=True):
         import rasterio
         src = rasterio.open(path)
         indx=1
         trying=True
         while trying:
             try:
@@ -651,19 +658,16 @@
                 
                 self.map.add_child(colormap)
                 self.map.add_child(BindColormap(feature_info,colormap))
             except:
                 trying=False
             indx+=1
 
-
-
-
     def _TimeData(self,geojson,predefined=None,**kwargs):
-        p = paramsObject('TimeData',predefined=predefined,**kwargs)
+        p = params_object('TimeData', predefined=predefined, **kwargs)
 
         for ii in range(len(geojson['features'])):
             geojson['features'][ii]['properties']['style'] = {}
             geojson['features'][ii]['properties']['style']["weight"]  = p['weight']
             geojson['features'][ii]['properties']['style']["color"]   = p['color']
             geojson['features'][ii]['properties']['style']["opacity"] = p['opacity']
 
@@ -678,18 +682,14 @@
             loop=False,
             loop_button=True,
             date_options='DD/MM/YYYY HH:mm:ss',
             add_last_point=p['point']
         ).add_to(self.map)
     
 
-
-
-
-
 # def TimeMapSDA(PATH,map):
 #     #'/Users/jsmith/Documents/Research/Researcher_BAS/RoutePlanning/SDADT-Positions'
 #     Info = SDAPosition(PATH)
 #     lines=[]
 #     Points = Info[['Long','Lat']].to_numpy()
 #     Points[:,0] = Points[:,0]-360
 #     entry = {}
@@ -829,8 +829,8 @@
 #             fields=['Ice Area', 'Land','Cx','Cy','Depth','Vector','Index'],
 #             aliases=['Ice Area (%)', 'Land','Centroid Cx [Long]','Centroid Cy [Lat]','Depth(m)','Vector (m/s)','Cell Index'],
 #             localize=True
 #         ),
 #         name='Land Grid'
 #     ).add_to(meshInfo)
 #     meshInfo.add_to(map)
-#     return map
+#     return map
```

### Comparing `bas_geoplot-0.0.19/bas_geoplot/static.py` & `bas_geoplot-0.0.20/bas_geoplot/static.py`

 * *Files identical despite different names*

### Comparing `bas_geoplot-0.0.19/bas_geoplot.egg-info/PKG-INFO` & `bas_geoplot-0.0.20/bas_geoplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bas-geoplot
-Version: 0.0.19
+Version: 0.0.20
 Summary: GeoPlot: BAS AI Lab plotting scripts built on Folium
 Home-page: https://github.com/antarctica/GeoPlot
 Author: BAS AI Lab
 Author-email: jonsmi@bas.ac.uk
 Maintainer: BAS AI Lab
 Maintainer-email: jonsmi@bas.ac.uk
 License: UNKNOWN
```

### Comparing `bas_geoplot-0.0.19/setup.py` & `bas_geoplot-0.0.20/setup.py`

 * *Files identical despite different names*

