# Comparing `tmp/LuaAutoDoc-0.9.0.tar.gz` & `tmp/LuaAutoDoc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LuaAutoDoc-0.9.0.tar", last modified: Fri Jun 16 16:29:28 2023, max compression
+gzip compressed data, was "LuaAutoDoc-0.9.1.tar", last modified: Fri Jun 16 21:05:14 2023, max compression
```

## Comparing `LuaAutoDoc-0.9.0.tar` & `LuaAutoDoc-0.9.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.749530 LuaAutoDoc-0.9.0/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/CHANGELOG
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1080 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/LICENSE
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    15997 2023-06-16 16:29:28.000000 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/PKG-INFO
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4066 2023-06-16 16:29:28.000000 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/SOURCES.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        1 2023-06-16 16:29:28.000000 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       63 2023-06-16 16:29:28.000000 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/entry_points.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       13 2023-06-16 16:29:28.000000 LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/top_level.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      419 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/MANIFEST.in
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    15997 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/PKG-INFO
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    14896 2023-06-16 15:01:15.000000 LuaAutoDoc-0.9.0/README.md
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    10121 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/BuyMeACoffee.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    42414 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/DarkModeButton.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4681 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Deprecated.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      988 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Discord.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2308 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/FolderClosed.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2365 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/FolderOpen.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      960 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/GitHub.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2424 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/GitLab.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3166 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Internal.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4398 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/JetBrainsMono fonts LICENSE.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)   185552 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/JetBrainsMono-VariableFont_wght.ttf
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    41196 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LightModeButton.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2536 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LuaFile.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2541 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LuaFileLight.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2050 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Patreon.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1152 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/PayPal.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    11358 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/RobotoSlab font LICENSE.txt
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)   203852 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/RobotoSlab-VariableFont_wght.ttf
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1105 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Twitter.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4312 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Config_LuaAutoDoc.json
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    28428 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/android-chrome-192x192.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    57659 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/android-chrome-512x512.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    16222 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/apple-touch-icon.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      246 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/browserconfig.xml
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    12661 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/favicon-16x16.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    13873 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/favicon-32x32.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    11731 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/mstile-150x150.png
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9706 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/safari-pinned-tab.svg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      426 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/site.webmanifest
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.737530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1903 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFifthLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3705 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFourthLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      471 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateSecondLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      218 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateSixthLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1634 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateThirdLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      607 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CodeObject.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      789 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateFourthLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      650 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateSecondLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1399 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateThirdLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1346 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/decorators.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/main_page/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      765 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/main_page/index.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.741530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/search_page/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4591 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/search_page/search_page.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      530 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SCFM_TemplateSecondLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      609 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SCM_TemplateSecondLayer.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      750 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeFolderMap.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1167 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeMirror.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/templates/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      588 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/templates/Template.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/user_essentials/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       50 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/user_essentials/CustomNavbar.html
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      170 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/user_essentials/Mandatory_user_data.html
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1555 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/ElementSizeObserver.js
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      813 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/LuaAutoDoc.js
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3646 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/NavBarListHandler.js
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1023 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/SearchHandler.js
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3835 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/SourceCodeFolderMap.js
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    18348 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/ThemeChanger.js
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8061 2023-06-16 13:11:05.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/CodeObjects.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      247 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/GenericPages.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     6285 2023-06-14 17:56:07.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/LuaAutoDoc.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1295 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SearchPage.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9142 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SourceCode.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2029 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SourceCodeFolderMap.css
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/__init__.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    32951 2023-06-16 13:35:21.000000 LuaAutoDoc-0.9.0/lua_auto_doc/lua_auto_doc.py
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/modules/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/__init__.py
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    10320 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/LuaBuiltInCache.json
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/__init__.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9425 2023-06-16 13:35:21.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/highlighter.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    27745 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/indexer.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8809 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/indexer_support_functions.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    50735 2023-06-16 13:53:55.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/lua_type_indexer.py
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/__init__.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8654 2023-06-16 13:51:12.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/data_store_maker.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    26280 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/doc_maker.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3886 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/fragment_reader.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    49217 2023-06-16 13:54:19.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/tag_mapper.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9508 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/tag_mapper_support_functions.py
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/__init__.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    66055 2023-06-16 13:58:44.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/doc_classes.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    14626 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/lua_documentation_parser.py
-drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 16:29:28.745530 LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/__init__.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9425 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/config_handler.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      734 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/misc.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     7015 2023-06-16 13:36:55.000000 LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/progress_bar.py
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       38 2023-06-16 16:29:28.749530 LuaAutoDoc-0.9.0/setup.cfg
--rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2021 2023-06-16 16:20:57.000000 LuaAutoDoc-0.9.0/setup.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       89 2023-06-16 20:55:46.000000 LuaAutoDoc-0.9.1/CHANGELOG
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1080 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/LICENSE
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.114403 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    16000 2023-06-16 21:05:14.000000 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4066 2023-06-16 21:05:14.000000 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        1 2023-06-16 21:05:14.000000 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       63 2023-06-16 21:05:14.000000 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/entry_points.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       13 2023-06-16 21:05:14.000000 LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      419 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/MANIFEST.in
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    16000 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/PKG-INFO
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    14899 2023-06-16 20:02:53.000000 LuaAutoDoc-0.9.1/README.md
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.114403 LuaAutoDoc-0.9.1/lua_auto_doc/
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    10121 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/BuyMeACoffee.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    42414 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/DarkModeButton.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4681 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Deprecated.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      988 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Discord.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2308 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/FolderClosed.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2365 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/FolderOpen.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      960 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/GitHub.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2424 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/GitLab.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3166 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Internal.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4398 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/JetBrainsMono fonts LICENSE.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)   185552 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/JetBrainsMono-VariableFont_wght.ttf
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    41196 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LightModeButton.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2536 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LuaFile.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2541 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LuaFileLight.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2050 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Patreon.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1152 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/PayPal.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    11358 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/RobotoSlab font LICENSE.txt
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)   203852 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/RobotoSlab-VariableFont_wght.ttf
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1105 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Twitter.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4312 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Config_LuaAutoDoc.json
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    28428 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/android-chrome-192x192.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    57659 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/android-chrome-512x512.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    16222 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/apple-touch-icon.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      246 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/browserconfig.xml
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    12661 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/favicon-16x16.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    13873 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/favicon-32x32.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    11731 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/mstile-150x150.png
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9706 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/safari-pinned-tab.svg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      426 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/site.webmanifest
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.114403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1903 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFifthLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3705 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFourthLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      471 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateSecondLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      218 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateSixthLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1634 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateThirdLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      607 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CodeObject.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      789 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateFourthLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      650 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateSecondLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1399 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateThirdLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1346 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/decorators.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/main_page/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      765 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/main_page/index.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/search_page/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     4591 2023-06-16 20:25:13.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/search_page/search_page.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      530 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SCFM_TemplateSecondLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      609 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SCM_TemplateSecondLayer.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      750 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeFolderMap.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1167 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeMirror.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/templates/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      588 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/templates/Template.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/user_essentials/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       50 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/user_essentials/CustomNavbar.html
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      170 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/user_essentials/Mandatory_user_data.html
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.118403 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1555 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/ElementSizeObserver.js
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      813 2023-06-16 20:42:13.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/LuaAutoDoc.js
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3646 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/NavBarListHandler.js
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1023 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/SearchHandler.js
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3835 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/SourceCodeFolderMap.js
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    18348 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/ThemeChanger.js
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8061 2023-06-16 13:11:05.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/CodeObjects.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      247 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/GenericPages.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     6285 2023-06-14 17:56:07.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/LuaAutoDoc.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     1295 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SearchPage.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9142 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SourceCode.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2029 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SourceCodeFolderMap.css
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/__init__.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    32951 2023-06-16 13:35:21.000000 LuaAutoDoc-0.9.1/lua_auto_doc/lua_auto_doc.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/modules/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/__init__.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    10320 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/LuaBuiltInCache.json
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/__init__.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9425 2023-06-16 13:35:21.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/highlighter.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    27745 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/indexer.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8809 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/indexer_support_functions.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    50735 2023-06-16 13:53:55.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/lua_type_indexer.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/__init__.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     8654 2023-06-16 13:51:12.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/data_store_maker.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    26280 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/doc_maker.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     3886 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/fragment_reader.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    49217 2023-06-16 13:54:19.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/tag_mapper.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9508 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/tag_mapper_support_functions.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/__init__.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    66055 2023-06-16 13:58:44.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/doc_classes.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)    14626 2023-06-16 13:31:01.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/lua_documentation_parser.py
+drwxrwxr-x   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)        0 2023-06-14 10:05:26.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/__init__.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     9425 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/config_handler.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)      734 2023-06-16 13:28:44.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/misc.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     7015 2023-06-16 13:36:55.000000 LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/progress_bar.py
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)       38 2023-06-16 21:05:14.122403 LuaAutoDoc-0.9.1/setup.cfg
+-rw-rw-r--   0 ulrikhd   (1000) ulrikhd   (1000)     2021 2023-06-16 21:02:37.000000 LuaAutoDoc-0.9.1/setup.py
```

### Comparing `LuaAutoDoc-0.9.0/LICENSE` & `LuaAutoDoc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/PKG-INFO` & `LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LuaAutoDoc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Generates full HTML documentation of a Lua project with LuaDoc tags.
 Home-page: https://gitlab.com/UlrikHD/LuaAutoDoc
 Author: Ulrik Holtgaard Digerud
 Author-email: githubuhd@runbox.com
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/UlrikHD/LuaAutoDoc/-/issues
 Keywords: Lua,documentation,LuaDoc,HTML,LuaAutoDoc,autodoc,auto documentation,Lua documentation
