# Comparing `tmp/cemconvert-0.4.0.tar.gz` & `tmp/cemconvert-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cemconvert-0.4.0.tar", last modified: Thu Mar 16 15:27:20 2023, max compression
+gzip compressed data, was "dist/cemconvert-0.5.1.tar", last modified: Fri Jun 16 19:42:26 2023, max compression
```

## Comparing `cemconvert-0.4.0.tar` & `cemconvert-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,18 @@
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-03-16 15:27:20.000000 cemconvert-0.4.0/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      353 2023-03-16 15:03:52.000000 cemconvert-0.4.0/setup.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      204 2023-03-16 15:27:20.000000 cemconvert-0.4.0/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-03-16 15:27:19.000000 cemconvert-0.4.0/bin/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     4792 2023-03-16 15:03:34.000000 cemconvert-0.4.0/bin/get_camd_cems
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.4.0/bin/cemconvert
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-03-16 15:27:20.000000 cemconvert-0.4.0/cemconvert/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-02-08 15:54:45.000000 cemconvert-0.4.0/cemconvert/tz.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/temporal.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10129 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/ff10.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/qa.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      242 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5091 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/proc.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5329 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/cem.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-03-16 15:27:20.000000 cemconvert-0.4.0/cemconvert/data/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.4.0/cemconvert/data/county_fips_tz.csv
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4663 2023-02-08 15:40:19.000000 cemconvert-0.4.0/cemconvert/run_parse.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-03-16 15:27:20.000000 cemconvert-0.4.0/setup.cfg
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      100 2022-11-17 21:36:14.000000 cemconvert-0.4.0/README.md
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-03-16 15:27:20.000000 cemconvert-0.4.0/cemconvert.egg-info/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      382 2023-03-16 15:27:18.000000 cemconvert-0.4.0/cemconvert.egg-info/SOURCES.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      204 2023-03-16 15:27:18.000000 cemconvert-0.4.0/cemconvert.egg-info/PKG-INFO
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-03-16 15:27:18.000000 cemconvert-0.4.0/cemconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-03-16 15:27:18.000000 cemconvert-0.4.0/cemconvert.egg-info/top_level.txt
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      341 2023-05-22 20:27:00.000000 cemconvert-0.5.1/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      198 2023-06-16 19:42:26.000000 cemconvert-0.5.1/PKG-INFO
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/bin/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.1/bin/get_camd_cems
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.1/bin/cemconvert
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/cemconvert/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/tz.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/temporal.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10129 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/ff10.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/qa.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.1/cemconvert/cemcorrect.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/proc.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.1/cemconvert/cem.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/cemconvert/data/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.5.1/cemconvert/data/county_fips_tz.csv
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/run_parse.py
```

### Comparing `cemconvert-0.4.0/bin/get_camd_cems` & `cemconvert-0.5.1/bin/get_camd_cems`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 import time
 import pandas as pd
 import os.path
 from optparse import OptionParser, OptionGroup
 import requests
 
@@ -22,20 +22,28 @@
         mondf = pd.DataFrame()
         for day in date_range(month, year):
             print(day, flush=True)
             daystr = day.strftime('%Y-%m-%d')
             # Dates YYYY-MM-DD
             params = {'api_key': API_KEY, 'beginDate': daystr, 'endDate' : daystr, 
               'operatingHoursOnly': False}
-            req = requests.get(camd_url, params=params)
-            df = pd.DataFrame(req.json())
-            print('\tStatus code: %s   Records: %s' %(req.status_code, len(df)), flush=True)
+            # Make up to 3 attempts
+            for n in range(3): 
+                req = requests.get(camd_url, params=params)
+                if req.status_code == 200:
+                    df = pd.DataFrame(req.json())
+                    time.sleep(10)
+                    break
+                else:
+                    print('\tTry: %s   Status: %s' %(n, req.status_code))
+                    time.sleep(15)
+            if req.status_code != 200:
+                raise ValueError('Could not read emissions day')
+            print('\tRecords: %s' %len(df), flush=True)
             mondf = pd.concat((mondf, df))
-            # 5 second timeout between requests
-            time.sleep(5)
         mondf.rename(columns=cems.colmap, inplace=True)
         monname = day.strftime('%b').lower()
         fn = os.path.join(opts.output_path.strip(),
           '%s.txt' %'-'.join((opts.prefix.strip(), str(year), day.strftime('%b').lower(), 'hourly')))
         print('Writing %s records to %s' %(len(mondf), fn))
         mondf.to_csv(fn, index=False, columns=cems.cols)
 
@@ -77,19 +85,20 @@
           'so2Mass': 'SO2 Mass (lbs)', 'so2RateMeasureFlg': 'SO2 Rate Measure Indicator',
           'co2MassMeasureFlg': 'CO2 Mass Measure Indicator', 'co2Rate': 'CO2 Rate (short tons/mmBtu)',
           'co2Mass': 'CO2 Mass (short tons)', 'co2RateMeasureFlg': 'CO2 Rate Measure Indicator',
           'noxMassMeasureFlg': 'NOx Mass Measure Indicator', 'noxRate': 'NOx Rate (lbs/mmBtu)',
           'noxMass': 'NOx Mass (lbs)', 'noxRateMeasureFlg': 'NOx Rate Measure Indicator',
           'primaryFuelInfo': 'Primary Fuel Type', 'secondaryFuelInfo': 'Secondary Fuel Type',
           'unitType': 'Unit Type', 'so2ControlInfo': 'SO2 Controls', 'noxControlInfo': 'NOx Controls',
-          'pmControlInfo': 'PM Controls', 'hgControlInfo': 'Hg Controls', 'programCodeInfo': 'Program Code'}
+          'pmControlInfo': 'PM Controls', 'hgControlInfo': 'Hg Controls', 'programCodeInfo': 'Program Code',
+          'heatInputMeasureFlg': 'Heat Input Measure Indicator'}
        self.cols = ['State','Facility Name','Facility ID','Unit ID','Associated Stacks','Date',
           'Hour','Operating Time','Gross Load (MW)','Steam Load (1000 lb/hr)','SO2 Mass (lbs)',
           'SO2 Mass Measure Indicator','SO2 Rate (lbs/mmBtu)','SO2 Rate Measure Indicator',
           'NOx Mass (lbs)','NOx Mass Measure Indicator','NOx Rate (lbs/mmBtu)',
           'NOx Rate Measure Indicator','CO2 Mass (short tons)','CO2 Mass Measure Indicator',
           'CO2 Rate (short tons/mmBtu)','CO2 Rate Measure Indicator','Heat Input (mmBtu)',
           'Primary Fuel Type','Secondary Fuel Type','Unit Type','SO2 Controls','PM Controls',
-          'NOx Controls','Hg Controls','Program Code']
+          'NOx Controls','Hg Controls','Program Code','Heat Input Measure Indicator']
 
 if __name__ == '__main__':
     main()
```

