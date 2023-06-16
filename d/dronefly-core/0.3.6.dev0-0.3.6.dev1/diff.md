# Comparing `tmp/dronefly_core-0.3.6.dev0.tar.gz` & `tmp/dronefly_core-0.3.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_core-0.3.6.dev0.tar", max compression
+gzip compressed data, was "dronefly_core-0.3.6.dev1.tar", max compression
```

## Comparing `dronefly_core-0.3.6.dev0.tar` & `dronefly_core-0.3.6.dev1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev0/LICENSE
--rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev0/README.md
--rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev0/dronefly/core/__init__.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev0/dronefly/core/clients/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev0/dronefly/core/clients/inat.py
--rw-r--r--   0        0        0     6065 2023-06-03 17:20:18.843066 dronefly_core-0.3.6.dev0/dronefly/core/commands/__init__.py
--rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev0/dronefly/core/constants.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev0/dronefly/core/formatters/__init__.py
--rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev0/dronefly/core/formatters/constants.py
--rw-r--r--   0        0        0    29903 2023-06-03 20:23:10.683148 dronefly_core-0.3.6.dev0/dronefly/core/formatters/generic.py
--rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev0/dronefly/core/models/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev0/dronefly/core/models/controlled_terms.py
--rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev0/dronefly/core/models/user.py
--rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev0/dronefly/core/parsers/__init__.py
--rw-r--r--   0        0        0     3672 2023-03-06 21:18:23.821142 dronefly_core-0.3.6.dev0/dronefly/core/parsers/constants.py
--rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev0/dronefly/core/parsers/natural.py
--rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev0/dronefly/core/parsers/unixlike.py
--rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev0/dronefly/core/parsers/url.py
--rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev0/dronefly/core/query/__init__.py
--rw-r--r--   0        0        0    19236 2023-04-16 13:38:29.366402 dronefly_core-0.3.6.dev0/dronefly/core/query/query.py
--rw-r--r--   0        0        0      527 2023-04-22 12:12:03.306747 dronefly_core-0.3.6.dev0/dronefly/core/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-06-03 20:27:06.376039 dronefly_core-0.3.6.dev0/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev0/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0    56815 2023-04-16 13:37:18.956988 dronefly_core-0.3.6.dev1/LICENSE
+-rw-r--r--   0        0        0      702 2023-01-28 19:16:26.368426 dronefly_core-0.3.6.dev1/README.md
+-rw-r--r--   0        0        0       53 2023-01-29 15:27:41.654095 dronefly_core-0.3.6.dev1/dronefly/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev1/dronefly/core/clients/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-13 15:05:57.725989 dronefly_core-0.3.6.dev1/dronefly/core/clients/inat.py
+-rw-r--r--   0        0        0     7532 2023-06-16 17:33:58.906636 dronefly_core-0.3.6.dev1/dronefly/core/commands/__init__.py
+-rw-r--r--   0        0        0      635 2023-03-19 08:14:11.111276 dronefly_core-0.3.6.dev1/dronefly/core/constants.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.620333 dronefly_core-0.3.6.dev1/dronefly/core/formatters/__init__.py
+-rw-r--r--   0        0        0      445 2023-04-16 10:53:39.829302 dronefly_core-0.3.6.dev1/dronefly/core/formatters/constants.py
+-rw-r--r--   0        0        0    29903 2023-06-03 20:23:10.683148 dronefly_core-0.3.6.dev1/dronefly/core/formatters/generic.py
+-rw-r--r--   0        0        0        0 2022-05-23 14:14:52.624333 dronefly_core-0.3.6.dev1/dronefly/core/models/__init__.py
+-rw-r--r--   0        0        0     1753 2023-04-09 09:38:32.529718 dronefly_core-0.3.6.dev1/dronefly/core/models/controlled_terms.py
+-rw-r--r--   0        0        0      188 2023-03-13 15:15:33.501579 dronefly_core-0.3.6.dev1/dronefly/core/models/user.py
+-rw-r--r--   0        0        0       49 2023-01-29 15:28:49.919496 dronefly_core-0.3.6.dev1/dronefly/core/parsers/__init__.py
+-rw-r--r--   0        0        0     3721 2023-06-14 15:48:19.092273 dronefly_core-0.3.6.dev1/dronefly/core/parsers/constants.py
+-rw-r--r--   0        0        0     9291 2023-02-18 13:51:02.476816 dronefly_core-0.3.6.dev1/dronefly/core/parsers/natural.py
+-rw-r--r--   0        0        0     6329 2023-03-19 08:21:31.268129 dronefly_core-0.3.6.dev1/dronefly/core/parsers/unixlike.py
+-rw-r--r--   0        0        0     2346 2023-01-29 15:35:29.175688 dronefly_core-0.3.6.dev1/dronefly/core/parsers/url.py
+-rw-r--r--   0        0        0       51 2023-01-29 15:27:27.497804 dronefly_core-0.3.6.dev1/dronefly/core/query/__init__.py
+-rw-r--r--   0        0        0    19768 2023-06-14 16:36:34.575475 dronefly_core-0.3.6.dev1/dronefly/core/query/query.py
+-rw-r--r--   0        0        0      527 2023-06-16 17:08:24.162383 dronefly_core-0.3.6.dev1/dronefly/core/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-16 19:09:05.170493 dronefly_core-0.3.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev1/setup.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 dronefly_core-0.3.6.dev1/PKG-INFO
```

### Comparing `dronefly_core-0.3.6.dev0/LICENSE` & `dronefly_core-0.3.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/README.md` & `dronefly_core-0.3.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/clients/inat.py` & `dronefly_core-0.3.6.dev1/dronefly/core/clients/inat.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/commands/__init__.py` & `dronefly_core-0.3.6.dev1/dronefly/core/commands/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -92,14 +92,53 @@
             rich_markdown = re.sub(RICH_NO_BQ_NEWLINE_PAT, r"\1 \\\n", rich_markdown)
             response = Markdown(rich_markdown)
         else:
             # Return the literal markdown for Discord to render
             response = markdown_text
         return response
 