@@ -150,16 +150,16 @@
    <li><code>\[abs_path: {path}]</code> - Will tell the script which file to search for the entry.</li>
    <li><code>\[rel_path: {path}]</code> - Will tell the script which file to search for the entry, relative to the 
    configured project root folder.</li>
    <li><code>\[module: {module_name}]</code> - Will tell the script which module to search for the function.</li>
 </ul>
   When trying to detect the correct reference, the script will search in the order: file -> module -> project.<br>
   Alternatively you can link to a webpage, webpage links are detected by starting with <code>https://</code> or
-<code>http://</code><br>**This tag can be used multiple times to add multiple links, and inside description docstrings 
-for inline references**<br>
+<code>http://</code><br><b>This tag can be used multiple times to add multiple links, and inside description docstrings 
+for inline references</b><br>
 Format: <code>--- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {description}</code>
 <br>or: 
 <code>--- @description {~fluff~} --- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {~fluff~}</code>
 </li>
 </ul>
   
 <h3> Error codes </h3>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LuaAutoDoc Version: 0.9.0 Summary: Generates full
+Metadata-Version: 2.1 Name: LuaAutoDoc Version: 0.9.1 Summary: Generates full
 HTML documentation of a Lua project with LuaDoc tags. Home-page: https://
 gitlab.com/UlrikHD/LuaAutoDoc Author: Ulrik Holtgaard Digerud Author-email:
 githubuhd@runbox.com License: MIT License Project-URL: Bug Tracker, https://
 gitlab.com/UlrikHD/LuaAutoDoc/-/issues Keywords:
 Lua,documentation,LuaDoc,HTML,LuaAutoDoc,autodoc,auto documentation,Lua
 documentation Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -165,16 +165,16 @@
             the entry, relative to the configured project root folder.
           o \[module: {module_name}] - Will tell the script which module to
             search for the function.
       When trying to detect the correct reference, the script will search in
       the order: file -> module -> project.
       Alternatively you can link to a webpage, webpage links are detected by
       starting with https:// or http://
