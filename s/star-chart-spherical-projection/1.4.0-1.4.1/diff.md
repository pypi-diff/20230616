# Comparing `tmp/star-chart-spherical-projection-1.4.0.tar.gz` & `tmp/star-chart-spherical-projection-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/star-chart-spherical-projection-1.4.0.tar", last modified: Fri Jan 20 01:56:32 2023, max compression
+gzip compressed data, was "dist/star-chart-spherical-projection-1.4.1.tar", last modified: Fri Jun 16 21:46:45 2023, max compression
```

## Comparing `star-chart-spherical-projection-1.4.0.tar` & `star-chart-spherical-projection-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:56:32.143294 star-chart-spherical-projection-1.4.0/
--rw-rw-r--   0 user      (1000) user      (1000)      102 2022-11-20 23:38:29.000000 star-chart-spherical-projection-1.4.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    13829 2023-01-20 01:56:32.143294 star-chart-spherical-projection-1.4.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    11145 2023-01-20 01:54:10.000000 star-chart-spherical-projection-1.4.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-01-20 01:56:32.143294 star-chart-spherical-projection-1.4.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1812 2023-01-20 01:54:52.000000 star-chart-spherical-projection-1.4.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:56:32.139294 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/
--rw-rw-r--   0 user      (1000) user      (1000)      494 2022-12-19 08:17:40.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-20 04:40:07.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/config.ini
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:56:32.143294 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/data/
--rw-rw-r--   0 user      (1000) user      (1000)    10908 2023-01-20 01:44:10.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
--rw-rw-r--   0 user      (1000) user      (1000)     4317 2023-01-20 01:44:28.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/data/star_data.csv
--rw-rw-r--   0 user      (1000) user      (1000)     2513 2022-11-20 22:32:39.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/declination_r_axis.py
--rw-rw-r--   0 user      (1000) user      (1000)     7200 2023-01-04 00:36:28.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    21909 2023-01-03 21:47:41.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/generate_star_chart.py
--rw-rw-r--   0 user      (1000) user      (1000)     9126 2022-11-27 07:09:03.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:56:32.143294 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    13829 2023-01-20 01:56:32.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-01-20 01:56:32.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-20 01:56:32.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-01-20 01:56:32.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       32 2023-01-20 01:56:32.000000 star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2022-11-20 23:38:29.000000 star-chart-spherical-projection-1.4.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    15187 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    12407 2023-06-15 20:36:51.000000 star-chart-spherical-projection-1.4.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1831 2023-06-16 21:45:35.000000 star-chart-spherical-projection-1.4.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.402627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/
+-rw-rw-r--   0 user      (1000) user      (1000)      494 2022-12-19 08:17:40.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-20 04:40:07.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/config.ini
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/
+-rw-rw-r--   0 user      (1000) user      (1000)    10908 2023-01-20 01:44:10.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4317 2023-01-20 01:44:28.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/star_data.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     2513 2022-11-20 22:32:39.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/declination_r_axis.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8082 2023-06-15 20:36:08.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21909 2023-06-15 20:26:39.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/generate_star_chart.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.406627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6842 2023-06-15 20:34:14.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12221 2023-06-15 20:13:50.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9126 2022-11-27 07:09:03.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/ra_dec_precession_vondrak.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 21:46:45.402627 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    15187 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-16 21:46:45.000000 star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/top_level.txt
```

### Comparing `star-chart-spherical-projection-1.4.0/PKG-INFO` & `star-chart-spherical-projection-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: star-chart-spherical-projection
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package to generate an astronomy star chart based on spherical projection that corrects for distortions with stereographic projection
 Home-page: https://github.com/cyschneck/Star-Chart-Spherical-Projection
 Author: cyschneck (C. Y. Schneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v1.4.1.tar.gz
 Description: # Star-Chart-Spherical-Projection
         
         ![PyPi](https://img.shields.io/pypi/v/star-chart-spherical-projection)
         ![license](https://img.shields.io/github/license/cyschneck/Star-Chart-Spherical-Projection)
+        [![pytests](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml/badge.svg?branch=main)](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml)
         
         A Python package to generate an astronomy star chart based on spherical projection with +90/-90° in the center based on a star's position (declination and right ascension): past, present, and future (proper motion and precession)
         
         The first step to plot the celestial sphere onto a 2D plot is to map the star's right ascension as hours along the plot (matplotlib polar plot's theta value) and declination as the distance from the center of the circle (matplotlib polar plot's radius value). However, attempting to map the right ascension and declination directly will cause distortion since the angles between the stars along the declination are no longer conserved. On the left, the constellation of the Big Dipper is stretched into an unfamiliar shape due to this distortion. By accounting for the spherical transformation, the star chart can be corrected as seen on the right.
         
         | Without Correction | With Correction |
         | ------------- | ------------- |
@@ -59,34 +60,49 @@
         
         ## Documentation
         
         **finalPositionOfStars()**
         
         Returns a dictionary for the final positions of the stars in the format: {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
         ```
-        finalPositionOfStars(userListOfStars=[], 
-        			northOrSouth=None, 
-        			yearSince2000=0,
+        finalPositionOfStars(yearSince2000=0, 
+        			userListOfStars=[],
         			isPrecessionIncluded=True,
         			declination_min=None,
         			declination_max=None)
         ```
-        - **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
         - *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-        - *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+        - *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
         - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-        - *[OPTIONAL]* declination_min: (int) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-        - *[OPTIONAL]* declination_max: (int) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+        - *[OPTIONAL]* declination_min: (int/float) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+        - *[OPTIONAL]* declination_max: (int/float) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+        
+        <details closed>
+        <summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+        <br>
+         ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+        'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
+        'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
+        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
+        'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
+        'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
+        'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
+        'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
+        'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
+        'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
+        'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
+        'Zubeneschamali']
+        </details>
         
         **plotStereographicProjection()**
         
         Plot stars on a Stereographic Polar Plot
         ```
-        plotStereographicProjection(userListOfStars=[], 
-        				northOrSouth=None, 
+        plotStereographicProjection(northOrSouth=None, 
+        				userListOfStars=[], 
         				declination_min=None,
         				yearSince2000=0,
         				displayStarNamesLabels=True,
         				displayDeclinationNumbers=True,
         				incrementBy=10,
         				isPrecessionIncluded=True,
         				maxMagnitudeFilter=None,
@@ -94,42 +110,45 @@
         				fig_plot_title=None,
         				fig_plot_color="C0",
         				figsize_n=12,
         				figsize_dpi=100,
         				save_plot_name=None)
         ```
         - **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
-        - *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-        - *[OPTIONAL]* declination_min: (int) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-        - *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+        - *[OPTIONAL]* userListOfStars: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
+        - *[OPTIONAL]* declination_min: (int/float) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+        - *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
         - *[OPTIONAL]* displayStarNamesLabels: (boolean) display the star name labels, defaults to True
         - *[OPTIONAL]* displayDeclinationNumbers: (boolean) display declination values, defaults to True
         - *[OPTIONAL]* incrementBy: (int) increment values for declination (either 1, 5, 10), defaults to 10
         - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-        - *[OPTIONAL]* maxMagnitudeFilter: (float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
-        - *[OPTIONAL]* returnData: (boolean) return a dictionary of stars with their final right ascension and declination ({"Vega" : [Declination (float) degrees, RA (str)]}, defaults to False
+        - *[OPTIONAL]* maxMagnitudeFilter: (int/float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
         - *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()) when finished running, defaults to True
         - *[OPTIONAL]* fig_plot_title: (string) figure title, defaults to "<North/South>ern Hemisphere [<YEAR NUMBERS> Years Since 2000 (YYYY)]: +/-90° to <DECLINATION MIN>°"
         - *[OPTIONAL]* fig_plot_color: (string) scatter plot star color, defaults to C0
-        - *[OPTIONAL]* figsize_n: (int) figure size, default to 12
-        - *[OPTIONAL]* figsize_dpi: (int) figure DPI, default to 100
+        - *[OPTIONAL]* figsize_n: (int/float) figure size, default to 12
+        - *[OPTIONAL]* figsize_dpi: (int/float) figure DPI, default to 100
         - *[OPTIONAL]* save_plot_name: (string) save plot with a string name, defaults to not saving
         
-        Current list of stars (to access via userListOfStar): ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+        <details closed>
+        <summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+        <br>
+         ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
         'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
         'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
-        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta cdPhoenicis', 'Betelgeuse', 'Canopus', 
+        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
         'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
         'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
         'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
         'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
         'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
         'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
         'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
         'Zubeneschamali']
+        </details>
         
         ## Dependencies
         
         Python 3.7+
         ```
         pip3 install -r requirements.txt
         ```
@@ -151,32 +170,25 @@
         Returns a dictionary: `{'Betelgeuse': {'Declination': -36.342836095268325, 'RA': '16.34.28'}, 'Polaris': {'Declination': 45.08038305067079, 'RA': '17.25.11'}, 'Vega': {'Declination': 83.6899118156341, 'RA': '05.38.21'}}`
         
         ```python
         import star_chart_spherical_projection as scsp
         
         scsp.plotStereographicProjection(northOrSouth="North")
         ```
-        ## Tests
-        
         ## Bibliography
         
         Star position (right ascension and declination) as well as the angle and speed of proper motion taken from [in-the-sky.org](in-the-sky.org)
         
         Precession model: [Vondrák, J., et al. “New Precession Expressions, Valid for Long Time Intervals.” Astronomy &amp; Astrophysics, vol. 534, 2011, https://doi.org/10.1051/0004-6361/201117274.](https://www.aanda.org/articles/aa/pdf/2011/10/aa17274-11.pdf)
         
         Precession code adapted to Python3 from [github.com/dreamalligator/vondrak](github.com/dreamalligator/vondrak)
         
-        
         ## TODO:
         
-        Add README badges: tests
-        
-        Pypi tests
-        
-         Testing for new function finalPositionOfStars(), still needs testing
+        Add README badges: pypi tests
         
 Keywords: astronomy,python,star charts,precession,proper motion,spherical projection,stereographic projection
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `star-chart-spherical-projection-1.4.0/README.md` & `star-chart-spherical-projection-1.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Star-Chart-Spherical-Projection
 
 ![PyPi](https://img.shields.io/pypi/v/star-chart-spherical-projection)
 ![license](https://img.shields.io/github/license/cyschneck/Star-Chart-Spherical-Projection)
+[![pytests](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml/badge.svg?branch=main)](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml)
 
 A Python package to generate an astronomy star chart based on spherical projection with +90/-90° in the center based on a star's position (declination and right ascension): past, present, and future (proper motion and precession)
 
 The first step to plot the celestial sphere onto a 2D plot is to map the star's right ascension as hours along the plot (matplotlib polar plot's theta value) and declination as the distance from the center of the circle (matplotlib polar plot's radius value). However, attempting to map the right ascension and declination directly will cause distortion since the angles between the stars along the declination are no longer conserved. On the left, the constellation of the Big Dipper is stretched into an unfamiliar shape due to this distortion. By accounting for the spherical transformation, the star chart can be corrected as seen on the right.
 
 | Without Correction | With Correction |
 | ------------- | ------------- |
@@ -51,34 +52,49 @@
 
 ## Documentation
 
 **finalPositionOfStars()**
 
 Returns a dictionary for the final positions of the stars in the format: {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
 ```
-finalPositionOfStars(userListOfStars=[], 
-			northOrSouth=None, 
-			yearSince2000=0,
+finalPositionOfStars(yearSince2000=0, 
+			userListOfStars=[],
 			isPrecessionIncluded=True,
 			declination_min=None,
 			declination_max=None)
 ```
-- **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
 - *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-- *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
 - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-- *[OPTIONAL]* declination_min: (int) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-- *[OPTIONAL]* declination_max: (int) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+- *[OPTIONAL]* declination_min: (int/float) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+- *[OPTIONAL]* declination_max: (int/float) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+
+<details closed>
+<summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+<br>
+ ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
+'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
+'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
+'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
+'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
+'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
+'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
+'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
+'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
+'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
+'Zubeneschamali']
+</details>
 
 **plotStereographicProjection()**
 
 Plot stars on a Stereographic Polar Plot
 ```
-plotStereographicProjection(userListOfStars=[], 
-				northOrSouth=None, 
+plotStereographicProjection(northOrSouth=None, 
+				userListOfStars=[], 
 				declination_min=None,
 				yearSince2000=0,
 				displayStarNamesLabels=True,
 				displayDeclinationNumbers=True,
 				incrementBy=10,
 				isPrecessionIncluded=True,
 				maxMagnitudeFilter=None,
@@ -86,42 +102,45 @@
 				fig_plot_title=None,
 				fig_plot_color="C0",
 				figsize_n=12,
 				figsize_dpi=100,
 				save_plot_name=None)
 ```
 - **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
-- *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-- *[OPTIONAL]* declination_min: (int) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-- *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- *[OPTIONAL]* userListOfStars: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
+- *[OPTIONAL]* declination_min: (int/float) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+- *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
 - *[OPTIONAL]* displayStarNamesLabels: (boolean) display the star name labels, defaults to True
 - *[OPTIONAL]* displayDeclinationNumbers: (boolean) display declination values, defaults to True
 - *[OPTIONAL]* incrementBy: (int) increment values for declination (either 1, 5, 10), defaults to 10
 - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-- *[OPTIONAL]* maxMagnitudeFilter: (float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
-- *[OPTIONAL]* returnData: (boolean) return a dictionary of stars with their final right ascension and declination ({"Vega" : [Declination (float) degrees, RA (str)]}, defaults to False
+- *[OPTIONAL]* maxMagnitudeFilter: (int/float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
 - *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()) when finished running, defaults to True
 - *[OPTIONAL]* fig_plot_title: (string) figure title, defaults to "<North/South>ern Hemisphere [<YEAR NUMBERS> Years Since 2000 (YYYY)]: +/-90° to <DECLINATION MIN>°"
 - *[OPTIONAL]* fig_plot_color: (string) scatter plot star color, defaults to C0
-- *[OPTIONAL]* figsize_n: (int) figure size, default to 12
-- *[OPTIONAL]* figsize_dpi: (int) figure DPI, default to 100
+- *[OPTIONAL]* figsize_n: (int/float) figure size, default to 12
+- *[OPTIONAL]* figsize_dpi: (int/float) figure DPI, default to 100
 - *[OPTIONAL]* save_plot_name: (string) save plot with a string name, defaults to not saving
 
-Current list of stars (to access via userListOfStar): ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+<details closed>
+<summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+<br>
+ ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
-'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta cdPhoenicis', 'Betelgeuse', 'Canopus', 
+'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
 'Zubeneschamali']
+</details>
 
 ## Dependencies
 
 Python 3.7+
 ```
 pip3 install -r requirements.txt
 ```
@@ -143,25 +162,18 @@
 Returns a dictionary: `{'Betelgeuse': {'Declination': -36.342836095268325, 'RA': '16.34.28'}, 'Polaris': {'Declination': 45.08038305067079, 'RA': '17.25.11'}, 'Vega': {'Declination': 83.6899118156341, 'RA': '05.38.21'}}`
 
 ```python
 import star_chart_spherical_projection as scsp
 
 scsp.plotStereographicProjection(northOrSouth="North")
 ```
-## Tests
-
 ## Bibliography
 
 Star position (right ascension and declination) as well as the angle and speed of proper motion taken from [in-the-sky.org](in-the-sky.org)
 
 Precession model: [Vondrák, J., et al. “New Precession Expressions, Valid for Long Time Intervals.” Astronomy &amp; Astrophysics, vol. 534, 2011, https://doi.org/10.1051/0004-6361/201117274.](https://www.aanda.org/articles/aa/pdf/2011/10/aa17274-11.pdf)
 
 Precession code adapted to Python3 from [github.com/dreamalligator/vondrak](github.com/dreamalligator/vondrak)
 
-
 ## TODO:
 
-Add README badges: tests
-
-Pypi tests
-
- Testing for new function finalPositionOfStars(), still needs testing
+Add README badges: pypi tests
```

### Comparing `star-chart-spherical-projection-1.4.0/setup.py` & `star-chart-spherical-projection-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.4.0"
+VERSION="1.4.1"
 DESCRIPTION="A Python package to generate an astronomy star chart based on spherical projection that corrects for distortions with stereographic projection"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="star-chart-spherical-projection",
@@ -38,12 +38,13 @@
 	],
 	packages=find_namespace_packages(include=['star_chart_spherical_projection',
 											'star_chart_spherical_projection.*']),
 	include_package_data=True,
 	install_requires=[
 		"configparser>=5.3.0",
 		"matplotlib>=3.1.0",
-		"numpy>=1.21.6",
-		"pandas>=1.3.5"
+		"numpy>=1.24.3",
+		"pandas>=1.3.5",
+		"pytest>=7.2.2"
 	],
 	python_requires='>=3.7'
 )
```

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/convert_lst_to_csv_data.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/data/star_data.csv` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/data/star_data.csv`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/declination_r_axis.py` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/declination_r_axis.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/error_handling.py` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/error_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,75 +35,92 @@
 
 	# Ensure that star list is a list
 	if type(userListOfStars) != list:
 		logger.critical("\nCRITICAL ERROR, [userListOfStars]: Must be a list, current type = '{0}'".format(type(userListOfStars)))
 		exit()
 	## Check that user list has stars that are found in current list
 	if len(userListOfStars) != 0:
+		userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
 		star_csv_file = os.path.join(os.path.dirname(__file__), 'data', 'star_data.csv')  # get file's directory, up one level, /data/star_data.csv
 		star_dataframe = pd.read_csv(star_csv_file)
 		all_star_names_in_csv = list(star_dataframe['Star Name'])
 		for star_given in userListOfStars:
 			if star_given not in all_star_names_in_csv:
 				logger.critical("\nCRITICAL ERROR, [userListOfStars]: '{0}' not a star in current list of stars, please select one of the following: {1}".format(star_given, all_star_names_in_csv))
 				exit()
 	logger.debug("userListOfStars = '{0}'".format(userListOfStars))
 
+	# Ensure that declination ranges are set and within within ranges
+	if declination_min is not None:
+		if type(declination_min) != int and type(declination_min) != float:
+			logger.critical("\nCRITICAL ERROR, [declination_min]: Must be a int or float, current type = '{0}'".format(type(declination_min)))
+			exit()
+		if declination_min not in np.arange(-89, 90): # if defined, but not in range
+			logger.critical("\nCRITICAL ERROR, [declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '{0}'".format(declination_min))
+			exit()
+	logger.debug("declination_min = '{0}'".format(declination_min))
+
 	# Ensure if a year is selected it is a float or int, set by default to 0 (the year = 2000)
 	if type(yearSince2000) != int and type(yearSince2000) != float:
 		logger.critical("\nCRITICAL ERROR, [yearSince2000]: Must be a int or float, current type = '{0}'".format(type(yearSince2000)))
 		exit()
 	logger.debug("yearSince2000 = '{0}'".format(yearSince2000))
 
 	# Ensure that precession options are booleans ["True", "False"]
 	if type(isPrecessionIncluded) != bool:
 		logger.critical("\nCRITICAL ERROR, [isPrecessionIncluded]: Must be a bool, current type = '{0}'".format(type(isPrecessionIncluded)))
 		exit()
 	logger.debug("isPrecessionIncluded = '{0}'".format(isPrecessionIncluded))
 
-	# Ensure that declination ranges are set and within within ranges
-	if declination_min is not None and declination_min not in np.arange(-89, 90): # if defined, but not in range
-		logger.critical("\nCRITICAL ERROR, [declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '{0}'".format(declination_min))
-		exit()
-	logger.debug("declination_min = '{0}'".format(declination_min))
-
 	# Error Handling for finalPositionOfStars() function
 	if not isPlotFunction:
 		# Ensure that declination ranges are set and within within ranges
-		if declination_max is not None and declination_max not in np.arange(-89, 90): # if defined, but not in range
-			logger.critical("\nCRITICAL ERROR, [declination_max]: Maximum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '{0}'".format(declination_max))
-			exit()
+		if declination_max is not None:
+			if type(declination_max) != int and type(declination_max) != float:
+				logger.critical("\nCRITICAL ERROR, [declination_max]: Must be a int or float, current type = '{0}'".format(type(declination_max)))
+				exit()
+			if declination_max not in np.arange(-89, 90): # if defined, but not in range
+				logger.critical("\nCRITICAL ERROR, [declination_max]: Maximum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '{0}'".format(declination_max))
+				exit()
 		logger.debug("declination_max = '{0}'".format(declination_max))
 
 	# Error Handling for plotStereographicProjection() function
 	if isPlotFunction:
 		# Ensure that Hemisphere selected are within options
-		if northOrSouth not in ["North", "South"]:
-			logger.critical("\nCRITICAL ERROR, [northOrSouth]: Hemisphere options are ['North', 'South'], current option = '{0}'".format(northOrSouth))
-			exit()
 		logger.debug("northOrSouth = '{0}'".format(northOrSouth))
+		if type(northOrSouth) != str:
+			logger.critical("\nCRITICAL ERROR, [northOrSouth]: Must be a str, current type = '{0}'".format(type(northOrSouth)))
+			exit()
+		else:
+			if northOrSouth not in ["North", "South"]:
+				logger.critical("\nCRITICAL ERROR, [northOrSouth]: Hemisphere options are ['North', 'South'], current option = '{0}'".format(northOrSouth))
+				exit()
 
 		# Ensure that maxMagnitudeFilter options is a float, set by default to None
-		if maxMagnitudeFilter is not None and type(maxMagnitudeFilter) != float:
-			logger.critical("\nCRITICAL ERROR, [maxMagnitudeFilter]: Must be a float, current type = '{0}'".format(type(maxMagnitudeFilter)))
-			exit()
+		if maxMagnitudeFilter is not None:
+			if type(maxMagnitudeFilter) != int and type(maxMagnitudeFilter) != float:
+				logger.critical("\nCRITICAL ERROR, [maxMagnitudeFilter]: Must be a int or float, current type = '{0}'".format(type(maxMagnitudeFilter)))
+				exit()
 		logger.debug("maxMagnitudeFilter = '{0}'".format(maxMagnitudeFilter))
 
 		# Ensure that the display options for star names and declination numbers are booleans ["True", "False"]
 		if type(displayStarNamesLabels) != bool:
 			logger.critical("\nCRITICAL ERROR, [displayStarNamesLabels]: Must be a bool, current type = '{0}'".format(type(displayStarNamesLabels)))
 			exit()
 		logger.debug("displayStarNamesLabels = '{0}'".format(displayStarNamesLabels))
 		if type(displayDeclinationNumbers) != bool:
 			logger.critical("\nCRITICAL ERROR, [displayDeclinationNumbers]: Must be a bool, current type = '{0}'".format(type(displayDeclinationNumbers)))
 			exit()
 		logger.debug("displayDeclinationNumbers = '{0}'".format(displayDeclinationNumbers))
 
 		# Ensure that increment options are 1, 5, 10
-		if type(incrementBy) != int or incrementBy not in [1, 5, 10]:
+		if type(incrementBy) != int:
+			logger.critical("\nCRITICAL ERROR, [incrementBy]: Must be a int, current type = '{0}'".format(type(incrementBy)))
+			exit()
+		if incrementBy not in [1, 5, 10]:
 			logger.critical("\nCRITICAL ERROR, [incrementBy]: Must be one of the options [1, 5, 10], current value = '{0}'".format(incrementBy))
 			exit()
 		logger.debug("incrementBy = '{0}'".format(incrementBy))
 
 		# Ensure that the only options for showPlot are booleans ["True", "False"]
 		if type(showPlot) != bool:
 			logger.critical("\nCRITICAL ERROR, [showPlot]: Must be a bool, current type = '{0}'".format(type(showPlot)))
```

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/generate_star_chart.py` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/generate_star_chart.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -191,22 +191,22 @@
 
 def finalPositionOfStars(userListOfStars=[], 
 						yearSince2000=0,
 						isPrecessionIncluded=True,
 						declination_min=None,
 						declination_max=None):
 	# return the final position of the stars as a dictionary
-	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
 
 	star_chart_spherical_projection.errorHandling(isPlotFunction=False,
 												userListOfStars=userListOfStars,
 												yearSince2000=yearSince2000,
 												isPrecessionIncluded=isPrecessionIncluded,
 												declination_min=declination_min,
 												declination_max=declination_max)
+	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
 
 	# Set declination min values when using the generateStereographicProjection() to capture all stars if not set
 	declination_min = -90
 	declination_max = 90
 
 	x_star_labels, x_ra_values, y_dec_values, finalPositionOfStarsDict = generateStereographicProjection(starList=userListOfStars, 
 																										northOrSouth="North", 
@@ -305,16 +305,14 @@
 								fig_plot_title=None,
 								fig_plot_color="C0",
 								figsize_n=12,
 								figsize_dpi=100,
 								save_plot_name=None):
 
 	# Catch errors in given arguments before plotting and set default constants
-	northOrSouth = northOrSouth.capitalize()
-	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
 	star_chart_spherical_projection.errorHandling(isPlotFunction=True,
 												userListOfStars=userListOfStars,
 												northOrSouth=northOrSouth, 
 												declination_min=declination_min,
 												yearSince2000=yearSince2000,
 												displayStarNamesLabels=displayStarNamesLabels,
 												displayDeclinationNumbers=displayDeclinationNumbers,
@@ -323,14 +321,16 @@
 												maxMagnitudeFilter=maxMagnitudeFilter,
 												showPlot=showPlot,
 												fig_plot_title=fig_plot_title,
 												fig_plot_color=fig_plot_color,
 												figsize_n=figsize_n,
 												figsize_dpi=figsize_dpi,
 												save_plot_name=save_plot_name)
+	northOrSouth = northOrSouth.capitalize()
+	userListOfStars = [x.title() for x in userListOfStars] # convert all names to capitalized
 
 	# plot star chart as a circular graph
 
 	# Set declination based on hemisphere selected
 	if declination_min is None:
 		if northOrSouth == "North": declination_min = int(config["declinationDefaultValues"]["northern_declination_min"])
 		if northOrSouth == "South": declination_min = int(config["declinationDefaultValues"]["southern_declination_min"])
```

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection/ra_dec_precession_vondrak.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/PKG-INFO` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: star-chart-spherical-projection
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python package to generate an astronomy star chart based on spherical projection that corrects for distortions with stereographic projection
 Home-page: https://github.com/cyschneck/Star-Chart-Spherical-Projection
 Author: cyschneck (C. Y. Schneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v1.4.1.tar.gz
 Description: # Star-Chart-Spherical-Projection
         
         ![PyPi](https://img.shields.io/pypi/v/star-chart-spherical-projection)
         ![license](https://img.shields.io/github/license/cyschneck/Star-Chart-Spherical-Projection)
+        [![pytests](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml/badge.svg?branch=main)](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml)
         
         A Python package to generate an astronomy star chart based on spherical projection with +90/-90° in the center based on a star's position (declination and right ascension): past, present, and future (proper motion and precession)
         
         The first step to plot the celestial sphere onto a 2D plot is to map the star's right ascension as hours along the plot (matplotlib polar plot's theta value) and declination as the distance from the center of the circle (matplotlib polar plot's radius value). However, attempting to map the right ascension and declination directly will cause distortion since the angles between the stars along the declination are no longer conserved. On the left, the constellation of the Big Dipper is stretched into an unfamiliar shape due to this distortion. By accounting for the spherical transformation, the star chart can be corrected as seen on the right.
         
         | Without Correction | With Correction |
         | ------------- | ------------- |
@@ -59,34 +60,49 @@
         
         ## Documentation
         
         **finalPositionOfStars()**
         
         Returns a dictionary for the final positions of the stars in the format: {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
         ```
-        finalPositionOfStars(userListOfStars=[], 
-        			northOrSouth=None, 
-        			yearSince2000=0,
+        finalPositionOfStars(yearSince2000=0, 
+        			userListOfStars=[],
         			isPrecessionIncluded=True,
         			declination_min=None,
         			declination_max=None)
         ```
-        - **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
         - *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-        - *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+        - *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
         - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-        - *[OPTIONAL]* declination_min: (int) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-        - *[OPTIONAL]* declination_max: (int) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+        - *[OPTIONAL]* declination_min: (int/float) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+        - *[OPTIONAL]* declination_max: (int/float) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+        
+        <details closed>
+        <summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+        <br>
+         ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+        'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
+        'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
+        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
+        'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
+        'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
+        'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
+        'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
+        'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
+        'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
+        'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
+        'Zubeneschamali']
+        </details>
         
         **plotStereographicProjection()**
         
         Plot stars on a Stereographic Polar Plot
         ```
-        plotStereographicProjection(userListOfStars=[], 
-        				northOrSouth=None, 
+        plotStereographicProjection(northOrSouth=None, 
+        				userListOfStars=[], 
         				declination_min=None,
         				yearSince2000=0,
         				displayStarNamesLabels=True,
         				displayDeclinationNumbers=True,
         				incrementBy=10,
         				isPrecessionIncluded=True,
         				maxMagnitudeFilter=None,
@@ -94,42 +110,45 @@
         				fig_plot_title=None,
         				fig_plot_color="C0",
         				figsize_n=12,
         				figsize_dpi=100,
         				save_plot_name=None)
         ```
         - **[REQUIRED]** northOrSouth: (string) map for either the "North" or "South" hemisphere
-        - *[OPTIONAL]* userListOfStar: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-        - *[OPTIONAL]* declination_min: (int) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-        - *[OPTIONAL]* yearSince2000: (float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+        - *[OPTIONAL]* userListOfStars: (list) a list of star names to include, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
+        - *[OPTIONAL]* declination_min: (int/float) outer declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+        - *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
         - *[OPTIONAL]* displayStarNamesLabels: (boolean) display the star name labels, defaults to True
         - *[OPTIONAL]* displayDeclinationNumbers: (boolean) display declination values, defaults to True
         - *[OPTIONAL]* incrementBy: (int) increment values for declination (either 1, 5, 10), defaults to 10
         - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-        - *[OPTIONAL]* maxMagnitudeFilter: (float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
-        - *[OPTIONAL]* returnData: (boolean) return a dictionary of stars with their final right ascension and declination ({"Vega" : [Declination (float) degrees, RA (str)]}, defaults to False
+        - *[OPTIONAL]* maxMagnitudeFilter: (int/float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
         - *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()) when finished running, defaults to True
         - *[OPTIONAL]* fig_plot_title: (string) figure title, defaults to "<North/South>ern Hemisphere [<YEAR NUMBERS> Years Since 2000 (YYYY)]: +/-90° to <DECLINATION MIN>°"
         - *[OPTIONAL]* fig_plot_color: (string) scatter plot star color, defaults to C0
-        - *[OPTIONAL]* figsize_n: (int) figure size, default to 12
-        - *[OPTIONAL]* figsize_dpi: (int) figure DPI, default to 100
+        - *[OPTIONAL]* figsize_n: (int/float) figure size, default to 12
+        - *[OPTIONAL]* figsize_dpi: (int/float) figure DPI, default to 100
         - *[OPTIONAL]* save_plot_name: (string) save plot with a string name, defaults to not saving
         
-        Current list of stars (to access via userListOfStar): ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
+        <details closed>
+        <summary>Stars that will be included by default when userListOfStars = [] (Click to view all)</summary>
+        <br>
+         ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 
         'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 
         'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 
-        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta cdPhoenicis', 'Betelgeuse', 'Canopus', 
+        'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 
         'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 
         'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 
         'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 
         'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 
         'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 
         'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 
         'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 
         'Zubeneschamali']
+        </details>
         
         ## Dependencies
         
         Python 3.7+
         ```
         pip3 install -r requirements.txt
         ```
@@ -151,32 +170,25 @@
         Returns a dictionary: `{'Betelgeuse': {'Declination': -36.342836095268325, 'RA': '16.34.28'}, 'Polaris': {'Declination': 45.08038305067079, 'RA': '17.25.11'}, 'Vega': {'Declination': 83.6899118156341, 'RA': '05.38.21'}}`
         
         ```python
         import star_chart_spherical_projection as scsp
         
         scsp.plotStereographicProjection(northOrSouth="North")
         ```
-        ## Tests
-        
         ## Bibliography
         
         Star position (right ascension and declination) as well as the angle and speed of proper motion taken from [in-the-sky.org](in-the-sky.org)
         
         Precession model: [Vondrák, J., et al. “New Precession Expressions, Valid for Long Time Intervals.” Astronomy &amp; Astrophysics, vol. 534, 2011, https://doi.org/10.1051/0004-6361/201117274.](https://www.aanda.org/articles/aa/pdf/2011/10/aa17274-11.pdf)
         
         Precession code adapted to Python3 from [github.com/dreamalligator/vondrak](github.com/dreamalligator/vondrak)
         
-        
         ## TODO:
         
-        Add README badges: tests
-        
-        Pypi tests
-        
-         Testing for new function finalPositionOfStars(), still needs testing
+        Add README badges: pypi tests
         
 Keywords: astronomy,python,star charts,precession,proper motion,spherical projection,stereographic projection
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `star-chart-spherical-projection-1.4.0/star_chart_spherical_projection.egg-info/SOURCES.txt` & `star-chart-spherical-projection-1.4.1/star_chart_spherical_projection.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 star_chart_spherical_projection/ra_dec_precession_vondrak.py
 star_chart_spherical_projection.egg-info/PKG-INFO
 star_chart_spherical_projection.egg-info/SOURCES.txt
 star_chart_spherical_projection.egg-info/dependency_links.txt
 star_chart_spherical_projection.egg-info/requires.txt
 star_chart_spherical_projection.egg-info/top_level.txt
 star_chart_spherical_projection/data/convert_lst_to_csv_data.py
-star_chart_spherical_projection/data/star_data.csv
+star_chart_spherical_projection/data/star_data.csv
+star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
+star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
```

