# Comparing `tmp/raspisump-1.8.tar.gz` & `tmp/raspisump-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.8.tar", last modified: Thu Jun 15 16:26:18 2023, max compression
+gzip compressed data, was "raspisump-1.8.1.tar", last modified: Fri Jun 16 18:15:34 2023, max compression
```

## Comparing `raspisump-1.8.tar` & `raspisump-1.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3969 2023-06-15 16:26:18.572954 raspisump-1.8/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8/README.md
--rw-r--r--   0 al        (1000) users      (984)       11 2023-06-15 16:24:24.000000 raspisump-1.8/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2023-06-02 22:51:18.000000 raspisump-1.8/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.562954 raspisump-1.8/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/css/includes.js
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/css/raspi.css
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8/conf/web/images/logo.png
--rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.566287 raspisump-1.8/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.569621 raspisump-1.8/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4680 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     1965 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4190 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2126 2023-06-15 16:24:24.000000 raspisump-1.8/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3969 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      809 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-06-15 16:26:18.000000 raspisump-1.8/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-06-15 16:26:18.572954 raspisump-1.8/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2402 2023-06-15 16:24:24.000000 raspisump-1.8/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-15 16:26:18.572954 raspisump-1.8/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.8/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8.1/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8.1/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3971 2023-06-16 18:15:34.076269 raspisump-1.8.1/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8.1/README.md
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-06-16 18:14:35.000000 raspisump-1.8.1/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8.1/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8.1/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     6100 2023-06-16 18:14:35.000000 raspisump-1.8.1/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.069602 raspisump-1.8.1/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8.1/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8.1/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8.1/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8.1/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.072935 raspisump-1.8.1/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8.1/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.1/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4788 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8.1/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2090 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4298 2023-06-16 18:14:35.000000 raspisump-1.8.1/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2126 2023-06-15 16:24:24.000000 raspisump-1.8.1/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8.1/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3971 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      809 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-06-16 18:15:33.000000 raspisump-1.8.1/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-06-16 18:15:34.076269 raspisump-1.8.1/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2404 2023-06-16 18:14:35.000000 raspisump-1.8.1/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-16 18:15:34.076269 raspisump-1.8.1/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8.1/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.8.1/tests/tests_sump.py
```

### Comparing `raspisump-1.8/LICENSE` & `raspisump-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/PKG-INFO` & `raspisump-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8
+Version: 1.8.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.8/README.md` & `raspisump-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/bin/rsump.py` & `raspisump-1.8.1/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/bin/rsumpchart.py` & `raspisump-1.8.1/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/bin/rsumpmonitor.py` & `raspisump-1.8.1/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/bin/rsumpwebchart.py` & `raspisump-1.8.1/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/conf/raspisump.conf` & `raspisump-1.8.1/conf/raspisump.conf`

 * *Files 6% similar despite different names*

```diff
@@ -91,27 +91,39 @@
 # SMTP Server requires authentication (0=No, 1=Yes)
 # If using localhost or possibly your ISP email this value
 # will most likely be 0.  Check your ISP's configuration docs.
 # For Gmail set this to 1 and fill out the corresponding 
 # username and password values in this file.
 smtp_authentication = 0
 
+
+# SMTP Server uses SSL (0=No, 1=Yes)
+# Most SMTP servers are now supporting ssl over tls.  However you can
+# explicitely request tls if need to.
+# leaving both tls and ssl to zero will omit encryption entirely.
+# Select 1 for either, but never both.
+# For Gmail set smtp_ssl to 1.  Gmail can also use tls if needed for the time
+# being.
+
 # SMTP Server uses TLS (0=No, 1=Yes)
-# If using localhost or possibly your ISP email this value
-# will most likely be 0.  Check your ISP's configuratin docs.
-# For Gmail set this to 1.
 smtp_tls = 0
+# SMTP Server uses SSL (0=No, 1=Yes)
+smtp_ssl = 0
 
 # If server requires authentication enter username and password.
-# For Gmail, activate these values with your gmail username and password.
+# For Gmail, activate these values with your gmail username and app password.
+# See https://support.google.com/mail/answer/185833?hl=en for instructions on 
+# setting an app password.
+
 username = 
 password = 
 
 # SMTP Server and Port
-# example --  smtp_server = smtp.gmail.com:587
+# example --  smtp_server = smtp.gmail.com:587  (TLS)
+# example --  smtp_server = smtp.gmail.com:465  (SSL)
 # if using a SMTP server on the Pi use localhost:25
 smtp_server = localhost:25
 
 # Notifications will be sent to the following address
 # example -- email_to = cellnumber@wireless_carrier (for sms email alerts)
 # You can also use a regular email address
 # To add multiple recipients seperate email addresses with a comma.
```

### Comparing `raspisump-1.8/conf/web/images/logo.png` & `raspisump-1.8.1/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/conf/web/index.html` & `raspisump-1.8.1/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/docs/install.md` & `raspisump-1.8.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/docs/install.pdf` & `raspisump-1.8.1/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump/alerts.py` & `raspisump-1.8.1/raspisump/alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     configs["alert_interval"] = 5
 
 try:
     configs["alert_when"] = config.get("pit", "alert_when")
 except configparser.NoOptionError:
     configs["alert_when"] = "high"
 
+try:
+    configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
+except configparser.NoSectionError:
+    configs["smtp_ssl"] = 0
+
 
 def current_time():
     """Return the current time as reported by the OS."""
     return time.strftime("%I:%M%P %Z")
 
 
 def host_name():
@@ -98,28 +103,25 @@
     )
 
 
 def smtp_alerts(water_depth):
     """Send email alert if water level greater than critical distance."""
     recipients = configs["email_to"].split(", ")
     email_body = email_content(water_depth)
