# Comparing `tmp/teedoc-1.8.4.tar.gz` & `tmp/teedoc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/teedoc-1.8.4.tar", last modified: Tue Mar  9 09:45:12 2021, max compression
+gzip compressed data, was "teedoc-1.9.0.tar", last modified: Tue Mar  9 15:57:20 2021, max compression
```

## Comparing `teedoc-1.8.4.tar` & `teedoc-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-03-09 09:45:12.000000 teedoc-1.8.4/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2960 2021-03-09 09:45:12.000000 teedoc-1.8.4/PKG-INFO
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     1939 2021-03-09 07:15:05.000000 teedoc-1.8.4/README.md
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       38 2021-03-09 09:45:12.000000 teedoc-1.8.4/setup.cfg
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3342 2021-03-06 06:57:43.000000 teedoc-1.8.4/setup.py
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      106 2021-03-06 06:54:50.000000 teedoc-1.8.4/teedoc/__init__.py
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      780 2021-02-05 07:11:56.000000 teedoc-1.8.4/teedoc/http_server.py
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     3232 2021-02-01 03:19:24.000000 teedoc-1.8.4/teedoc/logger.py
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2441 2021-02-07 07:08:41.000000 teedoc-1.8.4/teedoc/plugin.py
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc/static/
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc/static/js/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     8763 2021-02-01 03:44:53.000000 teedoc-1.8.4/teedoc/static/js/live.js
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      275 2021-03-09 08:04:15.000000 teedoc-1.8.4/teedoc/teedoc_debug.py
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)    60355 2021-03-09 09:36:42.000000 teedoc-1.8.4/teedoc/teedoc_main.py
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       22 2021-03-09 09:45:05.000000 teedoc-1.8.4/teedoc/version.py
-drwxr-xr-x   0 neucrack  (1000) neucrack  (1000)        0 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)     2960 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/PKG-INFO
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)      363 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/SOURCES.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)        1 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/dependency_links.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       52 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/entry_points.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)       28 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/requires.txt
--rw-r--r--   0 neucrack  (1000) neucrack  (1000)        7 2021-03-09 09:45:12.000000 teedoc-1.8.4/teedoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-09 15:57:20.601145 teedoc-1.9.0/
+-rw-rw-rw-   0        0        0     3025 2021-03-09 15:57:20.600649 teedoc-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1939 2021-03-09 13:30:11.000000 teedoc-1.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2021-03-09 15:57:20.601145 teedoc-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3342 2021-03-08 11:49:15.000000 teedoc-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-09 15:57:20.594698 teedoc-1.9.0/teedoc/
+-rw-rw-rw-   0        0        0      106 2021-03-08 11:49:15.000000 teedoc-1.9.0/teedoc/__init__.py
+-rw-rw-rw-   0        0        0      780 2021-03-05 15:59:30.000000 teedoc-1.9.0/teedoc/http_server.py
+-rw-rw-rw-   0        0        0     3232 2021-02-01 12:26:09.000000 teedoc-1.9.0/teedoc/logger.py
+-rw-rw-rw-   0        0        0     3154 2021-03-09 14:51:32.000000 teedoc-1.9.0/teedoc/plugin.py
+drwxrwxrwx   0        0        0        0 2021-03-09 15:57:20.588249 teedoc-1.9.0/teedoc/static/
+drwxrwxrwx   0        0        0        0 2021-03-09 15:57:20.599657 teedoc-1.9.0/teedoc/static/js/
+-rw-rw-rw-   0        0        0     8763 2021-02-01 12:26:09.000000 teedoc-1.9.0/teedoc/static/js/live.js
+-rw-rw-rw-   0        0        0      275 2021-03-09 13:30:11.000000 teedoc-1.9.0/teedoc/teedoc_debug.py
+-rw-rw-rw-   0        0        0    62770 2021-03-09 15:55:09.000000 teedoc-1.9.0/teedoc/teedoc_main.py
+-rw-rw-rw-   0        0        0       22 2021-03-09 15:56:49.000000 teedoc-1.9.0/teedoc/version.py
+drwxrwxrwx   0        0        0        0 2021-03-09 15:57:20.599161 teedoc-1.9.0/teedoc.egg-info/
+-rw-rw-rw-   0        0        0     3025 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-03-09 15:57:20.000000 teedoc-1.9.0/teedoc.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `teedoc-1.8.4/PKG-INFO` & `teedoc-1.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,47 @@
-Metadata-Version: 2.1
-Name: teedoc
-Version: 1.8.4
-Summary: doc site generator with multiple doc support
-Home-page: https://github.com/Neutree/teedoc
-Author: Neucrack
-Author-email: CZD666666@gmail.com
-License: MIT
-Description: teedoc
-        ===========
-        
-        [中文 README](./README_ZH.md)
-        
-        [![License](https://img.shields.io/github/license/teedoc/teedoc?color=red)](./LICENSE) [![PyPI](https://img.shields.io/pypi/v/teedoc)](https://pypi.org/project/teedoc/#history) ![PyPI - Downloads](https://img.shields.io/pypi/dm/teedoc?color=brightgreen) ![PyPI - Downloads](https://img.shields.io/pypi/dw/teedoc?color=brightgreen) [![GitHub Repo stars](https://img.shields.io/github/stars/teedoc/teedoc?style=social)](https://github.com/teedoc/teedoc)
-        
-        <img src="https://teedoc.github.io/static/image/logo.png" height=64/> 
-        
-        Official site: [teedoc.github.io](https://teedoc.github.io/) or [teedoc.gitee.io](https://teedoc.gitee.io/)
-        
-        documentation generate tool from markdown and jupyter notebook to html
-        
-        ![](./assets/images/teedoc_screenshot_0.png)
-        
-        `teedoc` can be used in the following scenarios:
-        * Build a document website, and it is best to support multiple documents and custom pages
-        * Build a `WiKi` website
-        * Build personal or corporate knowledge base
-        * Build personal or corporate website
-        
-        
-        ## Features
-        
-        - [x] Easy to use, cross platform, only need `Python3`
-        - [x] Easy to deploy, only copy generated staitc HTML files to your server or other host
-        - [x] Easy to write, markdown support
-        - [x] Jupyter notebook support
-        - [x] Multiple docs support
-        - [x] Plugin support
-        - [x] Multiple theme support(support by plugin)
-        - [x] Control the style accurate to the page through css (implemented by customizing the id and class of each page)
-        - [x] Multi-level directory support
-        - [x] Multiple language support(manually translate)
-        - [ ] Multiple language support(auto translate)
-        - [x] Multiple version support
-        - [x] Search support
-        - [x] SEO friendly
-        - [x] Real-time preview file changes
-        - [x] Multiple thread support, faster build speed
-        - [ ] Blog support
-        
-        
-        ## Get Started
-        
-        Visit official site: [teedoc.github.io](https://teedoc.github.io/) or [teedoc.gitee.io](https://teedoc.gitee.io/)
-        
-        
-Keywords: doc website markdown jupyter notbook generator teedoc
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+teedoc
+===========
+
+[中文 README](./README_ZH.md)
+
+[![License](https://img.shields.io/github/license/teedoc/teedoc?color=red)](./LICENSE) [![PyPI](https://img.shields.io/pypi/v/teedoc)](https://pypi.org/project/teedoc/#history) ![PyPI - Downloads](https://img.shields.io/pypi/dm/teedoc?color=brightgreen) ![PyPI - Downloads](https://img.shields.io/pypi/dw/teedoc?color=brightgreen) [![GitHub Repo stars](https://img.shields.io/github/stars/teedoc/teedoc?style=social)](https://github.com/teedoc/teedoc)
+
+<img src="https://teedoc.github.io/static/image/logo.png" height=64/> 
+
+Official site: [teedoc.github.io](https://teedoc.github.io/) or [teedoc.gitee.io](https://teedoc.gitee.io/)
+
+documentation generate tool from markdown and jupyter notebook to html
+
+![](./assets/images/teedoc_screenshot_0.png)
+
+`teedoc` can be used in the following scenarios:
+* Build a document website, and it is best to support multiple documents and custom pages
+* Build a `WiKi` website
+* Build personal or corporate knowledge base
+* Build personal or corporate website
+
+
+## Features
+
+- [x] Easy to use, cross platform, only need `Python3`
+- [x] Easy to deploy, only copy generated staitc HTML files to your server or other host
+- [x] Easy to write, markdown support
+- [x] Jupyter notebook support
+- [x] Multiple docs support
+- [x] Plugin support
+- [x] Multiple theme support(support by plugin)
+- [x] Control the style accurate to the page through css (implemented by customizing the id and class of each page)
+- [x] Multi-level directory support
+- [x] Multiple language support(manually translate)
+- [ ] Multiple language support(auto translate)
+- [x] Multiple version support
+- [x] Search support
+- [x] SEO friendly
+- [x] Real-time preview file changes
+- [x] Multiple thread support, faster build speed
+- [ ] Blog support
+
+
+## Get Started
+
+Visit official site: [teedoc.github.io](https://teedoc.github.io/) or [teedoc.gitee.io](https://teedoc.gitee.io/)
+
```

