# Comparing `tmp/ccfit2-4.5.1.tar.gz` & `tmp/ccfit2-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccfit2-4.5.1.tar", last modified: Sat Apr  1 07:46:03 2023, max compression
+gzip compressed data, was "ccfit2-5.0.0.tar", last modified: Fri Jun 16 14:31:56 2023, max compression
```

## Comparing `ccfit2-4.5.1.tar` & `ccfit2-5.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:46:03.818055 ccfit2-4.5.1/
--rw-r--r--   0 root         (0) root         (0)     2414 2023-04-01 07:46:03.817055 ccfit2-4.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-04-01 07:45:25.000000 ccfit2-4.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:46:03.814054 ccfit2-4.5.1/ccfit2/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-01 07:46:00.000000 ccfit2-4.5.1/ccfit2/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    67849 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/ac.py
--rw-rw-rw-   0 root         (0) root         (0)    27842 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    19008 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/dc.py
--rw-rw-rw-   0 root         (0) root         (0)     8485 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/gui.py
--rw-rw-rw-   0 root         (0) root         (0)   101187 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)    15111 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    28781 2023-04-01 07:45:25.000000 ccfit2-4.5.1/ccfit2/waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:46:03.817055 ccfit2-4.5.1/ccfit2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2414 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-01 07:46:03.000000 ccfit2-4.5.1/ccfit2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-01 07:45:26.000000 ccfit2-4.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 07:46:03.818055 ccfit2-4.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-01 07:46:00.000000 ccfit2-4.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.509508 ccfit2-5.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-16 14:31:56.508509 ccfit2-5.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-06-16 14:31:32.000000 ccfit2-5.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.507508 ccfit2-5.0.0/ccfit2/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-16 14:31:53.000000 ccfit2-5.0.0/ccfit2/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)   131893 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/ac.py
+-rw-rw-rw-   0 root         (0) root         (0)    67725 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    61106 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/dc.py
+-rw-rw-rw-   0 root         (0) root         (0)    20395 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)   167544 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)    10668 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-06-16 14:31:32.000000 ccfit2-5.0.0/ccfit2/waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:31:56.508509 ccfit2-5.0.0/ccfit2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-16 14:31:56.000000 ccfit2-5.0.0/ccfit2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-16 14:31:32.000000 ccfit2-5.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 14:31:56.509508 ccfit2-5.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-16 14:31:53.000000 ccfit2-5.0.0/setup.py
```

### Comparing `ccfit2-4.5.1/ccfit2/ac.py` & `ccfit2-5.0.0/ccfit2/dc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,2358 +1,2046 @@
-"""
-This module contains functions and objects for working with AC
-susceptibility data
-"""
+'''
+This module contains functions and objects for working with DC
+magnetisation decay data
+'''
 
-from abc import ABC, abstractmethod
-import numpy as np
 from math import isnan
-from scipy.optimize import least_squares, curve_fit
-import sys
-if sys.platform[0:3] == "win" or sys.platform == "darwin":
-    import matplotlib
-    matplotlib.use('TkAgg')
+import numpy as np
+import numpy.typing as npt
 import matplotlib.pyplot as plt
-import matplotlib.cm as cm
+from matplotlib.ticker import AutoMinorLocator
+from scipy.optimize import least_squares
+from abc import ABC, abstractmethod
 import copy
-import os
-import sys
-
-from . import gui
+import operator
+import warnings
 
+from . import utils as ut
+from . import stats
 