-    server = smtplib.SMTP(configs["smtp_server"])
 
-    # Check if smtp server uses TLS
-    if configs["smtp_tls"] == 1:
+    if configs["smtp_ssl"] == 1:
+        server = smtplib.SMTP_SSL(configs["smtp_server"])
+    elif configs["smtp_tls"] == 1:
+        server = smtplib.SMTP(configs["smtp_server"])
         server.starttls()
     else:
-        pass
-    # Check if smtp server uses authentication
+        server = smtplib.SMTP(configs["smtp_server"])
+
     if configs["smtp_authentication"] == 1:
-        username = configs["username"]
-        password = configs["password"]
-        server.login(username, password)
-    else:
-        pass
+        server.login(configs["username"], configs["password"])
 
     server.sendmail(configs["email_from"], recipients, email_body)
     server.quit()
 
 
 def determine_if_alert(water_depth):
     """Determine if an alert is required.  Only send if last alert has been
```

### Comparing `raspisump-1.8/raspisump/checkpid.py` & `raspisump-1.8.1/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump/emailtest.py` & `raspisump-1.8.1/raspisump/emailtest.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import os
+
+# import smtplib
 import smtplib
 import configparser
 from raspisump import alerts
 
 
 config = configparser.RawConfigParser()
 user = os.getlogin()
@@ -23,14 +25,19 @@
     "smtp_authentication": config.getint("email", "smtp_authentication"),
     "smtp_tls": config.getint("email", "smtp_tls"),
     "smtp_server": config.get("email", "smtp_server"),
     "username": config.get("email", "username"),
     "password": config.get("email", "password"),
 }
 
+try:
+    configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
+except configparser.NoSectionError:
+    configs["smtp_ssl"] = 0
+
 
 def test_email_content():
     """Build the contents of test email body."""
 
     time_of_day = alerts.current_time()
     hostname = alerts.host_name()
 
@@ -48,24 +55,20 @@
     )
 
 
 def test_email():
     """Send test email only."""
     recipients = configs["email_to"].split(", ")
     email_body = test_email_content()
-    server = smtplib.SMTP(configs["smtp_server"])
-
-    # Check if smtp server uses TLS
-    if configs["smtp_tls"] == 1:
+    if configs["smtp_ssl"] == 1:
+        server = smtplib.SMTP_SSL(configs["smtp_server"])
+    elif configs["smtp_tls"] == 1:
+        server = smtplib.SMTP(configs["smtp_server"])
         server.starttls()
     else:
-        pass
-    # Check if smtp server uses authentication
+        server = smtplib.SMTP(configs["smtp_server"])
+
     if configs["smtp_authentication"] == 1:
-        username = configs["username"]
-        password = configs["password"]
-        server.login(username, password)
-    else:
-        pass
+        server.login(configs["username"], configs["password"])
 
     server.sendmail(configs["email_from"], recipients, email_body)
     server.quit()
```

### Comparing `raspisump-1.8/raspisump/heartbeat.py` & `raspisump-1.8.1/raspisump/heartbeat.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 }
 
 try:
     configs["heartbeat_interval"] = config.getint("email", "heartbeat_interval")
 except configparser.NoOptionError:
     configs["heartbeat_interval"] = 10080
 
+try:
+    configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
+except configparser.NoSectionError:
+    configs["smtp_ssl"] = 0
+
 
 def get_last_alert_time():
     """Retrieve the last alert time string from logfile"""
     heartbeat_log = "/home/" + user + "/raspi-sump/logs/heartbeat_log"
     with open(heartbeat_log, "rt") as f:
         last_row = deque(csv.reader(f), 1)[0]
         return last_row[0]
@@ -76,28 +81,25 @@
 
 
 def heartbeat_alerts():
     """Send heartbeat email alert if water level greater
     than critical distance."""
     recipients = configs["email_to"].split(", ")
     email_body = heartbeat_email_content()
-    server = smtplib.SMTP(configs["smtp_server"])
 
-    # Check if smtp server uses TLS
-    if configs["smtp_tls"] == 1:
+    if configs["smtp_ssl"] == 1:
+        server = smtplib.SMTP_SSL(configs["smtp_server"])
+    elif configs["smtp_tls"] == 1:
+        server = smtplib.SMTP(configs["smtp_server"])
         server.starttls()
     else:
-        pass
-    # Check if smtp server uses authentication
+        server = smtplib.SMTP(configs["smtp_server"])
+
     if configs["smtp_authentication"] == 1:
-        username = configs["username"]
-        password = configs["password"]
-        server.login(username, password)
-    else:
-        pass
+        server.login(configs["username"], configs["password"])
 
     server.sendmail(configs["email_from"], recipients, email_body)
     server.quit()
 
 
 def determine_if_heartbeat():
     """Determine if a heartbeat notification is required and if so, send
```

### Comparing `raspisump-1.8/raspisump/log.py` & `raspisump-1.8.1/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump/reading.py` & `raspisump-1.8.1/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump/todaychart.py` & `raspisump-1.8.1/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump/webchart.py` & `raspisump-1.8.1/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/raspisump.egg-info/PKG-INFO` & `raspisump-1.8.1/raspisump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8
+Version: 1.8.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.8/raspisump.egg-info/SOURCES.txt` & `raspisump-1.8.1/raspisump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/setup.py` & `raspisump-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.8"
+version = "1.8.1"
 user = os.getlogin()
 
 homedir = "/home/" + user + "/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
```

### Comparing `raspisump-1.8/tests/tests_logging.py` & `raspisump-1.8.1/tests/tests_logging.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8/tests/tests_sump.py` & `raspisump-1.8.1/tests/tests_sump.py`

 * *Files identical despite different names*