+    def life(self, ctx: Context, *args):
+        main_query_str = None
+        taxon = None
+        per = None
+        if args:
+            query = self._parse(" ".join(args))
+            # TODO: Handle all query clauses, not just main.terms
+            # TODO: Doesn't do any ranking or filtering of results
+            if not query.main or not query.main.terms:
+                return "Not a taxon"
+            main_query_str = " ".join(query.main.terms)
+            per = query.per
+
+        with self.inat_client.set_ctx(ctx) as client:
+            params = {
+                "user_id": ctx.author.inat_user_id,
+            }
+            if main_query_str:
+                taxon = client.taxa.autocomplete(q=main_query_str).one()
+                if not taxon:
+                    return "No taxon found"
+                params["taxon_id"] = taxon.id
+            life_list = client.observations.life_list(**params)
+
+        thing = f"taxa in {taxon.name}" if taxon else "taxa"
+        rank = None
+        taxa = life_list.data
+        if per:
+            # A bit simplistic - just assume it's a rank with no validation
+            rank = per
+            taxa = [
+                life_list_taxon
+                for life_list_taxon in life_list.data
+                if life_list_taxon.rank == rank
+            ]
+        _rank = f"rank {rank}" if rank else "any rank"
+        response = f"Your life list has {len(taxa)} {thing} with {_rank}"
+        return response
+
     def taxon(self, ctx: Context, *args):
         query = self._parse(" ".join(args))
         # TODO: Handle all query clauses, not just main.terms
         # TODO: Doesn't do any ranking or filtering of results
         if not query.main or not query.main.terms:
             return "Not a taxon"
         main_query_str = " ".join(query.main.terms)