### Comparing `cemconvert-0.4.0/bin/cemconvert` & `cemconvert-0.5.1/bin/cemconvert`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/tz.py` & `cemconvert-0.5.1/cemconvert/tz.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/temporal.py` & `cemconvert-0.5.1/cemconvert/temporal.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/ff10.py` & `cemconvert-0.5.1/cemconvert/ff10.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/qa.py` & `cemconvert-0.5.1/cemconvert/qa.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/proc.py` & `cemconvert-0.5.1/cemconvert/proc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 # Misc processes
 
 import os.path
 import pandas as pd
 from cemconvert.cem import CEM
+from cemconvert.cemcorrect import CemCorrect
 
 def proc_hourly(opts, tz):
     '''
     Read in the hourly CEM values by month in the new format
     Write to the old format
     Return a pivoted version
     '''
-    cems_months = ('jan','feb','mar','apr','may','jun','jul','aug','sep','oct','nov','dec')
     cems = CEM()
-    # Init an empty dataframe to hold the hourly values
-    hourly = pd.DataFrame()
-    for n in opts.months:
-        month = cems_months[n-1]
-        print('Processing %s' %month, flush=True)
-        # Read in CAMPD CEM inputs
-        fn = os.path.join(opts.input_path, 'campd-%s-%s-hourly.txt' %(opts.year, month))
-        monthly = cems.read_cems_month(fn)
-        if opts.write_cems:
-            # Write out old CEM format
-            fn = os.path.join(opts.output_path, 'HOUR_UNIT_%s_%0.2d.txt' %(opts.year, n))
-            cems.write_old_cems(fn, monthly)
-        # Timeshift hourly FF10 to GMT
-        if opts.gmt_output:
-            monthly = tz.timeshift_to_gmt(monthly)
-        # Extract the hour into the hour column and reset the date
-        monthly['hour'] = monthly.date.dt.hour.astype(int)
-        monthly['date'] = monthly.date.dt.normalize()
-        # Pivot the hourly values to columns
-        monthly = cems.pivot_hourly(monthly)
-        hourly = pd.concat((hourly, monthly))
+    cems.load_cems_period(opts.input_path, opts.year, opts.months)
+    # Run CEMCorrect
+    if opts.cemcorrect:
+        correct = CemCorrect()
+        # Start by calculating the means of the non-flagged values
+        for col in correct.valcols:
+            correct.calc_mean(col, cems.hourly)
+        # Correct the heat input
+        cems.hourly = correct.fill_mean('HTINPUT', cems.hourly)
+        # Correct the mass values
+        for col in correct.valcols:
+            if col != 'HTINPUT':
+                correct.calc_rate(col, cems.hourly)
+                cems.hourly = correct.fill_rate(col, cems.hourly)
+        fn = os.path.join(opts.output_path, 'cemcorrect_qa_%s_%s.csv' %(opts.label, opts.year))
+        correct.write_qa(fn)
+    cems.write_old_cems(opts.input_path, opts.year, opts.months)
+    # Timeshift hourly FF10 to GMT
+    if opts.gmt_output:
+        cems.hourly = tz.timeshift_to_gmt(cems.hourly)
+    # Extract the hour into the hour column and reset the date
+    cems.hourly['hour'] = cems.hourly.date.dt.hour.astype(int)
+    cems.hourly['date'] = cems.hourly.date.dt.normalize()
+    # Pivot the hourly values to columns
+    cems.hourly = cems.pivot_hourly(cems.hourly)
     if opts.gmt_output and opts.ramp_up:
-        hourly = fill_ramp_up(hourly, opts.year)
+        cems.hourly = fill_ramp_up(cems.hourly, opts.year)
     idx = ['oris_facility_code','oris_boiler_id','date','poll']
-    hourly = hourly.groupby(idx, as_index=False).sum()
-    hourly['month'] = hourly.date.dt.month.astype(int).astype(str)
-    return hourly
+    cems.hourly = cems.hourly.groupby(idx, as_index=False).sum()
+    cems.hourly['month'] = cems.hourly.date.dt.month.astype(int).astype(str)
+    return cems.hourly
 
 def gapfill_dates(df, year):
     '''
     Gapfill the dates by unit/poll combo to have all dates for every month in the run
     '''
     cols = list(df.columns)
     # Find all the dates for the selected months
```

### Comparing `cemconvert-0.4.0/cemconvert/data/county_fips_tz.csv` & `cemconvert-0.5.1/cemconvert/data/county_fips_tz.csv`

 * *Files identical despite different names*

### Comparing `cemconvert-0.4.0/cemconvert/run_parse.py` & `cemconvert-0.5.1/cemconvert/run_parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
           help='List of CEM months to process as a comma-delimited list of integers \
            Default behavior is an annual run')
         self.parser.add_option('-l', '--label', dest='label', default='ptegu',
           help='Output inventory label')
         self.parser.add_option('-k', '--keep_annual', dest='keepann', action='store_true',
           default=False, help='Keep and temporalize annual temporal values in FF10 that match CEMs.\
             Default is to replace the emissions values with CEMs.')
+        self.parser.add_option('-e', '--cemcorrect', dest='cemcorrect', action='store_true',
+          default=False, help='Apply CEMCorrect to the CEMS')
         return self.parser.parse_args()
 
     def set_ev(self):
         '''
         Set the attributes with the environment variables
         '''
         self.evs = {'MONTHS': 'months', 'YEAR': 'year', 'CEMPATH': 'input_path',
```