### Comparing `teedoc-1.8.4/setup.py` & `teedoc-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `teedoc-1.8.4/teedoc/http_server.py` & `teedoc-1.9.0/teedoc/http_server.py`

 * *Files identical despite different names*

### Comparing `teedoc-1.8.4/teedoc/logger.py` & `teedoc-1.9.0/teedoc/logger.py`

 * *Files identical despite different names*

### Comparing `teedoc-1.8.4/teedoc/static/js/live.js` & `teedoc-1.9.0/teedoc/static/js/live.js`

 * *Files identical despite different names*

### Comparing `teedoc-1.8.4/teedoc/teedoc_main.py` & `teedoc-1.9.0/teedoc/teedoc_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -618,27 +618,28 @@
                     {}
                 </div>
             </div>'''.format(footer_top, footer_bottom)
         html["footer"] = footer_html
         htmls[file] = html
     return htmls
 
-def construct_html(htmls, header_items_in, js_items_in, site_config, sidebar_list, doc_config):
+def construct_html(htmls, header_items_in, js_items_in, site_config, sidebar_list, doc_config, doc_src_path):
     '''
         @htmls  {
             "title": "",
             "desc": "",
             "keywords": [],
             "tags": [],
             "body": "",
             "toc": "",
             "sidebar": "",
             "navbar": ""
             "metadata": {},
-            "footer": ""
+            "footer": "",
+            "show_source": "Edit this page" or no this key
         }
     '''
     files = {}
     items = list(htmls.items())
     for i, (file, html) in enumerate(items):
         if not html:
             files[file] = None
@@ -664,25 +665,38 @@
                         previous_item_html = '<a href="{}"><span class="icon"></span><span class="label">{}</span></a>'.format(sidebar_list[file]["previous"][0], sidebar_list[file]["previous"][1])
                     if sidebar_list[file]["next"]:
                         next_item_html = '<a href="{}"><span class="label">{}</span><span class="icon"></span></a>'.format(sidebar_list[file]["next"][0], sidebar_list[file]["next"][1])
                 menu_html = '''<div id="menu_wrapper">
                                     <div id="menu">
                                     </div>
                                 </div>'''
+                if "show_source" in html:
+                    source_url = site_config["source"]
+                    if source_url.endswith("/"):
+                        source_url = source_url[:-1]
+                    source_url += file.replace(doc_src_path, "")
+                    source_html = '''<div id="source_link"><a href="{}" target="_blank">{}</a></div>'''.format(
+                                    source_url, html["show_source"]
+                    )
+                else:
+                    source_html = ""
                 body_html = '''
         <div id="wrapper">
             {}
             {}
             <div id="article">
                 <div id="content_wrapper">
                     <div id="content_body">