-      **This tag can be used multiple times to add multiple links, and inside
-      description docstrings for inline references**
+      This tag can be used multiple times to add multiple links, and inside
+      description docstrings for inline references
       Format: --- @see {link} [link_text: 'text'](optional) {link_hint}
       (optional) {description}
       or: --- @description {~fluff~} --- @see {link} [link_text: 'text']
       (optional) {link_hint}(optional) {~fluff~}
 **** Error codes ****
     * SCH-0 - SourceCodeHighlighter.py could not locate SourceCodeMirror.html
       is either missing or your Config_LuaAutoDoc.py is misconfigured, and you
```

### Comparing `LuaAutoDoc-0.9.0/LuaAutoDoc.egg-info/SOURCES.txt` & `LuaAutoDoc-0.9.1/LuaAutoDoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/PKG-INFO` & `LuaAutoDoc-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LuaAutoDoc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Generates full HTML documentation of a Lua project with LuaDoc tags.
 Home-page: https://gitlab.com/UlrikHD/LuaAutoDoc
 Author: Ulrik Holtgaard Digerud
 Author-email: githubuhd@runbox.com
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/UlrikHD/LuaAutoDoc/-/issues
 Keywords: Lua,documentation,LuaDoc,HTML,LuaAutoDoc,autodoc,auto documentation,Lua documentation
@@ -150,16 +150,16 @@
    <li><code>\[abs_path: {path}]</code> - Will tell the script which file to search for the entry.</li>
    <li><code>\[rel_path: {path}]</code> - Will tell the script which file to search for the entry, relative to the 
    configured project root folder.</li>
    <li><code>\[module: {module_name}]</code> - Will tell the script which module to search for the function.</li>
 </ul>
   When trying to detect the correct reference, the script will search in the order: file -> module -> project.<br>
   Alternatively you can link to a webpage, webpage links are detected by starting with <code>https://</code> or
