# Comparing `tmp/IMDBTraktSyncer-1.4.0.tar.gz` & `tmp/IMDBTraktSyncer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.4.0.tar", last modified: Thu Jun 15 16:35:22 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.4.1.tar", last modified: Fri Jun 16 06:53:55 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.4.0.tar` & `IMDBTraktSyncer-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.982344 IMDBTraktSyncer-1.4.0/
-drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.949346 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    30500 2023-06-15 15:31:26.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     8169 2023-06-15 15:55:40.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10272 2023-06-15 14:00:20.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    11171 2023-06-15 16:19:15.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:35:22.979354 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12090 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 16:35:22.000000 IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    12090 2023-06-15 16:35:22.981345 IMDBTraktSyncer-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    11344 2023-06-15 16:29:38.000000 IMDBTraktSyncer-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 16:35:22.982344 IMDBTraktSyncer-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-15 15:51:23.000000 IMDBTraktSyncer-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:53:54.999406 IMDBTraktSyncer-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-06-16 06:53:54.964782 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    30520 2023-06-16 06:25:27.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4440 2023-05-28 13:20:16.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4209 2023-06-05 07:44:01.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 06:09:12.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     8515 2023-06-16 06:46:42.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10272 2023-06-15 14:00:20.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    11171 2023-06-15 16:19:15.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-16 06:53:54.996406 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-16 06:53:54.000000 IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-06-16 06:53:54.998406 IMDBTraktSyncer-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-06-16 06:52:26.000000 IMDBTraktSyncer-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 06:53:54.999406 IMDBTraktSyncer-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-16 06:52:11.000000 IMDBTraktSyncer-1.4.1/setup.py
```

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,21 +310,21 @@
 
             # loop through each movie and TV show rating and submit rating on IMDB website
             for i, item in enumerate(imdb_ratings_to_set, 1):
                 year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                 print(f'Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
                 driver.get(f'https://www.imdb.com/title/{item["IMDB_ID"]}/')
                 
-                # Wait until rate button is located and scroll to it
-                button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
-                driver.execute_script("arguments[0].scrollIntoView(true);", button)
-
-                # click on "Rate" button and select rating option, then submit rating
-                button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                 try:
+                    # Wait until rate button is located and scroll to it
+                    button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
+                    driver.execute_script("arguments[0].scrollIntoView(true);", button)
+
+                    # click on "Rate" button and select rating option, then submit rating
+                    button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
                     element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
                     if element_rating_bar:
                         driver.execute_script("arguments[0].click();", button)
                         rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
                         driver.execute_script("arguments[0].click();", rating_option_element)
                         submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
                         submit_element.click()
```

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/imdbData.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,66 +121,71 @@
             if results:
                 media_type = results[0].get('type')
                 return media_type
         return None
 
     #Get IMDB Reviews
     driver.get('https://www.imdb.com/profile')
-    reviews_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")))
-    reviews_link.click()
-
     reviews = []
     errors_found_getting_imdb_reviews = False