-# list of supported ac headers
-# These differ between magnetometers
-# One of each MUST be found in the input file
-HEADERS_SUPPORTED = {
-    'field': [
-        'Field (Oe)',
-        'Magnetic Field (Oe)'
+#: Supported DC Headers - One of each MUST be found in the input file.
+#:
+#:  Note - These differ between magnetometers\
+#:
+#:  These keys are the arguments to the Measurement constructor, but their
+#:  order does not matter
+HEADERS_SUPPORTED: dict[str, list[str]] = {
+    'dc_field': [
+        'Magnetic Field (Oe)',
+        'Field (Oe)'
     ],
     'temperature': [
         'Temperature (K)'
     ],
-    'sus_real': [
-        "m' (emu)",
-        "AC X'  (emu/Oe)",
-        "AC X' (emu/Oe)",
-        "M' (emu)",
-        "AC X' (emu/Oe)"
-    ],
-    'sus_imaginary': [
-        'm" (emu)',
-        'AC X" (emu/Oe)',
-        'AC X\'\' (emu/Oe)',
-        'M\'\' (emu)',
-        "AC X'' (emu/Oe)"
+    'time': [
+        'Time Stamp (sec)'
     ],
-    'ac_freq': [
-        'Wave Frequency (Hz)',
-        'AC Frequency (Hz)',
-        'Frequency (Hz)'
-    ],
-    'ac_field': [
-        'Drive Amplitude (Oe)',
-        'AC Drive (Oe)',
-        'Amplitude (Oe)'
+    'moment': [
+        'Moment (emu)',
+        'DC Moment Free Ctr (emu)',
+        'DC Moment Fixed Ctr (emu)'
     ]
 }
 
-# Generic ac magnetometer file header names
+# Generic dc magnetometer file header names
 HEADERS_GENERIC = HEADERS_SUPPORTED.keys()
 
 
-def locate_data_header(file: str, data_header: str = '[Data]') -> int:
-    """
-    Check whether data_header is in file.
+class Measurement():
+    '''
+    Stores data for a single DC Decay measurement at a
+    given temperature and applied field
 
     Parameters
     ----------
-    file : str
-        Name of magnetometer output file
-    data_header: str, default '[Data]'
-        Line which specifies the beginning of the data block in input file
+    dc_field : float
+        Applied dc field (Oe)
+    temperature : float
+        Temperature of datapoint (K)
+    moment : float
+        Magnetic moment of datapoint (emu)
+    time : float
+        Time of datapoint (s)
 
-    Returns
-    -------
-    int
-        line number containing data header, -1 if header not located.
-    """
-
-    data_line = -1
-
-    # Open file and store line containing data header
-    with open(file, 'r') as f:
-        for it, line in enumerate(f):
-            if data_header in line:
-                data_line = it + 1
-                break
-
-    return data_line
-
-
-def parse_headers(file: str,
-                  data_line: int) -> tuple[dict[str:int], dict[str:str]]:
-    """
-    Extracts headers from AC magnetometer output file and returns header name
-    and column position in file
+    Attributes
+    ----------
+    dc_field : float
+        Applied dc field (Oe)
+    temperature : float
+        Temperature of datapoint (K)
+    moment : float
+        Magnetic moment of datapoint (emu)
+    time : float
+        Time of datapoint (s)
+    rep_temperature : float
+        Representative temperature assigned to this datapoint (K)
+    rep_dc_field : float
+        Representative dc field assigned to this datapoint (Oe)
+    '''
+
+    def __init__(self, dc_field: float, temperature: float, time: float,
+                 moment: float):
+        self.dc_field = dc_field
+        self.temperature = temperature
+        self.time = time
+        self.moment = moment
+        self._rep_temperature = None
+        self._rep_dc_field = None
+
+    @property
+    def rep_temperature(self):
+        return self._rep_temperature
+
+    @rep_temperature.setter
+    def rep_temperature(self, value: float):
+        self._rep_temperature = value
+        return
+
+    @property
+    def rep_dc_field(self):
+        return self._rep_dc_field
+
+    @rep_dc_field.setter
+    def rep_dc_field(self, value: float):
+        self._rep_dc_field = value
+        return
+
+    @classmethod
+    def from_file(cls, file: str, header_indices: dict | str = 'find',
+                  data_header: str = '[Data]',
+                  verbose: bool = True) -> list['Measurement']:
+        '''
+        Extracts dc data from magnetometer output file and
+        returns list of datapoints, one for each valid measurement.\n
+        Incomplete lines are ignored
+
+        Parameters
+        ----------
+        file : str
+            Name of magnetometer output file
+        header_indices : str | dict, default 'find'
+            Default 'find' will automatically locate headers, else provide dict
+            with:\n
+            Keys as generic header names given in `HEADERS_GENERIC`\n
+            Values as column index (number) of header in file\n
+        data_header : str default '[Data]'
+            Contents of line which specifies the beginning of the data block
+            in input file.\n
+            Default is to find line containing '[Data]'
+        verbose: bool, default True
+            If True, issues parsing measurements are written to terminal
+        Returns
+        -------
+        list
+            Measurement objects, one per temperature, per field\n
+            List has the same order as the magnetometer file
+
+        '''
+
+        encoding = ut.detect_encoding(file)
+
+        # Check data_header is in file
+        data_index = ut.locate_data_header(file, data_header=data_header)
+
+        if header_indices == 'find':
+            # Get file headers
+            header_indices, _ = ut.parse_headers(
+                file, data_index, HEADERS_SUPPORTED
+            )
+
+        # Columns to extract from file
+        cols = {
+            gen: header_indices[gen] for gen in HEADERS_GENERIC
+        }
+
+        # Convert strings to floats, if not possible then mark as NaN
+        converters = {
+            it: lambda s: (float(s.strip() or np.NaN)) for it in cols.values()
+        }
+
+        # Read required columns of file
+        data = np.loadtxt(
+            file,
+            skiprows=data_index + 1,
+            delimiter=',',
+            converters=converters,
+            usecols=cols.values(),
+            encoding=encoding
+        )
+
+        # Remove missing entries that have been marked as nan
+        data = [
+            row for row in data
+            if not any(isnan(val) for val in row)
+        ]
+
+        # Convert array of floats into list of Measurement objects, one per
+        # line
+        # Remove positional nature of Measurement constructor args by using
+        # kwargs through dict
+        measurements = [
+            cls(**{
+                col: val
+                for col, val in zip(cols, row)
+            })
+            for row in data
+            if not any(isnan(val) for val in row)
+        ]
+
+        if not len(measurements) and verbose:
+            _msg = '\n Error: Cannot parse measurements from file {}'.format(
+                file
+            )
+            ut.cprint(_msg, 'red')
+
+        return measurements
+
+
+class Experiment():
+    '''
+    Stores data for multiple DC measurements at a
+    given temperature, given applied dc field
 
     Parameters
     ----------
-    file : str
-        Name of magnetometer output file
-    data_line: int
-        Line which specifies the beginning of the data block in input file
+    rep_temperature: float
+        Representative temperature of experiment (K)
+        e.g. mean of all datapoints (Measurements)
+    rep_dc_field : float
+        Representative dc field assigned to this experiment (Oe)
+        e.g. mean of all datapoints
+    raw_temperatures: array_like
+        Raw temperatures of experiment, one per datapoint (K)
+    times : array_like
+        Time value, one per datapoint (s)
+    moments : array_like
+        Measured moment, one value per datapoint (emu)
+    dc_fields : array_like
+        Applied dc field in Oe, one value per datapoint (Oe)
 
-    Returns
-    -------
-    dict
-        Keys are generic header names given in `HEADERS_GENERIC`
-        Values are column index of header in file
-        If header is not found, value is -1
-    dict
-        Keys are generic header names given in `HEADERS_GENERIC`
-        Values are specific header names found in file
-        If header is not found, value is empty string
-    """
-
-    # Open file and store all headers
-    with open(file, 'r') as f:
-        for it, line in enumerate(f):
-            if it == data_line:
-                ac_headers = line.split(',')
-                break
-
-    if '\n' in ac_headers:
-        ac_headers.pop(-1)
-
-    # Get indices of required headers in file
-    # Set default as -1 (not found)
-    header_indices = {name: -1 for name in HEADERS_GENERIC}
-    header_names = {name: "" for name in HEADERS_GENERIC}
-    for hit, header in enumerate(ac_headers):
-        for key, sup_heads in HEADERS_SUPPORTED.items():
-            for sup_head in sup_heads:
-                if header == sup_head:
-                    header_indices[key] = hit
-                    header_names[key] = header
-
-    return header_indices, header_names
-
-
-class ModelStore():
-    """
-    Stores information on selected model obtained from matplotlib radiobuttons
-    Necessary due to nature of tkinter callback, otherwise would require
-    use of global variables
-    """
-    def __init__(self):
-        self.model = None
+    Attributes
+    ----------
+    rep_temperature: float
+        Representative temperature of experiment
+        e.g. mean of all datapoints (Measurements)
+    rep_dc_field : float
+        Representative dc field assigned to this experiment (Oe)
+        e.g. mean of all datapoints
+    raw_temperatures: ndarray of floats
+        Raw temperatures of experiment, one per datapoint (K)
+    times : ndarray of floats
+        Time value, one per datapoint (s)
+    moments : ndarray of floats
+        Measured moment, one value per datapoint (emu)
+    dc_fields : ndarray of floats
+        Applied dc field in Oe, one value per datapoint (Oe)
+    meas_dc_fields : ndarray of floats
+        Applied dc field measured by the instrument\n
+        one value per datapoint (Oe)
+    '''
+
+    def __init__(self, rep_temperature: float, rep_dc_field: float,
+                 raw_temperatures: npt.ArrayLike,
+                 times: npt.ArrayLike, moments: npt.ArrayLike,
+                 dc_fields: npt.ArrayLike):
+
+        self.rep_temperature = rep_temperature
+        self.rep_dc_field = rep_dc_field
+        self.raw_temperatures = np.asarray(raw_temperatures)
+        self.times = np.asarray(times)
+        self.moments = np.asarray(moments)
+        self.dc_fields = np.asarray(dc_fields)
+        self._meas_dc_fields = np.copy(self.dc_fields)
 
-    def set_model(self, model: str) -> None:
-        """
-        Helper function which selects Model object from string
-        """
-        choices = {
-            model.NAME: model()
-            for model in [DebyeModel, GeneralisedDebyeModel, TwoMaximaModel]
-        }
-        self.model = choices[model]
         return
 
-    @staticmethod
-    def select_model(radio, modstore: 'ModelStore') -> None:
-        print("Model function \'{}\' has been selected.".format(
-            radio.value_selected
-        ))
-        """
-        Helper function which is fired as callback to button click
-        and assigns object specified by current radiobuttons selection
-        to the modelstore's model attribute
+    @property
+    def meas_dc_fields(self) -> npt.NDArray:
+        return self._meas_dc_fields
+
+    @meas_dc_fields.setter
+    def meas_dc_fields(self, value: npt.ArrayLike):
+        self._meas_dc_fields = np.asarray(value)
+        return
+
+    @classmethod
+    def _from_single(cls, measurements: list[Measurement],
+                     cut_moment: float = 0.01) -> 'Experiment':
+        '''
+        Creates experiment from single set of measurements
 
         Parameters
         ----------
-        radio: matplotlib.widgets.RadioButtons
-            Radiobuttons object
-        modstore: ModelStore
-            ModelStore object
+        measurements: list[Measurement]
+            Measurements constituting a single experiment
+        cut_moment: float, default 0.01
+            Specifies %% of initial moment\n
+            Moments smaller than this will be discarded
+        Returns
+        -------
+            Experiment
+        '''
+
+        # Remove moments less than cut_moment % of initial moment
+        measurements = [
+            mm
+            for mm in measurements
+            if mm.moment >= cut_moment * measurements[0].moment
+        ]
+
+        raw_temperatures = np.array([
+            mm.temperature for mm in measurements
+        ])
+
+        moments = np.array([
+            mm.moment for mm in measurements
+        ])
+
+        # Set start time to zero
+        mintime = np.min([
+            mm.time
+            for mm in measurements
+        ])
+
+        # Set start time of these measurements as zero
+        for mm in measurements:
+            mm.time -= mintime
+
+        times = np.array([
+            mm.time for mm in measurements
+        ])
+
+        dc_fields = np.array([
+            mm.dc_field for mm in measurements
+        ])
+
+        rep_temperature = measurements[0].rep_temperature
+        rep_dc_field = measurements[0].rep_dc_field
+
+        experiment = cls(
+            rep_temperature,
+            rep_dc_field,
+            raw_temperatures,
+            times,
+            moments,
+            dc_fields
+        )
+
+        return experiment
+
+    @classmethod
+    def from_measurements(cls, measurements: list[Measurement],
+                          temp_thresh: float = 0.1,
+                          field_thresh: float = 1,
+                          cut_moment: float = 0.01) -> list['Experiment']:
+        '''
+        Creates list of Experiment objects from a list of individual
+        Measurement objects. Experiments are defined as a set of measurements
+        with the same mean temperature and mean field - defined by thresholds
+
+        Parameters
+        ----------
+        measurement: list[Measurement]
+            Measurements at various temperatures and times
+        temp_thresh: float, default 0.1 K
+            Threshold used to discriminate between temperatures (K)
+        field_thresh: float, default 1 Oe
+            Threshold used to discriminate between dc field values (Oe)
+        cut_moment: float, default 0.01
+            Specifies %% of initial moment\n
+            Moments smaller than this will be discarded
+            after splitting by field and temperature.
 
         Returns
         -------
-        None
-        """
+        list[Experiment]
+            Each element is an Experiment\n
+            The list is sorted by\n
+            1. Mean dc_field (low to high)\n
+            2. then by mean temperature (low to high)\n
+        '''
+
+        # Sort measurements by dc field, temperature, and time
+        measurements = sorted(
+            measurements,
+            key=operator.attrgetter('dc_field', 'temperature', 'time')
+        )
+
+        # Find mean field values
+        mean_fields, fsi = ut.find_mean_values(
+            [
+                measurement.dc_field
+                for measurement in measurements
+            ],
+            thresh=field_thresh
+        )
 
-        modstore.set_model(radio.value_selected)
+        # Set each measurement's representative dc field, here the mean
+        for measurement, mean_field in zip(measurements, np.concatenate(mean_fields)): # noqa
+            measurement.rep_dc_field = mean_field
 
-        plt.pause(0.05)
-        plt.close('all')
+        # Re-sort using mean field
+        measurements = sorted(
+            measurements,
+            key=operator.attrgetter('rep_dc_field', 'temperature', 'time')
+        )
+        # Get indices which sort the above
+        order = sorted(
+            np.arange(len(measurements), dtype=int),
+            key=lambda k: (
+                measurements[k].rep_dc_field,
+                measurements[k].temperature,
+                measurements[k].time
+            )
+        )
+        # transfer field split points into new order
+        fsi = np.array([order[fs] for fs in fsi], dtype=int)
 
-        return
+        # Find mean temperature values
+        mean_temperatures, tsi = ut.find_mean_values(
+            [
+                measurement.temperature
+                for measurement in measurements
+            ],
+            thresh=temp_thresh
+        )
+
+        # Set each measurement's representative temperature, here the mean
+        for m, mt in zip(measurements, np.concatenate(mean_temperatures)):
+            m.rep_temperature = mt
+
+        # Re-sort using mean dc field and mean temperature
+        measurements = sorted(
+            measurements,
+            key=operator.attrgetter('rep_dc_field', 'rep_temperature', 'time')
+        )
+        # Get indices which sort the above
+        order = sorted(
+            np.arange(len(measurements), dtype=int),
+            key=lambda k: (
+                measurements[k].rep_dc_field,
+                measurements[k].rep_temperature,
+                measurements[k].time
+            )
+        )
+        # transfer temperature split points into new order
+        tsi = np.array([order[ts] for ts in tsi], dtype=int)
+        # transfer field split points into new order
+        fsi = np.array([order[fs] for fs in fsi], dtype=int)
+
+        # Split and field and temperature jumps
+        split_ind = np.concatenate([tsi, fsi])
+        # Remove duplicate split indices corresponding to field and temperature
+        # jump
+        split_ind = np.unique(split_ind)
+
+        # If only one experiment, then no need to split, just
+        # combine measurements into an experiment
+        if not len(split_ind):
+            experiments = [
+                cls._from_single(measurements, cut_moment=cut_moment)
+            ]
+        # >1 Experiment, then split up measurements from time jumps
+        else:
+            split_measurements: list[list[Measurement]] = np.split(
+                measurements,
+                split_ind + 1
+            )
+
+            # and combine each set of measurements into an experiment
+            experiments = [
+                cls._from_single(sm, cut_moment=cut_moment)
+                for sm in split_measurements
+            ]
+
+        return experiments
 
 
 class Model(ABC):
-    """
-    Abstract class on which all models of ac susceptibilities are based
-    """
+    '''
+    Abstract class on which all models of DC magnetisation decays are based
+    '''
 
     @property
     @abstractmethod
     def NAME() -> str:
-        "string name of model"
+        'String name of model'
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def FITHEADERS() -> str:
-        "string header for fit variables"
+    def DISP_NAME() -> str:
+        'Display name for interactive buttons'
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def MODELHEADERS() -> str:
-        "string header for computed model outputs"
+    def PARNAMES() -> list[str]:
+        'String names of parameters which can be fitted or fixed'
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def BOUNDS() -> tuple[list[float], list[float]]:
-        "Bounds for each parameter of model, used by scipy least_squares"
+    def VARNAMES_MM() -> dict[str, str]:
+        '''
+        Mathmode (i.e. $$, latex ) versions of PARNAMES\n
+        Keys are strings from PARNAMES plus any other variables which
+        might be plotted (e.g. lntau_expect)\n
+        Values are mathmode strings
+        '''
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def initial_params() -> list[float]:
-        "Initial (guess) values of parameters"
+    def UNITS() -> dict[str, str]:
+        '''
+        string names of units of PARNAMES\n
+        Keys are strings from PARNAMES
+        might be needed\n
+        Values are unit name strings
+        '''
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def fitted_params() -> list[float]:
-        "Final, fitted, values of parameters"
+    def UNITS_MM() -> dict[str, str]:
+        '''
+        Mathmode (i.e. $$, latex ) versions of UNITS\n
+        Keys are strings from PARNAMES
+        might be needed\n
+        Values are unit name strings
+        '''
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def flat_thresh() -> float:
-        "Threshold for fit of data to y=mx+b above which data is marked as flat" # noqa
+    def BOUNDS() -> dict[str, list[float, float]]:
+        '''
+        Bounds for each parameter of model
+        keys: parameter name
+        values: [upper, lower]
+        used by scipy least_squares
+        '''
         raise NotImplementedError
 
-    @property
-    @abstractmethod
-    def fit_status() -> bool:
-        "True if fit successful, else False"
-        raise NotImplementedError
-
-    @property
     @abstractmethod
-    def fit_temperature() -> float:
-        "Temperature of fit"
+    def calc_lntau_expect() -> float | list[float]:
+        '''
+        Calculates expectation value of ln(tau) from input parameters
+        '''
         raise NotImplementedError
 
-    @property
     @abstractmethod
-    def fit_dc_field() -> float:
-        "DC field of fit"
+    def calc_lntau_fit_ul() -> list[float]:
+        '''
+        Calculates upper and lower bounds of ln(tau) from fit uncertainty
+        in fitted parameters
+        '''
         raise NotImplementedError
 
-    @property
     @abstractmethod
-    def perr() -> float:
-        "Error in standard deviation of fit"
+    def calc_lntau_stdev() -> float | list[float]:
+        '''
+        Calculates standard deviation of ln(tau) from input paramaters
+        '''
         raise NotImplementedError
 
+    @staticmethod
     @abstractmethod
-    def model(parameters: list[float],
-              ac_freq_ang: list[float], ) -> tuple[list[float], list[float]]:
-        """
-        Computes model function of ac suceptibility
+    def model(parameters: dict[str, float], time: list[float]) -> list[float]:
+        '''
+        Evaluates model function of DC magnetisation decay
+        using provided parameter and time values.
 
         Parameters
         ----------
         parameters: list[float]
-            parameters used in model function
-
-        ac_freq_ang: list[float]
-            angular ac frequencies at which model will be evaluated
+            Parameters to use in model function
+        time: list[float]
+            Time values in seconds at which model function is evaluated
 
         Returns
         -------
         list[float]
-            real susceptibility
-        list[float]
-            imaginary susceptibility
+            Moment as a function of time
 
-        """
+        '''
         raise NotImplementedError
 
-    @abstractmethod
-    def discard() -> bool:
-        """Finds if an experimnet should be discarded due to poor fit"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def flat() -> bool:
-        """Finds if an experimnet should be discarded due to being flat"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def initial_params_from_experiment(self, experiment: 'Experiment') -> None:
-        """Finds guesses of initial fit parameters"""
-        raise NotImplementedError
-
-    @staticmethod
-    def from_experiments(experiments: list['Experiment'],
-                         verbose: bool = False) -> list['Model']:
-        """
-        Creates one model object per experiment, where the type of model
-        is set according to user input based on cole cole plot
+    @classmethod
+    def residuals(cls, params: dict[str, float], time: list[float],
+                  true_moment: list[float]) -> list[float]:
+        '''
+        Calculates difference between measured moment and
+        trial moment from model
 
         Parameters
         ----------
-        experiments: list[Experiment]
-            All experiments carried out at given value of dc field strength
-        verbose: bool, default False
-            If True, print initial parameter guesses to screen
+        params : list[float]
+            model parameter values
+        time: list[float]
+            time values in seconds at which model function is evaluated
+        moment : list[float]
+            true (experimental) values of magnetic moment
 
         Returns
-        ------
-        list[Model]
-            Instances of user-selected model, one per experiment
-
-        """
-
-        # Choose model to fit data of current set of experiments
-        current_model = Model.make_colecole_selector(
-            experiments
-        )
-
-        # Get initial parameter values from coldest experiment
-        current_model.initial_params_from_experiment(
-            experiments[0],
-            verbose=verbose
-        )
+        -------
+        list[float]
+            Residuals
+        '''
+        trial_moment = cls.model(params, time)
 
-        # Make copies of model, one per experiment
-        models = [
-            copy.deepcopy(current_model)
-            for _ in range(len(experiments))
-        ]
+        residuals = trial_moment - true_moment
+        return residuals
 
-        return models
+    def __init__(self):
+        '''
+        Set default values for mandatory attributes
+        '''
+
+        # Final model parameter values
+        self._final_var_values = {
+            var: None
+            for var in self.PARNAMES
+        }
 
-    @staticmethod
-    def make_colecole_selector(experiments: list['Experiment']) -> 'Model':
-        """
-        Creates cole cole plot of experimental data at a given field
-        with radiobuttons specifying which model the user wants to fit with.
+        # Fit status, temperature, and field
+        self._fit_status = False
+        self._temperature = None
+        self._dc_field = None
+        self._meas_dc_field = None
+
+        # Fit standard deviation
+        self._fit_stdev = {
+            var: None
+            for var in self.fit_vars.keys()
+        }
 
-        Parameters
-        ----------
-        experiments: list[Experiment]
-            List of experiments to plot
-        Returns
-        -------
-        Model
-            Name of model selected by user
-        """
+        # Expectation value and standard deviation of ln(tau)
+        self._lntau_expect = None
+        self._lntau_fit_ul = None
+        self._lntau_stdev = None
 
-        temperatures = [
-            experiment.temperatures[0] for experiment in experiments
-        ]
+        return
 
-        field = experiments[0].dc_field
+    @property
+    def fit_status(self) -> bool:
+        'True if fit successful, else False'
+        return self._fit_status
+
+    @fit_status.setter
+    def fit_status(self, value):
+        if isinstance(value, bool):
+            self._fit_status = value
+        else:
+            raise TypeError
+        return
 
-        colors = cm.coolwarm(np.linspace(0, 1, len(temperatures)))
-        fig, (ax1) = plt.subplots(
-            1,
-            1,
-            sharex='none',
-            sharey='none',
-            figsize=(7.5, 6),
-            num='Select Debye model'
-        )
-        supt = 'Cole-Cole plot at {:4.1f} Oe.'.format(field)
-        supt += '\nSelect model by clicking the circle -->'
-        fig.suptitle(supt, fontsize=10)
+    @property
+    def temperature(self) -> float:
+        'Temperature of fit (K)'
+        return self._temperature
+
+    @temperature.setter
+    def temperature(self, value):
+        if isinstance(value, (np.floating, float)):
+            self._temperature = value
+        else:
+            raise TypeError
+        return
 
-        # Plot cole-cole for each temperature
-        for it, experiment in enumerate(experiments):
+    @property
+    def dc_field(self) -> float:
+        'DC Field of fit (Oe)'
+        return self._dc_field
+
+    @dc_field.setter
+    def dc_field(self, value):
+        if isinstance(value, (np.floating, float)):
+            self._dc_field = value
+        else:
+            raise TypeError
+        return
 
-            if (it in [0, len(temperatures)-1] or it % 4 == 0):
-                _label = "{:.2f} K".format(experiment.temperatures[0])
-            else:
-                _label = ''
+    @property
+    def meas_dc_field(self) -> float:
+        'Measured DC Field of fit (Oe)'
+        return self._meas_dc_field
+
+    @meas_dc_field.setter
+    def meas_dc_field(self, value: float):
+        if isinstance(value, (np.floating, float)):
+            self._meas_dc_field = value
+        else:
+            raise TypeError
+        return
 
-            ax1.plot(
-                experiment.sus_re,
-                experiment.sus_im,
-                'o',
-                color=colors[it],
-                label=_label
-            )
+    @property
+    def final_var_values(self) -> float:
+        'Final values of parameters, both fitted and fixed'
+        return self._final_var_values
+
+    @final_var_values.setter
+    def final_var_values(self, value):
+        if isinstance(value, dict):
+            self._final_var_values = value
+        else:
+            raise TypeError
+        return
 
-        ax1.legend(
-            loc=0, fontsize='small', numpoints=1, ncol=2, frameon=False
-        )
-        ax1.set_xlabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        ax1.set_ylabel(r'$\chi^{,,}$ (cm$^{3}$mol$^{-1}$)')
+    @property
+    def fit_stdev(self) -> float:
+        'Standard deviation on fitted parameters, from fitting routine'
+        return self._fit_stdev
+
+    @fit_stdev.setter
+    def fit_stdev(self, value):
+        if isinstance(value, dict):
+            self._fit_stdev = value
+        else:
+            raise TypeError
+        return
 
-        print('\nField: {:6.2f} Oe.\nSelect the model function:'.format(field))
-        print('Debye               -> Single relaxation process.')
-        print('\nGeneralised Debye -> Single relaxation process with a distribution.') # noqa
-        print('\nTwo maxima     -> Two distinct relaxation processes, each with a distribution\n') # noqa
-
-        radio = gui.make_mpl_radiobuttons(
-            pos=[0.63, 0.878, 0.3, 0.13],
-            labels=(
-                DebyeModel.NAME,
-                GeneralisedDebyeModel.NAME,
-                TwoMaximaModel.NAME
-            ),
-            circle_radius=0.08,
-            figure=fig
-        )
+    @property
+    def fix_vars(self) -> dict[str, float]:
+        '''
+        Parameters to fix (i.e. not fit)
+        keys are names in PARNAMES, values are values
+        '''
+        return self._fix_vars
+
+    @fix_vars.setter
+    def fix_vars(self, value):
+        if isinstance(value, dict):
+            if any([key not in self.PARNAMES for key in value.keys()]):
+                raise KeyError('Unknown variable names provided to fix')
+            self._fix_vars = value
+        else:
+            raise TypeError('fix must be dictionary')
+        return
 
-        modstore = ModelStore()
-        radio.on_clicked(
-            lambda _: ModelStore.select_model(radio, modstore)
-        )
+    @property
+    def fit_vars(self) -> dict[str, float]:
+        '''
+        Parameters to fit
+        keys are names in PARNAMES, values are values
+        '''
+        return self._fit_vars
+
+    @fit_vars.setter
+    def fit_vars(self, value):
+        if isinstance(value, dict):
+            if any([key not in self.PARNAMES for key in value.keys()]):
+                raise KeyError('Unknown variable names provided to fit')
+            self._fit_vars = value
+        else:
+            raise TypeError('Fit must be dictionary')
+        return
 
-        plt.show()
+    @property
+    def lntau_stdev(self) -> float:
+        'Standard deviation of ln(tau)'
+        # If not calculated yet, then calculate
+        if self._lntau_stdev is None:
+            self.lntau_stdev = self.calc_lntau_stdev()
+        return self._lntau_stdev
+
+    @lntau_stdev.setter
+    def lntau_stdev(self, value):
+        self._lntau_stdev = value
 
-        if modstore.model is None:
-            sys.exit("Error: No Model Selected")
+    @property
+    def lntau_fit_ul(self) -> list[float]:
+        '''
+        Upper and lower (1 sigma) limits of ln(tau) from fit uncertainty
+        in fitted values
+        '''
+        # If not calculated yet, then calculate
+        if self._lntau_fit_ul is None:
+            self.lntau_fit_ul = self.calc_lntau_fit_ul()
+        return self._lntau_fit_ul
+
+    @lntau_fit_ul.setter
+    def lntau_fit_ul(self, value):
+        self._lntau_fit_ul = value
 
-        return modstore.model
+    @property
+    def lntau_expect(self) -> float:
+        'Expectation value of ln(tau)'
+        # If not calculated yet, then calculate
+        if self._lntau_expect is None:
+            self.lntau_expect = self.calc_lntau_expect()
+        return self._lntau_expect
+
+    @lntau_expect.setter
+    def lntau_expect(self, value):
+        self._lntau_expect = value
 
-    def residuals(cls, params, ac_freq_ang, true_sus_re, true_sus_im):
-        """
-        Calculates difference between true susceptibility and trial
-        susceptibility calculated using model
+    @classmethod
+    def residual_from_float_list(cls, new_vals: list[float],
+                                 fit_vars: dict[str, float],
+                                 fix_vars: dict[str, float],
+                                 time: list[float],
+                                 moment: list[float]) -> list[float]:
+        '''
+        Wrapper for `residuals` method, takes new values from fitting routine
+        which provides list[float], to construct new fit_vals dict, then
+        runs `residuals` method.
 
         Parameters
         ----------
-        params : list
-            model parameter values
-        ac_freq_ang : list
-            Angular AC Frequencies
-        true_sus_re : list
-            true (experimental) values of real part of susceptibility
-        true_sus_im : list
-            true (experimental) values of imaginary part of susceptibility
+
+        fit_vars: dict[str, float]
+            Parameter to fit in model function\n
+            keys are PARNAMES, values are float values
+        fix_vars: dict[str, float]
+            Parameter which remain fixed in model function\n
+            keys are PARNAMES, values are float values
+        time: list[float]
+            time values in seconds at which model function is evaluated
+        moment : list[float]
+            true (experimental) values of magnetic moment
 
         Returns
         -------
-        np.array
-            vector of residuals, real, then imaginary
-        """
-        [trial_sus_re, trial_sus_im] = cls.model(params, ac_freq_ang)
-        resid_re = trial_sus_re - true_sus_re
-        resid_im = trial_sus_im - true_sus_im
-        return np.concatenate((resid_re, resid_im))
-
-    def fit_model(self, experiment: 'Experiment', guess: list[float],
-                  no_discard: bool = False) -> None:
-        """
-        Fits model to susceptibility data
+        list[float]
+            Residuals
+        '''
+
+        # Swap fit values for new values from fit routine
+        new_fit_vars = {
+            name: guess
+            for guess, name in zip(new_vals, fit_vars.keys())
+        }
+
+        # And make combined dict of fit and fixed
+        # variable names (keys) and values
+        all_vars = {**fix_vars, **new_fit_vars}
+
+        return cls.residuals(all_vars, time, moment)
+
+    def fit_to(self, experiment: 'Experiment',
+               guess: str | list[float] = 'predefined',
+               verbose: bool = True) -> None:
+        '''
+        Fits model to Experiment
 
         Parameters
         ----------
         experiment : Experiment
             Experiment to which a model will be fitted
-        guess : list[float]
-            initial parameters used as starting guess
-        no_discard : bool, default False
-            If True, do not discard any fits
-        """
+        guess : str | list[float], default 'predefined'
+            Either string 'predefined', or dict of initial parameters
+            used as starting guess with keys as parameter names and values as
+            numerical values
+        verbose: bool, default True
+            If True, prints information to terminal
 
-        ac_freq_ang = 2.*np.pi*experiment.ac_freq
+        Returns
+        -------
+        None
+        '''
+
+        # Get starting guesses, either predefined in self or given
+        # by user
+        if guess != 'predefined':
+            guess = [
+                guess[key] for key in self.fit_vars.keys()
+            ]
+        else:
+            guess = [val for val in self.fit_vars.values()]
+
+        # Get bounds for variables to be fitted
+        bounds = np.array([
+            self.BOUNDS[name]
+            for name in self.fit_vars.keys()
+        ]).T
 
         curr_fit = least_squares(
-            fun=self.residuals,
+            self.residual_from_float_list,
+            args=[
+                self.fit_vars,
+                self.fix_vars,
+                experiment.times,
+                experiment.moments
+            ],
             x0=guess,
-            args=(
-                ac_freq_ang,
-                experiment.sus_re,
-                experiment.sus_im
-            ),
-            bounds=self.BOUNDS
+            bounds=bounds,
+            max_nfev=200 * (len(guess) + 1),
+            jac='3-point'
         )
 
-        self.fit_temperature = experiment.temperatures[0]
-        self.fit_dc_field = experiment.dc_field
-
-        # Fitted parameters
-        curr_fit.x = abs(curr_fit.x)
+        self.temperature = experiment.rep_temperature
+        self.dc_field = experiment.dc_fields[-1]
+        self.meas_dc_field = experiment.meas_dc_fields[-1]
 
         if curr_fit.status == 0:
-            print('Fit at {} Oe and {} K failed.'.format(
-                 self.fit_dc_field, self.fit_temperature
-            ))
-            print('Too many iterations')
-            self.fitted_params = []
-            self.perr = np.nan
-            self.fit_status = False
-        # Discard fit if resulting tau isnt within limits of frequency
-        elif self.discard(curr_fit.x, ac_freq_ang) and not no_discard:
-            message = 'At {: 6.1f} Oe and {: 6.2f} K'.format(
-                self.fit_dc_field, self.fit_temperature
-            )
-            message += ', no peak measured -> point discarded.'
-            print(message)
-            self.fitted_params = []
-            self.perr = np.nan
-            self.fit_status = False
-        elif self.flat(ac_freq_ang, experiment.sus_im, self.flat_thresh) and not no_discard: # noqa
-            message = 'At {: 6.1f} Oe and {: 6.2f} K'.format(
-                self.fit_dc_field, self.fit_temperature
-            )
-            message += ', data is flat -> point discarded.'
-            print(message)
-            self.fitted_params = []
-            self.perr = np.nan
+            if verbose:
+                ut.cprint(
+                    '\n Fit at {} K failed - Too many iterations'.format(
+                        self.temperature
+                    ),
+                    'black_yellowbg'
+                )
+
+            # Set fitted values
+            self.final_var_values = {
+                name: value
+                for name, value in zip(self.fit_vars, curr_fit.x)
+            }
+            # and fixed values
+            for key, val in self.fix_vars.items():
+                self.final_var_values[key] = val
+
+            self.fit_stdev = {
+                label: np.nan
+                for label in self.fit_vars.keys()
+            }
             self.fit_status = False
         else:
-            guess = curr_fit.x
-            # Calculate standard deviation error
-            J = curr_fit.jac
-            cov = np.linalg.inv(J.T.dot(J))
-            cov *= (curr_fit.fun**2).sum()/(
-                len(curr_fit.fun)-len(curr_fit.x)
-            )
+            stdev, nonzero_sing = stats.svd_stdev(curr_fit)
 
             # Standard deviation error on the parameters
-            self.fitted_params = curr_fit.x
-            self.perr = np.sqrt(np.diag(cov))
-            self.fit_status = True
-
-        return
-
-    @staticmethod
-    def write_model_data(experiments: list['Experiment'],
-                         models: list['Model'], filename=str):
-        """
-        Creates file containing chi' and chi'' calculated using the model
-        function with fitted parameters. Temperatures for which a fit was
-        not possible are not included.
-
-        Parameters
-        ----------
-        experiments : list[Experiment]
-            List of experiments to which a model was successfully fitted
-        models : list[Model]
-            List of models, one per experiment
-        filename: str
-            Name of output file
-
-        Returns
-        -------
-        None
-        """
-
-        f = open(filename, "w", encoding="utf-8")
-
-        # For each experiment and its corresponding model, calculate
-        # susceptibility using model parameters at experimental frequencies
-        for model, experiment in zip(models, experiments):
-
-            if not model.fit_status:
-                continue
+            self.fit_stdev = {
+                label: val
+                for label, val in zip(self.fit_vars.keys(), stdev)
+            }
 
-            freq_grid = np.logspace(
-                np.log10(np.min(experiment.ac_freq)),
-                np.log10(np.max(experiment.ac_freq)),
-                100
-            )
-
-            f.write('{:11} {:.5f}\n'.format('T = ', model.fit_temperature))
-
-            # Get model values at provided frequencies
-            [chips, chipps] = model.model(
-                model.fitted_params, freq_grid*2*np.pi
-            )
+            self.fit_status = True
 
-            f.write(model.MODELHEADERS)
-            for freq, chip, chipp in zip(freq_grid, chips, chipps):
-                f.write('{: 12.8E} {: 12.8E} {: 12.8E}\n'.format(
-                    freq, chip, chipp
-                ))
+            # Report singular values=0 of Jacobian
+            # and indicate that std_dev cannot be calculated
+            for par, si in zip(self.fit_vars.keys(), nonzero_sing):
+                if verbose and not si:
+                    ut.cprint(
+                        f'Warning: Jacobian is degenerate for {par}, standard deviation cannot be found, and is set to zero\n', # noqa
+                        'black_yellowbg'
+                    )
 
-        print("Model χ' and χ'' have been written to {}".format(filename))
+            # Set fitted values
+            self.final_var_values = {
+                name: value
+                for name, value in zip(self.fit_vars, curr_fit.x)
+            }
+            # and fixed values
+            for key, val in self.fix_vars.items():
+                self.final_var_values[key] = val
 
         return
 
-    @abstractmethod
-    def write_fit_params(cls) -> None:
-        """
-        Writes fitted parameters of model to file
-        """
-        raise NotImplementedError
-
-    @staticmethod
-    def plot_colecole(experiments: list['Experiment'],
-                      models: list['Model'],
-                      save_dir: str = "",
-                      file_head: str = "",
-                      save: bool = True) -> None:
-        """
-        Creates Cole-Cole plot as matplotlib figure
-
-        Parameters
-        ----------
-        experiments : list[Experiment]
-            List of experiments to which a model was successfully fitted
-        models : list[Model]
-            List of models, one per experiment
-        save_dir: str
-            Path to save directory
-        file_head: str
-            text added to head of file name
-        save: bool, default True
-            If true, saves plot to file as png
-        Returns
-        -------
-        None
-        """
-
-        fig, (ax1, ax2) = plt.subplots(
-            2,
-            1,
-            sharex='none',
-            sharey='none',
-            figsize=(5.1, 4.8),
-            gridspec_kw={"height_ratios": [0.03, 0.9]},
-            num='Cole-Cole fit'
-        )
-        fig.subplots_adjust(hspace=.02, wspace=.02)
-
-        fitted_temps = [
-            model.fit_temperature for model in models if model.fit_status
-        ]
-
-        n_temps = len(fitted_temps)
-
-        ratio = np.linspace(0, 1, np.sum(
-            [model.fit_status for model in models])
-        )
-        colors = cm.get_cmap('coolwarm', n_temps)
-
-        # Experimental data
-        count = -1
-        for experiment, model in zip(experiments, models):
-
-            if not model.fit_status:
-                continue
-
-            count += 1
-
-            # Plot Cole-Cole
-            ax2.plot(
-                experiment.sus_re,
-                experiment.sus_im,
-                'o',
-                markersize=4,
-                fillstyle='none',
-                label="{:.2f} K".format(model.fit_temperature),
-                color=colors(ratio[count])
-            )
 
-            # Convert linear to angular frequency
-            freq_grid = np.logspace(
-                np.log10(np.min(experiment.ac_freq*2.*np.pi)),
-                np.log10(np.max(experiment.ac_freq*2.*np.pi)),
-                100
-            )
+class ExponentialModel(Model):
+    '''
+    Exponential Model of Magnetisation decay with stretching parameters
+    '''
 
-            # Get model values at provided frequencies
-            [chips, chipps] = model.model(model.fitted_params, freq_grid)
+    #: Model name
+    NAME = 'Exponential'
 
-            ax2.plot(
-                chips,
-                chipps,
-                '-',
-                color=colors(ratio[count]),
-                lw=1
-            )
+    #: Display name for interactive buttons
+    DISP_NAME = copy.copy(NAME)
 
-        gui.create_ac_temp_colorbar(ax1, fig, fitted_temps, colors)
+    #: Model Parameter name strings
+    PARNAMES = [
+        'tau*', 'beta', 'm_eq', 'm_0', 't_offset'
+    ]
 
-        # Put the x-labels of the colourbar on top
-        ax1.xaxis.set_ticks_position('top')
+    #: Model Parameter bounds
+    BOUNDS = {
+        'tau*': [0., np.inf],
+        'beta': [0., 1.],
+        'm_eq': [-np.inf, np.inf],
+        'm_0': [0, np.inf],
+        't_offset': [0., np.inf]
+    }
 
-        # Remove frames
-        ax2.spines["top"].set_visible(False)
-        ax2.spines["right"].set_visible(False)
+    #: Model Parameter mathmode name strings
+    VARNAMES_MM = {
+        'tau*': r'$\tau^*$',
+        'lntau_expect': r'$\langle \ln \tau \rangle$',
+        'lntau_stdev': r'$\sigma_{\ln \tau}$',
+        'beta': r'$\beta$',
+        'm_eq': r'$M_\mathregular{eq}$',
+        'm_0': r'$M_0$',
+        't_offset': r'$\mathregular{t}_\mathregular{offset}$'
+    }
 
-        # Set labels for the axes
-        ax2.set_xlabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        ax2.set_ylabel(r'$\chi^{,,}$ (cm$^{3}$mol$^{-1}$)')
+    #: Model Parameter Unit strings
+    UNITS = {
+        'tau*': 's',
+        'beta': '',
+        'm_eq': 'emu',
+        'm_0': 'emu',
+        't_offset': 's'
+    }
 
-        fig.tight_layout()
+    #: Model Parameter Unit mathmode strings
+    UNITS_MM = {
+        'tau*': r'$\mathregular{s}$',
+        'beta': '',
+        'm_eq': r'$\mathregular{emu}$',
+        'm_0': r'$\mathregular{emu}$',
+        't_offset': r'$\mathregular{s}$',
+    }
 
-        if save:
+    def __init__(self, fit_vars: dict[str, float | str],
+                 fix_vars: dict[str, float | str], experiment: Experiment):
 
-            if len(file_head):
-                file_head = "{}_".format(file_head)
+        # Replace any 'guess' strings with proper guesses
+        self.fit_vars = self.set_initial_vals(fit_vars, experiment)
+        self.fix_vars = self.set_initial_vals(fix_vars, experiment)
+
+        # Check all PARNAMES are provided in fit+fix
+        input_names = [
+            name for name in {**self.fit_vars, **self.fix_vars}.keys()
+        ]
 
-            f_name = "{}Cole_Cole_model_{}_{:f}Oe.png".format(
-                file_head,
-                model.NAME.replace(" ", "_"),
-                experiments[0].dc_field
+        if any([req_name not in input_names for req_name in self.PARNAMES]):
+            raise ValueError(
+                'Missing fit/fix parameters in Exponential Model'
             )
 
-            f_name = os.path.join(save_dir, f_name)
-
-            fig.savefig(f_name, dpi=300)
-            print("\nCole-Cole plot saved to")
-            print("{}".format(f_name))
-
-        plt.show()
-        plt.close('all')
+        # Initialise remaining attributes required by Model superclass
+        super().__init__()
 
         return
 
     @staticmethod
-    def plot_susceptibility(experiments: list['Experiment'],
-                            models: list['Model'],
-                            save_dir: str = "",
-                            file_head: str = "",
-                            save: bool = True) -> None:
-        """
-
-        Creates plot of in- and out-of-phase susceptibilities
-        as matplotlib figure
+    def set_initial_vals(param_dict: dict[str, str | float],
+                         experiment: Experiment):
+        '''
+        Sets guess values for parameters if requested by user
 
         Parameters
         ----------
-        experiments : list[Experiment]
-            List of experiments to which a model was successfully fitted
-        models : list[Model]
-            List of models, one per experiment
-        save_dir: str
-            Path to save directory
-        file_head: str
-            text added to head of file name
-        save: bool, default True
-            If True, saves plot to file
+        param_dict: dict[str, str | float]
+            Keys are fit/fix parameter names (see class.PARNAMES)
+            values are either float (actual value) or the string 'guess'\n
+            If 'guess' then a parameter value is guessed using experiment
+        experiment : Experiment
+            Used to set guess values if specified
 
         Returns
         -------
-        None
-        """
-
-        fig, (ax1, ax2, ax3) = plt.subplots(
-            3,
-            1,
-            sharex='none',
-            sharey='none',
-            figsize=(6.5, 4.5),
-            gridspec_kw={"height_ratios": [0.05, 1, 1]},
-            num='AC susceptibility fits'
-        )  # 8.27, 11.69 A4
-        fig.subplots_adjust(hspace=.05, wspace=.02)
-
-        fitted_temps = [
-            model.fit_temperature for model in models if model.fit_status
-        ]
-
-        ratio = np.linspace(0, 1, np.sum(
-            [model.fit_status for model in models])
-        )
-
-        n_temps = len(fitted_temps)
-        colors = cm.get_cmap('coolwarm', n_temps)
-
-        # Experimental data
-        count = -1
-        for experiment, model in zip(experiments, models):
-
-            if not model.fit_status:
-                continue
-
-            count += 1
-
-            # Plots will be in linear frequency to compare to experiment
-            freq_grid = np.logspace(
-                np.log10(np.min(experiment.ac_freq)),
-                np.log10(np.max(experiment.ac_freq)),
-                100
-            )
-
-            # Get model values at provided frequencies
-            # Model takes angular frequencies
-            [chips, chipps] = model.model(
-                model.fitted_params,
-                freq_grid*2.*np.pi
-            )
-
-            # Real
-            ax2.semilogx(
-                experiment.ac_freq,
-                experiment.sus_re,
-                'o',
-                markersize=4,
-                fillstyle='none',
-                label='{:.1f} K'.format(model.fit_temperature),
-                color=colors(ratio[count])
-            )
-            ax2.semilogx(
-                freq_grid,
-                chips,
-                '-',
-                color=colors(ratio[count]),
-                lw=1
-            )
-            # Imaginary
-            ax3.semilogx(
-                experiment.ac_freq,
-                experiment.sus_im,
-                'o',
-                markersize=4,
-                fillstyle='none',
-                label='{:.1f} K'.format(model.fit_temperature),
-                color=colors(ratio[count])
-            )
-            ax3.semilogx(
-                freq_grid,
-                chipps,
-                '-',
-                color=colors(ratio[count]),
-                lw=1
-            )
-
-        # Do not share yax as it is linear and these are log
-        ax3.get_shared_x_axes().join(ax2, ax3)
-
-        gui.create_ac_temp_colorbar(ax1, fig, fitted_temps, colors)
-
-        ax1.xaxis.set_ticks_position('top')
-        ax1.xaxis.set_label_position('top')
-
-        ax2.set_xticklabels([])
-        ax2.set_ylabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        # Get rid of the frames of susceptibility plots
-        for axis in [ax2, ax3]:
-            axis.spines["top"].set_visible(False)
-            axis.spines["right"].set_visible(False)
-
-        # Get rid of the x-labels of real susceptibility
-        ax2.set_xticklabels([])
-        ax2.set_ylabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        ax3.set_xlabel('Wave Frequency (Hz)')
-        ax3.set_ylabel(r'$\chi^{,,}$ (cm$^{3}$mol$^{-1}$)')
-
-        if save:
-
-            if len(file_head):
-                file_head = "{}_".format(file_head)
-
-            f_name = "{}sus_components_model_{}_{:f}Oe.png".format(
-                file_head,
-                model.NAME.replace(" ", "_"),
-                experiments[0].dc_field
-            )
-
-            f_name = os.path.join(save_dir, f_name)
-
-            fig.savefig(f_name, dpi=400)
-
-            print("\nSusceptibility plot saved to")
-            print("{}".format(f_name))
-
-        plt.show()
-
-        return
-
-
-class DebyeModel(Model):
-
-    NAME: str = 'Debye'
-
-    BOUNDS: tuple[list] = (
-        [0., 0., 0.],
-        [np.inf, np.inf, np.inf]
-    )
-
-    FITHEADERS: str = '  {:10} {:16} {:18} {:14} {:18} {:18} {:18}\n'.format(
-        'T', 'tau', 'tau_err', 'chi_S', 'chi_S_err', 'chi_T', 'chi_T_err'
-    )
+        dict[str, float]
+            Keys are fit/fix parameter names (see class.PARNAMES)
+            values are float (actual value) which are initial values of
+            parameter
+        '''
+
+        # Make copy, any str values will be replaced
+        new_param_dict = copy.copy(param_dict)
+
+        # Guesses
+        guessdict = {
+            'tau*': 100.,
+            'm_eq': experiment.moments[-1],  # M_eq guess final measured moment
+            'm_0': experiment.moments[0],  # M_0 is first measured moment
+            'beta': 0.95,
+            't_offset': 0.
+        }
 
-    MODELHEADERS: str = '{:11} {:11} {:11}\n'.format(
-        "Wave Frequency (linear) (Hz)", "χ' (cm^{3}mol^{-1})",
-        "χ'' (cm^{3}mol^{-1})"
-    )
+        # Replace 'guess' with relevant guess
+        for var, val in param_dict.items():
+            if val == 'guess':
+                new_param_dict[var] = guessdict[var]
 
-    flat_thresh: float = 1E-06
-    # Parameters are ordered, Tau, Chi_S, Chi_T
-    initial_params: list = []
-    fitted_params: list = []
-    fit_status: bool = False
-    fit_temperature: float = np.nan
-    fit_dc_field: float = np.nan
-    perr: float = np.nan
+        return new_param_dict
 
     @staticmethod
-    def model(parameters: list[float],
-              ac_freq_ang: list[float], ) -> tuple[list[float], list[float]]:
-        """
-        Computes Debye model function of ac suceptibility
+    def model(parameters: dict[str, float], time: list[float]) -> list[float]:
+        '''
+        Evaluates exponential model function of DC magnetisation decay
+        using provided parameter and time values.
 
         Parameters
         ----------
-        parameters: list[float]
-            parameters used in model function
-            [Tau, Chi_S, Chi_T]
-
-        ac_freq_ang: list[float]
-            angular ac frequencies at which model will be evaluated
+        parameters: dict[str, float]
+            Parameters to use in model function, keys are given in
+            ExponentialModel.PARNAMES
+        time: list[float]
+            time values in seconds at which model function is evaluated
 
         Returns
         -------
         list[float]
-            real susceptibility
-        list[float]
-            imaginary susceptibility
-
-        """
+            moment as a function of time
 
-        tau, chi_S, chi_T = parameters
-        func_real = abs(chi_S)
-        func_real += (abs(chi_T)-abs(chi_S))/(1+(ac_freq_ang**2)*(abs(tau)**2))
-        func_im = ac_freq_ang*abs(tau)*(abs(chi_T)-abs(chi_S))
-        func_im /= (1.+(ac_freq_ang**2)*(abs(tau)**2))
+        '''
 
-        return func_real, func_im
+        m_eq = parameters['m_eq']
+        m_0 = parameters['m_0']
+        beta = parameters['beta']
+        tau_star = parameters['tau*']
+        t_offset = parameters['t_offset']
 
-    @staticmethod
-    def discard(fit_param: list[float], ac_freq_ang: list[float]) -> bool:
-        """
-        Decides whether fits should be discarded based on following criteria
+        mom = m_eq
+        mom += (m_0 - m_eq) * np.exp(-((time - t_offset) / tau_star)**beta)
 
-        1. tau^-1 < smallest ac frequency
+        return mom
 
-        2. tau^-1 > largest ac frequency
+    def calc_lntau_expect(self) -> float:
+        '''
+        Calculates expectation value of ln(tau)
 
         Parameters
         ----------
-        fit_param : list[float]
-            Fitted parameters tau, chi_S, chit_T, alpha
-        ac_freq_ang: list[float]
-            Angular ac frequencies
+        None
 
         Returns
         -------
-        bool
-            True if point should be discarded, else False
-        """
-
-        to_discard = False
-
-        if 1./(fit_param[0]) < np.min(ac_freq_ang):
-            to_discard = True
-        elif 1./(fit_param[0]) > np.max(ac_freq_ang):
-            to_discard = True
-
-        return to_discard
+        float
+            <ln(tau)> value in ln(seconds)
 
-    @staticmethod
-    def flat(ac_freq_ang: list[float], sus_im: list[float], threshold):
-        """
-        Calculates fit of data to y = mx+b to find if data is flat
-        If flat, the error of this fit will be very low
+        Raises
+        -----
+        ValueError
+            If required model parameters in self.final_var_values are undefined
+        '''
+
+        beta = self.final_var_values['beta']
+        tau_star = self.final_var_values['tau*']
+
+        if None in [beta, tau_star]:
+            _error = 'Cannot calculate ln(tau) expectation value '
+            _error += 'beta and/or tau* are undefined!'
+            raise ValueError(_error)
+
+        return (1 - (1 / beta)) * np.euler_gamma + np.log(tau_star)
+
+    def calc_lntau_stdev(self) -> float:
+        '''
+        Calculates standard deviation of ln(tau)
 
         Parameters
         ----------
-        ac_freq_ang : list[float]
-            Angular AC Frequency of each measurement
-        sus_im : list[float]
-            Imaginary component of susceptibility of each measurement
-        threshold : float
-            Threshold for data to be marked as flat
+        None
 
         Returns
         -------
-        bool
-            True if point is flat and should be discarded, else False
-        """
-
-        is_flat = False
-
-        linear_popt, _ = curve_fit(lambda a, x, b: a*x+b, ac_freq_ang, sus_im)
-        error = np.square(linear_popt[0]*ac_freq_ang + linear_popt[1] - sus_im)
-
-        if np.sqrt(np.sum(error)) < threshold:
-            is_flat = True
-
-        return is_flat
-
-    def initial_params_from_experiment(self, experiment: 'Experiment',
-                                       verbose: bool = False) -> None:
-        """
-        Generates initial guess of fitting parameters from experiment
-
-        Parameters and guesses are
-
-        Tau - Mean of smallest ac angular frequencies
-        Chi_S - Smallest real susceptibility
-        Chi_T - Range of real susceptibilities
-
-        Parameters
-        ----------
-        experiment: Experiment
-            Experiment object whose data is used for initial guesses
-        verbose: bool, default False
-            If True, print initial guesses to screen
-
-        """
-
-        # Mean of two lowest frequencies
-        mean_low_freq = np.mean(np.sort(experiment.ac_freq)[:2])
-
-        self.initial_params = [
-            1./(2.*np.pi*mean_low_freq),
-            np.min(experiment.sus_re),
-            np.max(experiment.sus_re) - np.min(experiment.sus_re)
-        ]
-
-        if verbose:
-            print(
-                '\nThe initial guesses are',
-                '\ntau = {}\nchi_S = {}\nchi_T = {}\n'.format(
-                    *self.initial_params
-                )
-            )
-
-        return
+        float
+            Standard deviation of ln(tau) in ln(seconds)
 
-    @staticmethod
-    def write_fit_params(models: list[Model], file_name: str):
-        """
-        Writes fitted parameters of models to file
+        Raises
+        -----
+        ValueError
+            If required model parameters in self.final_var_values are undefined
+        '''
+
+        beta = self.final_var_values['beta']
+
+        if beta is None:
+            _error = 'Error: Cannot calculate ln(tau) standard deviation'
+            _error += 'beta undefined!'
+            raise ValueError(_error)
+
+        return np.sqrt((1. / beta**2 - 1.) * np.pi**2 / 6.)
+
+    def calc_lntau_fit_ul(self) -> list[float]:
+        '''
+        Calculates upper and lower bounds of ln(tau) from fit uncertainty
+        in fitted parameters
 
         Parameters
         ----------
-        models : list[Model]
-            Models, one per temperature
-        file_name : str
-            Name of output file
-
-        Returns
-        -------
         None
-        """
-        f = open(file_name, "w")
-
-        f.write(models[0].FITHEADERS)
-
-        for model in models:
-            if not model.fit_status:
-                continue
-            f.write('{: 8.6f}   '.format(model.fit_temperature))
-            for j in range(len(model.fitted_params)):
-                f.write('   {: 12.8E}   {: 12.8E}'.format(
-                    model.fitted_params[j], model.perr[j]
-                ))
-            f.write('\n')
-
-        print("\nFit information has been written to {}\n".format(
-            file_name
-        ))
-
-        return
-
-
-class GeneralisedDebyeModel(Model):
-
-    NAME: str = 'Generalised Debye'
-
-    BOUNDS: tuple[list] = (
-        [0., 0., 0., 0.],
-        [np.inf, np.inf, np.inf, 1.0]
-    )
-
-    FITHEADERS: str = '  {:11} {:15} {:20} {:20} {:17} {:14} {:18} {:17} {:17} {:17} {:17}\n'.format( # noqa
-        'T', 'tau', 'tau_ln_err_up', 'tau_ln_err_lw', 'tau_err', 'chi_S',
-        'chi_S_err', 'chi_T', 'chi_T_err', 'alpha', 'alpha_err'
-    )
-
-    MODELHEADERS: str = '{:11} {:11} {:11}\n'.format(
-        "Wave Frequency (linear) (Hz)", "χ' (cm^{3}mol^{-1})",
-        "χ'' (cm^{3}mol^{-1})"
-    )
-
-    flat_thresh: float = 1E-06
-    # Parameters are ordered Tau, Chi_S, Chi_T, alpha
-    initial_params: list = []
-    fitted_params: list = []
-    fit_status: bool = False
-    fit_temperature: float = np.nan
-    fit_dc_field: float = np.nan
-    perr: float = np.nan
-
-    @staticmethod
-    def model(parameters: list[float],
-              ac_freq_ang: list[float], ) -> tuple[list[float], list[float]]:
-        """
-        Computes Generalised Debye model function of ac suceptibility
-
-        Parameters
-        ----------
-        parameters: list[float]
-            parameters used in model function
-            [Tau, Chi_S, Chi_T, alpha]
-
-        ac_freq_ang: list[float]
-            angular ac frequencies at which model will be evaluated
 
         Returns
         -------
         list[float]
-            real susceptibility
-        list[float]
-            imaginary susceptibility
+            upper and lower bounds of ln(tau) from fit uncertainty in fitted
+            parameters (upper > lower)
+        '''
 
-        """
-        tau, chi_S, chi_T, alpha = parameters
-        func_real = abs(chi_S)+(abs(chi_T)-abs(chi_S))*(1.+np.power((ac_freq_ang*abs(tau)),(1.-abs(alpha)))*np.sin(np.pi*abs(alpha)/2.))/(1.+2.*np.power((ac_freq_ang*abs(tau)),(1.-abs(alpha)))*np.sin(np.pi*abs(alpha)/2.)+np.power((ac_freq_ang*abs(tau)),(2.-2*abs(alpha)))) # noqa
-        func_im = (abs(chi_T)-abs(chi_S))*((np.power((ac_freq_ang*abs(tau)),(1.-abs(alpha)))*np.cos(np.pi*abs(alpha)/2.)))/(1.+2.*np.power((ac_freq_ang*abs(tau)),(1.-abs(alpha)))*np.sin(np.pi*abs(alpha)/2.)+np.power((ac_freq_ang*abs(tau)),(2.-2*abs(alpha)))) # noqa
-        return func_real, func_im
+        tau_star = self.final_var_values['tau*']
 
-    @staticmethod
-    def discard(fit_param: list[float], ac_freq_ang: list[float]) -> bool:
-        """
-        Decides whether fits should be discarded based on following criteria
+        if 'tau*' in self.fit_stdev:
+            tau_star_std = self.fit_stdev['tau*']
+        else:
+            tau_star_std = 0.
 
-        1. tau^-1 < smallest ac frequency
+        beta = self.final_var_values['beta']
 
-        2. tau^-1 > largest ac frequency
+        if 'beta' in self.fit_stdev:
+            beta_std = self.fit_stdev['beta']
+        else:
+            beta_std = 0.
 
-        Parameters
-        ----------
-        fit_param : list[float]
-            Fitted parameters tau, chi_S, chit_T, alpha
-        ac_freq_ang: list[float]
-            Angular ac frequencies
+        upper = (1 - (1 / (beta - beta_std))) * np.euler_gamma + np.log(tau_star + tau_star_std) # noqa
+        lower = (1 - (1 / (beta + beta_std))) * np.euler_gamma + np.log(tau_star - tau_star_std) # noqa
 
-        Returns
-        -------
-        bool
-            True if point should be discarded, else False
-        """
-
-        to_discard = False
-
-        if 1./(fit_param[0]) < np.min(ac_freq_ang):
-            to_discard = True
-        elif 1./(fit_param[0]) > np.max(ac_freq_ang):
-            to_discard = True
+        return sorted([upper, lower], reverse=True)
 
-        return to_discard
 
-    @staticmethod
-    def flat(ac_freq_ang: list[float], sus_im: list[float], threshold):
-        """
-        Calculates fit of data to y = mx+b to find if data is flat
-        If flat, the error of this fit will be very low
+class DoubleExponentialModel(Model):
+    '''
+    Double Exponential Model of Magnetisation decay
+    '''
 
-        Parameters
-        ----------
-        ac_freq_ang : list[float]
-            Angular AC Frequency of each measurement
-        sus_im : list[float]
-            Imaginary component of susceptibility of each measurement
-        threshold : float
-            Threshold for data to be marked as flat
+    #: Model Name
+    NAME = 'Double Exponential'
 
-        Returns
-        -------
-        bool
-            True if point is flat and should be discarded, else False
-        """
+    #: Display name for interactive buttons
+    DISP_NAME = copy.copy(NAME)
 
-        is_flat = False
+    #: Model Parameter name strings
+    PARNAMES = [
+        'tau*1', 'tau*2', 'beta1', 'beta2', 'm_eq', 'm_0', 't_offset', 'frac'
+    ]
 
-        linear_popt, _ = curve_fit(lambda a, x, b: a*x+b, ac_freq_ang, sus_im)
-        error = np.square(linear_popt[0]*ac_freq_ang + linear_popt[1] - sus_im)
+    #: Model Parameter bounds
+    BOUNDS = {
+        'tau*1': [0., np.inf],
+        'tau*2': [0., np.inf],
+        'beta1': [0., 1.],
+        'beta2': [0., 1.],
+        'frac': [0., 1.],
+        'm_eq': [-np.inf, np.inf],
+        'm_0': [0., np.inf],
+        't_offset': [0., np.inf]
+    }
 
-        if np.sqrt(np.sum(error)) < threshold:
-            is_flat = True
+    #: Model Parameter mathmode name strings
+    VARNAMES_MM = {
+        'tau*1': r'$\tau_{1}^*$',
+        'tau*2': r'$\tau_{2}^*$',
+        'lntau_expect1': r'$\langle \ln \tau 1 \rangle$',
+        'lntau_expect2': r'$\langle \ln \tau 2 \rangle$',
+        'lntau_stdev1': r'$\sigma_{\ln \tau 1}$',
+        'lntau_stdev2': r'$\sigma_{\ln \tau 2}$',
+        'beta1': r'$\beta_{1}$',
+        'beta2': r'$\beta_{2}$',
+        'frac': r'Fraction',
+        'm_eq': r'$M_\mathregular{eq}$',
+        'm_0': r'$M_0$',
+        't_offset': r'$\mathregular{t}_\mathregular{offset}$'
+    }
 
-        return is_flat
+    #: Model Parameter Unit strings
+    UNITS = {
+        'tau*1': 's',
+        'tau*2': 's',
+        'beta1': '',
+        'beta2': '',
+        'frac': '',
+        'm_eq': 'emu',
+        'm_0': 'emu',
+        't_offset': 's'
+    }
 
-    def initial_params_from_experiment(self, experiment: 'Experiment',
-                                       verbose: bool = False) -> None:
-        """
-        Generates initial guess of fitting parameters from experiment
+    #: Model Parameter Unit mathmode strings
+    UNITS_MM = {
+        'tau*1': r'$\mathregular{s}$',
+        'tau*2': r'$\mathregular{s}$',
+        'beta1': '',
+        'beta2': '',
+        'frac': '',
+        'm_eq': r'$\mathregular{emu}$',
+        'm_0': r'$\mathregular{emu}$',
+        't_offset': r'$\mathregular{s}$',
+    }
 
-        Parameters and guesses are
+    # Redefined for list
+    @property
+    def lntau_stdev(self) -> list[float]:
+        'Standard deviation of ln(tau)'
+        # If not calculated yet, then calculate
+        if None in self._lntau_stdev:
+            self._lntau_stdev = self.calc_lntau_stdev()
+        return self._lntau_stdev
 
-        Tau - Mean of smallest ac angular frequencies
-        Chi_S - Smallest real susceptibility
-        Chi_T - Range of real susceptibilities
-        alpha - 0.1
+    # Redefined for list
+    @property
+    def lntau_fit_ul(self) -> list[list[float]]:
+        '''
+        Upper and lower (1 sigma) limits of ln(tau) from fit uncertainty
+        in fitted values
+        '''
+        # If not calculated yet, then calculate
+        if None in self._lntau_fit_ul:
+            self._lntau_fit_ul = self.calc_lntau_fit_ul()
+        return self._lntau_fit_ul
 
-        Parameters
-        ----------
-        experiment: Experiment
-            Experiment object whose data is used for initial guesses
-        verbose: bool, default False
-            If True, print initial guesses to screen
-        """
-
-        # Mean of two lowest frequencies
-        mean_low_freq = np.mean(np.sort(experiment.ac_freq)[:2])
-
-        self.initial_params = [
-            1./(2.*np.pi*mean_low_freq),
-            np.min(experiment.sus_re),
-            np.max(experiment.sus_re) - np.min(experiment.sus_re),
-            0.1
+    # Redefined for list
+    @property
+    def lntau_expect(self) -> list[float]:
+        'Expectation value of ln(tau)'
+        # If not calculated yet, then calculate
+        if None in self._lntau_expect:
+            self._lntau_expect = self.calc_lntau_expect()
+        return self._lntau_expect
+
+    def __init__(self, fit_vars: dict[str, float | str],
+                 fix_vars: dict[str, float | str], experiment: Experiment):
+
+        # Replace any 'guess' strings with proper guesses
+        self.fit_vars = self.set_initial_vals(fit_vars, experiment)
+        self.fix_vars = self.set_initial_vals(fix_vars, experiment)
+
+        # Check all PARNAMES are provided in fit+fix
+        input_names = [
+            name for name in {**self.fit_vars, **self.fix_vars}.keys()
         ]
 
-        if verbose:
-            print(
-                '\nThe initial guesses are',
-                '\ntau = {}\nchi_S = {}\nchi_T = {}\nalpha = {}\n'.format(
-                    *self.initial_params
-                )
+        if any([req_name not in input_names for req_name in self.PARNAMES]):
+            raise ValueError(
+                'Missing fit/fix parameters in Double Exponential Model'
             )
 
-        return
-
-    @staticmethod
-    def log_normal_bounds(tau, alpha, sigma):
-        """
-        Calculates bounds of tau in log normal space
-
-        Parameters
-        ----------
-        tau : np.ndarray
-            Tau
-        alpha : np.ndarray
-            alpha
-        sigma : float
-            sigma
-
-        Returns
-        -------
-        float
-            Bound
-        """
+        # Initialise remaining attributes required by Model superclass
+        super().__init__()
 
-        bound = tau*np.exp((1.82*sigma*np.sqrt(alpha))/(1-alpha))
+        # Expectation value and standard deviation of ln(tau)
+        self._lntau_expect = [None, None]
+        self._lntau_fit_ul = [None, None]
+        self._lntau_stdev = [None, None]
 
-        return bound
+        return
 
     @staticmethod
-    def write_fit_params(models: list[Model], file_name: str):
-        """
-        Writes fitted parameters of models to file
+    def set_initial_vals(param_dict: dict[str, str | float],
+                         experiment: Experiment):
+        '''
+        Sets guess values for parameters if requested by user
 
         Parameters
         ----------
-        models : list[Model]
-            Models, one per temperature
-        file_name : str
-            Name of output file
+        param_dict: dict[str, str | float]
+            Keys are fit/fix parameter names (see class.PARNAMES)
+            values are either float (actual value) or the string 'guess'\n
+            If 'guess' then a parameter value is guessed using experiment
+        experiment : Experiment
+            Used to set guess values if specified
 
         Returns
         -------
-        None
-        """
-        f = open(file_name, "w")
-
-        f.write(models[0].FITHEADERS)
-
-        for model in models:
-            if not model.fit_status:
-                continue
-            f.write('{: 8.6f}   {: 12.8E}   '.format(
-                model.fit_temperature, model.fitted_params[0])
-            )
-            f.write(
-                '{: 12.8E}   {: 12.8E}   '.format(
-                    model.log_normal_bounds(
-                        model.fitted_params[0], model.fitted_params[3], 1
-                    ),
-                    model.log_normal_bounds(
-                        model.fitted_params[0], model.fitted_params[3], -1
-                    )
-                )
-            )
-            f.write('{: 12.8E}'.format(model.perr[0]))
-            for j in range(1, len(model.fitted_params)):
-                f.write('   {: 12.8E}   {: 12.8E}'.format(
-                    model.fitted_params[j], model.perr[j]
-                ))
-            f.write('\n')
-
-        print("\nFit information has been written to {}\n".format(
-            file_name
-        ))
-
-        return
-
-
-class TwoMaximaModel(Model):
-
-    NAME: str = 'Two Maxima'
-
-    BOUNDS: tuple[list] = (
-        [0., 0., 0., 0., 0., 0., 0.],
-        [np.inf, np.inf, 1.0, np.inf, np.inf, 1.0, np.inf]
-    )
-
-    FITHEADERS: str = '  {:12} {:16} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17} {:17}\n'.format( # noqa.
-        'T', 'tau1', 'tau1_err', 'D_chi1', 'D_chi1_err', 'alpha1',
-        'alpha1_err', 'tau2', 'tau2_err', 'D_chi2', 'D_chi2_err', 'alpha2',
-        'alpha2_err', 'chi_total', 'chi_total_err'
-    )
+        dict[str, float]
+            Keys are fit/fix parameter names (see class.PARNAMES)
+            values are float (actual value) which are initial values of
+            parameter
+        '''
+
+        # Make copy, any str values will be replaced
+        new_param_dict = copy.copy(param_dict)
+
+        # Guesses
+        guessdict = {
+            'tau*1': 50.,
+            'tau*2': 5000.,
+            'm_eq': experiment.moments[-1],  # M_eq guess final measured moment
+            'm_0': experiment.moments[0],  # M_0 is first measured moment
+            'frac': 0.5,
+            'beta1': 0.95,
+            'beta2': 0.95,
+            't_offset': 0.
+        }
 
-    MODELHEADERS: str = '{:11} {:11} {:11}\n'.format(
-        "Wave Frequency (linear) (Hz)", "χ' (cm^{3}mol^{-1})",
-        "χ'' (cm^{3}mol^{-1})"
-    )
+        # Replace 'guess' with relevant guess
+        for var, val in param_dict.items():
+            if val == 'guess':
+                new_param_dict[var] = guessdict[var]
 
-    flat_thresh: float = 1E-06
-    initial_params: list = []
-    fitted_params: list = []
-    fit_status: bool = False
-    fit_temperature: float = np.nan
-    fit_dc_field: float = np.nan
-    perr: float = np.nan
+        return new_param_dict
 
     @staticmethod
-    def model(parameters: list[float],
-              ac_freq_ang: list[float]) -> tuple[list[float], list[float]]:
-        """
-        Computes model function of ac suceptibility for two maxima
+    def model(parameters: dict[str, float], time: list[float]) -> list[float]:
+        '''
+        Evaluates exponential model function of DC magnetisation decay
+        using provided parameter and time values.
 
         Parameters
         ----------
-        parameters: list[float]
-            parameters used in model function
-
-        ac_freq_ang: list[float]
-            angular ac frequencies at which model will be evaluated
+        parameters: dict[str, float]
+            Parameters to use in model function, keys are given in
+            ExponentialModel.PARNAMES
+        time: list[float]
+            time values in seconds at which model function is evaluated
 
         Returns
         -------
         list[float]
-            real susceptibility
-        list[float]
-            imaginary susceptibility
+            Moment as a function of time
 
-        """
-        tau1, delta_chi1, alpha1 = parameters[:3]
-        tau2, delta_chi2, alpha2, chi_total = parameters[3:]
+        '''
 
-        func = abs(chi_total)
-        func += abs(delta_chi1)/(1+np.power((ac_freq_ang*abs(tau1)*1j),(1.-abs(alpha1)))) # noqa
-        func += abs(delta_chi2)/(1+np.power((ac_freq_ang*abs(tau2)*1j),(1.-abs(alpha2)))) # noqa
-
-        return np.real(func), np.abs(np.imag(func))
-
-    @staticmethod
-    def discard(fit_param: list[float], ac_freq_ang: list[float]) -> bool:
-        """
-        Decides whether fits should be discarded based on following criteria
-
-        1. tau^-1 < smallest ac frequency
-
-        2. tau^-1 > largest ac frequency
-
-        where both tau_1 and tau_2 (corresponding to the two peaks) are
-        checked
+        m_eq = parameters['m_eq']
+        m_0 = parameters['m_0']
+        beta1 = parameters['beta1']
+        beta2 = parameters['beta2']
+        tau_star1 = parameters['tau*1']
+        tau_star2 = parameters['tau*2']
+        frac = parameters['frac']
+        t_offset = parameters['t_offset']
+
+        sef1 = np.exp(-((time - t_offset) / tau_star1)**beta1)
+        sef2 = np.exp(-((time - t_offset) / tau_star2)**beta2)
+        mom = m_eq + (m_0 - m_eq) * ((frac * sef1) + ((1 - frac) * sef2))
+
+        return mom
+
+    def calc_lntau_expect(self) -> float:
+        '''
+        Calculates expectation value of ln(tau)
 
         Parameters
         ----------
-        fit_param : list[float]
-            Fitted parameters tau, chi_S, chit_T, alpha
-        ac_freq_ang: list[float]
-            Angular ac frequencies
+        None
 
         Returns
         -------
-        bool
-            True if point should be discarded, else False
-        """
-        to_discard = False
-
-        if 1./(fit_param[0]) < np.min(ac_freq_ang):
-            to_discard = True
-        elif 1./(fit_param[3]) < np.min(ac_freq_ang):
-            to_discard = True
-        elif 1./(fit_param[0]) > np.max(ac_freq_ang):
-            to_discard = True
-        elif 1./(fit_param[3]) > np.max(ac_freq_ang):
-            to_discard = True
+        float
+            <ln(tau)> value in ln(seconds)
 
-        return to_discard
-
-    @staticmethod
-    def flat(ac_freq_ang: list[float], sus_im: list[float], threshold):
-        """
-        Calculates fit of data to y = mx+b to find if data is flat
-        If flat, the error of this fit will be very low
+        Raises
+        -----
+        ValueError
+            If required model parameters in self.final_var_values are undefined
+        '''
+
+        beta1 = self.final_var_values['beta1']
+        beta2 = self.final_var_values['beta2']
+        tau_star1 = self.final_var_values['tau*1']
+        tau_star2 = self.final_var_values['tau*2']
+
+        if None in [beta1, beta2, tau_star1, tau_star2]:
+            _error = 'Cannot calculate ln(tau) expectation value '
+            _error += 'beta and/or tau* are undefined!'
+            raise ValueError(_error)
+
+        lntau1 = (1 - (1 / beta1)) * np.euler_gamma + np.log(tau_star1)
+        lntau2 = (1 - (1 / beta2)) * np.euler_gamma + np.log(tau_star2)
+
+        return [lntau1, lntau2]
+
+    def calc_lntau_stdev(self) -> float:
+        '''
+        Calculates standard deviation of ln(tau1) and ln(tau2)
 
         Parameters
         ----------
-        ac_freq_ang : list[float]
-            Angular AC Frequency of each measurement
-        sus_im : list[float]
-            Imaginary component of susceptibility of each measurement
-        threshold : float
-            Threshold for data to be marked as flat
+        None
 
         Returns
         -------
-        bool
-            True if point is flat and should be discarded, else False
-        """
-
-        is_flat = False
-
-        linear_popt, _ = curve_fit(lambda a, x, b: a*x+b, ac_freq_ang, sus_im)
-        error = np.square(linear_popt[0]*ac_freq_ang + linear_popt[1] - sus_im)
-
-        if np.sqrt(np.sum(error)) < threshold:
-            is_flat = True
-
-        return is_flat
-
-    def initial_params_from_experiment(self, experiment: 'Experiment',
-                                       verbose: bool = False) -> None:
-        """
-        Generates initial guess of fitting parameters from experiment
-
-        Let x = largest frequency at turning point of imaginary susceptibility with largest abs value
-
-        Parameters and guesses are
-
-        tau_1 - inverse of frequency for turning point with 2nd largest imaginary susceptibility
-
-        D_chi_1 - 2/3 * range of real susceptibility
-
-        alpha_1 - 0.1
-
-        tau_2 - inverse of frequency for turning point with largest imaginary susceptibility
-
-        D_chi_2 - 1/3 * range of real susceptibility
-
-        alpha_2 - 0.01
+        float
+            Standard deviation of ln(tau) in ln(seconds)
 
-        chi_total - minimum real susceptibility
+        Raises
+        -----
+        ValueError
+            If required model parameters in self.final_var_values are undefined
+        '''
+
+        beta1 = self.final_var_values['beta1']
+        beta2 = self.final_var_values['beta2']
+
+        if None in [beta1, beta2]:
+            _error = 'Error: Cannot calculate ln(tau) standard deviation'
+            _error += 'beta undefined!'
+            raise ValueError(_error)
+
+        sd1 = np.sqrt((1. / beta1**2 - 1.) * np.pi**2 / 6.)
+        sd2 = np.sqrt((1. / beta2**2 - 1.) * np.pi**2 / 6.)
+
+        return [sd1, sd2]
+
+    def calc_lntau_fit_ul(self) -> list[float]:
+        '''
+        Calculates upper and lower bounds of ln(tau) from fit uncertainty
+        in fitted parameters
 
         Parameters
         ----------
-        experiment: Experiment
-            Experiment object whose data is used for initial guesses
-        verbose: bool, default False
-            If True, print initial guesses to screen
+        None
 
         Returns
         -------
-        None
-        """ # noqa
-
-        # Calculate gradient of imaginary susceptibility and retrieve indexes
-        # where there is a change of sign.
-        dsus_im = np.gradient(experiment.sus_im)
-        zero_crossings_freq = np.where(np.diff(np.sign(dsus_im)))
-
-        # Get frequency for turning point with largest imaginary
-        # susceptibility
-        sus_im_cross = experiment.sus_im[zero_crossings_freq]
-        indices = np.argsort(-sus_im_cross)
-        ac_freq_cross = experiment.ac_freq[zero_crossings_freq]
-        ac_freq_cross = [ac_freq_cross[ind] for ind in indices]
-
-        crossing_freq_largest = max(ac_freq_cross[:2])
-        crossing_freq_2nd_largest = min(ac_freq_cross[:2])
-
-        range_real = np.max(experiment.sus_re) - np.min(experiment.sus_re)
-        self.initial_params = [
-            1./(2.*np.pi*crossing_freq_2nd_largest),
-            2.*range_real/3.,
-            0.1,
-            1./(2.*np.pi*crossing_freq_largest),
-            range_real/3.,
-            0.01,
-            np.min(experiment.sus_re)
-        ]
-
-        if verbose:
-            print(
-                '\nThe initial guesses are',
-                '\ntau_1 = {}\ndelta_chi_1 = {}\nalpha_1 = {}\ntau_2 = {}\ndelta_chi_2 = {}\nalpha_2 = {}\nchi_total = {}'.format( # noqa
-                    *self.initial_params
-                )
-            )
+        list[float]
+            upper and lower bounds of ln(tau) from fit uncertainty in fitted
+            parameters (upper > lower)
+        '''
 
-        return
+        tau_star1 = self.final_var_values['tau*1']
 
-    @staticmethod
-    def write_fit_params(models: list[Model], file_name: str):
-        """
-        Writes fitted parameters of models to file
+        if 'tau*1' in self.fit_stdev:
+            tau_star1_std = self.fit_stdev['tau*1']
+        else:
+            tau_star1_std = 0.
 
-        Parameters
-        ----------
-        models : list[Model]
-            Models, one per temperature
-        file_name : str
-            Name of output file
+        beta1 = self.final_var_values['beta1']
 
-        Returns
-        -------
-        None
-        """
-        f = open(file_name, "w")
+        if 'beta1' in self.fit_stdev:
+            beta1_std = self.fit_stdev['beta1']
+        else:
+            beta1_std = 0.
 
-        f.write(models[0].FITHEADERS)
+        tau_star2 = self.final_var_values['tau*2']
 
-        for model in models:
-            if not model.fit_status:
-                continue
-            f.write('{: 8.6f}   '.format(model.fit_temperature))
-            for j in range(len(model.fitted_params)):
-                f.write('   {: 12.8E}   {: 12.8E}'.format(
-                    model.fitted_params[j], model.perr[j]
-                ))
-            f.write('\n')
+        if 'tau*2' in self.fit_stdev:
+            tau_star2_std = self.fit_stdev['tau*2']
+        else:
+            tau_star2_std = 0.
 
-        print("\nFit information has been written to {}\n".format(
-            file_name
-        ))
+        beta2 = self.final_var_values['beta2']
 
-        return
+        if 'beta2' in self.fit_stdev:
+            beta2_std = self.fit_stdev['beta2']
+        else:
+            beta2_std = 0.
 
+        warnings.filterwarnings('ignore', 'invalid value encountered in log')
 
-def find_mean_values(values: list[float], thresh: float = 0.1) -> tuple[
-        list[float], list[int]]:
-    """
-    Finds mean value from a list of values by locating
-    values for which step size is >= `thresh`
+        upper1 = (1 - (1 / (beta1 - beta1_std))) * np.euler_gamma + np.log(tau_star1 + tau_star1_std) # noqa
+        lower1 = (1 - (1 / (beta1 + beta1_std))) * np.euler_gamma + np.log(tau_star1 - tau_star1_std) # noqa
 
-    Returns list of same length with all values replaced by mean(s)
+        upper2 = (1 - (1 / (beta2 - beta2_std))) * np.euler_gamma + np.log(tau_star2 + tau_star2_std) # noqa
+        lower2 = (1 - (1 / (beta2 + beta2_std))) * np.euler_gamma + np.log(tau_star2 - tau_star2_std) # noqa
 
-    Parameters
-    ----------
-    values: list[float]
-        Values to look at
-    thresh: float, default 0.1
-        Threshold used to discriminate between values
+        warnings.filterwarnings('default', 'invalid value encountered in log')
 
-    Returns
-    -------
-    list[float]
-        Mean values
-    list[int]
-        indices of original list at which value changes by more than
-        0.1
-    """
-
-    # Find values for which step size is >= thresh
-    mask = np.abs(np.diff(values)) >= thresh
-    # and mark indices at which to split
-    split_indices = np.where(mask)[0]
-
-    # For values with similar step size, record mean temperature
-    means = [
-        [np.mean(grp)]*grp.size
-        for grp in np.split(values, split_indices + 1)
-    ]
+        ul1 = sorted([upper1, lower1], reverse=True)
+        ul2 = sorted([upper2, lower2], reverse=True)
 
-    return means, split_indices
+        return [ul1, ul2]
 
 
-class Measurement():
-    """
-    Stores data for a single AC Susceptibility measurement at a
-    given temperature, given applied dc field, and given ac frequency
+def write_model_params(models: list[Model], file_name: str,
+                       verbose: bool = True) -> None:
+    '''
+    Writes fitted parameters of a set of models to file.\n
+    Assumes models are all of the same type, e.g. all Exponential
 
     Parameters
     ----------
-    dc_field : float
-        Applied dc field
-    temperature : float
-        Temperature of experiment
-    sus_re : float
-        real part of susceptibility
-    sus_im : float
-        imaginary part of susceptibility
-    ac_freq : float
-        linear ac frequency of experiment
-    ac_field : float
-        ac field
-
-    Attributes
-    ----------
-    dc_field : float
-        Applied dc field
-    temperature : float
-        Temperature of experiment
-    ac_freq : float
-        linear ac frequency of experiment
-    sus_re : float
-        real part of susceptibility
-    sus_im : float
-        imaginary part of susceptibility
-    ac_field : float
-        ac field
-    mean_temperature : float
-        Mean or representative temperature assigned to this experiment
-    mean_dc_field : float
-        Mean or representative dc field assigned to this experiment
-    """
+    models : list[Model]
+        Models, one per temperature, must all be same type
+    file_name : str
+        Name of output file
+    verbose: bool, default True
+        If True, file location is printed to terminal
 
-    def __init__(self, dc_field, temperature, sus_re,
-                 sus_im, ac_freq, ac_field):
-
-        self.dc_field = dc_field
-        self.temperature = temperature
-        self.sus_re = sus_re
-        self.sus_im = sus_im
-        self.ac_freq = ac_freq
-        self.ac_field = ac_field
-
-        self.mean_temperature = None
-        self._mean_dc_field = None
-
-        return
-
-    def convert_susc(self, in_susc_units, mw, mass):
-        """
-        Converts imaginary and real susceptibilities from input units to
-        cm3 mol-1
-
-        Parameters
-        ----------
-        in_susc_units : str
-            {"emu/Oe", "emu"}
-        mw : float
-            Molecular weight
-        mass : float
-            sample mass
-        """
-
-        if in_susc_units == "emu/Oe":
-            self.sus_re *= mw/(mass/1000.)
-            self.sus_im *= mw/(mass/1000.)
-        elif in_susc_units == "emu":
-            self.sus_re *= mw/(self.ac_field*mass/1000.)
-            self.sus_im *= mw/(self.ac_field*mass/1000.)
-        return
-
-    @property
-    def mean_temperature(self):
-        return self._mean_temperature
+    Returns
+    -------
+    None
+    '''
 
-    @mean_temperature.setter
-    def mean_temperature(self, value: float):
-        self._mean_temperature = value
-        return
+    f = open(file_name, 'w', encoding='utf-8')
 
-    @property
-    def mean_dc_field(self):
-        return self._mean_dc_field
+    f.write(' {:^12} '.format('T'))
+    f.write('{:^12} '.format('H'))
 
-    @mean_dc_field.setter
-    def mean_dc_field(self, value: float):
-        self._mean_dc_field = value
-        return
+    if all([model.dc_field != model.meas_dc_field for model in models]):
+        f.write('{:^12} '.format('H_measured'))
 
-    @staticmethod
-    def check_pos_sus(s):
-        try:
-            s = float(s.strip())
-            if s < 0.:
-                s = np.NaN
-                # print("Negative susceptibility, skipping")
-        except TypeError:
-            s = np.NaN
-
-        return s
+    # Fitted parameters
+    for name in models[0].fit_vars.keys():
+        f.write('{:^17} {:^17} '.format(name, name + '-s-dev'))
 
-    @classmethod
-    def from_file(cls, file: str, header_indices: dict,
-                  data_line: int) -> list['Measurement']:
-        """
-        Extracts ac susceptibility from magnetometer output file and
-        returns list of experiments, one for each valid measurment
-        Incomplete lines and negative values of susceptibility are ignored
+    # Fixed parameters
+    for name in models[0].fix_vars.keys():
+        f.write('{:^17} '.format(name))
 
-        Parameters
-        ----------
-        file : str
-            Name of magnetometer output file
-        header_indices : dict
-            Keys are generic header names given in `HEADERS_GENERIC`
-            Values are column index of header in file
-        data_line: int
-            Line which specifies the beginning of the data block in input file
-
-        Returns
-        -------
-        list
-            Measurement objects, one per temperature, per field
-            List has the same order as the magnetometer file
-        """
-
-        # Columns to extract from file
-        cols = [header_indices[gen] for gen in HEADERS_GENERIC]
+    if all({isinstance(model, DoubleExponentialModel) for model in models}):
+        model_type = DoubleExponentialModel
+    else:
+        model_type = None
 
-        # Convert strings to floats, if not possible then mark as NaN
-        converters = {
-            it: lambda s: (float(s.strip() or np.NaN)) for it in cols
-        }
+    if model_type == DoubleExponentialModel:
+        f.write('{:^17} '.format('<ln(tau1)>'))
+        f.write('{:^17} '.format('sigma_ln(tau1)'))
+        f.write('{:^17} '.format('fit_upper_ln(tau1)'))
+        f.write('{:^17} '.format('fit_lower_ln(tau1)'))
+        f.write('{:^17} '.format('<ln(tau2)>'))
+        f.write('{:^17} '.format('sigma_ln(tau2)'))
+        f.write('{:^17} '.format('fit_upper_ln(tau2)'))
+        f.write('{:^17} '.format('fit_lower_ln(tau2)'))
+    else:
+        f.write('{:^17} '.format('<ln(tau)>'))
+        f.write('{:^17} '.format('sigma_ln(tau)'))
+        f.write('{:^17} '.format('fit_upper_ln(tau)'))
+        f.write('{:^17} '.format('fit_lower_ln(tau)'))
+
+    f.write('\n')
+
+    for model in models:
+        if not model.fit_status:
+            continue
+
+        f.write('{:12.10f} '.format(model.temperature))
+        f.write('{:12.10f} '.format(model.dc_field))
+
+        if model.dc_field != model.meas_dc_field:
+            f.write('{:12.10f} '.format(model.meas_dc_field))
+
+        for name in model.fit_vars.keys():
+            f.write('{: 1.10E} {: 1.10E} '.format(
+                model.final_var_values[name], model.fit_stdev[name]
+            ))
 
-        # Check for positive susceptibility
-        converters[header_indices['sus_real']] = cls.check_pos_sus
-        converters[header_indices['sus_imaginary']] = cls.check_pos_sus
+        for value in model.fix_vars.values():
+            f.write('{: 1.10E} '.format(value))
 
-        # Read required columns of file
-        data = np.loadtxt(
-            file,
-            skiprows=data_line+1,
-            delimiter=',',
-            converters=converters,
-            usecols=cols
+        if model_type == DoubleExponentialModel:
+            f.write('{: 1.10E} '.format(model.lntau_expect[0]))
+            f.write('{: 1.10E} '.format(model.lntau_stdev[0]))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[0][0]))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[0][1]))
+            f.write('{: 1.10E} '.format(model.lntau_expect[1]))
+            f.write('{: 1.10E} '.format(model.lntau_stdev[1]))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[1][0]))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[1][1]))
+        else:
+            f.write('{: 1.10E} '.format(model.lntau_expect))
+            f.write('{: 1.10E} '.format(model.lntau_stdev))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[0]))
+            f.write('{: 1.10E} '.format(model.lntau_fit_ul[1]))
+
+        f.write('\n')
+
+    if verbose:
+        ut.cprint(
+            f'\n Model parameters written to \n {file_name}\n',
+            'cyan'
         )
-
-        # Convert array of floats into list of Measurement objects, one per
-        # line
-        # Check for missing entries which have been marked as NaN
-        # and skip if found
-        measurements = [
-            cls(*row)
-            for row in data
-            if not any(isnan(val) for val in row)
-        ]
-
-        return measurements
+    return
 
 
-class Experiment():
-    """
-    Stores data for multiple AC Susceptibility measurements at a
-    given temperature, given applied dc field, and multiple ac frequencies
+def write_model_data(experiments: list['Experiment'],
+                     models: list['Model'], file_name: str,
+                     verbose: bool = True) -> None:
+    '''
+    Creates file containing time, and moment using the model
+    function with fitted and fixed parameters.
+    Temperatures for which a fit was not possible are not included.
 
     Parameters
     ----------
-    temperature: float
-        Temperature of experiment
-    sus_re : list
-        real part of susceptibility
-    sus_im : list
-        imaginary part of susceptibility
-    ac_freq : list
-        linear ac frequency of experiment
-    dc_field : float
-        Applied dc field strength in Oe
-
-    Attributes
-    ----------
-    temperatures: list
-        Temperature of experiment
-    sus_re : list
-        real part of susceptibility
-    sus_im : list
-        imaginary part of susceptibility
-    ac_freq : list
-        linear ac frequency of experiment
-    dc_field : float
-        Applied dc field strength in Oe
-    """
-
-    def __init__(self, temperatures, raw_temperatures, sus_re, sus_im,
-                 ac_freq, dc_field):
-
-        self.temperatures = temperatures
-        self.raw_temperatures = raw_temperatures
-        self.sus_re = sus_re
-        self.sus_im = sus_im
-        self.ac_freq = ac_freq
-        self.dc_field = dc_field
-
-        return
-
-    @classmethod
-    def from_measurements(cls,
-                          measurements: list[Measurement],
-                          temp_thresh: float = 0.1,
-                          field_thresh: float = 1) -> list[list['Experiment']]: # noqa
-        """
-        Creates list of Experiment objects from a list of individual
-        Measurement objects. Experiments are defined as a set of measurements
-        with the same temperature and DC field strength
-
-        Parameters
-        ----------
-        measurement: list[Measurement]
-            Measurements at various temperatures and DC fields
-        temp_thresh: float, default 0.1 K
-            Threshold used to discriminate between temperatures
-        field_thresh: float, default 1 Oe
-            Threshold used to discriminate between dc field values
-
-        Returns
-        -------
-        list[list[Experiment]]
-            Each element is a list of Experiments at the same DC field
-            sorted low to high DC field strength
-
-            Within each sublist the elements are single experiments
-            which are each a set of measurements with the same temperature
-            and DC field strength
+    experiments : list[Experiment]
+        List of experiments to which a model was fitted
+    models : list[Model]
+        List of models, one per experiment
+    file_name: str
+        Name of output file
+    verbose: bool, default True
+        If True, file location is printed to terminal
 
-            The sublists are sorted low to high mean temperature.
-        """ # noqa
+    Returns
+    -------
+    None
+    '''
 
-        # Sort measurements by dc field then temperature
-        measurements.sort(key=lambda k: (k.dc_field, k.temperature))
+    f = open(file_name, 'w', encoding='utf-8')
 
-        mean_fields, split_ind = find_mean_values(
-            [
-                measurement.dc_field
-                for measurement in measurements
-            ],
-            thresh=field_thresh
+    # For each experiment and its corresponding model, calculate
+    # moment at experimental time values
+    for model, experiment in zip(models, experiments):
+
+        moments = model.model(
+            model.final_var_values,
+            experiment.times,
         )
 
-        # Set each measurement's "mean", or representative field
-        for measurement, mean_field in zip(measurements, np.concatenate(mean_fields)): # noqa
-            measurement.mean_dc_field = mean_field
+        f.write('{:11} {:.5f} K\n'.format('T = ', model.temperature))
+        f.write('{:11} {:.5f} Oe\n'.format('H = ', model.dc_field))
 
-        # Re-sort using mean dc field
-        measurements.sort(key=lambda k: (k.mean_dc_field, k.temperature))
+        f.write('{:^15} {:^15}\n'.format(
+            'Time (s)', 'Moment (emu)'
+        ))
+        for t, mo in zip(experiment.times, moments):
+            f.write('{: 1.8E} {: 1.8E}\n'.format(t, mo))
 
-        # And split based on changing dc field values
-        measurements: list[list[Measurement]] = np.split(
-            measurements, split_ind + 1
+    if verbose:
+        ut.cprint(
+            f'\n Model decays written to \n {file_name}\n',
+            'cyan'
         )
+    return
 
-        # Back to list...
-        measurements = [measurements.tolist() for measurements in measurements]
-
-        experiments = []
 
-        for sf_measurments in measurements:
-
-            mean_temps, split_ind = find_mean_values(
-                [
-                    measurement.temperature
-                    for measurement in sf_measurments
-                ],
-                thresh=temp_thresh
-            )
+def plot_decays_and_fields(experiments: list[Experiment], show: bool = True,
+                           save: bool = False,
+                           save_name: str = 'decays_and_fields.png',
+                           x_scale: str = 'linear', y_scale: str = 'linear',
+                           verbose: bool = True) -> tuple[plt.Figure, list[plt.Axes]]: # noqa:
+    '''
+    Plots a list of experimental decays as moment vs time and field vs time,
+    on one figure with two plots.
 
-            # Set each measurement's "mean", or representative temperature
-            for measurement, mean_temp in zip(sf_measurments, np.concatenate(mean_temps)): # noqa
-                measurement.mean_temperature = mean_temp
-
-            # sort measurements by ac frequency
-            sf_measurments.sort(
-                key=lambda k: (k.mean_temperature, k.ac_freq)
-            )
-
-            raw_temperatures = [
-                measurement.temperature
-                for measurement in sf_measurments
-            ]
-
-            raw_temperatures = np.split(
-                raw_temperatures,
-                split_ind + 1
-            )
-
-            sus_res = np.split(
-                [
-                    measurement.sus_re
-                    for measurement in sf_measurments
-                ],
-                split_ind + 1
-            )
-
-            sus_ims = np.split(
-                [
-                    measurement.sus_im
-                    for measurement in sf_measurments
-                ],
-                split_ind + 1
-            )
-
-            ac_freqs = np.split(
-                [
-                    measurement.ac_freq
-                    for measurement in sf_measurments
-                ],
-                split_ind + 1
-            )
-
-            dc_fields = np.split(
-                [
-                    measurement.dc_field
-                    for measurement in sf_measurments
-                ],
-                split_ind + 1
-            )
-
-            experiments.append([
-                cls(
-                    mean_temp, raw_temp, sus_re, sus_im, ac_freq,
-                    dc_field[0]
-                )
-                for (
-                        mean_temp, raw_temp, sus_re, sus_im, ac_freq,
-                        dc_field
-                    ) in zip(
-                        mean_temps, raw_temperatures, sus_res,
-                        sus_ims, ac_freqs, dc_fields
-                    )
-            ])
-
-        return experiments
-
-    @staticmethod
-    def plot_susceptibility(experiments: list['Experiment'],
-                            save_dir: str = "", file_head: str = "",
-                            save: bool = True) -> None:
-        """
-
-        Creates plot of in- and out-of-phase raw susceptibilities as matplotlib
-        figure
-
-        Parameters
-        ----------
-        experiments : list[Experiment]
-            List of experiments to which a model was successfully fitted
-        save_dir: str
-            Path to save directory
-        file_head: str
-            text added to head of file name
-        save: bool, default True
-            If True, saves plot to file
-
-        Returns
-        -------
-        None
-        """
-
-        fig, (ax1, ax2) = plt.subplots(
-            2,
-            1,
-            sharex='none',
-            sharey='none',
-            figsize=(7., 4.5),
-            num='Raw AC susceptibility'
-        )  # 8.27, 11.69 A4
-        fig.subplots_adjust(hspace=.5, wspace=.02)
-
-        cmap = cm.get_cmap("tab20")
-
-        # Experimental data
-        for eit, experiment in enumerate(experiments):
-
-            # Real
-            ax1.semilogx(
-                experiment.ac_freq,
-                experiment.sus_re,
-                '-o',
-                markersize=4,
-                fillstyle='none',
-                label='{:.2f} K'.format(experiment.temperatures[0]),
-                color=cmap.colors[eit]
-            )
-            # Imaginary
-            ax2.semilogx(
-                experiment.ac_freq,
-                experiment.sus_im,
-                '-o',
-                markersize=4,
-                fillstyle='none',
-                color=cmap.colors[eit]
-            )
-
-        ax2.get_shared_x_axes().join(ax1, ax2)
+    Parameters
+    ----------
+    experiment: list[Experiment]
+        Experiments to plot
+    show: bool, default True
+        If True, shows plot on screen
+    save: bool, default False
+        If True, saves plot to file
+    save_name : str, default 'decays_and_fields.png'
+        If save is True, saves plot to this file name
+    x_scale : str {'linear', 'log'}
+        Scale of x-axis
+    y_scale : str {'linear', 'log'}
+        Scale of y-axis
+    verbose: bool, default True
+        If True, plot file location is written to terminal
 
-        ax1.set_xticklabels([])
-        ax1.set_ylabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        # Get rid of the frames of susceptibility plots
-        for axis in [ax1, ax2]:
-            axis.spines["top"].set_visible(False)
-            axis.spines["right"].set_visible(False)
-
-        # Get rid of the x-labels of real susceptibility
-        ax1.set_xticklabels([])
-        ax1.set_ylabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        ax2.set_xlabel('Wave Frequency (Hz)')
-        ax2.set_ylabel(r'$\chi^{,,}$ (cm$^{3}$mol$^{-1}$)')
-
-        fig.legend(
-            frameon=False,
-            loc=7
+    Returns
+    -------
+    plt.Figure
+        Matplotlib figure object
+    list[plt.Axes]
+        List of Matplotlib axis objects
+    '''
+
+    fig, (ax1, ax2) = plt.subplots(1, 2, sharex=True, figsize=(10, 5))
+    for experiment in experiments:
+
+        experiment.times -= np.min(experiment.times)
+        ax1.plot(
+            experiment.times,
+            experiment.moments,
+            lw=2,
+            marker='x',
+            label='{:.2f} K'.format(experiment.rep_temperature)
+        )
+        ax2.plot(
+            experiment.times,
+            experiment.dc_fields,
+            lw=2,
+            marker='x',
+            label='{:.2f} K'.format(experiment.rep_temperature)
         )
 
-        fig.tight_layout(rect=[0, 0, 0.85, 1])
-
-        if save:
-
-            if len(file_head):
-                file_head = "{}_".format(file_head)
+    ax1.set_xlabel('Time (s)')
+    ax1.set_ylabel('Moment (emu)')
+    ax2.set_xlabel('Time (s)')
+    ax2.set_ylabel('DC Field (Oe)')
+
+    if len(np.unique([e.rep_temperature for e in experiments])) > 1:
+        ax1.legend()
+        ax2.legend()
+    else:
+        fig.suptitle(
+            'T = {:.2f} K'.format(
+                experiments[0].rep_temperature
+            ),
+            fontsize='medium'
+        )
 
-            f_name = "{}sus_components_{:f}Oe.png".format(
-                file_head,
-                experiments[0].dc_field
-            )
+    ax1.set_xscale(x_scale)
+    ax1.set_yscale(y_scale)
 
-            f_name = os.path.join(save_dir, f_name)
+    if y_scale == 'linear':
+        ax1.yaxis.set_minor_locator(AutoMinorLocator())
+    if x_scale == 'linear':
+        ax1.xaxis.set_minor_locator(AutoMinorLocator())
 
-            fig.savefig(f_name, dpi=400)
+    ax2.xaxis.set_minor_locator(AutoMinorLocator())
+    ax2.yaxis.set_minor_locator(AutoMinorLocator())
 
-            print("\nSusceptibility plot saved to")
-            print("{}".format(f_name))
+    fig.tight_layout()
 
+    if save:
+        plt.savefig(save_name, dpi=500)
+        if verbose:
+            ut.cprint(
+                f'\n Decay plot saved to \n {save_name}\n',
+                'cyan'
+            )
+    if show:
         plt.show()
 
-        return
+    plt.close('all')
 
-    @staticmethod
-    def plot_colecole(experiments: list['Experiment'], save_dir: str = "",
-                      file_head: str = "", save: bool = True) -> None:
-        """
-        Creates Cole-Cole plot as matplotlib figure
+    return fig, [ax1, ax2]
 
-        Parameters
-        ----------
-        experiments : list[Experiment]
-            List of experiments to which a model was successfully fitted
-        save_dir: str
-            Path to save directory
-        file_head: str
-            text added to head of file name
-        save: bool, default True
-            If true, saves plot to file as png
-        Returns
-        -------
-        None
-        """
-
-        fig, ax1 = plt.subplots(
-            1,
-            1,
-            sharex='none',
-            sharey='none',
-            figsize=(7.1, 4.8),
-            num='Raw Cole-Cole'
-        )
-        fig.subplots_adjust(hspace=.02, wspace=.02)
-
-        cmap = cm.get_cmap("tab20")
 
-        # Experimental data
-        for eit, experiment in enumerate(experiments):
+def plot_decays(experiments: list[Experiment], show: bool = True,
+                save: bool = False, save_name: str = 'decays.png',
+                x_scale: str = 'linear', y_scale: str = 'linear',
+                verbose: bool = True) -> tuple[plt.Figure, plt.Axes]:
+    '''
+    Plots a list of experimental decays (moment vs time) on one plot.
 
-            # Plot Cole-Cole
-            ax1.plot(
-                experiment.sus_re,
-                experiment.sus_im,
-                '-o',
-                markersize=4,
-                fillstyle='none',
-                label="{:.2f} K".format(experiment.temperatures[0]),
-                color=cmap.colors[eit]
-            )
+    Parameters
+    ----------
+    experiment: list[Experiment]
+        Experiments to plot
+    show: bool, default True
+        If True, shows plot on screen
+    save: bool, default False
+        If True, saves plot to file
+    save_name : str, default 'decays.png'
+        If save is True, saves plot to this file name
+    x_scale : str {'linear', 'log'}
+        Scale of x-axis
+    y_scale : str {'linear', 'log'}
+        Scale of y-axis
+    verbose: bool, default True
+        If True, plot file location is written to terminal
 
-        fig.legend(
-            frameon=False,
-            loc=7
+    Returns
+    -------
+    plt.Figure
+        Matplotlib figure object
+    plt.Axes
+        Matplotlib axis object
+    '''
+
+    fig, ax = plt.subplots(1, 1, figsize=(6, 5))
+    for experiment in experiments:
+
+        experiment.times -= np.min(experiment.times)
+        ax.plot(
+            experiment.times,
+            experiment.moments,
+            lw=2,
+            marker='x',
+            label='{:.2f} K'.format(experiment.rep_temperature)
         )
 
-        # Remove frames
-        ax1.spines["top"].set_visible(False)
-        ax1.spines["right"].set_visible(False)
+    ax.set_xlabel('Time (s)')
+    ax.set_ylabel('Moment (emu)')
 
-        # Set labels for the axes
-        ax1.set_xlabel(r'$\chi^{,}$  (cm$^{3}$mol$^{-1}$)')
-        ax1.set_ylabel(r'$\chi^{,,}$ (cm$^{3}$mol$^{-1}$)')
+    if len(np.unique([e.rep_temperature for e in experiments])) > 1:
+        ax.legend()
+    else:
+        fig.suptitle(
+            'T = {:.2f} K'.format(
+                experiments[0].rep_temperature
+            ),
+            fontsize='medium'
+        )
 
-        fig.tight_layout(rect=[0, 0, 0.85, 1])
+    if y_scale == 'linear':
+        ax.yaxis.set_minor_locator(AutoMinorLocator())
+    if x_scale == 'linear':
+        ax.xaxis.set_minor_locator(AutoMinorLocator())
 
-        if save:
+    ax.set_xscale(x_scale)
 
-            if len(file_head):
-                file_head = "{}_".format(file_head)
+    fig.tight_layout()
 
-            f_name = "{}Cole_Cole_{:f}Oe.png".format(
-                file_head,
-                experiments[0].dc_field
+    if save:
+        plt.savefig(save_name, dpi=500)
+        if verbose:
+            ut.cprint(
+                f'\n Decay plot saved to \n {save_name}\n',
+                'cyan'
             )
-
-            f_name = os.path.join(save_dir, f_name)
-
-            fig.savefig(f_name, dpi=300)
-            print("\nCole-Cole plot saved to")
-            print("{}".format(f_name))
-
+    if show:
         plt.show()
-        plt.close('all')
 
-        return
+    plt.close('all')
 
+    return fig, ax
 
-class Dataset():
-    """
-    Stores data for multiple AC Susceptibility measurements at a
-    given temperature, given applied dc field, and multiple ac frequencies
 
-    Parameters
-    ----------
-    temperatures: list
-        Temperature of experiment
-    sus_re : list
-        real part of susceptibility
-    sus_im : list
-        imaginary part of susceptibility
-    ac_freq : list
-        linear ac frequency of experiment
-    dc_field : float
-        Applied dc field strength in Oe
+def plot_decay(experiment: Experiment, show: bool = True,
+               save: bool = False, save_name: str = 'decay.png',
+               x_scale: str = 'linear', y_scale: str = 'linear',
+               verbose: bool = True) -> tuple[plt.Figure, plt.Axes]:
+    '''
+    Plots an experimental decay (moment vs time) on one plot.
 
-    Attributes
+    Parameters
     ----------
-    temperatures: list
-        Temperature of experiment
-    sus_re : list
-        real part of susceptibility
-    sus_im : list
-        imaginary part of susceptibility
-    ac_freq : list
-        linear ac frequency of experiment
-    dc_field : float
-        Applied dc field strength in Oe
-    """
-
-    def __init__(self, temperatures, raw_temperatures, sus_re, sus_im,
-                 ac_freq, dc_field):
+    experiment: Experiment
+        Experiment to plot
+    show: bool, default True
+        If True, shows plot on screen
+    save: bool, default False
+        If True, saves plot to file
+    save_name : str, default 'decay.png'
+        If save is True, saves plot to this file name
+    x_scale : str {'linear', 'log'}
+        Scale of x-axis
+    y_scale : str {'linear', 'log'}
+        Scale of y-axis
+    verbose: bool, default True
+        If True, plot file location is written to terminal
 
-        self.temperatures = temperatures
-        self.raw_temperatures = raw_temperatures
-        self.sus_re = sus_re
-        self.sus_im = sus_im
-        self.ac_freq = ac_freq
-        self.dc_field = dc_field
-        self.n_experiments = np.size(self.temperatures)
-        return
+    Returns
+    -------
+    plt.Figure
+        Matplotlib figure object
+    plt.Axes
+        Matplotlib axis object
+    '''
+
+    fig, ax = plt.subplots(1, 1, figsize=(6, 5))
+    experiment.times -= np.min(experiment.times)
+    ax.plot(
+        experiment.times,
+        experiment.moments,
+        lw=2,
+        marker='x',
+        label='{:.2f} K'.format(experiment.rep_temperature)
+    )
 
-    @classmethod
-    def from_experiments(cls,
-                         experiments: list[Experiment]) -> list['Dataset']:
+    ax.set_xlabel('Time (s)')
+    ax.set_ylabel('Moment (emu)')
 
-        # Get indices at which dc field strength changes
-        _, field_switch_ind = np.unique(
-            [exp.dc_field for exp in experiments],
-            return_index=True
-        )
-        field_switch_ind = np.append(field_switch_ind, None)
+    if y_scale == 'linear':
+        ax.yaxis.set_minor_locator(AutoMinorLocator())
+    if x_scale == 'linear':
+        ax.xaxis.set_minor_locator(AutoMinorLocator())
 
-        # # Partition data based on dc field, then calculate average
-        # temperatures which fall within some similarity window
-        # Window is +- 0.1 K
-        datasets = []
-        for sw_it in range(1, len(field_switch_ind)):
-            start = field_switch_ind[sw_it-1]
-            end = field_switch_ind[sw_it]
-
-            current_experiments = experiments[start:end]
-
-            mean_temps = [
-                experiment.temperatures
-                for experiment in current_experiments
-            ]
+    ax.set_xscale(x_scale)
 
-            raw_temps = [
-                experiment.raw_temperatures
-                for experiment in current_experiments
-            ]
+    fig.tight_layout()
 
-            datasets.append(
-                cls(
-                    mean_temps,
-                    raw_temps,
-                    [
-                        experiment.sus_re
-                        for experiment in current_experiments
-                    ],
-                    [
-                        experiment.sus_im
-                        for experiment in current_experiments
-                    ],
-                    [
-                        experiment.ac_freq
-                        for experiment in current_experiments
-                    ],
-                    current_experiments[0].dc_field
-                )
+    if save:
+        plt.savefig(save_name, dpi=500)
+        if verbose:
+            ut.cprint(
+                f'\n Decay plot saved to \n {save_name}\n',
+                'cyan'
             )
+    if show:
+        plt.show()
+
+    plt.close('all')
 
-        return datasets
+    return fig, ax
 
 
-def interactive_t_select(experiments: list[Experiment]):
-    """
-    Creates interactive figure which allows user to select which temperatures
-    they would like to fit by clicking on the plots, and then returns a new
-    list of experiments.
+def plot_fitted_decay(experiment: Experiment, model: Model,
+                      show: bool = True, save: bool = False,
+                      save_name: str = 'fitted_decay.png',
+                      show_params: bool = True,
+                      x_scale: str = 'linear', y_scale: str = 'linear',
+                      verbose: bool = True) -> tuple[plt.Figure, plt.Axes]:
+    '''
+    Plots experimental and fitted (model) decay together (moment vs time),
+    displays on screen.
 
     Parameters
     ----------
-        experiments: list[Experiment]
-            Experiments, ordered  low to high temperature
+    experiment: Experiment
+        Experiment to plot
+    model: Model
+        Model (fitted) to plot
+    show: bool, default True
+        If True, shows plot on screen
+    save: bool, default False
+        If True, saves plot to file
+    save_name : str, default 'fitted_decay.png'
+        If save is True, saves plot to this file name
+    show_params: bool, default True
+        If True, shows fitted parameters on decay plots
+    x_scale : str {'linear', 'log'}
+        Scale of x-axis
+    y_scale : str {'linear', 'log'}
+        Scale of y-axis
+    verbose: bool, default True
+        If True, plot file location is written to terminal
 
     Returns
     -------
-        list[Experiment]
-            Same as before, with user-specified entries removed
-    """
-
-    unique_temps = np.unique(
-        [experiment.temperatures[0] for experiment in experiments]
-    )
+    plt.Figure
+        Matplotlib figure object
+    plt.Axes
+        Matplotlib axis object
+    '''
 
-    n_temps = unique_temps.size
-
-    if n_temps == 1:
-        n_cols = 1
-    elif n_temps < 5:
-        n_cols = 2
-    elif n_temps < 10:
-        n_cols = 3
-    elif n_temps < 17:
-        n_cols = 4
+    if show_params:
+        figsize = (4.5, 5)
     else:
-        n_cols = 5
-
-    n_rows = int(np.ceil(n_temps/n_cols))
+        figsize = (4.5, 4)
 
-    figsize = 7./3. * n_rows
-    if figsize > 7:
-        figsize = 7
-
-    # Show each data set individually for identification of peaks
-    fig, axs = plt.subplots(
-        n_rows,
-        n_cols,
-        sharex='none',
-        sharey='none',
-        figsize=(figsize, figsize),
-        num="Select temperatures to fit",
+    # Plot the figure.
+    fig, ax = plt.subplots(
+        1,
+        1,
+        sharex=True,
+        sharey=True,
+        figsize=figsize,
+        num='Fitted DC Decay at {:6.2f} K and {:6.2f} Oe'.format(
+            experiment.rep_temperature, experiment.dc_fields[-1]
+        )
     )
 
-    axs = axs.ravel()
+    expression = ''
 
-    suptitle = r'$\chi^{{,,}}$ vs wave frequency under {:2.1f} Oe field'.format( # noqa
-        experiments[0].dc_field
+    for name in model.PARNAMES:
+        if np.abs(model.final_var_values[name]) > 1E-8:
+            # Meq format as x.yz x 10^a
+            if name == 'm_eq':
+                # Convert to scientific string, then split at E
+                # to get mantissa and exponent separately
+                _tmp = f'{model.final_var_values[name]:.4E}'
+                _tmp = _tmp.split('E')
+                _mant = float(_tmp[0])
+                _exp = int(_tmp[1])
+                expression += f'{model.VARNAMES_MM[name]} = {_mant:.4f}'
+                expression += r' $\times \ \mathregular{10}'
+                expression += r'^\mathregular{{{:d}}}$'.format(_exp)
+                if 'm_eq' in model.fit_vars.keys():
+                    expression += r' $\pm$'
+                    _tmp = f'{model.fit_stdev[name]:.4E}'
+                    _tmp = _tmp.split('E')
+                    _mant = float(_tmp[0])
+                    _exp = int(_tmp[1])
+                    expression += f' {_mant:.4f}'
+                    expression += r' $\times \ \mathregular{10}'
+                    expression += r'^\mathregular{{{:d}}}$'.format(_exp)
+            else:
+                # All others format as float
+                expression += '{} = {:.4f} '.format(
+                    model.VARNAMES_MM[name],
+                    model.final_var_values[name],
+                )
+                if name in model.fit_vars.keys():
+                    expression += r'$\pm$'
+                    expression += ' {:.4f}'.format(model.fit_stdev[name])
+            expression += f' {model.UNITS_MM[name]} '
+            expression += '\n'
+
+    if show_params:
+        ax.text(0.0, 1.02, s=expression, fontsize=10, transform=ax.transAxes)
+
+    label_fit = 'Fit'
+
+    ax.plot(
+        experiment.times,
+        experiment.moments,
+        lw=0,
+        marker='o',
+        fillstyle='none',
+        label='Experiment'
     )
-
-    suptitle += "\n Select (click) the temperatures to fit (green)"
-    suptitle += "\n then close this window."
-
-    fig.subplots_adjust(hspace=.4, wspace=.08)
-    plt.suptitle(suptitle, fontsize=11)
-
-    for experiment, ax in zip(experiments, axs):
-        ax.semilogx(
-            experiment.ac_freq,
-            experiment.sus_im,
-            marker='o',
-            markeredgewidth=1,
-            markeredgecolor='b',
-            markerfacecolor='w',
-            markersize=5,
-            c='b',
-            lw=.5
-        )
-        ax.set_yticklabels([])
-        ax.set_yticks([])
-        ax.set_xticklabels([])
-        ax.set_xticks([])
-
-        ax.set_xlabel("{:.2f} K".format(experiment.temperatures[0]))
-
-        ax.set_box_aspect(aspect=1)
-
-    # Remove empty axes
-    for _ in range(len(axs)-n_temps):
-        fig.delaxes(axs[-1])
-        axs = np.delete(axs, -1)
-
-    for ax in axs:
-        ax.set_facecolor("White")
-
-    fig.tight_layout()
-
-    # Store object, one per temperature
-    stores = [Toggle(temp) for temp in unique_temps]
-
-    def onclick(event, axs_to_store):
-        """
-        Callback for mouse click.
-        If an axis is clicked, then switch the corresponding store
-        object and the axis' color
-        """
-        if event.inaxes is not None:
-            axs_to_store[event.inaxes].switch(event.inaxes)
-        return
-
-    axs_to_store = {
-        ax: store
-        for ax, store in zip(axs, stores)
-    }
-
-    # Connect mouse click to callback
-    cid = fig.canvas.mpl_connect(
-        'button_press_event',
-        lambda event: onclick(event, axs_to_store)
+    ax.plot(
+        experiment.times,
+        model.model(
+            model.final_var_values,
+            experiment.times,
+        ),
+        lw=1.5,
+        label=label_fit
     )
 
-    print("Select (click) the temperatures you want to fit, then close this figure.") # noqa
-
-    plt.show()
-
-    experiments = [
-        experiment
-        for experiment, store in zip(experiments, stores)
-        if store.on
-    ]
-
-    fig.canvas.mpl_disconnect(cid)
-
-    if not len(experiments):
-        sys.exit("No data selected")
-
-    return experiments
-
+    ax.legend(loc=0, fontsize='10', numpoints=1, ncol=1, frameon=False)
+    ax.set_ylabel('Moment (emu)')
+    ax.set_xlabel('Time (s)')
+
+    ax.set_xscale(x_scale)
+    ax.set_yscale(y_scale)
+
+    if y_scale == 'linear':
+        ax.yaxis.set_minor_locator(AutoMinorLocator())
+    if x_scale == 'linear':
+        ax.xaxis.set_minor_locator(AutoMinorLocator())
 
-class Toggle():
-    """
-    Helper class for interactive_t_select
-    """
-
-    def __init__(self, temperature):
-
-        self.on = False
-        self.temperature = temperature
-
-    def switch(self, ax):
-
-        if self.on:
-            self.on = False
-            ax.set_facecolor("White")
-        else:
-            self.on = True
-            ax.set_facecolor("Green")
+    fig.tight_layout()
 
-        plt.draw()
+    if save:
+        plt.savefig(save_name, dpi=500)
+        if verbose:
+            ut.cprint(
+                f'\n Fitted decay plot saved to \n {save_name}\n',
+                'cyan'
+            )
+    if show:
+        plt.show()
 
-        return
+    plt.close()
+    return fig, ax
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ccfit2-4.5.1/ccfit2/dc.py` & `ccfit2-5.0.0/ccfit2/waveform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,622 +1,707 @@
-"""
-This module contains functions and objects for working with DC
-magnetisation decay data
-"""
+'''
+This module contains functions and objects for working with waveform data
+'''
+
+from . import utils as ut
+from . import dc
+from . import ac
 
-from math import isnan
 import numpy as np
-import collections
-import sys
-if sys.platform[0:3] == "win" or sys.platform == "darwin":
-    import matplotlib
-    matplotlib.use('TkAgg')
+import numpy.typing as npt
 import matplotlib.pyplot as plt
-from scipy.optimize import curve_fit
+from math import isnan
+import operator
+import scipy.signal as signal
+from itertools import groupby
 
 
-# Generic dc magnetometer file header names
-HEADERS_GENERIC = [
-    "field",
-    "temperature",
-    "time",
-    "moment"
-]
-
-# list of supported dc headers
-# These differ between magnetometers
-# One of each MUST be found in the input file
-HEADERS_SUPPORTED = {
-    'field': [
+#: Supported Waveform Headers - One of each MUST be found in the input file.
+#:
+#:  Note - These differ between magnetometers\
+#:
+#:  These keys are the arguments to the Measurement constructor, but their
+#:  order does not matter
+HEADERS_SUPPORTED: dict[str, list[str]] = {
+    'dc_field': [
         'Magnetic Field (Oe)',
         'Field (Oe)'
     ],
     'temperature': [
         'Temperature (K)'
     ],
-    "time": [
+    'time': [
         'Time Stamp (sec)'
     ],
-    "moment": [
-        'Moment (emu)'
+    'moment': [
+        'Moment (emu)',
+    ],
+    'moment_err': [
+        'M. Std. Err. (emu)',
     ]
 }
 
+# Generic dc magnetometer file header names
+HEADERS_GENERIC = HEADERS_SUPPORTED.keys()
+
 
-class Measurement():
-    """
-    Stores data for a single DC Decay measurement at a
+class Measurement(dc.Measurement):
+    '''
+    Stores data for a single Waveform measurement at a
     given temperature and applied field
 
     Parameters
     ----------
     dc_field : float
-        Applied dc field
+        Applied dc field (Oe)
     temperature : float
-        Temperature of experiment
+        Temperature of datapoint (K)
     moment : float
-        Magnetic moment of experiment
+        Magnetisation of datapoint (emu)
     time : float
-        Time of experiment
+        Time of datapoint (s)
 
     Attributes
     ----------
     dc_field : float
-        Applied dc field
+        Applied dc field (Oe)
     temperature : float
-        Temperature of experiment
+        Temperature of datapoint (K)
     moment : float
-        Magnetic moment of experiment
+        Magnetic moment of datapoint (emu)
     time : float
-        Time of experiment
-    mean_temperature : float
-        Mean or representative temperature assigned to this experiment
-    """
-
-    def __init__(self, dc_field, temperature, time, moment):
-        self.dc_field = dc_field
-        self.temperature = temperature
-        self.time = time
-        self.moment = moment
+        Time of datapoint (s)
+    rep_temperature : float
+        Representative temperature assigned to this datapoint (K)
+    rep_dc_field : float
+        Representative dc field assigned to this datapoint (Oe)
+    '''
 
-    def set_mean_temp(self, value: float) -> None:
-        """
-        Sets mean or representative value of temperature for this
-        experiment
-
-        Parameters
-        ----------
-        value : float
-            mean value
-
-        """
-        self.mean_temperature = value
-
-        return
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
     @classmethod
-    def from_file(cls, file: str, header_indices: dict) -> list['Measurement']:
-        """
-        Extracts dc data from magnetometer output file and
-        returns list of experiments, one for each valid measurment
+    def from_file(cls, file: str, header_indices: dict | str = 'find',
+                  data_header: str = '[Data]',
+                  verbose: bool = True) -> list['Measurement']:
+        '''
+        Extracts waveform data from magnetometer output file and
+        returns list of datapoints, one for each valid measurement
         Incomplete lines are ignored
 
         Parameters
         ----------
         file : str
             Name of magnetometer output file
-
-        header_indices : dict
-            Keys are generic header names given in `HEADERS_GENERIC`
-            Values are column index of header in file
+        header_indices : str | dict, default 'find'
+            Default 'find' will automatically locate headers, else provide dict
+            with:
+            Keys as generic header names given in `HEADERS_GENERIC`
+            Values as column index (number) of header in file
+        data_header : str default '[Data]'
+            Contents of line which specifies the beginning of the data block
+            in input file default is to find line containing '[Data]'
+        verbose: bool, default True
+            If True, issues parsing measurements are written to terminal
 
         Returns
         -------
         list
-            Measurement objects, one per temperature, per field
+            Measurement objects, each specifying a single datapoint
             List has the same order as the magnetometer file
+        '''
+
+        # Find encoding of input file
+        encoding = ut.detect_encoding(file)
 
-        """
+        # Check data_header is in file
+        data_index = ut.locate_data_header(file, data_header=data_header)
 
-        # Open file and store all headers
-        with open(file, 'r') as f:
-            for it, line in enumerate(f):
-                if '[Data]' in line:
-                    header_line = it + 1
+        if header_indices == 'find':
+            # Get file headers
+            header_indices, _ = ut.parse_headers(
+                file, data_index, HEADERS_SUPPORTED
+            )
 
-        # Columns to extract from file - n.b. these are ordered
-        cols = [header_indices[gen] for gen in HEADERS_GENERIC]
+        # Columns to extract from file
+        cols = {
+            gen: header_indices[gen] for gen in HEADERS_GENERIC
+        }
 
         # Convert strings to floats, if not possible then mark as NaN
         converters = {
-            it: lambda s: (float(s.strip() or np.NaN)) for it in cols
+            it: lambda s: (float(s.strip() or np.NaN)) for it in cols.values()
         }
 
         # Read required columns of file
         data = np.loadtxt(
             file,
-            skiprows=header_line+1,
+            skiprows=data_index + 1,
             delimiter=',',
             converters=converters,
-            usecols=cols
+            usecols=cols.values(),
+            encoding=encoding
         )
 
+        # Remove missing entries that have been marked as nan
+        data = [
+            row for row in data
+            if not any(isnan(val) for val in row)
+        ]
+
+        # Keep moments smaller than their error (remove noisy data)
+        # and keep only the field values which fall outside window
+        mom_col = list(cols.keys()).index('moment')
+        err_col = list(cols.keys()).index('moment_err')
+
+        data = np.array([
+            np.delete(row, err_col) for row in data
+            if row[err_col] / row[mom_col] <= 0.3
+        ])
+
         # Convert array of floats into list of Measurement objects, one per
         # line
-        # Check for missing entries which have been marked as NaN
-        # and skip if found
-
+        # Remove positional nature of Measurement constructor args by using
+        # kwargs through dict
         measurements = [
-            cls(*row)
+            cls(**{
+                col: val
+                for col, val in zip(cols, row)
+            })
             for row in data
             if not any(isnan(val) for val in row)
         ]
 
-        return measurements
-
-
-def find_mean_temperatures(temperatures: list[float]
-                           ) -> tuple[list[float], list[int]]:
-
-    # Find values for which step size is >= 0.1 K
-    mask = np.abs(np.diff(temperatures)) >= 0.1
-    # and mark indices at which to split
-    split_indices = np.where(mask)[0]
-
-    # For values with similar step size, record mean temperature
-    mean_temps = [
-        [np.mean(grp)]*grp.size
-        for grp in np.split(temperatures, split_indices + 1)
-    ]
+        if not len(measurements) and verbose:
+            _msg = '\n Error: Cannot parse measurements from file {}'.format(
+                file
+            )
+            ut.cprint(_msg, 'red')
 
-    return mean_temps, split_indices
+        return measurements
 
 
-class Experiment():
-    """
-    Stores data for multiple DC measurements at a
-    given temperature, given applied dc field
+class Experiment(dc.Experiment):
+    '''
+    Stores data for multiple waveform measurements at a
+    given temperature and oscillating dc field frequency
 
     Parameters
     ----------
-    temperature: float
-        Temperature of experiment
-    dc_field : float
-        Applied dc field strength in Oe
+    rep_temperature: float
+        Representative temperature of experiment (K) e.g. mean
+    rep_dc_field : float
+        Representative dc field assigned to this experiment (Oe)
+    raw_temperatures: array_like
+        Raw temperatures of experiment, one per measurement (K)
+    times : array_like
+        Time value, one per measurement (s)
+    moments : array_like
+        Measured moment, one value per measurement (emu)
+    dc_fields : array_like
+        Applied dc field in Oe, one value per measurement (Oe)
 
     Attributes
     ----------
-    temperatures: list
-        Temperature of experiment
-    dc_field : float
-        Applied dc field strength in Oe
-    """
-
-    def __init__(self, temperatures, raw_temperatures, time, moment,
-                 dc_field):
-
-        self.temperatures = temperatures
-        self.raw_temperatures = raw_temperatures
-        self.time = time
-        self.moment = moment
-        self.dc_field = dc_field
-
-        return
+    rep_temperature: float
+        Representative temperature of experiment e.g. mean (K)
+    raw_temperatures: ndarray of floats
+        Raw temperatures of experiment, one per measurement (K)
+    times : ndarray of floats
+        Time value, one per measurement (s)
+    moments : ndarray of floats
+        Measured moment, one value per measurement (emu)
+    dc_fields : ndarray of floats
+        Applied dc field in Oe, one value per measurement (Oe)
+    rep_dc_field : float
+        Representative dc field assigned to this experiment (Oe)
+    '''
 
     @classmethod
     def from_measurements(cls,
-                          measurements: list[Measurement]) -> list['Experiment']: # noqa
+                          measurements: list[Measurement],
+                          field_window: list[float],
+                          temp_thresh: float = .1) -> list[list['Experiment']]:
+        '''
+        Creates list of Experiment objects from a list of individual
+        Measurement objects. An experiment is defined as a set of measurements
+        which have the same temperature and DC Field period.
 
-        # Sort measurements by dc field
-        measurements.sort(key=lambda k: (k.dc_field, k.temperature))
+        Parameters
+        ----------
+        measurement: list[Measurement]
+            Measurements at various times but same temperatures and
+            dc field period.
+        field_window: list[float], default [-0.5, 0.5]
+            Range of values at which DC Field is sampled to determine
+            different DC field periods
+        temp_thresh: float, default 0.1 K
+            Threshold used to discriminate between temperatures (K)
 
-        mean_temps, split_ind = find_mean_temperatures(
-            [
-                measurement.temperature
-                for measurement in measurements
-            ]
-        )
+        Returns
+        -------
+        list[list[Experiment]]
+            Experiments
+        '''
 
-        # Set each measurement's "mean", or representative temperature
-        for measurement, mean_temp in zip(measurements, np.concatenate(mean_temps)): # noqa
-            measurement.set_mean_temp(mean_temp)
-
-        # sort measurements by field, then temperature
-        measurements.sort(
-            key=lambda k: (k.dc_field, k.mean_temperature)
+        # Sort measurements by temperature then time
+        measurements = sorted(
+            measurements,
+            key=operator.attrgetter('temperature', 'time', )
         )
 
-        raw_temperatures = [
-            measurement.temperature
-            for measurement in measurements
-        ]
-
-        times = np.split(
+        # Find mean temperature values
+        mean_temperatures, split_ind = ut.find_mean_values(
             [
-                measurement.time
+                measurement.temperature
                 for measurement in measurements
             ],
-            split_ind + 1
+            thresh=temp_thresh
         )
 
-        moments = np.split(
-            [
-                measurement.moment
-                for measurement in measurements
-            ],
-            split_ind + 1
+        # Set each measurement's representative temperature, here the mean
+        for mm, mt in zip(measurements, np.concatenate(mean_temperatures)):
+            mm.rep_temperature = mt
+
+        # Re-sort using mean temperatures
+        measurements = sorted(
+            measurements,
+            key=operator.attrgetter('rep_temperature', 'time', )
         )
 
-        dc_fields = np.split(
-            [
-                measurement.dc_field
-                for measurement in measurements
-            ],
+        # Split by temperature
+        measurements: list[list[Measurement]] = np.split(
+            measurements,
             split_ind + 1
         )
 
-        experiments = [
-            cls(
-                mean_temp, raw_temp, time, moment,
-                dc_field[0]
-            )
-            for (
-                    mean_temp, raw_temp, time,
-                    moment,
-                    dc_field
-                ) in zip(
-                    mean_temps, raw_temperatures, times,
-                    moments, dc_fields
-                )
-        ]
-
-        for experiment in experiments:
-            print(experiment.time)
-
-        return experiments
+        field_window = np.sort(field_window)
 
-    @staticmethod
-    def split_by_field(experiments: list['Experiment']) -> list[list['Experiment']]: # noqa
+        exp = []
 
-        # Split experiments into list of lists using dc field value
-        # Find values for which step size is >= 1e-8 Oe
-        mask = np.abs(
-            np.diff([experiment.dc_field for experiment in experiments])
-        ) >= 1e-8
-        # and mark indices at which to split
-        split_ind = np.where(mask)[0]
+        # Split measurements into experiments based on dc field
+        # oscillation frequency
+        for mm in measurements:
+            fields = np.array([
+                m.dc_field
+                for m in mm
+            ])
+
+            # Find indices of points where field is changing, rather than
+            # those where it is saturated.
+            indxs = np.where(
+                (fields > field_window[0]) & (fields < field_window[1])
+            )[0]
+
+            if len(indxs) <= 1:
+                raise ValueError('No waveform data detected in file')
+
+            # Ignore single data points that accidentally fall within the
+            # field_window
+            delete = []
+            for i in range(1, len(indxs) - 1):
+                if abs(indxs[i - 1] - indxs[i]) > 1 and abs(indxs[i] - indxs[i + 1]) > 1: # noqa
+                    delete += indxs[i]
+            indxs = [i for i in indxs if i not in delete]
+
+            # Find breaks in indices, these correspond to a change in field
+            # frequency
+            # Store all breaks identified by groupby (where field is flat).
+            lims = []
+            for k, g in groupby(enumerate(indxs), lambda ix: ix[0] - ix[1]):
+                lims.append(list(g))
+
+            # Collect first and last element of list; these are tuples with
+            # index and value of indxs array, respectively.
+            limits = []
+            for i in lims:
+                limits.append((i[0][1], i[-1][1]))
+
+            # Find bounds of each experiment's datapoints
+            bounds = []
+            for i in range(len(limits) - 1):
+                bounds.append((limits[i][1] + 1, limits[i + 1][0] - 1))
+
+            times = np.array([
+                m.time
+                for m in mm
+            ])
+
+            moments = np.array([
+                m.moment
+                for m in mm
+            ])
+
+            temperatures = np.array([
+                m.temperature
+                for m in mm
+            ])
 
-        experiments: list[list[Experiment]] = np.split(
-            experiments, split_ind + 1
-        )
-
-        return experiments
-
-
-class Read_Raw_DC_Data():
-    def __init__(self, time, field, temperature, moment):
-        self.time = float(time)
-        self.field = float(field)
-        self.temperature = float(temperature)
-        self.moment = float(moment)
+            time = [
+                times[i:j] for i, j in bounds
+            ]
 
+            field = [
+                fields[i:j] for i, j in bounds
+            ]
 
-class Process_DC():
+            temperature = [
+                temperatures[i:j] for i, j in bounds
+            ]
 
-    def __init__(self, user_args):
-        self.guess = user_args.guess
-        self.hide_plots = user_args.hide_plots
-        self.save_plots = user_args.save_plots
+            moment = [
+                moments[i:j] for i, j in bounds
+            ]
 
-    def read_input(self, mag_decays_file, points_to_discard):
-        '''
-        Returns a dictionary ordered by field.
-        '''
+            _exp = []
+            for ti, fi, te, mo in zip(time, field, temperature, moment):
+                # Set zero time for each experiment
+                ti -= ti[0]
+                _exp.append(
+                    cls(
+                        mm[0].rep_temperature,
+                        0.,
+                        te,
+                        ti,
+                        mo,
+                        fi
+                    )
+                )
 
-        # Data will be stored in a dictionary where the keys and values
-        # will be the fields and (temperature, time, moment), respectively.
-        data = {}
+            exp.append(_exp)
 
-        with open(mag_decays_file, 'r') as f:
+        return exp
 
-            # Needed to avoid UnboundLocalError: local variable 'time'
-            # referenced before assignment
-            temp, time, moment = None, None, None
 
-            for line in f:
+class FTResult():
 
-                if 'Field =' in line:
+    '''
+    Contains result of Fourier Transforming an Experiment.
 
-                    if time is not None:
-                        # Save previous dataset
-                        # TODO refactor to avoid undefined key
-                        data[key][1].append(time)
-                        data[key][2].append(moment)
-                        # Reset
-                        temp, time, moment = None, None, None
+    Parameters
+    ----------
+    ft_fields: array_like
+        Fourier Transform of DC Fields
+    ft_moments: array_like
+        Fourier Transform of Magnetic Moments
+    ft_freqs: array_like
+        Frequencies associated with above fourier transformation
+    temperature: float
+        Temperature associated with this Experiment
+    period: float
+        Period associated with the oscillating DC field
 
-                    # initialise each value of the field (key) as a tuple of 3
-                    # empty lists (temperature, time, moment)
-                    key = float(line.split()[2])
-                    data[key] = ([], [], [])
+    Attributes
+    ----------
+    ft_fields: ndarray of floats
+        Fourier Transform of DC Fields, ordered by low to high frequency
+    ft_moments: ndarray of floats
+        Fourier Transform of Magnetic Moments, ordered by low to high
+        frequency
+    ft_freqs: ndarray of floats
+        Frequencies associated with above fourier transformation, ordered
+        low to high
+    temperature: float
+        Temperature associated with this Experiment
+    period: float
+        Period associated with the oscillating DC field
 
-                elif 'T' in line:
-                    data[key][0].append(float(line.split()[2]))
+    '''
 
-                    # reset lists for the current dataset
-                    temp = []
+    def __init__(self, ft_fields: npt.NDArray, ft_moments: npt.NDArray,
+                 ft_freqs: npt.NDArray, temperature: float,
+                 period: float) -> None:
 
-                elif 'time' in line:
+        order = np.argsort(ft_freqs)
 
-                    # skip the points measured with a saturating field.
-                    for _ in range(points_to_discard):
-                        next(f)
+        self.ft_fields = np.asarray(ft_fields)[order]
+        self.ft_moments = np.asarray(ft_moments)[order]
+        self.ft_freqs = np.asarray(ft_freqs)[order]
+        self.temperature = temperature
+        self.period = period
 
-                    # add completed lists from previous dataset to dictionary
-                    if None not in [temp, time, moment]:
-                        data[key][1].append(time)
-                        data[key][2].append(moment)
+        pass
 
-                    # reset lists for the current dataset
-                    time = []
-                    moment = []
+    @classmethod
+    def from_experiment(cls, experiment: Experiment) -> 'FTResult':
+        '''
+        Fourier Transforms waveform Experiment to give FTResult object
+        containing fourier transform data
 
-                else:
+        Parameters
+        ----------
+        experiment: Experiment
+            Waveform Experiment object which will be fourier transformed
 
-                    time.append(float(line.split()[0]))
-                    moment.append(float(line.split()[1]))
+        Returns
+        -------
+        FTResult
+            FTResult object containing fft data
+        '''
 
-        # To collect the last data set for which there is no next(f)
-        data[key][1].append(time)
-        data[key][2].append(moment)
+        # Calculate the sample spacing (inverse of sampling rate).
+        # Sampling rate is defined as npoints/measurement_time.
+        spacing = experiment.times[-1] / len(experiment.times)
 
-        # for key,vals in data.items():
-        #    print(key, len(vals[0]), len(vals[1][0]))
+        # Retreive the associated frequencies.
+        ft_freqs = np.fft.fftfreq(len(experiment.times), d=spacing)
 
-        if len(data) == 0:
-            print('\n***Error***:')
-            print('The program could not find information on the temperature.')
-            exit('Make sure the data format is: T = X K.')
+        # Calculate the Fourier transform of field and moment
+        ft_fields = np.fft.fft(experiment.dc_fields)
+        ft_moments = np.fft.fft(experiment.moments)
 
-        return collections.OrderedDict(sorted(data.items()))
+        # Calculate period of experimental DC field
+        period = calculate_period(experiment)
 
-    def define_DC_model(self, user_args):
+        result = cls(
+            ft_fields, ft_moments, ft_freqs, experiment.rep_temperature, period
+        )
 
-        if user_args.model == 'single':
-            self.model_name = 'single'
+        return result
 
-            if user_args.M_eq != 'free':
-                self.model_function = self.single_exponential
-                # tau
-                self.bounds = ([0.0], [np.inf])
+    @staticmethod
+    def create_ac_experiment(ft_results: list['FTResult'],
+                             experiments: list[Experiment],
+                             mass: float, mw: float) -> ac.Experiment:
+        '''
+        Creates ac.Experiment using a list of Fourier Transform results
 
-            else:
-                self.model_function = self.single_exponential_2
-                # tau, Meq
-                self.bounds = ([0.0, -np.inf], [np.inf, np.inf])
+        Parameters
+        ----------
+        ft_results: list[FTResult]
+            Fourier transform results, each constituting a single
+            datapoint in an AC susceptiblity experiment
+        exepriments: list[Experiments]
+            Waveform experiments which accompany ft_results, order must match
+        mass: float
+            Mass of sample, used to convert real and imaginary susceptibility
+            from emu/Oe to cm3 mol^{-1}\n
+            Set to None for no conversion
+        mw: float
+            Molecular weight of sample, used to convert real and imaginary
+            susceptibility from emu/Oe to cm3 mol^{-1}\n
+            Set to None for no conversion
 
-        elif user_args.model == 'stretched':
-            self.model_name = 'stretched'
+        Returns
+        -------
+        ac.Experiment
+            ccfit2.ac.Experiment object for this set of AC Susceptibility data
+        '''
 
-            if user_args.M_eq != 'free':
-                self.model_function = self.stretched_exponential
-                # tau, beta
-                self.bounds = ([0.0, 0.0], [np.inf, 1.0])
+        ac_freqs = []
+        real_sus = []
+        imag_sus = []
+
+        for ftr in ft_results:
+
+            # Find largest FT field index
+            idx_field = np.argmax(np.abs(ftr.ft_fields))
+            ac_freqs.append(np.abs(ftr.ft_freqs[idx_field]))
+
+            # Calculate susceptibility as M/H at maximum (emu/Oe)
+            chi = np.abs(ftr.ft_moments[idx_field])
+            chi /= np.abs(ftr.ft_fields[idx_field])
+
+            # Calculate the phase angle (rad) of the ratio between field and
+            # moment spectra at their fundamental frequency.
+            # It is the ratio because any function of the type:
+            # Acos(X) + Bsin(X) = Ccos(X + phasefactor)
+            # This phasefactor angle is determined by the ratio of A/B
+            phi = calculate_phase(
+                ftr.ft_fields[idx_field], ftr.ft_moments[idx_field]
+            )
 
-            else:
-                self.model_function = self.stretched_exponential_2
-                # tau, beta, Meq
-                self.bounds = ([0.0, 0.0, -np.inf], [np.inf, 1.0, np.inf])
-        return
+            # Calculate real and imaginary susceptibility components
+            real_sus.append(abs(chi * np.cos(phi)))
+            imag_sus.append(abs(chi * np.sin(phi)))
+
+        real_sus = np.array(real_sus)
+        imag_sus = np.array(imag_sus)
+        ac_freqs = np.array(ac_freqs)
+
+        # Convert real and imaginary susceptibility from (emu/Oe)
+        # to cm^3mol^(-1)
+        if None not in (mw, mass):
+            real_sus *= mw / (mass / 1000.)
+            imag_sus *= mw / (mass / 1000.)
+
+        # Collect temperature data
+        temperatures = np.array([ftr.temperature for ftr in ft_results])
+        mean_temp = np.mean(temperatures)
+
+        ac_fields = np.array([
+            calculate_ac_field(exp)
+            for exp in experiments
+        ])
+
+        # Sort all data by ac frequency, low to high
+        order = np.argsort(ac_freqs)
+
+        # Create AC experiment using waveform susceptibility data
+        ac_experiment = ac.Experiment(
+            mean_temp,
+            temperatures[order],
+            real_sus[order],
+            imag_sus[order],
+            ac_freqs[order],
+            0.,
+            np.zeros(len(temperatures)),
+            ac_fields[order]
+        )
+
+        return ac_experiment
+
+
+def calculate_period(experiment: Experiment) -> float:
+    '''
+    Calculates the period of a waveform experiment's square wave
 
-    def single_exponential(self, time, tau):
-        # M(t) = Meq + (M0 - Meq) * exp( -t / tau)
-        return self.Meq + (self.M0 - self.Meq)*np.exp(-time/tau)
+    Parameters
+    ----------
+    experiment: Experiment
+        Waveform experiment object
 
-    def single_exponential_2(self, time, tau, Meq):
-        # M(t) = Meq + (M0 - Meq) * exp( -t / tau)
-        return Meq + (self.M0 - Meq)*np.exp(-time/tau)
+    Returns
+    -------
+    float
+        period of square wave
+    '''
 
-    def stretched_exponential(self, time, tau, beta):
-        # M(t) = Meq + (M0 - Meq) * exp( -t / tau)**beta
-        return self.Meq + (self.M0 - self.Meq)*np.exp(-(time/tau)**beta)
+    dfields = np.diff(experiment.dc_fields)
 
-    def stretched_exponential_2(self, time, tau, beta, Meq):
-        # M(t) = Meq + (M0 - Meq) * exp( -t / tau)**beta
-        return Meq + (self.M0 - Meq)*np.exp(-(time/tau)**beta)
+    dpeaks = signal.find_peaks(
+        np.abs(dfields),
+        threshold=0.7 / 2
+    )[0]
 
-    def fit_decays(self, field, decays, DC_filename, params_fit, vals_fit,
-                   M_eq, meq_multiple):
+    # Forward difference of time values at turning points will give period
+    periods = np.diff(experiment.times[dpeaks])
 
-        for it, temp in enumerate(decays[0]):
+    # Take mean
+    period = np.mean(periods)
 
-            time = decays[1][it]
-            moment = decays[2][it]
+    return period
 
-            fit_failed = None
 
-            # set initial measurement to t = 0.
-            time = [i - time[0] for i in time]
-            self.M0 = moment[0]
-            if M_eq != 'free' and M_eq != 'exp' and M_eq != 'multiple':
-                self.Meq = float(M_eq)
-                if self.M0 < self.Meq:
-                    print('\n***Error***:')
-                    print(
-                        'At {} K and {} Oe'.format(temp, field),
-                        ', the provided M_eq = {} is smaller'.format(
-                            self.M_eq
-                        ),
-                        ' than M0 = {}'.format(self.M0)
-                    )
-                    exit('Please revise.\n')
-            elif M_eq == 'multiple':
-                # check how many lines to decide how to index it.
-                if np.ndim(meq_multiple) == 1:
-                    self.Meq = meq_multiple[1]
-                else:
-                    self.Meq = meq_multiple[it, 1]
-            else:
-                self.Meq = moment[-1]
-
-            if it == 0:
-                guess = self.guess
-
-            # Fit the curve and update the guess.
-            # TODO: Wrap curve_fit into a class and adapt model_function(),
-            # write_params_fit(), write_vals_fit() and plot()
-            # to work with new class, to avoid logic with fit_failed
-            try:
-                popt, pcov = curve_fit(
-                    self.model_function, time, moment, p0=guess,
-                    bounds=self.bounds
-                )
-            except RuntimeError:
-                fit_failed = True
+def calculate_ac_field(experiment: Experiment):
+    '''
+    Calculates the ac field of single waveform experiment
 
-            if not fit_failed:
-                # compute one standard deviation errors on the parameters
-                perr = np.sqrt(np.diag(pcov))
-                guess = popt
-                # print('    T =  {:04.2f} K; Field = {:06.2f} Oe: DONE. '.format( temp, field ), end='\r', flush=True ) # noqa
-
-                # Calculate the model function with the optimised parameters.
-                model = self.model_function(np.array(time), *popt)
-
-                # Write the parameters of the fit.
-                self.write_params_fit(params_fit, temp, field, self.M0,
-                                      self.Meq, popt, perr, model, M_eq)
-
-                # Write the values of the fit.
-                self.write_vals_fit(vals_fit, temp, time, field, moment, model)
-
-                # Plot the results.
-                self.plot(temp, field, time, moment, model, popt, DC_filename)
-
-            else:
-
-                # Write the parameters of the fit.
-                params_fit.write('{: 06.2f}  {: 06.2f} {:^10}\n'.format(
-                    temp, field, 'Fit failed'
-                ))
-
-                # Write the values of the fit.
-                vals_fit.write('{: 06.2f}  {: 06.2f} {:^10}\n'.format(
-                    temp, field, 'Fit failed'
-                ))
-
-                pass
-
-        params_fit.close()
-        vals_fit.close()
-        print('\n\n    Parameters written to')
-        print('     {}_params.out'.format(DC_filename))
-        print('    Fit written to')
-        print('     {}_fit.out'.format(DC_filename))
-
-        return
-
-    def write_params_fit(self, out_obj, temperature, field, M0, Meq, popt,
-                         perr, model, M_eq):
-
-        # Calculate the ESD on tau associated with beta.
-        if self.model_name == 'stretched':
-            # tau, beta
-            tau_ESD = self.johnston(popt[0], popt[1])
-
-        # Write the parameters of the fit.
-        if M_eq == 'free':
-            out_obj.write(' {: 06.2f}  {: 06.2f}  {: 08.4E}'.format(
-                temperature,
-                field,
-                M0
-            ))
-            # Meq is the last optimised parameter.
-            out_obj.write(' {: 08.4E} '.format(popt[-1]))
-            # exclude the last item corresponding to Meq
-            for i, j in zip(popt[0:-1], perr[0:-1]):
-                out_obj.write(' {: 08.4E} {: 08.4E} '.format(i, j))
-
-        else:
-            out_obj.write(' {: 06.2f}  {: 06.2f}  {: 08.4E}  {: 08.4E}'.format(
-                temperature, field, M0, Meq
-            ))
-            for i, j in zip(popt, perr):
-                out_obj.write(' {: 08.4E} {: 08.4E} '.format(i, j))
-
-        if self.model_name == 'stretched':
-            out_obj.write(' {: 08.4E} {: 08.4E}'.format(
-                tau_ESD[0], tau_ESD[1]
-            ))
-        out_obj.write('\n')
+    Parameters
+    ----------
+    experiment: Experiment
+        Waveform experiment object
 
-        return
+    Returns
+    -------
+    float
+        ac field
+    '''
 
-    def johnston(self, tau, beta):
+    # low to high field values
+    sorted_fields = np.sort(experiment.dc_fields)
 
-        J_err_upper = tau*np.exp(
-            (1.64*np.tan(np.pi*(1-beta)/2.)) / ((1 - beta)**0.141)
-        )
-        J_err_lower = tau*np.exp(
-            -(1.64*np.tan(np.pi*(1-beta)/2.)) / ((1 - beta)**0.141)
-        )
+    n_fields = len(sorted_fields)
 
-        return J_err_upper, J_err_lower
+    # Take upper and lower 50%
+    low = np.mean(sorted_fields[:n_fields // 2])
+    high = np.mean(sorted_fields[n_fields // 2:])
 
-    def write_vals_fit(self, filename, temperature, time, field, moment,
-                       model):
+    # and average them to get the ac field
+    acf = abs((high - low) / 2.)
 
-        # Write the values of the fit.
-        filename.write('T = {:04.2f} K, field = {:04.2f} Oe\n'.format(
-            temperature, field
-        ))
-        filename.write(' {:^10} {:^10} {:^10}\n'.format(
-            'time (s)', 'moment', 'fit'
-        ))
-        for i, j, k in zip(time, moment, model):
-            filename.write(' {: 08.4E} {: 08.4E} {: 08.4E}\n'.format(i, j, k))
-
-        return
-
-    def plot(self, temperature, field, time, moment, model, popt, DC_filename):
-
-        if self.model_name == 'single':
-            label_fit = r'$\tau={:06.2f}\ $(s)'.format(popt[0])
-        elif self.model_name == 'stretched':
-            label_fit = r'$\tau={:06.2f}$ (s), $\beta={:04.3f}$'.format(
-                popt[0], popt[1]
-            )
+    return acf
 
-        # Plot the figure.
-        fig, ax = plt.subplots(
-            1, 1, sharex=True, sharey=True, figsize=(4.5, 3.5)
-        )
-        ax.plot(
-            time,
-            moment,
-            lw=0,
-            marker='o',
-            fillstyle='none',
-            label='{:f} K, {:f} Oe'.format(temperature, field)
-        )
-        ax.plot(time, model, lw=1.5, label=label_fit)
 
-        ax.legend(loc=0, fontsize='10', numpoints=1, ncol=1, frameon=False)
-        ax.set_ylabel('Moment')
-        ax.set_xlabel('time (s)')
+def calculate_phase(ft_field: float, ft_moment: float):
+    '''
+    Calculates phase between fourier tranformed dc field and moment values
 
-        fig.tight_layout()
+    Parameters
+    ----------
+    ft_field: float
+        Fourier Transformed dc field value
+    ft_moment: float
+        Fourier Transformed moment value
+
+    Returns
+    -------
+    float
+        Phase in radians
+    '''
+
+    phase = abs(
+        np.angle(
+            ft_field / ft_moment,
+            deg=False
+        )
+    )
+
+    return phase
+
+
+def plot_waveform_data(ft_result: FTResult, save: bool = True,
+                       show: bool = True,
+                       save_name: str = 'FT_waveform.png',
+                       window_title: str = 'Fourier Transformed Data',
+                       verbose: bool = True) -> tuple[plt.Figure, list[plt.Axes]]: # noqa
+    '''
+    Plot fourier transform data for a given waveform experiment
 
-        if self.save_plots:
-            _filename = '{}_{}K_{}Oe_{}'.format(
-                DC_filename, temperature, field, model
+    Parameters
+    ----------
+    ft_result: FTResult
+        Fts
+    save: bool, default True
+        If True, saves plot to file
+    show: bool, default True
+        If True, shows plot on screen
+    save_name: str, default 'FT_waveform.png'
+        If save is True, will save plot to this file name
+    window_title: str, default 'Fourier Transformed Data'
+        Title of figure window, not of plot
+    verbose: bool, default True
+        If True, plot file location is written to terminal
+
+    Returns
+    -------
+    plt.Figure
+        Matplotlib figure object
+    list[plt.Axes]
+        Matplotlib axis objects, first contains FT of field, second
+        contains FT of moment
+    '''
+
+    # Define canvas object.
+    fig, ax1 = plt.subplots(1, 1, num=window_title)
+
+    ax2 = ax1.twinx()
+
+    # Plot the data.
+    ax1.plot(ft_result.ft_freqs, np.abs(ft_result.ft_fields), color='k')
+    ax2.plot(
+        ft_result.ft_freqs, np.abs(ft_result.ft_moments), color='tab:blue'
+    )
+
+    ax1.set_ylabel(r'|FT$^\mathregular{D}$ (H)|')
+    ax2.set_ylabel(r'|FT$^\mathregular{D}$ (M)|')
+
+    ax1.yaxis.label.set_color('k')
+    ax2.yaxis.label.set_color('tab:blue')
+
+    ax1.set_xscale('log')
+
+    ax1.set_xlabel('Frequency (Hz)')
+
+    fig.tight_layout()
+
+    if save:
+        fig.savefig(save_name, dpi=400)
+        if verbose:
+            ut.cprint(
+                f'\n Fourier Transform plot saved to \n {save_name}\n',
+                'cyan'
             )
-            fig.savefig('{}.png'.format(_filename), dpi=200)
-            print('\n    Plot of magnetisation decay saved as')
-            print('     {}'.format(_filename))
-
-        if not self.hide_plots:
-            plt.show()
-
-        plt.close('all')
+    if show:
+        plt.show()
 
-        return
+    return fig, [ax1, ax2]
```

### Comparing `ccfit2-4.5.1/setup.py` & `ccfit2-5.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "4.5.1"
+__version__ = "5.0.0"
 
 setuptools.setup(
     name='ccfit2',
     version=__version__,
     author='Daniel Reta',
     author_email='danielreta1@gmail.com',
     description='CCFIT2 is a program for fitting AC and DC magnetisation data', # noqa
@@ -24,25 +24,28 @@
         "Bug Tracker": "https://gitlab.com/chilton-group/cc-fit2/-/issues",
         "Documentation": "https://chilton-group.gitlab.io/cc-fit2"
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent'
-        ],
-    python_requires='>=3.9',
+    ],
+    python_requires='>=3.10',
     install_requires=[
-        'numpy',
-        'scipy',
-        'matplotlib',
-        'pillow',
-	'requests'
-        ],
+        'numpy>=1.24.3',
+        'scipy>=1.10.1',
+        'matplotlib>=3.7.1',
+        'pillow>=9.5.0',
+        'requests>=2.31.0',
+        'qtpy>=2.3.1',
+        'pyqtgraph>=0.13.2',
+        'charset_normalizer>=3.1.0'
+    ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'ccfit2 = ccfit2.cli:main',
             'cc_fit2 = ccfit2.cli:main',
             'cc-fit2 = ccfit2.cli:main'
-            ]
-        }
-    )
+        ]
+    }
+)
```