-<code>http://</code><br>**This tag can be used multiple times to add multiple links, and inside description docstrings 
-for inline references**<br>
+<code>http://</code><br><b>This tag can be used multiple times to add multiple links, and inside description docstrings 
+for inline references</b><br>
 Format: <code>--- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {description}</code>
 <br>or: 
 <code>--- @description {~fluff~} --- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {~fluff~}</code>
 </li>
 </ul>
   
 <h3> Error codes </h3>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LuaAutoDoc Version: 0.9.0 Summary: Generates full
+Metadata-Version: 2.1 Name: LuaAutoDoc Version: 0.9.1 Summary: Generates full
 HTML documentation of a Lua project with LuaDoc tags. Home-page: https://
 gitlab.com/UlrikHD/LuaAutoDoc Author: Ulrik Holtgaard Digerud Author-email:
 githubuhd@runbox.com License: MIT License Project-URL: Bug Tracker, https://
 gitlab.com/UlrikHD/LuaAutoDoc/-/issues Keywords:
 Lua,documentation,LuaDoc,HTML,LuaAutoDoc,autodoc,auto documentation,Lua
 documentation Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -165,16 +165,16 @@
             the entry, relative to the configured project root folder.
           o \[module: {module_name}] - Will tell the script which module to
             search for the function.
       When trying to detect the correct reference, the script will search in
       the order: file -> module -> project.
       Alternatively you can link to a webpage, webpage links are detected by
       starting with https:// or http://
-      **This tag can be used multiple times to add multiple links, and inside
-      description docstrings for inline references**
+      This tag can be used multiple times to add multiple links, and inside
+      description docstrings for inline references
       Format: --- @see {link} [link_text: 'text'](optional) {link_hint}
       (optional) {description}
       or: --- @description {~fluff~} --- @see {link} [link_text: 'text']
       (optional) {link_hint}(optional) {~fluff~}
 **** Error codes ****
     * SCH-0 - SourceCodeHighlighter.py could not locate SourceCodeMirror.html
       is either missing or your Config_LuaAutoDoc.py is misconfigured, and you
```

### Comparing `LuaAutoDoc-0.9.0/README.md` & `LuaAutoDoc-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,16 @@
    <li><code>\[abs_path: {path}]</code> - Will tell the script which file to search for the entry.</li>
    <li><code>\[rel_path: {path}]</code> - Will tell the script which file to search for the entry, relative to the 
    configured project root folder.</li>
    <li><code>\[module: {module_name}]</code> - Will tell the script which module to search for the function.</li>
 </ul>
   When trying to detect the correct reference, the script will search in the order: file -> module -> project.<br>
   Alternatively you can link to a webpage, webpage links are detected by starting with <code>https://</code> or
-<code>http://</code><br>**This tag can be used multiple times to add multiple links, and inside description docstrings 
-for inline references**<br>
+<code>http://</code><br><b>This tag can be used multiple times to add multiple links, and inside description docstrings 
+for inline references</b><br>
 Format: <code>--- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {description}</code>
 <br>or: 
 <code>--- @description {~fluff~} --- @see {link} [link_text: 'text'](optional) {link_hint}(optional) {~fluff~}</code>
 </li>
 </ul>
   
 <h3> Error codes </h3>
```

#### html2text {}

```diff
@@ -150,16 +150,16 @@
             the entry, relative to the configured project root folder.
           o \[module: {module_name}] - Will tell the script which module to
             search for the function.
       When trying to detect the correct reference, the script will search in
       the order: file -> module -> project.
       Alternatively you can link to a webpage, webpage links are detected by
       starting with https:// or http://
-      **This tag can be used multiple times to add multiple links, and inside
-      description docstrings for inline references**
+      This tag can be used multiple times to add multiple links, and inside
+      description docstrings for inline references
       Format: --- @see {link} [link_text: 'text'](optional) {link_hint}
       (optional) {description}
       or: --- @description {~fluff~} --- @see {link} [link_text: 'text']
       (optional) {link_hint}(optional) {~fluff~}
 **** Error codes ****
     * SCH-0 - SourceCodeHighlighter.py could not locate SourceCodeMirror.html
       is either missing or your Config_LuaAutoDoc.py is misconfigured, and you