-    while True:
-        try:
-            try:
-                review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
-            except (NoSuchElementException, TimeoutException):
-                # No review elements found. There are no reviews. Exit the loop without an error.
-                break
-            
-            for element in review_elements:
-                review = {}
-                # Extract review details
-                review['Title'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").text
-                review['Year'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header span").text.strip('()').split('–')[0].strip()
-                review['IMDB_ID'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").get_attribute("href").split('/')[4]
-                review['IMDBReviewID'] = element.get_attribute("data-review-id")
-                review['Comment'] = element.find_element(By.CSS_SELECTOR, ".content > .text").text.strip()
-                spoiler_warning_elements = element.find_elements(By.CSS_SELECTOR, ".spoiler-warning")
-                review['Spoiler'] = len(spoiler_warning_elements) > 0
-                # Get the media type using Trakt API
-                media_type = get_media_type(review['IMDB_ID'])
-                if media_type:
-                    review['Type'] = media_type
-                else:
-                    review['Type'] = 'unknown'
-
-                reviews.append(review)
+    try:
+        reviews_link = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")))
+        reviews_link.click()
 
+        while True:
             try:
-                # Check if "Next" link exists
-                next_link = driver.find_element(By.CSS_SELECTOR, "a.next-page")
-                if next_link.get_attribute("href") == "#":
-                    break  # No more pages, exit the loop
-
-                next_link.click()
-
-                # Wait until the URL changes
-                wait.until(EC.url_changes(current_url))
+                try:
+                    review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
+                except (NoSuchElementException, TimeoutException):
+                    # No review elements found. There are no reviews. Exit the loop without an error.
+                    break
                 
-                # Refresh review_elements
-                review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
-
-            except (NoSuchElementException, TimeoutException):
-                break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop without error.
-        except Exception as e:
-            errors_found_getting_imdb_reviews = True
-            print(f"Exception occurred while getting IMDB reviews: {type(e)}")
-            break
+                for element in review_elements:
+                    review = {}
+                    # Extract review details
+                    review['Title'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").text
+                    review['Year'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header span").text.strip('()').split('–')[0].strip()
+                    review['IMDB_ID'] = element.find_element(By.CSS_SELECTOR, ".lister-item-header a").get_attribute("href").split('/')[4]
+                    review['IMDBReviewID'] = element.get_attribute("data-review-id")
+                    review['Comment'] = element.find_element(By.CSS_SELECTOR, ".content > .text").text.strip()
+                    spoiler_warning_elements = element.find_elements(By.CSS_SELECTOR, ".spoiler-warning")
+                    review['Spoiler'] = len(spoiler_warning_elements) > 0
+                    # Get the media type using Trakt API
+                    media_type = get_media_type(review['IMDB_ID'])
+                    if media_type:
+                        review['Type'] = media_type
+                    else:
+                        review['Type'] = 'unknown'
+
+                    reviews.append(review)
+
+                try:
+                    # Check if "Next" link exists
+                    next_link = driver.find_element(By.CSS_SELECTOR, "a.next-page")
+                    if next_link.get_attribute("href") == "#":
+                        break  # No more pages, exit the loop
+
+                    next_link.click()
+
+                    # Wait until the URL changes
+                    wait.until(EC.url_changes(current_url))
+                    
+                    # Refresh review_elements
+                    review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
+
+                except (NoSuchElementException, TimeoutException):
+                    break  # "Next" link not found or timed out waiting for the 'Next' link, exit the loop without error.
+            except Exception as e:
+                errors_found_getting_imdb_reviews = True
+                print(f"Exception occurred while getting IMDB reviews: {type(e)}")
+                break
+    
+    except Exception as e:
+        errors_found_getting_imdb_reviews = True
+        print(f"Exception occurred while getting IMDB reviews: {type(e)}")
 
     # Filter out duplicate reviews for the same item based on ID
     filtered_reviews = []
     seen = set()
     for item in reviews:
         if item['IMDB_ID'] not in seen:
             seen.add(item['IMDB_ID'])
```

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.4.0
+Version: 1.4.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,14 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
-- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -99,14 +98,15 @@
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
```

### Comparing `IMDBTraktSyncer-1.4.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.4.1/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/LICENSE` & `IMDBTraktSyncer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.4.0/PKG-INFO` & `IMDBTraktSyncer-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.4.0
+Version: 1.4.1
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,14 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
-- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -99,14 +98,15 @@
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
```

### Comparing `IMDBTraktSyncer-1.4.0/README.md` & `IMDBTraktSyncer-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook
 - If IMDB requires a captcha on login, and you see "Not signed in" appear in the script, the captcha is likely the cause. To fix this, navigate to the IMDB website in your browser (preferably Chrome) from the same computer. If you're already logged in, log out and log back in. It may ask you to fill in a captcha. Complete the captcha and finish logging in. After successfully logging in on your browser, run the script again, and it should work. You may need to repeat this step once or twice if the issue persists. Adding a captcha solver to the script is being considered but not currently implemented. [Issue #2](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2)
 - If you see an error about having the incorrect version of Chromedriver, uninstall it by running the following command in the command line: `python -m pip uninstall chromedriver-py`. In your Chrome browser, go to Settings > About Chrome and check the prefix for your version (e.g., 112... or 111). If the prefix matches your Chrome version, navigate to the [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that matches the prefix for your Chrome version. Copy the version number you need (e.g 113.0.5672.63), then run the following command in the command line: `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct version of Chromedriver. Run the script again, and it should work. [Issue #16](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/16)
 - If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 - Due to IMDB's lack of API and rating import ability, this script uses an unconventional method that mimics using a web browser to set ratings on IMDB. Therefore, there are many points of failure that could arise. The script will be updated as best as possible.
-- Add optional setting to remove watched items from watchlists [Issue #44](https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/44)
 
 ## Screenshot
 ![Demo](https://i.imgur.com/QXCtGrr.png)
 
 ## Sponsorships, Donations, and Custom Projects
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -83,14 +82,15 @@
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
```

### Comparing `IMDBTraktSyncer-1.4.0/setup.py` & `IMDBTraktSyncer-1.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.4.0'
+VERSION = '1.4.1'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