```

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/constants.py` & `dronefly_core-0.3.6.dev1/dronefly/core/constants.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/formatters/generic.py` & `dronefly_core-0.3.6.dev1/dronefly/core/formatters/generic.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/models/controlled_terms.py` & `dronefly_core-0.3.6.dev1/dronefly/core/models/controlled_terms.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/parsers/constants.py` & `dronefly_core-0.3.6.dev1/dronefly/core/parsers/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,23 @@
     "not_id",
     "order",
     "order_by",
     "out_of_range",
     "page",
     "pcid",
     "photos",
+    "place_id",
     "popular",
+    "project_id",
     "q",
     "quality_grade",
     "rank",
     "search_on",
     "sounds",
     "taxon_geoprivacy",
     "taxon_ids",
     "threatened",
+    "user_id",
     "verifiable",
     "without_taxon_id",
     "year",
 ]
```

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/parsers/natural.py` & `dronefly_core-0.3.6.dev1/dronefly/core/parsers/natural.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/parsers/unixlike.py` & `dronefly_core-0.3.6.dev1/dronefly/core/parsers/unixlike.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/parsers/url.py` & `dronefly_core-0.3.6.dev1/dronefly/core/parsers/url.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/query/query.py` & `dronefly_core-0.3.6.dev1/dronefly/core/query/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,18 +389,30 @@
             if with_adjectives and self.adjectives:
                 _of.append(", ".join(self.adjectives))
             _of.append("taxa")
             _taxa_description.append(" ".join(_of))
         message += " ".join(_taxa_description)
         if self.project:
             message += " in " + self.project.title
+        elif self.options:
+            project_id = self.options.get("project_id")
+            if project_id:
+                message += " in project #" + project_id.replace(",", ", ")
         if self.place:
             message += " from " + self.place.display_name
+        elif self.options:
+            place_id = self.options.get("place_id")
+            if place_id:
+                message += " from place #" + place_id.replace(",", ", ")
         if self.user:
             message += " by " + format_user_name(self.user)
+        elif self.options:
+            user_id = self.options.get("user_id")
+            if user_id:
+                message += " by user #" + user_id.replace(",", ", ")
         if self.unobserved_by:
             message += " unobserved by " + format_user_name(self.unobserved_by)
         if self.id_by:
             message += " identified by " + format_user_name(self.id_by)
         if self.except_by:
             message += " except by " + format_user_name(self.except_by)
         if self.observed and self.observed.on or self.observed.d1 or self.observed.d2:
```

### Comparing `dronefly_core-0.3.6.dev0/dronefly/core/utils/__init__.py` & `dronefly_core-0.3.6.dev1/dronefly/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dronefly_core-0.3.6.dev0/pyproject.toml` & `dronefly_core-0.3.6.dev1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 exclude_dirs = ["tests"]
 
 [tool.flake8]
 max-line-length = 100
 
 [tool.poetry]
 name = "dronefly-core"
-version = "0.3.6.dev0"
+version = "0.3.6.dev1"
 description = "Core dronefly components"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
 	{ include = "dronefly/core" },
 ]
```

### Comparing `dronefly_core-0.3.6.dev0/setup.py` & `dronefly_core-0.3.6.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'html2markdown>=0.1.7,<0.2.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20',
  'rich>=10.9,<14']
 
 setup_kwargs = {
     'name': 'dronefly-core',
-    'version': '0.3.6.dev0',
+    'version': '0.3.6.dev1',
     'description': 'Core dronefly components',
     'long_description': "# Dronefly core\n\nThis is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io)\nDiscord bot's core components. We're not yet making version guarantees until\nit is more usable.\n\n# Related packages\n\n## Dronefly command-line client\n\nThe [dronefly-cli](https://github.com/dronefly-garden/dronefly-cli) command-line\nclient will provide a standalone text user interface that can perform a usable\nsubset of Dronefly Discord bot's capabilities, built solely with Dronefly core.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_core-0.3.6.dev0/PKG-INFO` & `dronefly_core-0.3.6.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-core
-Version: 0.3.6.dev0
+Version: 0.3.6.dev1
 Summary: Core dronefly components
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