```

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/BuyMeACoffee.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/BuyMeACoffee.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/DarkModeButton.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/DarkModeButton.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Deprecated.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Deprecated.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Discord.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Discord.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/FolderClosed.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/FolderClosed.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/FolderOpen.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/FolderOpen.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/GitHub.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/GitHub.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/GitLab.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/GitLab.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Internal.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Internal.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/JetBrainsMono fonts LICENSE.txt` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/JetBrainsMono fonts LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/JetBrainsMono-VariableFont_wght.ttf` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/JetBrainsMono-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LightModeButton.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LightModeButton.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LuaFile.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LuaFile.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/LuaFileLight.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/LuaFileLight.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Patreon.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Patreon.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/PayPal.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/PayPal.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/RobotoSlab font LICENSE.txt` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/RobotoSlab font LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/RobotoSlab-VariableFont_wght.ttf` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/RobotoSlab-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Assets/Twitter.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Assets/Twitter.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Config_LuaAutoDoc.json` & `LuaAutoDoc-0.9.1/lua_auto_doc/Config_LuaAutoDoc.json`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/android-chrome-192x192.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/android-chrome-512x512.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/apple-touch-icon.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/favicon-16x16.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/favicon-32x32.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/mstile-150x150.png` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Favicon/safari-pinned-tab.svg` & `LuaAutoDoc-0.9.1/lua_auto_doc/Favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFifthLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFifthLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFourthLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateFourthLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateThirdLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CO_TemplateThirdLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/code_objects/CodeObject.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/code_objects/CodeObject.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateFourthLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateFourthLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateSecondLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateSecondLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/EX_TemplateThirdLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/EX_TemplateThirdLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/extra/decorators.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/extra/decorators.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/main_page/index.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/main_page/index.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/search_page/search_page.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/search_page/search_page.html`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 	<script>
 		// Get the query from the URL
 		let params = new URLSearchParams(window.location.search);
 		let query = params.get('q');
 
 		// Fetch the datastore.json file
-		fetch('../data/datastore.json')
+		fetch('../data/DataStore.json')
 			.then(response => response.json())
 			.then(data => {
 				// Split the query into words and phrases
 				let queryWords = splitQuery(query);
 
 				// Search the index for the query
 				let results = Object.keys(data)
```

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SCFM_TemplateSecondLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SCFM_TemplateSecondLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SCM_TemplateSecondLayer.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SCM_TemplateSecondLayer.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeFolderMap.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeFolderMap.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeMirror.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/source_code_mirror/SourceCodeMirror.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/HTMLFragments/templates/Template.html` & `LuaAutoDoc-0.9.1/lua_auto_doc/HTMLFragments/templates/Template.html`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/ElementSizeObserver.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/ElementSizeObserver.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/LuaAutoDoc.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/LuaAutoDoc.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/NavBarListHandler.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/NavBarListHandler.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/SearchHandler.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/SearchHandler.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/SourceCodeFolderMap.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/SourceCodeFolderMap.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/Scripts/ThemeChanger.js` & `LuaAutoDoc-0.9.1/lua_auto_doc/Scripts/ThemeChanger.js`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/CodeObjects.css` & `LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/CodeObjects.css`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/LuaAutoDoc.css` & `LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/LuaAutoDoc.css`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SearchPage.css` & `LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SearchPage.css`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SourceCode.css` & `LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SourceCode.css`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/StyleSheets/SourceCodeFolderMap.css` & `LuaAutoDoc-0.9.1/lua_auto_doc/StyleSheets/SourceCodeFolderMap.css`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/lua_auto_doc.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/lua_auto_doc.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/LuaBuiltInCache.json` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/LuaBuiltInCache.json`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/highlighter.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/highlighter.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/indexer.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/indexer.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/indexer_support_functions.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/indexer_support_functions.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/highlighter/lua_type_indexer.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/highlighter/lua_type_indexer.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/data_store_maker.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/data_store_maker.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/doc_maker.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/doc_maker.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/fragment_reader.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/fragment_reader.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/tag_mapper.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/tag_mapper.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/html_handler/tag_mapper_support_functions.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/html_handler/tag_mapper_support_functions.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/doc_classes.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/doc_classes.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/lua_parser/lua_documentation_parser.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/lua_parser/lua_documentation_parser.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/config_handler.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/config_handler.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/misc.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/misc.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/lua_auto_doc/modules/tools/progress_bar.py` & `LuaAutoDoc-0.9.1/lua_auto_doc/modules/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `LuaAutoDoc-0.9.0/setup.py` & `LuaAutoDoc-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name='LuaAutoDoc',
-    version='0.9.0',
+    version='0.9.1',
     description='Generates full HTML documentation of a Lua project with LuaDoc tags.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://gitlab.com/UlrikHD/LuaAutoDoc',
     project_urls={
         'Bug Tracker': 'https://gitlab.com/UlrikHD/LuaAutoDoc/-/issues',
     },
```