-                        <div id="article_title">
-                            <h1>{}</h1>
-                        </div>
-                        <div id="article_tags">
+                        <div id="article_head">
+                            <div id="article_title">
+                                <h1>{}</h1>
+                            </div>
+                            <div id="article_tags">
+                                {}
+                            </div>
                             {}
                         </div>
                         <div id="article_content">
                             {}
                         </div>
                     </div>
                     <div id="previous_next">
@@ -705,14 +719,15 @@
         <div id="doc_footer">
                         {}
                     </div>'''.format(
                         html["sidebar"],
                         menu_html,
                         article_title,
                         tags_html,
+                        source_html,
                         html["body"],
                         previous_item_html, 
                         next_item_html,
                         html["toc"] if "toc" in html else "",
                         footer_html,
                 )
             else: # not "sidebar" in html
@@ -823,14 +838,48 @@
     if "class" in html["metadata"]:
         classes.extend(html["metadata"]["class"].split(","))
     if "" in classes:
         classes.remove("")
     html_start = '<html {} {}>'.format(f'id="{id}"' if id else "", 'class="{}"'.format(" ".join(classes)) if classes else "")
     return html_start
 
+def htmls_add_source(htmls, repo_addr, label):
+    '''
+        @htmls {
+            "file_path": {
+                "metadata": {
+                    "show_source": "Edit this page"
+                }
+            }
+        }
+        @repo_addr https://github.com/teedoc/teedoc
+
+        @return {
+            "file_path": {
+                "metadata": {
+                    "show_source": "Edit this page"
+                },
+                "show_source": "Edit this page"
+            }
+        }
+    '''
+    if not repo_addr:
+        return htmls
+    for file, v in htmls.items():
+        # not show source
+        if "show_source" in v["metadata"]:
+            show_source = v["metadata"]["show_source"].strip().lower()
+            if show_source == "false":
+                continue
+            elif show_source != "true":
+                label = v["metadata"]["show_source"]
+        htmls[file]["show_source"] = label
+
+    return htmls
+
 def parse(name, plugin_func, routes, site_config, doc_src_path, config_template_dir, log, out_dir, plugins_objs, header_items, js_items, sidebar, allow_no_navbar, update_files):
     '''
         @return {
             "doc_url", {
                 "page_url": {
                     "title": "",
                     "desc": "",
@@ -909,15 +958,19 @@
                     in_path = in_path[:-1]
                 if out_path.endswith("/"):
                     out_path = out_path[:-1]
                 # call plugins to parse files
                 result_htmls = {}
                 for plugin in plugins_objs:
                     # parse file content
-                    result = plugin.__getattribute__(plugin_func)(files)
+                    if plugin.name in plugins_new_config:
+                        new_config = plugins_new_config[plugin.name]["config"]
+                    else:
+                        new_config = {}
+                    result = plugin.__getattribute__(plugin_func)(files, new_config=new_config)
                     if result:
                         if not result['ok']:
                             log.e("plugin <{}> {} error: {}".format(plugin.name, plugin_func, result['msg']))
                             on_err()
                             return False
                         else:
                             for key in result['htmls']:
@@ -946,16 +999,26 @@
                 # generate navbar to html
                 if navbar:
                     htmls = generate_navbar_html(htmls, navbar, dir, url, plugins_objs, plugins_new_config)
                 if footer:
                     htmls = generate_footer_html(htmls, footer, dir, url, plugins_objs)
                 if is_err():
                     return False
+                # show source code url
+                if "source" in site_config:
+                    label = None
+                    if not "show_source" in doc_config:
+                        label = "Edit this page"
+                    elif doc_config["show_source"]:
+                        label = doc_config["show_source"]
+                    if label:
+                        htmls = htmls_add_source(htmls, site_config["source"], label)
+
                 # consturct html page
-                htmls_str = construct_html(htmls, header_items, js_items, site_config, sidebar_list, doc_config)
+                htmls_str = construct_html(htmls, header_items, js_items, site_config, sidebar_list, doc_config, doc_src_path)
                 if is_err():
                     return False
                 # check abspath
                 if site_root_url != "/":
                     htmls_str = update_html_abs_path(htmls_str, site_root_url)
                 if is_err():
                     return False
@@ -1200,15 +1263,15 @@
             log.i("convert json from yaml complete, file at: {}".format(json_path))
         return 0
     t = None
     t2 = None
     while 1: # for rebuild all files
         try:
             # doc source code root path
-            doc_src_path = os.path.abspath(args.dir)
+            doc_src_path = os.path.abspath(args.dir).replace("\\", "/")
             # parse site config
             ok, site_config = parse_site_config(doc_src_path)
             if not ok:
                 log.e(site_config)
                 return 1
             if "config_template_dir" in site_config:
                 config_template_dir = os.path.abspath(os.path.join(doc_src_path, site_config["config_template_dir"]))
```

