# Comparing `tmp/pyqt-openai-0.1.61.tar.gz` & `tmp/pyqt-openai-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-openai-0.1.61.tar", last modified: Tue Jun  6 13:44:24 2023, max compression
+gzip compressed data, was "pyqt-openai-0.1.72.tar", last modified: Fri Jun 16 09:01:23 2023, max compression
```

## Comparing `pyqt-openai-0.1.61.tar` & `pyqt-openai-0.1.72.tar`

### file list

```diff
@@ -1,88 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.640789 pyqt-openai-0.1.61/
--rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.61/LICENSE
--rw-rw-rw-   0        0        0     9704 2023-06-06 13:44:24.638794 pyqt-openai-0.1.61/PKG-INFO
--rw-rw-rw-   0        0        0     9222 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.268123 pyqt-openai-0.1.61/pyqt_openai/
--rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/__init__.py
--rw-rw-rw-   0        0        0     6737 2023-06-04 01:26:54.000000 pyqt-openai-0.1.61/pyqt_openai/a.py
--rw-rw-rw-   0        0        0     2756 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/aboutDialog.py
--rw-rw-rw-   0        0        0     2144 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/apiData.py
--rw-rw-rw-   0        0        0    16579 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/chatWidget.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/circleProfileImage.py
--rw-rw-rw-   0        0        0     3337 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/commandCompleter.py
--rw-rw-rw-   0        0        0     5078 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/convListWidget.py
--rw-rw-rw-   0        0        0     7574 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/customizeDialog.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.459606 pyqt-openai-0.1.61/pyqt_openai/ico/
--rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.61/pyqt_openai/ico/__init__.py
--rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/add.svg
--rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.61/pyqt_openai/ico/close.svg
--rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/ico/customize.svg
--rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/delete.svg
--rw-rw-rw-   0        0        0     1542 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/discord.svg
--rw-rw-rw-   0        0        0     1552 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/github.svg
--rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/help.svg
--rw-rw-rw-   0        0        0      712 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/history.svg
--rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.61/pyqt_openai/ico/openai.svg
--rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/ico/prompt.svg
--rw-rw-rw-   0        0        0      654 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/ico/save.svg
--rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/search.svg
--rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/ico/setting.svg
--rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.61/pyqt_openai/ico/sidebar.svg
--rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.61/pyqt_openai/ico/stackontop.svg
--rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.61/pyqt_openai/ico/user.svg
--rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.61/pyqt_openai/ico/vertical_three_dots.svg
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.526531 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/
--rw-rw-rw-   0        0        0        0 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/currentImageView.py
--rw-rw-rw-   0        0        0     1735 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/explorerWidget.py
--rw-rw-rw-   0        0        0     3581 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageDallEPage.py
--rw-rw-rw-   0        0        0     4558 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py
--rw-rw-rw-   0        0        0     5090 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageListWidget.py
--rw-rw-rw-   0        0        0    18549 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageSqlite.py
--rw-rw-rw-   0        0        0    11118 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
--rw-rw-rw-   0        0        0     3867 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/leftSideBar.py
--rw-rw-rw-   0        0        0     1077 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/rightSideBar.py
--rw-rw-rw-   0        0        0     4044 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/thumbnailView.py
--rw-rw-rw-   0        0        0     2229 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/viewWidget.py
--rw-rw-rw-   0        0        0     1444 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/inputDialog.py
--rw-rw-rw-   0        0        0     3764 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/leftSideBar.py
--rw-rw-rw-   0        0        0    11458 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/main.py
--rw-rw-rw-   0        0        0     1787 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/modelTable.py
--rw-rw-rw-   0        0        0     3293 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/notifier.py
--rw-rw-rw-   0        0        0    11028 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/openAiChatBotWidget.py
--rw-rw-rw-   0        0        0     3048 2023-06-03 03:53:41.000000 pyqt-openai-0.1.61/pyqt_openai/openAiThread.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.542478 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/
--rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/__init__.py
--rw-rw-rw-   0        0        0     2423 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py
--rw-rw-rw-   0        0        0     1768 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py
--rw-rw-rw-   0        0        0     9467 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPage.py
--rw-rw-rw-   0        0        0     1755 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py
--rw-rw-rw-   0        0        0     9492 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePage.py
--rw-rw-rw-   0        0        0     1778 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.547452 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/
--rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/__init__.py
--rw-rw-rw-   0        0        0      988 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/commandSuggestionWidget.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.591924 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/
--rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/__init__.py
--rw-rw-rw-   0        0        0     2060 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
--rw-rw-rw-   0        0        0     4706 2023-05-05 03:03:16.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/chatPage.py
--rw-rw-rw-   0        0        0    10982 2023-05-20 05:39:27.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/completionPage.py
--rw-rw-rw-   0        0        0     1623 2023-05-07 22:16:16.000000 pyqt-openai-0.1.61/pyqt_openai/right_sidebar/imagePage.py
--rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.61/pyqt_openai/searchBar.py
--rw-rw-rw-   0        0        0   112813 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/sqlite.py
--rw-rw-rw-   0        0        0     5934 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/svgButton.py
--rw-rw-rw-   0        0        0      738 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/svgLabel.py
--rw-rw-rw-   0        0        0     5951 2023-06-06 02:12:45.000000 pyqt-openai-0.1.61/pyqt_openai/svgToolButton.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.635806 pyqt-openai-0.1.61/pyqt_openai/test/
--rw-rw-rw-   0        0        0        0 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/htmlformat.py
--rw-rw-rw-   0        0        0      761 2023-05-21 02:10:54.000000 pyqt-openai-0.1.61/pyqt_openai/test/sqlalchemy_example.py
--rw-rw-rw-   0        0        0     4884 2023-06-06 13:23:05.000000 pyqt-openai-0.1.61/pyqt_openai/toast.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:44:24.306025 pyqt-openai-0.1.61/pyqt_openai.egg-info/
--rw-rw-rw-   0        0        0     9704 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2629 2023-06-06 13:44:24.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 13:44:23.000000 pyqt-openai-0.1.61/pyqt_openai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 13:44:24.641788 pyqt-openai-0.1.61/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-06-06 13:44:08.000000 pyqt-openai-0.1.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.470410 pyqt-openai-0.1.72/
+-rw-rw-rw-   0        0        0     1091 2023-02-05 10:57:11.000000 pyqt-openai-0.1.72/LICENSE
+-rw-rw-rw-   0        0        0    10567 2023-06-16 09:01:23.469412 pyqt-openai-0.1.72/PKG-INFO
+-rw-rw-rw-   0        0        0    10062 2023-06-16 09:00:57.000000 pyqt-openai-0.1.72/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:22.960713 pyqt-openai-0.1.72/pyqt_openai/
+-rw-rw-rw-   0        0        0       25 2023-05-05 02:56:55.000000 pyqt-openai-0.1.72/pyqt_openai/__init__.py
+-rw-rw-rw-   0        0        0     6737 2023-06-04 01:26:54.000000 pyqt-openai-0.1.72/pyqt_openai/a.py
+-rw-rw-rw-   0        0        0     2756 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/aboutDialog.py
+-rw-rw-rw-   0        0        0     1958 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/apiData.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.064049 pyqt-openai-0.1.72/pyqt_openai/chat_widget/
+-rw-rw-rw-   0        0        0       37 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/aiChatUnit.py
+-rw-rw-rw-   0        0        0     4629 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/chatBrowser.py
+-rw-rw-rw-   0        0        0     7317 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/prompt.py
+-rw-rw-rw-   0        0        0     1254 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/textEditPrompt.py
+-rw-rw-rw-   0        0        0     3576 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/textEditPropmtGroup.py
+-rw-rw-rw-   0        0        0     1677 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/chat_widget/userChatUnit.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 23:44:44.000000 pyqt-openai-0.1.72/pyqt_openai/circleProfileImage.py
+-rw-rw-rw-   0        0        0     3287 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/commandCompleter.py
+-rw-rw-rw-   0        0        0     5078 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/convListWidget.py
+-rw-rw-rw-   0        0        0     7574 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/customizeDialog.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.222317 pyqt-openai-0.1.72/pyqt_openai/ico/
+-rw-rw-rw-   0        0        0        0 2023-03-05 08:26:40.000000 pyqt-openai-0.1.72/pyqt_openai/ico/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-04-22 00:05:31.000000 pyqt-openai-0.1.72/pyqt_openai/ico/add.svg
+-rw-rw-rw-   0        0        0      526 2023-03-18 12:17:19.000000 pyqt-openai-0.1.72/pyqt_openai/ico/close.svg
+-rw-rw-rw-   0        0        0      504 2023-06-16 09:00:57.000000 pyqt-openai-0.1.72/pyqt_openai/ico/copy.svg
+-rw-rw-rw-   0        0        0      518 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/copy_light.svg
+-rw-rw-rw-   0        0        0      823 2023-05-05 23:44:44.000000 pyqt-openai-0.1.72/pyqt_openai/ico/customize.svg
+-rw-rw-rw-   0        0        0      215 2023-04-22 00:05:31.000000 pyqt-openai-0.1.72/pyqt_openai/ico/delete.svg
+-rw-rw-rw-   0        0        0     1542 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/discord.svg
+-rw-rw-rw-   0        0        0     1552 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/github.svg
+-rw-rw-rw-   0        0        0      839 2023-03-18 12:14:31.000000 pyqt-openai-0.1.72/pyqt_openai/ico/help.svg
+-rw-rw-rw-   0        0        0      712 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/history.svg
+-rw-rw-rw-   0        0        0     1355 2023-02-26 06:14:05.000000 pyqt-openai-0.1.72/pyqt_openai/ico/openai.svg
+-rw-rw-rw-   0        0        0      501 2023-05-05 02:56:55.000000 pyqt-openai-0.1.72/pyqt_openai/ico/prompt.svg
+-rw-rw-rw-   0        0        0      654 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/save.svg
+-rw-rw-rw-   0        0        0      669 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/ico/save_light.svg
+-rw-rw-rw-   0        0        0     1039 2023-04-22 00:05:31.000000 pyqt-openai-0.1.72/pyqt_openai/ico/search.svg
+-rw-rw-rw-   0        0        0     1283 2023-04-22 00:05:31.000000 pyqt-openai-0.1.72/pyqt_openai/ico/setting.svg
+-rw-rw-rw-   0        0        0      247 2023-03-19 00:44:25.000000 pyqt-openai-0.1.72/pyqt_openai/ico/sidebar.svg
+-rw-rw-rw-   0        0        0     1933 2023-03-19 00:51:10.000000 pyqt-openai-0.1.72/pyqt_openai/ico/stackontop.svg
+-rw-rw-rw-   0        0        0     1096 2023-05-05 23:44:44.000000 pyqt-openai-0.1.72/pyqt_openai/ico/user.svg
+-rw-rw-rw-   0        0        0      432 2023-05-07 05:04:02.000000 pyqt-openai-0.1.72/pyqt_openai/ico/vertical_three_dots.svg
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.333241 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/
+-rw-rw-rw-   0        0        0        0 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/currentImageView.py
+-rw-rw-rw-   0        0        0     1735 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/explorerWidget.py
+-rw-rw-rw-   0        0        0     3581 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageDallEPage.py
+-rw-rw-rw-   0        0        0     4558 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py
+-rw-rw-rw-   0        0        0     5090 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageListWidget.py
+-rw-rw-rw-   0        0        0    18549 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageSqlite.py
+-rw-rw-rw-   0        0        0    11118 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py
+-rw-rw-rw-   0        0        0     3867 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/leftSideBar.py
+-rw-rw-rw-   0        0        0     1077 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/rightSideBar.py
+-rw-rw-rw-   0        0        0     4044 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/thumbnailView.py
+-rw-rw-rw-   0        0        0     2229 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/viewWidget.py
+-rw-rw-rw-   0        0        0     1444 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/inputDialog.py
+-rw-rw-rw-   0        0        0     3762 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/leftSideBar.py
+-rw-rw-rw-   0        0        0    11457 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/main.py
+-rw-rw-rw-   0        0        0     1787 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/modelTable.py
+-rw-rw-rw-   0        0        0     3293 2023-06-06 02:12:45.000000 pyqt-openai-0.1.72/pyqt_openai/notifier.py
+-rw-rw-rw-   0        0        0    12106 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/openAiChatBotWidget.py
+-rw-rw-rw-   0        0        0     2899 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/openAiThread.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.389710 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/__init__.py
+-rw-rw-rw-   0        0        0     2423 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py
+-rw-rw-rw-   0        0        0     1768 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py
+-rw-rw-rw-   0        0        0     9467 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/propPage.py
+-rw-rw-rw-   0        0        0     1755 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py
+-rw-rw-rw-   0        0        0     9491 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/templatePage.py
+-rw-rw-rw-   0        0        0     1778 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.399480 pyqt-openai-0.1.72/pyqt_openai/propmt_command_completer/
+-rw-rw-rw-   0        0        0        0 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/propmt_command_completer/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/propmt_command_completer/commandSuggestionWidget.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.435417 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/
+-rw-rw-rw-   0        0        0       39 2023-05-05 02:56:55.000000 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-05-20 05:39:27.000000 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/aiPlaygroundWidget.py
+-rw-rw-rw-   0        0        0     4894 2023-06-16 09:00:57.000000 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/chatPage.py
+-rw-rw-rw-   0        0        0    10944 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/completionPage.py
+-rw-rw-rw-   0        0        0     1623 2023-05-07 22:16:16.000000 pyqt-openai-0.1.72/pyqt_openai/right_sidebar/imagePage.py
+-rw-rw-rw-   0        0        0     2866 2023-04-22 00:05:31.000000 pyqt-openai-0.1.72/pyqt_openai/searchBar.py
+-rw-rw-rw-   0        0        0   113289 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/sqlite.py
+-rw-rw-rw-   0        0        0     5934 2023-06-06 02:12:45.000000 pyqt-openai-0.1.72/pyqt_openai/svgButton.py
+-rw-rw-rw-   0        0        0      738 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/svgLabel.py
+-rw-rw-rw-   0        0        0     5951 2023-06-06 02:12:45.000000 pyqt-openai-0.1.72/pyqt_openai/svgToolButton.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.444357 pyqt-openai-0.1.72/pyqt_openai/test/
+-rw-rw-rw-   0        0        0        0 2023-05-21 02:10:54.000000 pyqt-openai-0.1.72/pyqt_openai/test/__init__.py
+-rw-rw-rw-   0        0        0      761 2023-05-21 02:10:54.000000 pyqt-openai-0.1.72/pyqt_openai/test/sqlalchemy_example.py
+-rw-rw-rw-   0        0        0     4884 2023-06-06 13:23:05.000000 pyqt-openai-0.1.72/pyqt_openai/toast.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:23.467446 pyqt-openai-0.1.72/pyqt_openai/util/
+-rw-rw-rw-   0        0        0       30 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/util/__init__.py
+-rw-rw-rw-   0        0        0     2630 2023-06-15 11:14:42.000000 pyqt-openai-0.1.72/pyqt_openai/util/script.py
+-rw-rw-rw-   0        0        0       91 2023-06-04 10:09:52.000000 pyqt-openai-0.1.72/pyqt_openai/util/version.py
+drwxrwxrwx   0        0        0        0 2023-06-16 09:01:22.992184 pyqt-openai-0.1.72/pyqt_openai.egg-info/
+-rw-rw-rw-   0        0        0    10567 2023-06-16 09:01:22.000000 pyqt-openai-0.1.72/pyqt_openai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3019 2023-06-16 09:01:22.000000 pyqt-openai-0.1.72/pyqt_openai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 09:01:22.000000 pyqt-openai-0.1.72/pyqt_openai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-16 09:01:22.000000 pyqt-openai-0.1.72/pyqt_openai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-16 09:01:22.000000 pyqt-openai-0.1.72/pyqt_openai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 09:01:23.471408 pyqt-openai-0.1.72/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2023-06-16 09:00:57.000000 pyqt-openai-0.1.72/setup.py
```

### Comparing `pyqt-openai-0.1.61/LICENSE` & `pyqt-openai-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/PKG-INFO` & `pyqt-openai-0.1.72/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.61
+Version: 0.1.72
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pyqt-openai
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
-</p>
+<div align="center">
+  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png" width="150px" height="150px"><br/><br/>
+  
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/cHekprskVE)
+</div>
+
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
 This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
+Latest model such as gpt-3.5-turbo-0613 is also available
+
 Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
 
 <b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
 
 But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
@@ -49,17 +54,18 @@
 * [Note](#note)
 * [See Also](#see-also)
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+  * support copy button
 * conversation management
   * add & delete conversations
-  * save conversations
+  * save conversations - SQlite db, text files compressed file, html files compressed file (both are zip)
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
 * support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
@@ -71,14 +77,15 @@
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 * aiohttp - for openai dependency 
 * pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
+* jinja2 - for saving the conversation with html file
 
 ## Preview & Usage
 ### Overview
 #### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
@@ -96,14 +103,19 @@
 I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
 
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 #### Preview 2 (using prompt feature)
 
 https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
+#### Conversation Save Feature
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a)
+
+You can save checked conversation units to SQlite db file or compressed file (zip) which contains each conversation as text/html file.
+
 ### Prompt Generator
 #### How to Generate
 This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
 
 Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
 
 For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
@@ -143,15 +155,15 @@
 
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
 1. git clone ~
 2. cd pyqt-openai
-3. pip install -r requirements.txt
+3. pip install -r requirements.txt --upgrade
 4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
@@ -167,14 +179,15 @@
 
 run this command:
 ```
 sudo apt-get install libxcb-xinerama0
 ```
 
 ## Troubleshooting
+### subprocess-exited-with-error
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
@@ -182,24 +195,34 @@
 python setup.py install
 ```
 
 That will install the openai.
 
 Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
 
+### qtpy.QtBindingsNotFoundError: No Qt bindings could be found
+first, do this:
+```
+pip uninstall -r requirements.txt
+```
+second, do this:
+```
+pip install -r requirements.txt --upgrade
+```
+then it will work :)
+
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
 
 ## TODO list
 * DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
-* save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
```

#### html2text {}

```diff
@@ -1,115 +1,127 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.61 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.72 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
+
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/
+                                  cHekprskVE)
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
 Stable Diffusion as a image generation tool. Even though this project has
 become too huge to be called an 'example'. The major advantage of this package
 is that you don't need to know other language aside from Python. If you want to
 study openai with Python-only good old desktop software, this is for you. The
 OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
-functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
-feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
-used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
-stable-diffusion-webgui. But this is very lightweight and more accessible.
-don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
-database. You can select the model at the right side bar. An internet
-connection is required. ## Table of Contents * [Feature](#feature) *
-[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
-Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
-(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
-is desktop application version of ChatGPT with image generation tool. * text
-streaming (enable by default, you can disable it) * AI remembers past
-conversation * conversation management * add & delete conversations * save
-conversations * rename conversation * everything above is saved in an SQLite
-database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database) * support slash
-commands * support beginning and ending part of the prompt * you can run this
-in background application * notification will pop up when response is generated
-* you can make window stack on top or control its transparency * image
-generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
-download the image if you want. just hover the mouse cursor over the image. ##
-Requirements * qtpy - the package allowing you to write code that works with
+functional as ChatGPT) by default. You can use gpt-4 as well. Latest model such
+as gpt-3.5-turbo-0613 is also available Image generation feature(DALL-E and
+Stable Diffusion) available since v0.1.4. Stable Diffusion used [DreamStudio
+API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-
+webgui. But this is very lightweight and more accessible. don't need CUDA,
+torch, expansive PC, anything. This is using sqlite as a database. You can
+select the model at the right side bar. An internet connection is required. ##
+Table of Contents * [Feature](#feature) * [Requirements](#requirements) *
+[Preview & Usage](#preview-usage) * [How to Install](#how-to-install) *
+[Troubleshooting](#troubleshooting) * [Contact](#contact) * [Note](#note) *
+[See Also](#see-also) ## Feature * basically this is desktop application
+version of ChatGPT with image generation tool. * text streaming (enable by
+default, you can disable it) * AI remembers past conversation * support copy
+button * conversation management * add & delete conversations * save
+conversations - SQlite db, text files compressed file, html files compressed
+file (both are zip) * rename conversation * everything above is saved in an
+SQLite database file named conv.db. * support GPT-4 and every other models
+below GPT3 * support prompt generator (manageable, autosaved in database) *
+support slash commands * support beginning and ending part of the prompt * you
+can run this in background application * notification will pop up when response
+is generated * you can make window stack on top or control its transparency *
+image generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy
+and download the image if you want. just hover the mouse cursor over the image.
+## Requirements * qtpy - the package allowing you to write code that works with
 both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
 dependency * pyperclip - to copy prompt text from prompt generator *
-stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
-Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
-inside the red box. see [How to install](#how-to-install) You can change screen
-between text chatbot and image generating tool screen. ![image](https://
-github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
-please give me the pyqt-openai screen image from it. ### Conversation ####
-Preview 1 I recorded this preview long time ago so GUI is different from the
-current version, but way of operating it is pretty much the same. https://user-
+stability_sdk - for Stable Diffusion * jinja2 - for saving the conversation
+with html file ## Preview & Usage ### Overview #### Windows ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-
+ec56331b8361) You have to write your openai api key inside the red box. see
+[How to install](#how-to-install) You can change screen between text chatbot
+and image generating tool screen. ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061) #### Linux
+(Ubuntu) ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS, please give me the
+pyqt-openai screen image from it. ### Conversation #### Preview 1 I recorded
+this preview long time ago so GUI is different from the current version, but
+way of operating it is pretty much the same. https://user-
 images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
 f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
-yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
-Prompt Generator #### How to Generate This application has two types of
-prompts. One is "Properties" and the other one is "Template". Properties are
-sets of attributes that are useful for forming the premises of a question.
-Templates are sentences that correspond to a single command. You can input a
-command to generate a sentence. This can be used as a question in itself. Both
-types can be managed as groups. After cloning or installing, if you run the
-program immediately, you will be able to see the default group and the items
-included in the group, just like the screen. For properties, there is a group
-named "Default" that provides a set of attributes referenced here. For
-templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
-prompt for Alex Brogan) groups provided. Any custom template items created
-prior to version 0.1.6 will be moved to the Miscellaneous group. !
-[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
-much get any response you want. You can use the additional prompt feature by
-"prompt menu" right next to "prompt input" field. ![image](https://github.com/
-yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
-Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
-#### Prompt Generator Preview Generating the prompt (Properties) https://
-github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
-3c42c9c23602 I recorded using the Windows recording feature. As a result, the
-"Add Dialog" that prompts for entering a group name does not appear in the
-preview. When you add a group, you will see the Add Dialog as expected. Then,
-how to generate template type prompt? Click any item in the group, it will be
-shown in the preview. You can copy that generated text with clicking "copy"
-button and include it to your prompt input. If you add a property group or
-template group with items, you can use it as a command by typing its name to
-the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
-pressed the keyboard shortcut of each actions(show beginning, show ending,
-support prompt command) to use it rather than clicking them with mouse. I made
-the command suggestion GUI resemble the Discord command autocomplete popup,
-with which a lot of people have become accustomed. ### Image Generation !
-[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
-4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
-pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 6. python
-main.py If installation doesn't work, you can contact me with bring up new
-issue in issue tab or check the troubleshooting below even it is only about
-very specific error. ### Note If you use Linux and see this error: ```
-qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
-was found this application failed to start because no qt platform plugin could
-be initialized, reinstalling the application may fix this problem ``` run this
-command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
-you see this error while installing the openai package ``` subprocess-exited-
-with-error ``` download the package itself from pypi. Unzip it, access the
-package directory, type ``` python setup.py install ``` That will install the
-openai. Note: I don't know this can happen in newer version of openai as well,
-so tell me if you know about something ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-I recommend to install sqlite management software. It's not necessary to run
-this app (obviously), but it's good practice to manage database about
-conversation history with AI and to know how this works. ## TODO list * DB for
-images (to further experiement of both DALL-E and Stable Diffusion or other
-image generation engine) * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ####
+Conversation Save Feature ![image](https://github.com/yjg30737/pyqt-openai/
+assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a) You can save checked
+conversation units to SQlite db file or compressed file (zip) which contains
+each conversation as text/html file. ### Prompt Generator #### How to Generate
+This application has two types of prompts. One is "Properties" and the other
+one is "Template". Properties are sets of attributes that are useful for
+forming the premises of a question. Templates are sentences that correspond to
+a single command. You can input a command to generate a sentence. This can be
+used as a question in itself. Both types can be managed as groups. After
+cloning or installing, if you run the program immediately, you will be able to
+see the default group and the items included in the group, just like the
+screen. For properties, there is a group named "Default" that provides a set of
+attributes referenced here. For templates, there are the
+"awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan)
+groups provided. Any custom template items created prior to version 0.1.6 will
+be moved to the Miscellaneous group. ![prompt_list_image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394) With
+using these prompts you can pretty much get any response you want. You can use
+the additional prompt feature by "prompt menu" right next to "prompt input"
+field. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+c9ca84af-0088-4435-854d-7feca9e2e663) Since v0.1.6, awesome-chatgpt-prompt is
+included as template group by default. #### Prompt Generator Preview Generating
+the prompt (Properties) https://github.com/yjg30737/pyqt-openai/assets/
+55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602 I recorded using the Windows
+recording feature. As a result, the "Add Dialog" that prompts for entering a
+group name does not appear in the preview. When you add a group, you will see
+the Add Dialog as expected. Then, how to generate template type prompt? Click
+any item in the group, it will be shown in the preview. You can copy that
+generated text with clicking "copy" button and include it to your prompt input.
+If you add a property group or template group with items, you can use it as a
+command by typing its name to the prompt input. Use prompt as a command https:/
+/github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-
+4e4d1e572553 In this preview, i pressed the keyboard shortcut of each actions
+(show beginning, show ending, support prompt command) to use it rather than
+clicking them with mouse. I made the command suggestion GUI resemble the
+Discord command autocomplete popup, with which a lot of people have become
+accustomed. ### Image Generation ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install
+1. git clone ~ 2. cd pyqt-openai 3. pip install -r requirements.txt --upgrade
+4. cd pyqt_openai 5. You should put your api key in the line edit. You can get
+it in official_site of openai. Sign up and log in before you get it. Be sure,
+this is a very important API key that belongs to you only, so you should
+remember it and keep it secure. 6. python main.py If installation doesn't work,
+you can contact me with bring up new issue in issue tab or check the
+troubleshooting below even it is only about very specific error. ### Note If
+you use Linux and see this error: ``` qt.qpa.plugin: could not load the qt
+platform plugin "xcb" in "" even though it was found this application failed to
+start because no qt platform plugin could be initialized, reinstalling the
+application may fix this problem ``` run this command: ``` sudo apt-get install
+libxcb-xinerama0 ``` ## Troubleshooting ### subprocess-exited-with-error If you
+see this error while installing the openai package ``` subprocess-exited-with-
+error ``` download the package itself from pypi. Unzip it, access the package
+directory, type ``` python setup.py install ``` That will install the openai.
+Note: I don't know this can happen in newer version of openai as well, so tell
+me if you know about something ### qtpy.QtBindingsNotFoundError: No Qt bindings
+could be found first, do this: ``` pip uninstall -r requirements.txt ```
+second, do this: ``` pip install -r requirements.txt --upgrade ``` then it will
+work :) ## Contact You can join pyqt-openai's Discord_Server to have a
+conversation about it or AI-related stuff ð ## Note I recommend to install
+sqlite management software. It's not necessary to run this app (obviously), but
+it's good practice to manage database about conversation history with AI and to
+know how this works. ## TODO list * DB for images (to further experiement of
+both DALL-E and Stable Diffusion or other image generation engine) * show the
+explanation of every model and terms related to AI (e.g. temperature, topp..) *
+tokenizer * highlight the source (optional, eventually) * support multiple
+language * use SQLAlchemy (maybe not) * show reason when the chat input is
+disabled for some reasons * add the basic example sources of making deep
+learning model with PyTorch (eventually) ## See Also * Azure_OpenAI_service *
+join_gpt4_waitlist - i took 1 month to get access from it * join_chatgpt
+plugins_waitlist
```

### Comparing `pyqt-openai-0.1.61/README.md` & `pyqt-openai-0.1.72/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # pyqt-openai
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
-</p>
+<div align="center">
+  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png" width="150px" height="150px"><br/><br/>
+  
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/cHekprskVE)
+</div>
+
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
 This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
+Latest model such as gpt-3.5-turbo-0613 is also available
+
 Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
 
 <b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
 
 But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
@@ -37,17 +42,18 @@
 * [Note](#note)
 * [See Also](#see-also)
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+  * support copy button
 * conversation management
   * add & delete conversations
-  * save conversations
+  * save conversations - SQlite db, text files compressed file, html files compressed file (both are zip)
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
 * support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
@@ -59,14 +65,15 @@
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 * aiohttp - for openai dependency 
 * pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
+* jinja2 - for saving the conversation with html file
 
 ## Preview & Usage
 ### Overview
 #### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
@@ -84,14 +91,19 @@
 I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
 
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 #### Preview 2 (using prompt feature)
 
 https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
+#### Conversation Save Feature
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a)
+
+You can save checked conversation units to SQlite db file or compressed file (zip) which contains each conversation as text/html file.
+
 ### Prompt Generator
 #### How to Generate
 This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
 
 Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
 
 For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
@@ -131,15 +143,15 @@
 
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
 1. git clone ~
 2. cd pyqt-openai
-3. pip install -r requirements.txt
+3. pip install -r requirements.txt --upgrade
 4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
@@ -155,14 +167,15 @@
 
 run this command:
 ```
 sudo apt-get install libxcb-xinerama0
 ```
 
 ## Troubleshooting
+### subprocess-exited-with-error
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
@@ -170,24 +183,34 @@
 python setup.py install
 ```
 
 That will install the openai.
 
 Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
 
+### qtpy.QtBindingsNotFoundError: No Qt bindings could be found
+first, do this:
+```
+pip uninstall -r requirements.txt
+```
+second, do this:
+```
+pip install -r requirements.txt --upgrade
+```
+then it will work :)
+
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
 
 ## TODO list
 * DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
-* save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
```

#### html2text {}

```diff
@@ -1,112 +1,124 @@
 # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
+
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/
+                                  cHekprskVE)
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
 Stable Diffusion as a image generation tool. Even though this project has
 become too huge to be called an 'example'. The major advantage of this package
 is that you don't need to know other language aside from Python. If you want to
 study openai with Python-only good old desktop software, this is for you. The
 OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
-functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
-feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
-used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
-stable-diffusion-webgui. But this is very lightweight and more accessible.
-don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
-database. You can select the model at the right side bar. An internet
-connection is required. ## Table of Contents * [Feature](#feature) *
-[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
-Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
-(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
-is desktop application version of ChatGPT with image generation tool. * text
-streaming (enable by default, you can disable it) * AI remembers past
-conversation * conversation management * add & delete conversations * save
-conversations * rename conversation * everything above is saved in an SQLite
-database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database) * support slash
-commands * support beginning and ending part of the prompt * you can run this
-in background application * notification will pop up when response is generated
-* you can make window stack on top or control its transparency * image
-generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
-download the image if you want. just hover the mouse cursor over the image. ##
-Requirements * qtpy - the package allowing you to write code that works with
+functional as ChatGPT) by default. You can use gpt-4 as well. Latest model such
+as gpt-3.5-turbo-0613 is also available Image generation feature(DALL-E and
+Stable Diffusion) available since v0.1.4. Stable Diffusion used [DreamStudio
+API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-
+webgui. But this is very lightweight and more accessible. don't need CUDA,
+torch, expansive PC, anything. This is using sqlite as a database. You can
+select the model at the right side bar. An internet connection is required. ##
+Table of Contents * [Feature](#feature) * [Requirements](#requirements) *
+[Preview & Usage](#preview-usage) * [How to Install](#how-to-install) *
+[Troubleshooting](#troubleshooting) * [Contact](#contact) * [Note](#note) *
+[See Also](#see-also) ## Feature * basically this is desktop application
+version of ChatGPT with image generation tool. * text streaming (enable by
+default, you can disable it) * AI remembers past conversation * support copy
+button * conversation management * add & delete conversations * save
+conversations - SQlite db, text files compressed file, html files compressed
+file (both are zip) * rename conversation * everything above is saved in an
+SQLite database file named conv.db. * support GPT-4 and every other models
+below GPT3 * support prompt generator (manageable, autosaved in database) *
+support slash commands * support beginning and ending part of the prompt * you
+can run this in background application * notification will pop up when response
+is generated * you can make window stack on top or control its transparency *
+image generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy
+and download the image if you want. just hover the mouse cursor over the image.
+## Requirements * qtpy - the package allowing you to write code that works with
 both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
 dependency * pyperclip - to copy prompt text from prompt generator *
-stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
-Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
-inside the red box. see [How to install](#how-to-install) You can change screen
-between text chatbot and image generating tool screen. ![image](https://
-github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
-please give me the pyqt-openai screen image from it. ### Conversation ####
-Preview 1 I recorded this preview long time ago so GUI is different from the
-current version, but way of operating it is pretty much the same. https://user-
+stability_sdk - for Stable Diffusion * jinja2 - for saving the conversation
+with html file ## Preview & Usage ### Overview #### Windows ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-
+ec56331b8361) You have to write your openai api key inside the red box. see
+[How to install](#how-to-install) You can change screen between text chatbot
+and image generating tool screen. ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061) #### Linux
+(Ubuntu) ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS, please give me the
+pyqt-openai screen image from it. ### Conversation #### Preview 1 I recorded
+this preview long time ago so GUI is different from the current version, but
+way of operating it is pretty much the same. https://user-
 images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
 f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
-yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
-Prompt Generator #### How to Generate This application has two types of
-prompts. One is "Properties" and the other one is "Template". Properties are
-sets of attributes that are useful for forming the premises of a question.
-Templates are sentences that correspond to a single command. You can input a
-command to generate a sentence. This can be used as a question in itself. Both
-types can be managed as groups. After cloning or installing, if you run the
-program immediately, you will be able to see the default group and the items
-included in the group, just like the screen. For properties, there is a group
-named "Default" that provides a set of attributes referenced here. For
-templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
-prompt for Alex Brogan) groups provided. Any custom template items created
-prior to version 0.1.6 will be moved to the Miscellaneous group. !
-[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
-much get any response you want. You can use the additional prompt feature by
-"prompt menu" right next to "prompt input" field. ![image](https://github.com/
-yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
-Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
-#### Prompt Generator Preview Generating the prompt (Properties) https://
-github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
-3c42c9c23602 I recorded using the Windows recording feature. As a result, the
-"Add Dialog" that prompts for entering a group name does not appear in the
-preview. When you add a group, you will see the Add Dialog as expected. Then,
-how to generate template type prompt? Click any item in the group, it will be
-shown in the preview. You can copy that generated text with clicking "copy"
-button and include it to your prompt input. If you add a property group or
-template group with items, you can use it as a command by typing its name to
-the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
-pressed the keyboard shortcut of each actions(show beginning, show ending,
-support prompt command) to use it rather than clicking them with mouse. I made
-the command suggestion GUI resemble the Discord command autocomplete popup,
-with which a lot of people have become accustomed. ### Image Generation !
-[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
-4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
-pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 6. python
-main.py If installation doesn't work, you can contact me with bring up new
-issue in issue tab or check the troubleshooting below even it is only about
-very specific error. ### Note If you use Linux and see this error: ```
-qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
-was found this application failed to start because no qt platform plugin could
-be initialized, reinstalling the application may fix this problem ``` run this
-command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
-you see this error while installing the openai package ``` subprocess-exited-
-with-error ``` download the package itself from pypi. Unzip it, access the
-package directory, type ``` python setup.py install ``` That will install the
-openai. Note: I don't know this can happen in newer version of openai as well,
-so tell me if you know about something ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-I recommend to install sqlite management software. It's not necessary to run
-this app (obviously), but it's good practice to manage database about
-conversation history with AI and to know how this works. ## TODO list * DB for
-images (to further experiement of both DALL-E and Stable Diffusion or other
-image generation engine) * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ####
+Conversation Save Feature ![image](https://github.com/yjg30737/pyqt-openai/
+assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a) You can save checked
+conversation units to SQlite db file or compressed file (zip) which contains
+each conversation as text/html file. ### Prompt Generator #### How to Generate
+This application has two types of prompts. One is "Properties" and the other
+one is "Template". Properties are sets of attributes that are useful for
+forming the premises of a question. Templates are sentences that correspond to
+a single command. You can input a command to generate a sentence. This can be
+used as a question in itself. Both types can be managed as groups. After
+cloning or installing, if you run the program immediately, you will be able to
+see the default group and the items included in the group, just like the
+screen. For properties, there is a group named "Default" that provides a set of
+attributes referenced here. For templates, there are the
+"awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan)
+groups provided. Any custom template items created prior to version 0.1.6 will
+be moved to the Miscellaneous group. ![prompt_list_image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394) With
+using these prompts you can pretty much get any response you want. You can use
+the additional prompt feature by "prompt menu" right next to "prompt input"
+field. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+c9ca84af-0088-4435-854d-7feca9e2e663) Since v0.1.6, awesome-chatgpt-prompt is
+included as template group by default. #### Prompt Generator Preview Generating
+the prompt (Properties) https://github.com/yjg30737/pyqt-openai/assets/
+55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602 I recorded using the Windows
+recording feature. As a result, the "Add Dialog" that prompts for entering a
+group name does not appear in the preview. When you add a group, you will see
+the Add Dialog as expected. Then, how to generate template type prompt? Click
+any item in the group, it will be shown in the preview. You can copy that
+generated text with clicking "copy" button and include it to your prompt input.
+If you add a property group or template group with items, you can use it as a
+command by typing its name to the prompt input. Use prompt as a command https:/
+/github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-
+4e4d1e572553 In this preview, i pressed the keyboard shortcut of each actions
+(show beginning, show ending, support prompt command) to use it rather than
+clicking them with mouse. I made the command suggestion GUI resemble the
+Discord command autocomplete popup, with which a lot of people have become
+accustomed. ### Image Generation ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install
+1. git clone ~ 2. cd pyqt-openai 3. pip install -r requirements.txt --upgrade
+4. cd pyqt_openai 5. You should put your api key in the line edit. You can get
+it in official_site of openai. Sign up and log in before you get it. Be sure,
+this is a very important API key that belongs to you only, so you should
+remember it and keep it secure. 6. python main.py If installation doesn't work,
+you can contact me with bring up new issue in issue tab or check the
+troubleshooting below even it is only about very specific error. ### Note If
+you use Linux and see this error: ``` qt.qpa.plugin: could not load the qt
+platform plugin "xcb" in "" even though it was found this application failed to
+start because no qt platform plugin could be initialized, reinstalling the
+application may fix this problem ``` run this command: ``` sudo apt-get install
+libxcb-xinerama0 ``` ## Troubleshooting ### subprocess-exited-with-error If you
+see this error while installing the openai package ``` subprocess-exited-with-
+error ``` download the package itself from pypi. Unzip it, access the package
+directory, type ``` python setup.py install ``` That will install the openai.
+Note: I don't know this can happen in newer version of openai as well, so tell
+me if you know about something ### qtpy.QtBindingsNotFoundError: No Qt bindings
+could be found first, do this: ``` pip uninstall -r requirements.txt ```
+second, do this: ``` pip install -r requirements.txt --upgrade ``` then it will
+work :) ## Contact You can join pyqt-openai's Discord_Server to have a
+conversation about it or AI-related stuff ð ## Note I recommend to install
+sqlite management software. It's not necessary to run this app (obviously), but
+it's good practice to manage database about conversation history with AI and to
+know how this works. ## TODO list * DB for images (to further experiement of
+both DALL-E and Stable Diffusion or other image generation engine) * show the
+explanation of every model and terms related to AI (e.g. temperature, topp..) *
+tokenizer * highlight the source (optional, eventually) * support multiple
+language * use SQLAlchemy (maybe not) * show reason when the chat input is
+disabled for some reasons * add the basic example sources of making deep
+learning model with PyTorch (eventually) ## See Also * Azure_OpenAI_service *
+join_gpt4_waitlist - i took 1 month to get access from it * join_chatgpt
+plugins_waitlist
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/a.py` & `pyqt-openai-0.1.72/pyqt_openai/a.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/aboutDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/aboutDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/apiData.py` & `pyqt-openai-0.1.72/pyqt_openai/apiData.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 import openai
 
 # static
 # https://platform.openai.com/docs/models/model-endpoint-compatibility
 ENDPOINT_DICT = {
-    '/v1/chat/completions': ['gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314', 'gpt-3.5-turbo', 'gpt-3.5-turbo-0301'],
+    '/v1/chat/completions': ['gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613',
+                             'gpt-3.5-turbo', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo-16k', 'gpt-3.5-turbo-16k-0613', 'gpt-3.5-turbo-0301'],
     '/v1/completions': [
         'text-davinci-003', 'text-davinci-002', 'text-curie-001', 'text-babbage-001', 'text-ada-001', 'davinci',
         'curie', 'babbage', 'ada'
     ],
     '/v1/edits': ['text-davinci-edit-001', 'code-davinci-edit-001'],
     '/v1/audio/transcriptions': ['whisper-1'],
     '/v1/audio/translations': ['whisper-1'],
     '/v1/fine-tunes': ['davinci', 'curie', 'babbage', 'ada'],
     '/v1/embeddings': ['text-embedding-ada-002', 'text-search-ada-doc-001'],
     '/vi/moderations': ['text-moderation-stable', 'text-moderation-latest']
 }
 
 def getModelEndpoint(model):
-    print(model)
     for k, v in ENDPOINT_DICT.items():
         endpoint_group = list(v)
         if model in endpoint_group:
             return k
 
-# legacy
-def getLatestModel():
-    return ['gpt-3.5-turbo',
-            'gpt-3.5-turbo-0301',
-            'text-davinci-003',
-            'text-davinci-002',
-            'code-davinci-002']
-
 # new
 def getCompletionModel():
     return [
         'text-davinci-003',
         'text-davinci-002',
         'text-curie-001',
         'text-babbage-001',
         'text-ada-001'
     ]
 
 def getChatModel():
-    return [
-        'gpt-3.5-turbo',
-        'gpt-3.5-turbo-0301',
-        'gpt-4',
-        'gpt-4-32k',
-    ]
+    return ENDPOINT_DICT['/v1/chat/completions']
 
 # dynamic
 class ModelData:
     def __init__(self):
         super().__init__()
         self.__modelList = []
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/chatWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageSqlite.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,466 +1,428 @@
-from qtpy.QtCore import Qt, Signal
-from qtpy.QtGui import QFont, QTextCursor
-from qtpy.QtWidgets import QScrollArea, QCompleter, QVBoxLayout, QToolButton, QMenu, QAction, QWidget, QLabel, \
-    QHBoxLayout, QTextEdit, QStackedWidget
-
-from pyqt_openai.commandCompleter import CommandCompleter
-from pyqt_openai.propmt_command_completer.commandSuggestionWidget import CommandSuggestionWidget
-from pyqt_openai.sqlite import SqliteDatabase
-from pyqt_openai.svgToolButton import SvgToolButton
+import sqlite3, json, shutil
 
+# TODO
+class SqliteDatabase:
+    """
+    functions which only meant to be used frequently are defined.
 
-class ChatBrowser(QScrollArea):
-    convUnitUpdated = Signal(int, int, str)
-
+    if there is no functions you want to use, use ``getCursor`` instead
+    """
     def __init__(self):
         super().__init__()
         self.__initVal()
-        self.__initUi()
+        self.__initDb()
+        self.__createImage()
 
     def __initVal(self):
-        self.__cur_id = 0
-
-    def __initUi(self):
-        self.__homeWidget = QLabel('Home')
-        self.__homeWidget.setAlignment(Qt.AlignCenter)
-        self.__homeWidget.setFont(QFont('Arial', 32))
-
-        lay = QVBoxLayout()
-        lay.setAlignment(Qt.AlignTop)
-        lay.setSpacing(0)
-        lay.setContentsMargins(0, 0, 0, 0)
-
-        self.__chatWidget = QWidget()
-        self.__chatWidget.setLayout(lay)
-
-        widget = QStackedWidget()
-        widget.addWidget(self.__homeWidget)
-        widget.addWidget(self.__chatWidget)
-        self.setWidget(widget)
-        self.setWidgetResizable(True)
-
-    def getChatWidget(self):
-        return self.__chatWidget
-
-    def showLabel(self, text, user_f, stream_f):
-        self.showText(text, stream_f, user_f)
-        if not stream_f:
-            # change user_f type from bool to int to insert in db
-            self.convUnitUpdated.emit(self.__cur_id, int(user_f), text)
-
-    def streamFinished(self):
-        self.convUnitUpdated.emit(self.__cur_id, 0, self.getLastResponse())
+        # db names
+        self.__db_filename = 'image.db'
 
-    def showText(self, text, stream_f, user_f):
-        if self.widget().currentWidget() == self.__chatWidget:
-            pass
-        else:
-            self.widget().setCurrentIndex(1)
-        self.__setLabel(text, stream_f, user_f)
+        # image table names
+        self.__image_tb_nm = 'image_tb'
+        self.__image_tb_tr_nm = 'image_tr'
+        self.__image_unit_tb_nm = 'image_unit_tb'
+
+        # info table names
+        self.__dall_e_info_tb_nm = 'dall_e_info_tb'
+        self.__stable_diffusion_info_tb_nm = 'stable_diffusion_tb'
+
+        # model type (chat, etc.)
+        self.__model_type = 1
+
+        # DALL-E
+        self.__image_dall_e_default_value = {
+            'engine': "DALL-E",
+            'n': 1,
+            'width': 1024,
+            'height': 1024,
+            # 'response_format':
+        }
+        
+        # SD
+        self.__image_sd_default_value = {
+            'height': 512,
+            'width': 512,
+            'steps': 30,
+            'samples': 1,
+            'cfg_scale': 7,
+            'engine': 'stable-diffusion-xl-beta-v2-2-2',
+            'sampler': 'k_dpmpp_2m',
+            'seed': 0, # random
+        }
+        
+        self.__each_info_dict = {1: [self.__dall_e_info_tb_nm, self.__image_dall_e_default_value],
+                                 2: [self.__stable_diffusion_info_tb_nm, self.__image_sd_default_value], }
 
-    def __setLabel(self, text, stream_f, user_f):
-        chatLbl = QLabel(text)
-        chatLbl.setWordWrap(True)
-        chatLbl.setTextInteractionFlags(Qt.TextSelectableByMouse)
-        if user_f:
-            chatLbl.setStyleSheet('QLabel { padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignRight)
+    def __initDb(self):
+        try:
+            # Connect to the database (create a new file if it doesn't exist)
+            self.__conn = sqlite3.connect(self.__db_filename)
+            self.__conn.execute('PRAGMA foreign_keys = ON;')
+            self.__conn.commit()
+
+            self.__c = self.__conn.cursor()
+            self.__createInfo()
+        except sqlite3.Error as e:
+            print(f"An error occurred while connecting to the database: {e}")
+            raise
+
+    def __createDallE(self):
+        # Check if the table exists
+        self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__dall_e_info_tb_nm}'")
+        if self.__c.fetchone()[0] == 1:
+            # Check if each column already exists in the table
+            existing_columns = [row[1] for row in self.__c.execute(f"PRAGMA table_info({self.__dall_e_info_tb_nm});")]
+            new_columns = [col for col in self.__image_dall_e_default_value.keys() if col not in existing_columns]
+            # Add the new columns if they don't already exist
+            # TODO specify the type
+            for col in new_columns:
+                d_value = self.__image_dall_e_default_value[col]
+                if isinstance(self.__image_dall_e_default_value[col], str):
+                    d_value = f'"{d_value}"' if len(self.__image_dall_e_default_value[col].split()) > 0 else d_value
+                self.__c.execute(f"ALTER TABLE {self.__dall_e_info_tb_nm} ADD COLUMN {col} DEFAULT {d_value}")
         else:
-            if stream_f:
-                lbl = self.getChatWidget().layout().itemAt(self.getChatWidget().layout().count()-1).widget()
-                if isinstance(lbl, QLabel) and lbl.alignment() == Qt.AlignLeft:
-                    lbl.setText(lbl.text()+text)
-                    return
-            chatLbl.setStyleSheet('QLabel { background-color: #DDD; padding: 1em }')
-            chatLbl.setAlignment(Qt.AlignLeft)
-            chatLbl.setOpenExternalLinks(True)
-        self.getChatWidget().layout().addWidget(chatLbl)
-
-    def event(self, e):
-        if e.type() == 43:
-            self.verticalScrollBar().setSliderPosition(self.verticalScrollBar().maximum())
-        return super().event(e)
-
-    def getAllText(self):
-        all_text_lst = []
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()):
-                if lay.itemAt(i) and lay.itemAt(i).widget():
-                    widget = lay.itemAt(i).widget()
-                    if isinstance(widget, QLabel):
-                        all_text_lst.append(widget.text())
-
-        return '\n'.join(all_text_lst)
-
-    def getLastResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            i = lay.count()-1
-            if lay.itemAt(i) and lay.itemAt(i).widget():
-                widget = lay.itemAt(i).widget()
-                if isinstance(widget, QLabel):
-                    return widget.text()
-        return ''
-
-    def getEveryResponse(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            text_lst = []
-            for i in range(lay.count()):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    widget = item.widget()
-                    if isinstance(widget, QLabel) and i % 2 == 1:
-                        text_lst.append(widget.text())
-            return '\n'.join(text_lst)
+            self.__c.execute(f'''CREATE TABLE {self.__dall_e_info_tb_nm}
+                                     (id INTEGER PRIMARY KEY,
+                                      n TEXT DEFAULT '{self.__image_dall_e_default_value['n']}',
+                                      width INTEGER DEFAULT {self.__image_dall_e_default_value['width']},
+                                      height INTEGER DEFAULT {self.__image_dall_e_default_value['height']},
+                                      update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                      insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
+
+            # Commit the transaction
+            self.__conn.commit()
+
+            # insert default record
+            self.__c.execute(f'''INSERT INTO {self.__dall_e_info_tb_nm}
+                                            (
+                                                n,
+                                                width,
+                                                height
+                                            ) VALUES
+                                            (
+                                                {','.join(['?' for _ in range(len(self.__image_dall_e_default_value))])}
+                                            )
+                                         ''', tuple(self.__image_dall_e_default_value.values()))
+
+    def __createStableDiffusion(self):
+        # Check if the table exists
+        self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__stable_diffusion_info_tb_nm}'")
+        if self.__c.fetchone()[0] == 1:
+            pass
         else:
-            return ''
-
-    def clear(self):
-        lay = self.getChatWidget().layout()
-        if lay:
-            for i in range(lay.count()-1, -1, -1):
-                item = lay.itemAt(i)
-                if item and item.widget():
-                    lay.removeWidget(item.widget())
-        self.widget().setCurrentIndex(0)
-
-    def isNew(self):
-        return self.widget().currentIndex() == 0
-
-    def setCurId(self, id):
-        self.__cur_id = id
-
-    def resetChatWidget(self, id):
-        self.clear()
-        self.setCurId(id)
-
-    def replaceConv(self, id, conv_data):
-        self.clear()
-        self.setCurId(id)
-        self.widget().setCurrentIndex(1)
-        for i in range(len(conv_data)):
-            self.__setLabel(conv_data[i], False, not bool(i % 2))
-
-
-class TextEditPrompt(QTextEdit):
-    returnPressed = Signal()
-    sendSuggestionWidget = Signal(str)
-
-    def __init__(self):
-        super().__init__()
-        self.__initVal()
-        self.__initUi()
-
-    def __initVal(self):
-        self.__commandSuggestionEnabled = False
-
-    def __initUi(self):
-        self.setStyleSheet('QTextEdit { border: 1px solid #AAA; } ')
-
-    def setCommandSuggestionEnabled(self, f):
-        self.__commandSuggestionEnabled = f
-
-    def keyPressEvent(self, e):
-        if self.__commandSuggestionEnabled:
-            if e.key() == Qt.Key_Up:
-                self.sendSuggestionWidget.emit('up')
-            elif e.key() == Qt.Key_Down:
-                self.sendSuggestionWidget.emit('down')
-
-        if e.key() == Qt.Key_Return or e.key() == Qt.Key_Enter:
-            if e.modifiers() == Qt.ShiftModifier:
-                return super().keyPressEvent(e)
+            self.__c.execute(f'''CREATE TABLE {self.__stable_diffusion_info_tb_nm}
+                                             (
+                                                id INTEGER PRIMARY KEY,
+                                                height INTEGER DEFAULT '{self.__image_sd_default_value['height']},
+                                                width INTEGER DEFAULT '{self.__image_sd_default_value['width']},
+                                                steps INTEGER DEFAULT '{self.__image_sd_default_value['steps']},
+                                                samples INTEGER DEFAULT '{self.__image_sd_default_value['samples']},
+                                                cfg_scale INTEGER DEFAULT '{self.__image_sd_default_value['cfg_scale']},
+                                                engine VARCHAR(50) DEFAULT '{self.__image_sd_default_value['engine']},
+                                                sampler VARCHAR(50) DEFAULT '{self.__image_sd_default_value['sampler']},
+                                                seed INTEGER DEFAULT '{self.__image_sd_default_value['seed']},
+                                              update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                              insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
+
+            # Commit the transaction
+            self.__conn.commit()
+
+            # insert default record
+            self.__c.execute(f'''INSERT INTO {self.__stable_diffusion_info_tb_nm}
+                                                    (
+                                                        height,
+                                                        width,
+                                                        steps,
+                                                        samples,
+                                                        cfg_scale,
+                                                        engine,
+                                                        sampler,
+                                                        seed
+                                                    ) VALUES
+                                                    (
+                                                        {','.join(['?' for _ in range(len(self.__image_sd_default_value))])}
+                                                    )
+                                                 ''', tuple(self.__image_sd_default_value.values()))
+
+    def __createInfo(self):
+        try:
+            self.__createDallE()
+            self.__createStableDiffusion()
+            # Commit the transaction
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred while creating the table: {e}")
+            raise
+
+    def __createImage(self):
+        try:
+            # Check if the table exists
+            self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__image_tb_nm}'")
+            if self.__c.fetchone()[0] == 1:
+                # each image table already exists
+                pass
             else:
-                if self.__commandSuggestionEnabled:
-                    self.sendSuggestionWidget.emit('enter')
-                else:
-                    self.returnPressed.emit()
-        else:
-            return super().keyPressEvent(e)
-
-
-class TextEditPropmtGroup(QWidget):
-    textChanged = Signal()
-    onUpdateSuggestion = Signal()
-    onSendKeySignalToSuggestion = Signal(str)
+                # Create a table with update_dt and insert_dt columns
+                self.__c.execute(f'''CREATE TABLE {self.__image_tb_nm}
+                             (id INTEGER PRIMARY KEY,
+                              name TEXT,
+                              update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                              insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP)''')
+                # Create a trigger to update the update_dt column with the current timestamp
+                self.__c.execute(f'''CREATE TRIGGER {self.__image_tb_tr_nm}
+                             AFTER UPDATE ON {self.__image_tb_nm}
+                             FOR EACH ROW
+                             BEGIN
+                               UPDATE {self.__image_tb_nm}
+                               SET update_dt=CURRENT_TIMESTAMP
+                               WHERE id=OLD.id;
+                             END;''')
+                # Commit the transaction
+                self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred while creating the table: {e}")
+            raise
 
-    def __init__(self, db: SqliteDatabase):
-        super().__init__()
-        self.__initVal(db)
-        self.__initUi()
+    def selectAllInfo(self):
+        """
+        select all info
+        FIXME
+        """
+        try:
+            # filter bool type fields
+            bool_type_column = [row[1] for row in self.__c.execute(f'PRAGMA table_info({self.__dall_e_info_tb_nm})').fetchall() if row[2] == 'BOOL']
+
+            # Execute the SELECT statement
+            self.__c.execute(f'SELECT {",".join(list(self.__image_dall_e_default_value.keys()))} FROM {self.__dall_e_info_tb_nm}')
+
+            # Get the column names
+            column_names = [description[0] for description in self.__c.description]
+
+            rows = self.__c.fetchall()
+
+            info_dict_arr = []
+
+            # Get the rows with field names and values
+            for row in rows:
+                info_dict = {}
+                for i, value in enumerate(row):
+                    if column_names[i] in bool_type_column:
+                        value = True if value == 1 else False
+                    info_dict[column_names[i]] = value
+                info_dict_arr.append(info_dict)
+
+            return info_dict_arr
+        except sqlite3.Error as e:
+            print(f"An error occurred while creating the table: {e}")
+            raise
+
+    def selectInfo(self, id=None):
+        try:
+            id = id if id else self.__model_type
+
+            # filter bool type fields
+            bool_type_column = [row[1] for row in self.__c.execute(f'PRAGMA table_info({self.__each_info_dict[id][0]})').fetchall() if row[2] == 'BOOL']
+
+            # Execute the SELECT statement
+            self.__c.execute(f'SELECT {",".join(list(self.__each_info_dict[id][1].keys()))} FROM {self.__each_info_dict[id][0]}')
+
+            # Get the column names
+            column_names = [description[0] for description in self.__c.description]
+
+            row = self.__c.fetchone()
+
+            info_dict = {}
+            for i, value in enumerate(row):
+                if column_names[i] in bool_type_column:
+                    value = True if value == 1 else False
+                info_dict[column_names[i]] = value
+
+            return info_dict
+        except sqlite3.Error as e:
+            print(f"An error occurred while creating the table: {e}")
+            raise
+
+    def updateInfo(self, id, field, value):
+        try:
+            self.__c.execute(f'UPDATE {self.__each_info_dict[id][0]} SET {field}=(?) WHERE id=1', (value,))
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
 
-    def __initVal(self, db):
-        self.__db = db
+    def selectAllImage(self):
+        """
+        select all image
+        """
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__image_tb_nm}')
+            return self.__c.fetchall()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
 
-    def __initUi(self):
-        self.__beginningTextEdit = TextEditPrompt()
-        self.__beginningTextEdit.setPlaceholderText('Beginning')
-
-        self.__textEdit = TextEditPrompt()
-        self.__textEdit.setPlaceholderText('Write some text...')
-
-        # old code
-        # self.__textEdit.textChanged.connect(self.textChanged)
-        # self.__textEdit.sendSuggestionWidget.connect(self.__initPromptCommandAutocomplete)
-        # self.__textEdit.setPlaceholderText('Write some text...')
-
-        self.__endingTextEdit = TextEditPrompt()
-        self.__endingTextEdit.setPlaceholderText('Ending')
-
-        # all false by default
-        self.__beginningTextEdit.setVisible(False)
-        self.__endingTextEdit.setVisible(False)
-
-        self.__textGroup = [self.__beginningTextEdit, self.__textEdit, self.__endingTextEdit]
-        for w in self.__textGroup:
-            w.textChanged.connect(self.onUpdateSuggestion)
-            w.textChanged.connect(self.textChanged)
-            w.sendSuggestionWidget.connect(self.onSendKeySignalToSuggestion)
-
-        lay = QVBoxLayout()
-        for w in self.__textGroup:
-            lay.addWidget(w)
-        lay.setContentsMargins(0, 0, 0, 0)
-        lay.setSpacing(0)
-
-        self.setLayout(lay)
-
-    def executeCommand(self, item, grp):
-        command_key = item.text()
-        command = ''
-        for i in range(len(grp)):
-            if grp[i].get('name', '') == command_key:
-                command = grp[i].get('value', '')
-
-        w = self.getCurrentTextEdit()
-        if w:
-            cursor = w.textCursor()
-            cursor.deletePreviousChar()
-            cursor.select(QTextCursor.WordUnderCursor)
-            w.setTextCursor(cursor)
-            w.insertPlainText(command)
-
-            self.adjustHeight()
-
-    def getCurrentTextEdit(self):
-        for w in self.__textGroup:
-            if w.hasFocus():
-                return w
-
-    def setCommandEnabled(self, f: bool):
-        for w in self.__textGroup:
-            w.setCommandSuggestionEnabled(f)
+    def selectImage(self, id):
+        """
+        select specific image
+        """
+        try:
+            self.__c.execute(f'SELECT * FROM {self.__image_tb_nm} WHERE id={id}')
+            return self.__c.fetchone()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def insertImage(self, name):
+        try:
+            # Insert a row into the table
+            self.__c.execute(f'INSERT INTO {self.__image_tb_nm} (name) VALUES (?)', (name,))
+            new_id = self.__c.lastrowid
+            # Commit the transaction
+            self.__conn.commit()
+            self.__createImageUnit(new_id)
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def updateImage(self, id, name):
+        try:
+            self.__c.execute(f'UPDATE {self.__image_tb_nm} SET name=(?) WHERE id={id}', (name,))
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def deleteImage(self, id):
+        try:
+            self.__c.execute(f'DELETE FROM {self.__image_tb_nm} WHERE id={id}')
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def __createImageUnit(self, id_fk):
+        try:
+            # Check if the table exists
+            self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__image_unit_tb_nm}{id_fk}'")
+            if self.__c.fetchone()[0] == 1:
+                # each image table already exists
+                pass
+            else:
+                self.__c.execute(f'''CREATE TABLE {self.__image_unit_tb_nm}{id_fk}
+                                         (id INTEGER PRIMARY KEY,
+                                          id_fk INTEGER,
+                                          is_user INTEGER,
+                                          image TEXT,
+                                          update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                          insert_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
+                                          FOREIGN KEY (id_fk) REFERENCES {self.__image_tb_nm}(id) ON DELETE CASCADE)''')
+
+                # insert trigger
+                self.__c.execute(f'''
+                    CREATE TRIGGER image_tb_updated_by_unit_inserted_tr{id_fk}
+                    AFTER INSERT ON {self.__image_unit_tb_nm}{id_fk}
+                    BEGIN
+                      UPDATE {self.__image_tb_nm} SET update_dt = CURRENT_TIMESTAMP WHERE id = NEW.id_fk;
+                    END
+                ''')
+
+                # update trigger
+                self.__c.execute(f'''
+                    CREATE TRIGGER image_tb_updated_by_unit_updated_tr{id_fk}
+                    AFTER UPDATE ON {self.__image_unit_tb_nm}{id_fk}
+                    BEGIN
+                      UPDATE {self.__image_tb_nm} SET update_dt = CURRENT_TIMESTAMP WHERE id = NEW.id_fk;
+                    END
+                ''')
+
+                # delete trigger
+                self.__c.execute(f'''
+                    CREATE TRIGGER image_tb_updated_by_unit_deleted_tr{id_fk}
+                    AFTER DELETE ON {self.__image_unit_tb_nm}{id_fk}
+                    BEGIN
+                      UPDATE {self.__image_tb_nm} SET update_dt = CURRENT_TIMESTAMP WHERE id = OLD.id_fk;
+                    END
+                ''')
+                # Commit the transaction
+                self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def selectImageUnit(self, id):
+        self.__c.execute(f'SELECT * FROM {self.getImageUnitTableName()}{id}')
+        return [elem[3] for elem in self.__c.fetchall()]
+
+    def insertImageUnit(self, id, user_f, image):
+        try:
+            # Insert a row into the table
+            self.__c.execute(
+                f'INSERT INTO {self.__image_unit_tb_nm}{id} (id_fk, is_user, image) VALUES (?, ?, ?)',
+                (id, user_f, image,))
+            # Commit the transaction
+            self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
 
-    def adjustHeight(self) -> int:
+    def setModelType(self, model_type: int):
         """
-        adjust overall height of text edit group based on their contents and return adjusted height
+        :param model_type: it starts from 1
         :return:
         """
-        groupHeight = 0
-        for w in self.__textGroup:
-            document = w.document()
-            height = document.size().height()
-            overallHeight = int(height+document.documentMargin())
-            w.setMaximumHeight(overallHeight)
-            groupHeight += overallHeight
-        return groupHeight
-
-    def getGroup(self):
-        return self.__textGroup
-
-    def getContent(self):
-        b = self.__textGroup[0].toPlainText().strip()
-        m = self.__textGroup[1].toPlainText().strip()
-        e = self.__textGroup[2].toPlainText().strip()
-
-        content = ''
-        if b:
-            content = b + '\n'
-        content += m
-        if e:
-            content += '\n' + e
-
-        return content
-
-
-class Prompt(QWidget):
-    def __init__(self, db: SqliteDatabase):
-        super().__init__()
-        self.__initVal(db)
-        self.__initUi()
-
-    def __initVal(self, db):
-        self.__db = db
-
-        # prompt group
-        self.__p_grp = []
-
-        # False by default
-        self.__commandEnabled = False
-
-    def __initUi(self):
-        # Create the command suggestion list
-        self.__suggestionWidget = CommandSuggestionWidget()
-        self.__suggestion_list = self.__suggestionWidget.getCommandList()
-
-        self.__textEditGroup = TextEditPropmtGroup(self.__db)
-        self.__textEditGroup.textChanged.connect(self.updateHeight)
-
-        # set command suggestion
-        self.__textEditGroup.onUpdateSuggestion.connect(self.__updateSuggestions)
-        self.__textEditGroup.onSendKeySignalToSuggestion.connect(self.__sendKeysignalToSuggestion)
-        
-        self.__suggestion_list.itemClicked.connect(self.executeCommand)
-
-        lay = QVBoxLayout()
-        lay.addWidget(self.__suggestionWidget)
-        lay.addWidget(self.__textEditGroup)
-        lay.setContentsMargins(0, 0, 0, 0)
-        lay.setSpacing(0)
-
-        leftWidget = QWidget()
-        leftWidget.setLayout(lay)
-
-        settingsBtn = SvgToolButton()
-        settingsBtn.setIcon('ico/vertical_three_dots.svg')
-        settingsBtn.setToolTip('Prompt Settings')
-
-        # Create the menu
-        menu = QMenu(self)
-
-        # Create the actions
-        beginningAction = QAction("Show Beginning", self)
-        beginningAction.setShortcut('Ctrl+B')
-        beginningAction.setCheckable(True)
-        beginningAction.toggled.connect(self.__showBeginning)
-
-        endingAction = QAction("Show Ending", self)
-        endingAction.setShortcut('Ctrl+E')
-        endingAction.setCheckable(True)
-        endingAction.toggled.connect(self.__showEnding)
-
-        supportPromptCommandAction = QAction('Support Prompt Command', self)
-        supportPromptCommandAction.setShortcut('Ctrl+Shift+P')
-        supportPromptCommandAction.setCheckable(True)
-        supportPromptCommandAction.toggled.connect(self.__supportPromptCommand)
-
-        # Add the actions to the menu
-        menu.addAction(beginningAction)
-        menu.addAction(endingAction)
-        menu.addAction(supportPromptCommandAction)
-
-        # Connect the button to the menu
-        settingsBtn.setMenu(menu)
-        settingsBtn.setPopupMode(QToolButton.InstantPopup)
-
-        lay = QVBoxLayout()
-        lay.addWidget(settingsBtn)
-        lay.setContentsMargins(1, 1, 1, 1)
-        lay.setAlignment(Qt.AlignBottom)
-
-        rightWidget = QWidget()
-        rightWidget.setLayout(lay)
-
-        lay = QHBoxLayout()
-        lay.addWidget(leftWidget)
-        lay.addWidget(rightWidget)
-        lay.setContentsMargins(0, 0, 0, 0)
-        lay.setSpacing(0)
-        self.setLayout(lay)
-
-        self.__suggestionWidget.setVisible(False)
-
-        self.updateHeight()
-
-    def __getEveryPromptCommands(self):
-        # get prop group
-        p_grp = []
-        for group in self.__db.selectPropPromptGroup():
-            p_grp_attr = [attr for attr in self.__db.selectPropPromptAttribute(group[0])]
-            p_grp_value = ''
-            for attr_obj in p_grp_attr:
-                name = attr_obj[2]
-                value = attr_obj[3]
-                if value and value.strip():
-                    p_grp_value += f'{name}: {value}\n'
-            p_grp.append({'name': group[1], 'value': p_grp_value})
-
-        # get template group
-        t_grp = []
-        for group in self.__db.selectTemplatePromptGroup():
-            t_grp_attr = [attr for attr in self.__db.selectTemplatePromptUnit(group[0])]
-            t_grp_value = ''
-            for attr_obj in t_grp_attr:
-                name = attr_obj[2]
-                value = attr_obj[3]
-                t_grp.append({'name': f'{attr_obj[2]}({group[1]})', 'value': value})
-
-        self.__p_grp = p_grp+t_grp
-
-        # TODO will include value as well
-        return [command['name'] for command in self.__p_grp]
-
-    def __updateSuggestions(self):
-        w = self.__textEditGroup.getCurrentTextEdit()
-        if w and self.__commandEnabled:
-            input_text_chunk = w.toPlainText().split()
-            input_text_chunk_exists = len(input_text_chunk) > 0
-            self.__suggestionWidget.setVisible(input_text_chunk_exists)
-            if input_text_chunk_exists:
-                input_text_chunk = input_text_chunk[-1]
-                starts_with_f = input_text_chunk.startswith('/')
-                self.__suggestionWidget.setVisible(starts_with_f)
-                w.setCommandSuggestionEnabled(starts_with_f)
-                if starts_with_f:
-                    command_word = input_text_chunk[1:]
-
-                    # Example: Add some dummy command suggestions
-                    commands = self.__getEveryPromptCommands()
-                    filtered_commands = commands
-                    if command_word:
-                        filtered_commands = [command for command in commands if command_word.lower() in command.lower()]
-                    filtered_commands_exists_f = len(filtered_commands) > 0
-                    self.__suggestionWidget.setVisible(filtered_commands_exists_f)
-                    if filtered_commands_exists_f:
-                        # Clear previous suggestions
-                        self.__suggestion_list.clear()
-
-                        # Add the filtered suggestions to the list
-                        self.__suggestion_list.addItems(filtered_commands)
-                        self.__suggestion_list.setCurrentRow(0)
-
-    def __sendKeysignalToSuggestion(self, key):
-        if key == 'up':
-            self.__suggestion_list.setCurrentRow(max(0, self.__suggestion_list.currentRow() - 1))
-        elif key == 'down':
-            self.__suggestion_list.setCurrentRow(
-                min(self.__suggestion_list.currentRow() + 1, self.__suggestion_list.count() - 1))
-        elif key == 'enter':
-            self.executeCommand(self.__suggestion_list.currentItem())
-
-    def executeCommand(self, item):
-        self.__textEditGroup.executeCommand(item, self.__p_grp)
-
-    def updateHeight(self):
-        overallHeight = self.__textEditGroup.adjustHeight()
-        self.setMaximumHeight(overallHeight + self.__suggestionWidget.maximumHeight())
-
-    def getTextEdit(self):
-        return self.__textEditGroup.getGroup()[1]
-
-    def getContent(self):
-        return self.__textEditGroup.getContent()
-
-    def __showBeginning(self, f):
-        self.__textEditGroup.getGroup()[0].setVisible(f)
-
-    def __showEnding(self, f):
-        self.__textEditGroup.getGroup()[-1].setVisible(f)
-
-    def __supportPromptCommand(self, f):
-        self.__commandEnabled = f
-        self.__textEditGroup.setCommandEnabled(f)
-
+        self.__model_type = model_type
 
+    def export(self, ids, saved_filename):
+        shutil.copy2(self.__db_filename, saved_filename)
+        conn = sqlite3.connect(saved_filename)
+
+        placeholders = ','.join('?' for _ in ids)
+        cursor = conn.cursor()
+        for i in range(len(ids)):
+            delete_image_q = f"DELETE FROM {self.__image_tb_nm} WHERE id in ({placeholders})"
+            cursor.execute(delete_image_q, ids)
+            drop_image_unit_tb_q = f"DROP TABLE {self.__image_unit_tb_nm}{ids[i]}"
+            cursor.execute(drop_image_unit_tb_q)
+            conn.commit()
+
+        conn.close()
+
+    def imageertJsonIntoSql(self):
+        try:
+            # Read data from json
+            with open('test/image_history.json', 'r') as f:
+                data = json.load(f)
+                for obj in list(data.values())[0]:
+                    id, title, image_data = obj.values()
+                    # start from 1 in sql unlike json which starts from 0
+                    id += 1
+                    self.insertImage(title)
+                    for i in range(len(image_data)):
+                        # Insert a row into the table
+                        self.__c.execute(
+                            f'INSERT INTO {self.__image_unit_tb_nm}{id} (id_fk, is_user, image) VALUES (?, ?, ?)',
+                            (id, i % 2 == 0, image_data[i],))
+                        # Commit the transaction
+                        self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred: {e}")
+            raise
+
+    def getCursor(self):
+        return self.__c
+
+    def getImageTableName(self):
+        return self.__image_tb_nm
+
+    def getImageUnitTableName(self):
+        return self.__image_unit_tb_nm
+
+    def close(self):
+        self.__conn.close()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        # Close the connection
+        self.__conn.close()
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/circleProfileImage.py` & `pyqt-openai-0.1.72/pyqt_openai/circleProfileImage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/commandCompleter.py` & `pyqt-openai-0.1.72/pyqt_openai/commandCompleter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtWidgets import QWidget, QTableWidget, QHeaderView, QVBoxLayout, QLineEdit, QScrollArea, QLabel, \
-    QStyledItemDelegate, \
+from qtpy.QtCore import Qt, pyqtSignal
+from qtpy.QtWidgets import QTableWidget, QHeaderView, QScrollArea, QStyledItemDelegate, \
     QStyle, QTableWidgetItem
 
 
 class CommandCompleterTableWidgetDelegate(QStyledItemDelegate):
     def paint(self, painter, option, index):
         # Check if the item is selected
         if option.state & QStyle.State_Active:
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/convListWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/convListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/customizeDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/customizeDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/close.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/close.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/customize.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/customize.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/discord.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/discord.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/github.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/github.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/help.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/help.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/history.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/history.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/openai.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/openai.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/save.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/save.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/search.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/search.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/setting.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/setting.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/stackontop.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/stackontop.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/ico/user.svg` & `pyqt-openai-0.1.72/pyqt_openai/ico/user.svg`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/currentImageView.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/currentImageView.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/explorerWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/explorerWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageDallEPage.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageDallEPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageGeneratingToolWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageListWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageListWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/imageStableDiffusionPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/leftSideBar.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/leftSideBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,17 @@
     # 
     def __deleteClicked(self):
         # get the ID of row, not actual index (because list is in a stacked form)
         rows = self.__imageListWidget.getCheckedRowsIds()
         self.__imageListWidget.removeCheckedRows()
         self.deleted.emit(rows)
         self.__allCheckBox.setChecked(False)
+
     def __saveClicked(self):
-        self.export.emit(self.__imageListWidget.getUncheckedRowsIds())
+        self.export.emit(self.__imageListWidget.getCheckedRowsIds())
     # 
     def __stateChanged(self, f):
         self.__imageListWidget.toggleState(f)
     # 
     def __search(self, text):
         for i in range(self.__imageListWidget.count()):
             item = self.__imageListWidget.item(i)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/rightSideBar.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/rightSideBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/thumbnailView.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/thumbnailView.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/image_gen_widget/viewWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/image_gen_widget/viewWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/inputDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/leftSideBar.py` & `pyqt-openai-0.1.72/pyqt_openai/leftSideBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         # get the ID of row, not actual index (because list is in a stacked form)
         rows = self.__convListWidget.getCheckedRowsIds()
         self.__convListWidget.removeCheckedRows()
         self.deleted.emit(rows)
         self.__allCheckBox.setChecked(False)
 
     def __saveClicked(self):
-        self.export.emit(self.__convListWidget.getUncheckedRowsIds())
+        self.export.emit(self.__convListWidget.getCheckedRowsIds())
 
     def __stateChanged(self, f):
         self.__convListWidget.toggleState(f)
 
     def __search(self, text):
         for i in range(self.__convListWidget.count()):
             item = self.__convListWidget.item(i)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/main.py` & `pyqt-openai-0.1.72/pyqt_openai/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def __setAIEnabled(self, f):
         self.__openAiChatBotWidget.setAIEnabled(f)
         self.__imageGeneratingToolWidget.setAIEnabled(f)
 
     def __setApi(self):
         try:
             api_key = self.__apiLineEdit.text()
-            response = requests.get('https://api.openai.com/v1/engines', headers={'Authorization': f'Bearer {api_key}'})
+            response = requests.get('https://api.openai.com/v1/models', headers={'Authorization': f'Bearer {api_key}'})
             f = response.status_code == 200
             self.__setAIEnabled(f)
             if f:
                 self.__setApiKey(api_key)
                 self.__settings_struct.setValue('API_KEY', api_key)
 
                 self.__openAiChatBotWidget.setModelInfoByModel(True)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/modelTable.py` & `pyqt-openai-0.1.72/pyqt_openai/modelTable.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/notifier.py` & `pyqt-openai-0.1.72/pyqt_openai/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/openAiChatBotWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/openAiChatBotWidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import os
 import webbrowser
 
 from qtpy.QtCore import Qt, QSettings, Signal
 from qtpy.QtWidgets import QHBoxLayout, QWidget, QSizePolicy, QVBoxLayout, QFrame, QSplitter, \
     QListWidgetItem, QFileDialog
 
-from pyqt_openai.apiData import ModelData
-from pyqt_openai.chatWidget import Prompt, ChatBrowser
+from pyqt_openai.apiData import ModelData, getChatModel
+from pyqt_openai.chat_widget.chatBrowser import ChatBrowser
+from pyqt_openai.chat_widget.prompt import Prompt
 from pyqt_openai.leftSideBar import LeftSideBar
 from pyqt_openai.notifier import NotifierWidget
 from pyqt_openai.openAiThread import OpenAIThread
 from pyqt_openai.prompt_gen_widget.promptGeneratorWidget import PromptGeneratorWidget
 from pyqt_openai.right_sidebar.aiPlaygroundWidget import AIPlaygroundWidget
+from pyqt_openai.util.script import open_directory, get_generic_ext_out_of_qt_ext, conv_unit_to_txt, conv_unit_to_html, \
+    add_file_to_zip
 from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgButton import SvgButton
 
 
 class OpenAIChatBotWidget(QWidget):
     notifierWidgetActivated = Signal()
 
@@ -201,18 +204,18 @@
         if self.__remember_past_conv:
             convs = []
             with open('conv.json', 'r') as f:
                 for line in f:
                     conv = json.loads(line.strip())
                     convs.append(conv)
         # TODO refactoring
-        if info_dict['engine'] in ['gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4']:
+        if info_dict['model'] in getChatModel():
             # "assistant" below is for making the AI remember the last question
             openai_arg = {
-                'model': info_dict['engine'],
+                'model': info_dict['model'],
                 'messages': [
                     {"role": "system", "content": info_dict['system']},
                     {"role": "assistant", "content": self.__browser.getAllText()},
                     {"role": "user", "content": self.__prompt.getContent()},
                 ],
                 # 'temperature': info_dict['temperature'],
 
@@ -221,29 +224,29 @@
                 # https://platform.openai.com/docs/api-reference/chat/create
                 # 'max_tokens': self.__max_tokens,
 
                 # 'top_p': info_dict['top_p'],
                 # 'frequency_penalty': info_dict['frequency_penalty'],
                 # 'presence_penalty': info_dict['presence_penalty'],
 
-                'stream': info_dict['stream'],
+                'stream': True if info_dict['stream'] == 1 else False,
             }
         else:
             openai_arg = info_dict
         if self.__leftSideBarWidget.isCurrentConvExists():
             pass
         else:
             self.__addConv()
 
         self.__lineEdit.setEnabled(False)
         self.__leftSideBarWidget.setEnabled(False)
 
         self.__browser.showLabel(self.__prompt.getContent(), True, False)
 
-        self.__t = OpenAIThread(info_dict['engine'], openai_arg, self.__remember_past_conv)
+        self.__t = OpenAIThread(info_dict['model'], openai_arg, self.__remember_past_conv)
         self.__t.replyGenerated.connect(self.__browser.showLabel)
         self.__t.streamFinished.connect(self.__browser.streamFinished)
         self.__lineEdit.clear()
         self.__t.start()
         self.__t.finished.connect(self.__afterGenerated)
 
     def __afterGenerated(self):
@@ -256,15 +259,15 @@
             self.__notifierWidget.doubleClicked.connect(self.notifierWidgetActivated)
 
     def __changeConv(self, item: QListWidgetItem):
         # If a 'change' event occurs but there are no items, it should mean that list is empty
         # so reset conv_history.json
         if item:
             id = item.data(Qt.UserRole)
-            conv = self.__db.selectConvUnit(id)
+            conv = self.__db.selectCertainConvHistory(id)
             self.__browser.replaceConv(id, conv)
         else:
             self.__browser.resetChatWidget(0)
 
 
     def __addConv(self):
         cur_id = self.__db.insertConv('New Chat')
@@ -272,22 +275,31 @@
         self.__leftSideBarWidget.addToList(cur_id)
         self.__lineEdit.setFocus()
 
     def __updateConv(self, id, title=None):
         if title:
             self.__db.updateConv(id, title)
 
-
     def __deleteConv(self, id_lst):
         for id in id_lst:
             self.__db.deleteConv(id)
 
-
     def __export(self, ids):
-        filename = QFileDialog.getSaveFileName(self, 'Save', os.path.expanduser('~'), 'SQLite DB file (*.db)')
-        if filename[0]:
-            filename = filename[0]
-            self.__db.export(ids, filename)
+        file_data = QFileDialog.getSaveFileName(self, 'Save', os.path.expanduser('~'), 'SQLite DB file (*.db);;txt files Compressed File (*.zip);;html files Compressed File (*.zip)')
+        if file_data[0]:
+            filename = file_data[0]
+            ext = os.path.splitext(filename)[-1] or get_generic_ext_out_of_qt_ext(file_data[1])
+            if ext == '.zip':
+                compressed_file_type = file_data[1].split(' ')[0].lower()
+                ext_dict = {'txt': {'ext':'.txt', 'func':conv_unit_to_txt}, 'html': {'ext':'.html', 'func':conv_unit_to_html}}
+                for id in ids:
+                    title = self.__db.selectConv(id)[1]
+                    txt_filename = f'{title}{ext_dict[compressed_file_type]["ext"]}'
+                    txt_content = ext_dict[compressed_file_type]['func'](self.__db, id, title)
+                    add_file_to_zip(txt_content, txt_filename, os.path.splitext(filename)[0] + '.zip')
+            elif ext == '.db':
+                self.__db.export(ids, filename)
+            open_directory(os.path.dirname(filename))
 
     def __updateConvUnit(self, id, user_f, conv_unit=None):
         if conv_unit:
             self.__db.insertConvUnit(id, user_f, conv_unit)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/openAiThread.py` & `pyqt-openai-0.1.72/pyqt_openai/openAiThread.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     replyGenerated = Signal(str, bool, bool)
     streamFinished = Signal()
 
     def __init__(self, model, openai_arg, remember_f, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__model = model
+        print(model)
         self.__endpoint = getModelEndpoint(model)
         self.__openai_arg = openai_arg
         self.__remember_f = remember_f
 
     def run(self):
         try:
             if self.__endpoint == '/v1/chat/completions':
@@ -61,11 +62,10 @@
 
                     with open('conv.json', 'a') as f:
                         f.write(json.dumps(conv) + '\n')
 
                 self.replyGenerated.emit(response_text, False, False)
         except openai.error.InvalidRequestError as e:
             print(e)
-            self.replyGenerated.emit('<p style="color:red">Your request was rejected as a result of our safety system.<br/>'
-                                     'Your prompt may contain text that is not allowed by our safety system.</p>', False, False)
+            self.replyGenerated.emit(f'<p style="color:red">{e}</p>', False, False)
         except openai.error.RateLimitError as e:
             self.replyGenerated.emit(f'<p style="color:red">{e}<br/>Check the usage: https://platform.openai.com/account/usage<br/>Update to paid account: https://platform.openai.com/account/billing/overview', False, False)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/promptGeneratorWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/promptGroupInputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPage.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/propPage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/propPromptUnitInputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePage.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/templatePage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QLabel, QSpacerItem, QListWidget, QListWidgetItem, QSizePolicy, QStackedWidget, QSplitter
+from qtpy.QtWidgets import QLabel, QSpacerItem, QListWidget, QListWidgetItem, QSizePolicy, QStackedWidget, QSplitter
 from qtpy.QtWidgets import QWidget, QDialog, QTableWidget, QVBoxLayout, QHBoxLayout, QHeaderView, QTableWidgetItem, QAbstractItemView
 from qtpy.QtCore import Signal, Qt
 
 from pyqt_openai.inputDialog import InputDialog
 from pyqt_openai.prompt_gen_widget.promptGroupInputDialog import PromptGroupInputDialog
 from pyqt_openai.prompt_gen_widget.templatePromptUnitInputDialog import TemplatePromptUnitInputDialog
 from pyqt_openai.sqlite import SqliteDatabase
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py` & `pyqt-openai-0.1.72/pyqt_openai/prompt_gen_widget/templatePromptUnitInputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/propmt_command_completer/commandSuggestionWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/propmt_command_completer/commandSuggestionWidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5.QtWidgets import QListWidget, QWidget, QVBoxLayout, QLabel
+from qtpy.QtWidgets import QListWidget, QWidget, QVBoxLayout, QLabel
 
 
 class CommandSuggestionWidget(QWidget):
     def __init__(self):
         super().__init__()
         self.__initUi()
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/aiPlaygroundWidget.py` & `pyqt-openai-0.1.72/pyqt_openai/right_sidebar/aiPlaygroundWidget.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/chatPage.py` & `pyqt-openai-0.1.72/pyqt_openai/right_sidebar/chatPage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from qtpy.QtWidgets import QWidget, QComboBox, QTextEdit, QLabel, QVBoxLayout, QApplication, QCheckBox, QDoubleSpinBox, \
-    QSpinBox, QPushButton
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import QWidget, QSizePolicy, QComboBox, QTextEdit, QLabel, QVBoxLayout, QCheckBox, QPushButton
 
 from pyqt_openai.apiData import getChatModel
 from pyqt_openai.sqlite import SqliteDatabase
 
 
 class ChatPage(QWidget):
     def __init__(self, db: SqliteDatabase, ini_etc_dict):
@@ -12,38 +12,39 @@
         self.__initUi()
 
     def __setChatInfo(self, db):
         self.__db = db
         self.__info_dict = self.__db.selectInfo(1)
 
         # # set each field as variable since these are being used a lot
-        # engine = info_dict['engine']
+        # model = info_dict['model']
         # temperature = info_dict['temperature']
         # max_tokens = info_dict['max_tokens']
         # top_p = info_dict['top_p']
         # frequency_penalty = info_dict['frequency_penalty']
         # presence_penalty = info_dict['presence_penalty']
         # stream = info_dict['stream']
 
-    def __initVal(self, db, ini_etc_dict):
-        self.__setChatInfo(db)
-
         # set each field as variable since these are being used a lot
         self.__stream = self.__info_dict.get('stream', False)
 
+    def __initVal(self, db, ini_etc_dict):
+        self.__setChatInfo(db)
         self.__ini_etc_dict = ini_etc_dict
 
     def __initUi(self):
         systemlbl = QLabel('System')
         self.__systemTextEdit = QTextEdit()
         self.__systemTextEdit.setText('You are a helpful assistant.')
+        self.__systemTextEdit.setSizePolicy(QSizePolicy.MinimumExpanding, QSizePolicy.Preferred)
         saveSystemBtn = QPushButton('Save System')
         saveSystemBtn.clicked.connect(self.__saveSystem)
         modelCmbBox = QComboBox()
         modelCmbBox.addItems(getChatModel())
+        modelCmbBox.setCurrentText(self.__info_dict['model'])
         modelCmbBox.currentTextChanged.connect(self.__modelChanged)
 
         # temperatureSpinBox = QDoubleSpinBox()
         # temperatureSpinBox.setRange(0, 1)
         # temperatureSpinBox.setAccelerated(True)
         # temperatureSpinBox.setSingleStep(0.01)
         # # temperatureSpinBox.setValue(self.__info_dict['temperature'])
@@ -90,25 +91,26 @@
         lay = QVBoxLayout()
         lay.addWidget(systemlbl)
         lay.addWidget(self.__systemTextEdit)
         lay.addWidget(saveSystemBtn)
         lay.addWidget(modelCmbBox)
         lay.addWidget(streamChkBox)
         lay.addWidget(finishReasonChkBox)
+        lay.setAlignment(Qt.AlignTop)
 
         self.setLayout(lay)
 
     def __saveSystem(self):
         self.__info_dict['system'] = self.__systemTextEdit.toPlainText()
         self.__db.updateInfo(1, 'system', self.__info_dict['system'])
 
     def __modelChanged(self, v):
-        self.__info_dict['engine'] = v
+        self.__info_dict['model'] = v
         # self.setModelInfoByModel()
-        self.__db.updateInfo(1, 'engine', v)
+        self.__db.updateInfo(1, 'model', v)
 
     def __streamChecked(self, f):
         self.__stream = f
         self.__db.updateInfo(1, 'stream', f)
 
     def __finishReasonChecked(self, f):
         self.__finishReason = f
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/completionPage.py` & `pyqt-openai-0.1.72/pyqt_openai/right_sidebar/completionPage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import platform, subprocess
+import platform
+import subprocess
 
+from qtpy.QtCore import Qt, QSettings
 from qtpy.QtGui import QFont
-from qtpy.QtWidgets import QWidget, QComboBox, QTextEdit, QLabel, QVBoxLayout, QApplication, QCheckBox, QDoubleSpinBox, \
+from qtpy.QtWidgets import QWidget, QComboBox, QLabel, QVBoxLayout, QCheckBox, QDoubleSpinBox, \
     QSpinBox, QFormLayout, QHBoxLayout, QFileDialog, QPushButton, QLineEdit, QGroupBox
-from qtpy.QtCore import Qt, QSettings
 
-from pyqt_openai.apiData import getCompletionModel, getLatestModel
+from pyqt_openai.apiData import getCompletionModel
 from pyqt_openai.modelTable import ModelTable
 from pyqt_openai.sqlite import SqliteDatabase
 from pyqt_openai.svgLabel import SvgLabel
 
 
 class CompletionPage(QWidget):
     def __init__(self, db: SqliteDatabase, ini_etc_dict, model_data):
@@ -28,15 +29,15 @@
 
         self.__modelData = model_data
         self.__ini_etc_dict = ini_etc_dict
 
     def __initUi(self):
         self.__modelComboBox = QComboBox()
         self.__modelComboBox.addItems(getCompletionModel())
-        self.__modelComboBox.setCurrentText(self.__info_dict['engine'])
+        self.__modelComboBox.setCurrentText(self.__info_dict['model'])
         self.__modelComboBox.currentTextChanged.connect(self.__modelChanged)
 
         self.__fineTuningBtn = QPushButton('Fine Tuning')
         self.__fineTuningBtn.clicked.connect(self.__fineTuning)
 
         # find the training data
         self.__findDataLineEdit = QLineEdit()
@@ -212,15 +213,15 @@
         self.__modelComboBox.currentTextChanged.connect(self.__modelChanged)
         self.__modelComboBox.setCurrentText(curModel)
 
     # for fine-tuning, showing the detailed information of the model
     def setModelInfoByModel(self, init_model: bool = False):
         if init_model:
             self.__modelData.setModelData()
-        self.__modelTable.setModelInfo(self.__modelData.getModelData(), self.__info_dict['engine'], 'allow_fine_tuning')
+        self.__modelTable.setModelInfo(self.__modelData.getModelData(), self.__info_dict['model'], 'allow_fine_tuning')
         self.__fineTuningBtn.setEnabled(self.__modelTable.getModelInfo())
 
     def __findData(self):
         filename = QFileDialog.getOpenFileName(self, 'Open', '', 'JSONL Files (*.jsonl)')
         if filename[0]:
             filename = filename[0]
             self.__findDataLineEdit.setText(filename)
@@ -254,13 +255,13 @@
         # and other information
         # subprocess.run('openai api fine_tunes.get -i [YOUR_FINE_TUNE_JOB_ID]')
 
         # cancel the job
         # subprocess.run('openai api fine_tunes.cancel -i [YOUR_FINE_TUNE_JOB_ID]')
 
     def __modelChanged(self, v):
-        self.__info_dict['engine'] = v
+        self.__info_dict['model'] = v
         self.setModelInfoByModel()
-        self.__db.updateInfo(2, 'engine', v)
+        self.__db.updateInfo(2, 'model', v)
 
     def __rememberPastConversationChkBoxToggled(self, f):
         self.__settings_struct.setValue('REMEMBER_PAST_CONVERSATION', str(int(f)))
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/right_sidebar/imagePage.py` & `pyqt-openai-0.1.72/pyqt_openai/right_sidebar/imagePage.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/searchBar.py` & `pyqt-openai-0.1.72/pyqt_openai/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/sqlite.py` & `pyqt-openai-0.1.72/pyqt_openai/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 class SqliteDatabase:
     """
     functions which only meant to be used frequently are defined.
 
     if there is no functions you want to use, use ``getCursor`` instead
     """
-    def __init__(self):
+    def __init__(self, db_filename='conv.db'):
         super().__init__()
-        self.__initVal()
+        self.__initVal(db_filename)
         self.__initDb()
         self.__createConv()
 
-    def __initVal(self):
+    def __initVal(self, db_filename):
         # db names
-        self.__db_filename = 'conv.db'
+        self.__db_filename = db_filename or 'conv.db'
 
         # conv table names
         self.__conv_tb_nm = 'conv_tb'
         self.__conv_tb_tr_nm = 'conv_tr'
         self.__conv_unit_tb_nm = 'conv_unit_tb'
 
         # info table names
@@ -35,38 +35,38 @@
 
         # model type (chat, etc.)
         self.__model_type = 1
 
         # default value of each properties based on https://platform.openai.com/docs/api-reference/chat/create
         # GPT-3.5(ChatGPT), GPT-4
         self.__chat_default_value = {
-            'engine': "gpt-3.5-turbo",
+            'model': "gpt-3.5-turbo",
             'system': "You are a helpful assistant.",
             'temperature': 0.7,
             # -1 means infinite, not currently used in this application
             'max_tokens': -1,
             'top_p': 1,
             'frequency_penalty': 0,
             'presence_penalty': 0,
             'stream': True
         }
 
         # GPT-3, etc.
         self.__completion_default_value = {
-            'engine': "text-davinci-003",
+            'model': "text-davinci-003",
             'temperature': 0.7,
             'max_tokens': 4096,
             'top_p': 1,
             'frequency_penalty': 0,
             'presence_penalty': 0,
         }
 
         # DALL-E
         self.__image_default_value = {
-            'engine': "DALL-E",
+            'model': "DALL-E",
             'n': 1,
             'width': 1024,
             'height': 1024,
             # 'response_format':
         }
 
         self.__each_info_dict = {1: [self.__info_tb_nm, self.__chat_default_value],
@@ -115,15 +115,15 @@
                 d_value = self.__chat_default_value[col]
                 if isinstance(self.__chat_default_value[col], str):
                     d_value = f'"{d_value}"' if len(self.__chat_default_value[col].split()) > 0 else d_value
                 self.__c.execute(f"ALTER TABLE {self.__info_tb_nm} ADD COLUMN {col} DEFAULT {d_value}")
         else:
             self.__c.execute(f'''CREATE TABLE {self.__info_tb_nm}
                                      (id INTEGER PRIMARY KEY,
-                                      engine VARCHAR(50) DEFAULT '{self.__chat_default_value['engine']}',
+                                      model VARCHAR(50) DEFAULT '{self.__chat_default_value['model']}',
                                       system TEXT DEFAULT '{self.__chat_default_value['system']}',
                                       temperature INTEGER DEFAULT {self.__chat_default_value['temperature']},
                                       max_tokens INTEGER DEFAULT {self.__chat_default_value['max_tokens']},
                                       top_p INTEGER DEFAULT {self.__chat_default_value['top_p']},
                                       frequency_penalty INTEGER DEFAULT {self.__chat_default_value['frequency_penalty']},
                                       presence_penalty INTEGER DEFAULT {self.__chat_default_value['presence_penalty']},
                                       stream BOOL DEFAULT {self.__chat_default_value['stream']},
@@ -133,15 +133,15 @@
 
             # Commit the transaction
             self.__conn.commit()
 
             # insert default record
             self.__c.execute(f'''INSERT INTO {self.__info_tb_nm}
                                             (
-                                                engine,
+                                                model,
                                                 system,
                                                 temperature,
                                                 max_tokens,
                                                 top_p,
                                                 frequency_penalty,
                                                 presence_penalty,
                                                 stream
@@ -156,15 +156,15 @@
         self.__c.execute(
             f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__completion_info_tb_nm}'")
         if self.__c.fetchone()[0] == 1:
             pass
         else:
             self.__c.execute(f'''CREATE TABLE {self.__completion_info_tb_nm}
                                              (id INTEGER PRIMARY KEY,
-                                              engine VARCHAR(50) DEFAULT '{self.__completion_default_value['engine']}',
+                                              model VARCHAR(50) DEFAULT '{self.__completion_default_value['model']}',
                                               temperature INTEGER DEFAULT {self.__completion_default_value['temperature']},
                                               max_tokens INTEGER DEFAULT {self.__completion_default_value['max_tokens']},
                                               top_p INTEGER DEFAULT {self.__completion_default_value['top_p']},
                                               frequency_penalty INTEGER DEFAULT {self.__completion_default_value['frequency_penalty']},
                                               presence_penalty INTEGER DEFAULT {self.__completion_default_value['presence_penalty']},
 
                                               update_dt DATETIME DEFAULT CURRENT_TIMESTAMP,
@@ -172,15 +172,15 @@
 
             # Commit the transaction
             self.__conn.commit()
 
             # insert default record
             self.__c.execute(f'''INSERT INTO {self.__completion_info_tb_nm}
                                                     (
-                                                        engine,
+                                                        model,
                                                         temperature,
                                                         max_tokens,
                                                         top_p,
                                                         frequency_penalty,
                                                         presence_penalty
                                                     ) VALUES
                                                     (
@@ -476,20 +476,41 @@
             self.__createChat()
             self.__createCompletion()
 
             # prompt information
             self.__createPropPromptGroup()
             self.__createTemplatePromptGroup()
 
+            # engine -> model
+            self.__updateColumnName(self.__info_tb_nm)
+            self.__updateColumnName(self.__completion_info_tb_nm)
+
             # Commit the transaction
             self.__conn.commit()
         except sqlite3.Error as e:
             print(f"An error occurred while creating the table: {e}")
             raise
 
+    def __updateColumnName(self, tb_name):
+        try:
+            # Get the table information
+            self.__c.execute(f"PRAGMA table_info({tb_name})")
+            columns = self.__c.fetchall()
+
+            # Check if "name" column exists
+            column_exists = any(column[1] == "engine" for column in columns)
+
+            # Alter column name if it exists
+            if column_exists:
+                self.__c.execute(f"ALTER TABLE {tb_name} RENAME COLUMN engine TO model")
+                self.__conn.commit()
+        except sqlite3.Error as e:
+            print(f"An error occurred while creating the table: {e}")
+            raise
+
     def __createConv(self):
         try:
             # Check if the table exists
             self.__c.execute(f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{self.__conv_tb_nm}'")
             if self.__c.fetchone()[0] == 1:
                 # each conv table already exists
                 pass
@@ -688,17 +709,20 @@
                 ''')
                 # Commit the transaction
                 self.__conn.commit()
         except sqlite3.Error as e:
             print(f"An error occurred: {e}")
             raise
 
-    def selectConvUnit(self, id):
+    def selectCertainConv(self, id):
         self.__c.execute(f'SELECT * FROM {self.getConvUnitTableName()}{id}')
-        return [elem[3] for elem in self.__c.fetchall()]
+        return self.__c.fetchall()
+
+    def selectCertainConvHistory(self, id):
+        return [elem[3] for elem in self.selectCertainConv(id)]
 
     def insertConvUnit(self, id, user_f, conv):
         try:
             # Insert a row into the table
             self.__c.execute(
                 f'INSERT INTO {self.__conv_unit_tb_nm}{id} (id_fk, is_user, conv) VALUES (?, ?, ?)',
                 (id, user_f, conv,))
@@ -715,26 +739,14 @@
         :param model_type: it starts from 1
         :return:
         """
         self.__model_type = model_type
 
     def export(self, ids, saved_filename):
         shutil.copy2(self.__db_filename, saved_filename)
-        conn = sqlite3.connect(saved_filename)
-
-        placeholders = ','.join('?' for _ in ids)
-        cursor = conn.cursor()
-        for i in range(len(ids)):
-            delete_conv_q = f"DELETE FROM {self.__conv_tb_nm} WHERE id in ({placeholders})"
-            cursor.execute(delete_conv_q, ids)
-            drop_conv_unit_tb_q = f"DROP TABLE {self.__conv_unit_tb_nm}{ids[i]}"
-            cursor.execute(drop_conv_unit_tb_q)
-            conn.commit()
-
-        conn.close()
 
     # legacy
     def convertJsonIntoSql(self):
         try:
             # Read data from json
             with open('test/conv_history.json', 'r') as f:
                 data = json.load(f)
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai/svgButton.py` & `pyqt-openai-0.1.72/pyqt_openai/svgButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/svgLabel.py` & `pyqt-openai-0.1.72/pyqt_openai/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/svgToolButton.py` & `pyqt-openai-0.1.72/pyqt_openai/svgToolButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/test/sqlalchemy_example.py` & `pyqt-openai-0.1.72/pyqt_openai/test/sqlalchemy_example.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai/toast.py` & `pyqt-openai-0.1.72/pyqt_openai/toast.py`

 * *Files identical despite different names*

### Comparing `pyqt-openai-0.1.61/pyqt_openai.egg-info/PKG-INFO` & `pyqt-openai-0.1.72/pyqt_openai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: pyqt-openai
-Version: 0.1.61
+Version: 0.1.72
 Summary: PyQt OpenAI example
 Home-page: https://github.com/yjg30737/pyqt-openai.git
 Author: Jung Gyu Yoon
 Author-email: yjg30737@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pyqt-openai
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png">
-</p>
+<div align="center">
+  <img src="https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-400f-9628-b8e0044d3f7b.png" width="150px" height="150px"><br/><br/>
+  
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/cHekprskVE)
+</div>
+
 
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit)
 
 This shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or Stable Diffusion as a image generation tool.
 
 Even though this project has become too huge to be called an 'example'.
 
 The major advantage of this package is that you don't need to know other language aside from Python.
 
 If you want to study openai with Python-only good old desktop software, this is for you.
 
 The OpenAI model this package uses is the <a href="https://platform.openai.com/docs/models/gpt-3-5">gpt-3.5-turbo</a> model(which is nearly as functional as <b>ChatGPT</b>) by default. You can use gpt-4 as well.
 
+Latest model such as gpt-3.5-turbo-0613 is also available
+
 Image generation feature(DALL-E and Stable Diffusion) available since v0.1.4.
 
 <b>Stable Diffusion</b> used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-webgui. 
 
 But this is very lightweight and more accessible. don't need CUDA, torch, expansive PC, anything.
 
 This is using <b>sqlite</b> as a database.
@@ -49,17 +54,18 @@
 * [Note](#note)
 * [See Also](#see-also)
 
 ## Feature
 * basically this is <b>desktop application version of ChatGPT</b> with image generation tool. 
   * text streaming (enable by default, you can disable it)
   * AI remembers past conversation
+  * support copy button
 * conversation management
   * add & delete conversations
-  * save conversations
+  * save conversations - SQlite db, text files compressed file, html files compressed file (both are zip)
   * rename conversation
   * everything above is saved in an SQLite database file named conv.db.
 * support GPT-4 and every other models below GPT3
 * support prompt generator (manageable, autosaved in database) 
 * support slash commands
 * support beginning and ending part of the prompt
 * you can run this in background application
@@ -71,14 +77,15 @@
 ## Requirements
 * qtpy - the package allowing you to write code that works with both PyQt and PySide
 * PyQt5 >= 5.14 or PySide6
 * openai
 * aiohttp - for openai dependency 
 * pyperclip - to copy prompt text from prompt generator
 * stability_sdk - for Stable Diffusion
+* jinja2 - for saving the conversation with html file
 
 ## Preview & Usage
 ### Overview
 #### Windows
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-ec56331b8361)
 <b>You have to write your openai api key inside the red box.</b> see [How to install](#how-to-install)
 
@@ -96,14 +103,19 @@
 I recorded this preview long time ago so GUI is different from the current version, but way of operating it is pretty much the same.
 
 https://user-images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-f60d8b2d6ced.mp4
 #### Preview 2 (using prompt feature)
 
 https://github.com/yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead
 
+#### Conversation Save Feature
+![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a)
+
+You can save checked conversation units to SQlite db file or compressed file (zip) which contains each conversation as text/html file.
+
 ### Prompt Generator
 #### How to Generate
 This application has two types of prompts. One is <b>"Properties"</b> and the other one is <b>"Template"</b>. Properties are sets of attributes that are useful for forming the premises of a question. Templates are sentences that correspond to a single command. You can input a command to generate a sentence. This can be used as a question in itself.
 
 Both types can be managed as groups. After cloning or installing, if you run the program immediately, you will be able to see the default group and the items included in the group, just like the screen.
 
 For properties, there is a group named "Default" that provides a set of attributes referenced <a href="https://gptforwork.com/tools/prompt-generator">here</a>.
@@ -143,15 +155,15 @@
 
 ### Image Generation
 ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d)
 
 ## How to Install
 1. git clone ~
 2. cd pyqt-openai
-3. pip install -r requirements.txt
+3. pip install -r requirements.txt --upgrade
 4. cd pyqt_openai
 5. You should put your api key in the line edit. You can get it in <a href="https://platform.openai.com/account/api-keys">official site</a> of openai. Sign up and log in before you get it.
 
 Be sure, this is a very important API key that belongs to you only, so you should remember it and keep it secure.
 
 6. python main.py
 
@@ -167,14 +179,15 @@
 
 run this command:
 ```
 sudo apt-get install libxcb-xinerama0
 ```
 
 ## Troubleshooting
+### subprocess-exited-with-error
 If you see this error while installing the openai package
 ```
 subprocess-exited-with-error
 ```
 download the package itself from <a href="https://pypi.org/project/openai/#files">pypi</a>. 
 
 Unzip it, access the package directory, type 
@@ -182,24 +195,34 @@
 python setup.py install
 ```
 
 That will install the openai.
 
 Note: I don't know this can happen in newer version of openai as well, so tell me if you know about something
 
+### qtpy.QtBindingsNotFoundError: No Qt bindings could be found
+first, do this:
+```
+pip uninstall -r requirements.txt
+```
+second, do this:
+```
+pip install -r requirements.txt --upgrade
+```
+then it will work :)
+
 ## Contact
 You can join pyqt-openai's <a href="https://discord.gg/cHekprskVE">Discord Server</a> to have a conversation about it or AI-related stuff 🙂
 
 ## Note
 I recommend to install sqlite management software. It's not necessary to run this app (obviously), but it's good practice to manage database about conversation history with AI and to know how this works.
 
 ## TODO list
 * DB for images (to further experiement of both DALL-E and Stable Diffusion or other image generation engine)
 * show the explanation of every model and terms related to AI (e.g. temperature, topp..)
-* save conversation history with other format (xlsx, csv, etc.)
 * tokenizer
 * highlight the source (optional, eventually)
 * support multiple language
 * use SQLAlchemy (maybe not)
 * show reason when the chat input is disabled for some reasons
 * add the basic example sources of making deep learning model with PyTorch (eventually)
```

#### html2text {}

```diff
@@ -1,115 +1,127 @@
-Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.61 Summary: PyQt OpenAI
+Metadata-Version: 2.1 Name: pyqt-openai Version: 0.1.72 Summary: PyQt OpenAI
 example Home-page: https://github.com/yjg30737/pyqt-openai.git Author: Jung Gyu
 Yoon Author-email: yjg30737@gmail.com License: MIT Description-Content-Type:
 text/markdown License-File: LICENSE # pyqt-openai
  [https://user-images.githubusercontent.com/55078043/229002952-9afe57de-b0b6-
                           400f-9628-b8e0044d3f7b.png]
+
+  [![](https://dcbadge.vercel.app/api/server/cHekprskVE)](https://discord.gg/
+                                  cHekprskVE)
 Example of using OpenAI with PyQt (Python cross-platform GUI toolkit) This
 shows an example of using OpenAI with PyQt as a chatbot and using DALL-E or
 Stable Diffusion as a image generation tool. Even though this project has
 become too huge to be called an 'example'. The major advantage of this package
 is that you don't need to know other language aside from Python. If you want to
 study openai with Python-only good old desktop software, this is for you. The
 OpenAI model this package uses is the gpt-3.5-turbo model(which is nearly as
-functional as ChatGPT) by default. You can use gpt-4 as well. Image generation
-feature(DALL-E and Stable Diffusion) available since v0.1.4. Stable Diffusion
-used [DreamStudio API](https://dreamstudio.ai/). This is not entirely free like
-stable-diffusion-webgui. But this is very lightweight and more accessible.
-don't need CUDA, torch, expansive PC, anything. This is using sqlite as a
-database. You can select the model at the right side bar. An internet
-connection is required. ## Table of Contents * [Feature](#feature) *
-[Requirements](#requirements) * [Preview & Usage](#preview-usage) * [How to
-Install](#how-to-install) * [Troubleshooting](#troubleshooting) * [Contact]
-(#contact) * [Note](#note) * [See Also](#see-also) ## Feature * basically this
-is desktop application version of ChatGPT with image generation tool. * text
-streaming (enable by default, you can disable it) * AI remembers past
-conversation * conversation management * add & delete conversations * save
-conversations * rename conversation * everything above is saved in an SQLite
-database file named conv.db. * support GPT-4 and every other models below GPT3
-* support prompt generator (manageable, autosaved in database) * support slash
-commands * support beginning and ending part of the prompt * you can run this
-in background application * notification will pop up when response is generated
-* you can make window stack on top or control its transparency * image
-generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy and
-download the image if you want. just hover the mouse cursor over the image. ##
-Requirements * qtpy - the package allowing you to write code that works with
+functional as ChatGPT) by default. You can use gpt-4 as well. Latest model such
+as gpt-3.5-turbo-0613 is also available Image generation feature(DALL-E and
+Stable Diffusion) available since v0.1.4. Stable Diffusion used [DreamStudio
+API](https://dreamstudio.ai/). This is not entirely free like stable-diffusion-
+webgui. But this is very lightweight and more accessible. don't need CUDA,
+torch, expansive PC, anything. This is using sqlite as a database. You can
+select the model at the right side bar. An internet connection is required. ##
+Table of Contents * [Feature](#feature) * [Requirements](#requirements) *
+[Preview & Usage](#preview-usage) * [How to Install](#how-to-install) *
+[Troubleshooting](#troubleshooting) * [Contact](#contact) * [Note](#note) *
+[See Also](#see-also) ## Feature * basically this is desktop application
+version of ChatGPT with image generation tool. * text streaming (enable by
+default, you can disable it) * AI remembers past conversation * support copy
+button * conversation management * add & delete conversations * save
+conversations - SQlite db, text files compressed file, html files compressed
+file (both are zip) * rename conversation * everything above is saved in an
+SQLite database file named conv.db. * support GPT-4 and every other models
+below GPT3 * support prompt generator (manageable, autosaved in database) *
+support slash commands * support beginning and ending part of the prompt * you
+can run this in background application * notification will pop up when response
+is generated * you can make window stack on top or control its transparency *
+image generation (DALL-E, Stable Diffusion with DreamStudio API) * you can copy
+and download the image if you want. just hover the mouse cursor over the image.
+## Requirements * qtpy - the package allowing you to write code that works with
 both PyQt and PySide * PyQt5 >= 5.14 or PySide6 * openai * aiohttp - for openai
 dependency * pyperclip - to copy prompt text from prompt generator *
-stability_sdk - for Stable Diffusion ## Preview & Usage ### Overview ####
-Windows ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-51667298-2c3f-4846-a8c9-ec56331b8361) You have to write your openai api key
-inside the red box. see [How to install](#how-to-install) You can change screen
-between text chatbot and image generating tool screen. ![image](https://
-github.com/yjg30737/pyqt-openai/assets/55078043/78260aaf-2626-4267-9309-
-07655cab2061) #### Linux (Ubuntu) ![image](https://github.com/yjg30737/pyqt-
-openai/assets/55078043/4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS,
-please give me the pyqt-openai screen image from it. ### Conversation ####
-Preview 1 I recorded this preview long time ago so GUI is different from the
-current version, but way of operating it is pretty much the same. https://user-
+stability_sdk - for Stable Diffusion * jinja2 - for saving the conversation
+with html file ## Preview & Usage ### Overview #### Windows ![image](https://
+github.com/yjg30737/pyqt-openai/assets/55078043/51667298-2c3f-4846-a8c9-
+ec56331b8361) You have to write your openai api key inside the red box. see
+[How to install](#how-to-install) You can change screen between text chatbot
+and image generating tool screen. ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/78260aaf-2626-4267-9309-07655cab2061) #### Linux
+(Ubuntu) ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+4005c085-53f4-406f-adb0-4fb4d87d88ba) If you use MacOS, please give me the
+pyqt-openai screen image from it. ### Conversation #### Preview 1 I recorded
+this preview long time ago so GUI is different from the current version, but
+way of operating it is pretty much the same. https://user-
 images.githubusercontent.com/55078043/236583883-8e9732a3-1223-4b28-85f1-
 f60d8b2d6ced.mp4 #### Preview 2 (using prompt feature) https://github.com/
-yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ###
-Prompt Generator #### How to Generate This application has two types of
-prompts. One is "Properties" and the other one is "Template". Properties are
-sets of attributes that are useful for forming the premises of a question.
-Templates are sentences that correspond to a single command. You can input a
-command to generate a sentence. This can be used as a question in itself. Both
-types can be managed as groups. After cloning or installing, if you run the
-program immediately, you will be able to see the default group and the items
-included in the group, just like the screen. For properties, there is a group
-named "Default" that provides a set of attributes referenced here. For
-templates, there are the "awesome_chatGPT_prompt" and "alex_brogan" (example
-prompt for Alex Brogan) groups provided. Any custom template items created
-prior to version 0.1.6 will be moved to the Miscellaneous group. !
-[prompt_list_image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
-ce40139a-c03f-42ef-abd8-4a610d762394) With using these prompts you can pretty
-much get any response you want. You can use the additional prompt feature by
-"prompt menu" right next to "prompt input" field. ![image](https://github.com/
-yjg30737/pyqt-openai/assets/55078043/c9ca84af-0088-4435-854d-7feca9e2e663)
-Since v0.1.6, awesome-chatgpt-prompt is included as template group by default.
-#### Prompt Generator Preview Generating the prompt (Properties) https://
-github.com/yjg30737/pyqt-openai/assets/55078043/e168c0e6-41b4-4ad5-95e6-
-3c42c9c23602 I recorded using the Windows recording feature. As a result, the
-"Add Dialog" that prompts for entering a group name does not appear in the
-preview. When you add a group, you will see the Add Dialog as expected. Then,
-how to generate template type prompt? Click any item in the group, it will be
-shown in the preview. You can copy that generated text with clicking "copy"
-button and include it to your prompt input. If you add a property group or
-template group with items, you can use it as a command by typing its name to
-the prompt input. Use prompt as a command https://github.com/yjg30737/pyqt-
-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-4e4d1e572553 In this preview, i
-pressed the keyboard shortcut of each actions(show beginning, show ending,
-support prompt command) to use it rather than clicking them with mouse. I made
-the command suggestion GUI resemble the Discord command autocomplete popup,
-with which a lot of people have become accustomed. ### Image Generation !
-[image](https://github.com/yjg30737/pyqt-openai/assets/55078043/d0903a76-bf4f-
-4900-bfea-89da6f072c9d) ## How to Install 1. git clone ~ 2. cd pyqt-openai 3.
-pip install -r requirements.txt 4. cd pyqt_openai 5. You should put your api
-key in the line edit. You can get it in official_site of openai. Sign up and
-log in before you get it. Be sure, this is a very important API key that
-belongs to you only, so you should remember it and keep it secure. 6. python
-main.py If installation doesn't work, you can contact me with bring up new
-issue in issue tab or check the troubleshooting below even it is only about
-very specific error. ### Note If you use Linux and see this error: ```
-qt.qpa.plugin: could not load the qt platform plugin "xcb" in "" even though it
-was found this application failed to start because no qt platform plugin could
-be initialized, reinstalling the application may fix this problem ``` run this
-command: ``` sudo apt-get install libxcb-xinerama0 ``` ## Troubleshooting If
-you see this error while installing the openai package ``` subprocess-exited-
-with-error ``` download the package itself from pypi. Unzip it, access the
-package directory, type ``` python setup.py install ``` That will install the
-openai. Note: I don't know this can happen in newer version of openai as well,
-so tell me if you know about something ## Contact You can join pyqt-openai's
-Discord_Server to have a conversation about it or AI-related stuff ð ## Note
-I recommend to install sqlite management software. It's not necessary to run
-this app (obviously), but it's good practice to manage database about
-conversation history with AI and to know how this works. ## TODO list * DB for
-images (to further experiement of both DALL-E and Stable Diffusion or other
-image generation engine) * show the explanation of every model and terms
-related to AI (e.g. temperature, topp..) * save conversation history with other
-format (xlsx, csv, etc.) * tokenizer * highlight the source (optional,
-eventually) * support multiple language * use SQLAlchemy (maybe not) * show
-reason when the chat input is disabled for some reasons * add the basic example
-sources of making deep learning model with PyTorch (eventually) ## See Also *
-Azure_OpenAI_service * join_gpt4_waitlist - i took 1 month to get access from
-it * join_chatgpt_plugins_waitlist
+yjg30737/pyqt-openai/assets/55078043/841a1505-f1cc-452e-99ab-0a9c661e6ead ####
+Conversation Save Feature ![image](https://github.com/yjg30737/pyqt-openai/
+assets/55078043/908ed185-06a6-4f7a-9626-92141ba24e1a) You can save checked
+conversation units to SQlite db file or compressed file (zip) which contains
+each conversation as text/html file. ### Prompt Generator #### How to Generate
+This application has two types of prompts. One is "Properties" and the other
+one is "Template". Properties are sets of attributes that are useful for
+forming the premises of a question. Templates are sentences that correspond to
+a single command. You can input a command to generate a sentence. This can be
+used as a question in itself. Both types can be managed as groups. After
+cloning or installing, if you run the program immediately, you will be able to
+see the default group and the items included in the group, just like the
+screen. For properties, there is a group named "Default" that provides a set of
+attributes referenced here. For templates, there are the
+"awesome_chatGPT_prompt" and "alex_brogan" (example prompt for Alex Brogan)
+groups provided. Any custom template items created prior to version 0.1.6 will
+be moved to the Miscellaneous group. ![prompt_list_image](https://github.com/
+yjg30737/pyqt-openai/assets/55078043/ce40139a-c03f-42ef-abd8-4a610d762394) With
+using these prompts you can pretty much get any response you want. You can use
+the additional prompt feature by "prompt menu" right next to "prompt input"
+field. ![image](https://github.com/yjg30737/pyqt-openai/assets/55078043/
+c9ca84af-0088-4435-854d-7feca9e2e663) Since v0.1.6, awesome-chatgpt-prompt is
+included as template group by default. #### Prompt Generator Preview Generating
+the prompt (Properties) https://github.com/yjg30737/pyqt-openai/assets/
+55078043/e168c0e6-41b4-4ad5-95e6-3c42c9c23602 I recorded using the Windows
+recording feature. As a result, the "Add Dialog" that prompts for entering a
+group name does not appear in the preview. When you add a group, you will see
+the Add Dialog as expected. Then, how to generate template type prompt? Click
+any item in the group, it will be shown in the preview. You can copy that
+generated text with clicking "copy" button and include it to your prompt input.
+If you add a property group or template group with items, you can use it as a
+command by typing its name to the prompt input. Use prompt as a command https:/
+/github.com/yjg30737/pyqt-openai/assets/55078043/df0d3923-1fbe-4dda-af6f-
+4e4d1e572553 In this preview, i pressed the keyboard shortcut of each actions
+(show beginning, show ending, support prompt command) to use it rather than
+clicking them with mouse. I made the command suggestion GUI resemble the
+Discord command autocomplete popup, with which a lot of people have become
+accustomed. ### Image Generation ![image](https://github.com/yjg30737/pyqt-
+openai/assets/55078043/d0903a76-bf4f-4900-bfea-89da6f072c9d) ## How to Install
+1. git clone ~ 2. cd pyqt-openai 3. pip install -r requirements.txt --upgrade
+4. cd pyqt_openai 5. You should put your api key in the line edit. You can get
+it in official_site of openai. Sign up and log in before you get it. Be sure,
+this is a very important API key that belongs to you only, so you should
+remember it and keep it secure. 6. python main.py If installation doesn't work,
+you can contact me with bring up new issue in issue tab or check the
+troubleshooting below even it is only about very specific error. ### Note If
+you use Linux and see this error: ``` qt.qpa.plugin: could not load the qt
+platform plugin "xcb" in "" even though it was found this application failed to
+start because no qt platform plugin could be initialized, reinstalling the
+application may fix this problem ``` run this command: ``` sudo apt-get install
+libxcb-xinerama0 ``` ## Troubleshooting ### subprocess-exited-with-error If you
+see this error while installing the openai package ``` subprocess-exited-with-
+error ``` download the package itself from pypi. Unzip it, access the package
+directory, type ``` python setup.py install ``` That will install the openai.
+Note: I don't know this can happen in newer version of openai as well, so tell
+me if you know about something ### qtpy.QtBindingsNotFoundError: No Qt bindings
+could be found first, do this: ``` pip uninstall -r requirements.txt ```
+second, do this: ``` pip install -r requirements.txt --upgrade ``` then it will
+work :) ## Contact You can join pyqt-openai's Discord_Server to have a
+conversation about it or AI-related stuff ð ## Note I recommend to install
+sqlite management software. It's not necessary to run this app (obviously), but
+it's good practice to manage database about conversation history with AI and to
+know how this works. ## TODO list * DB for images (to further experiement of
+both DALL-E and Stable Diffusion or other image generation engine) * show the
+explanation of every model and terms related to AI (e.g. temperature, topp..) *
+tokenizer * highlight the source (optional, eventually) * support multiple
+language * use SQLAlchemy (maybe not) * show reason when the chat input is
+disabled for some reasons * add the basic example sources of making deep
+learning model with PyTorch (eventually) ## See Also * Azure_OpenAI_service *
+join_gpt4_waitlist - i took 1 month to get access from it * join_chatgpt
+plugins_waitlist
```

### Comparing `pyqt-openai-0.1.61/pyqt_openai.egg-info/SOURCES.txt` & `pyqt-openai-0.1.72/pyqt_openai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 pyqt_openai/__init__.py
 pyqt_openai/a.py
 pyqt_openai/aboutDialog.py
 pyqt_openai/apiData.py
-pyqt_openai/chatWidget.py
 pyqt_openai/circleProfileImage.py
 pyqt_openai/commandCompleter.py
 pyqt_openai/convListWidget.py
 pyqt_openai/customizeDialog.py
 pyqt_openai/inputDialog.py
 pyqt_openai/leftSideBar.py
 pyqt_openai/main.py
@@ -24,26 +23,36 @@
 pyqt_openai/svgToolButton.py
 pyqt_openai/toast.py
 pyqt_openai.egg-info/PKG-INFO
 pyqt_openai.egg-info/SOURCES.txt
 pyqt_openai.egg-info/dependency_links.txt
 pyqt_openai.egg-info/requires.txt
 pyqt_openai.egg-info/top_level.txt
+pyqt_openai/chat_widget/__init__.py
+pyqt_openai/chat_widget/aiChatUnit.py
+pyqt_openai/chat_widget/chatBrowser.py
+pyqt_openai/chat_widget/prompt.py
+pyqt_openai/chat_widget/textEditPrompt.py
+pyqt_openai/chat_widget/textEditPropmtGroup.py
+pyqt_openai/chat_widget/userChatUnit.py
 pyqt_openai/ico/__init__.py
 pyqt_openai/ico/add.svg
 pyqt_openai/ico/close.svg
+pyqt_openai/ico/copy.svg
+pyqt_openai/ico/copy_light.svg
 pyqt_openai/ico/customize.svg
 pyqt_openai/ico/delete.svg
 pyqt_openai/ico/discord.svg
 pyqt_openai/ico/github.svg
 pyqt_openai/ico/help.svg
 pyqt_openai/ico/history.svg
 pyqt_openai/ico/openai.svg
 pyqt_openai/ico/prompt.svg
 pyqt_openai/ico/save.svg
+pyqt_openai/ico/save_light.svg
 pyqt_openai/ico/search.svg
 pyqt_openai/ico/setting.svg
 pyqt_openai/ico/sidebar.svg
 pyqt_openai/ico/stackontop.svg
 pyqt_openai/ico/user.svg
 pyqt_openai/ico/vertical_three_dots.svg
 pyqt_openai/image_gen_widget/__init__.py
@@ -69,9 +78,11 @@
 pyqt_openai/propmt_command_completer/commandSuggestionWidget.py
 pyqt_openai/right_sidebar/__init__.py
 pyqt_openai/right_sidebar/aiPlaygroundWidget.py
 pyqt_openai/right_sidebar/chatPage.py
 pyqt_openai/right_sidebar/completionPage.py
 pyqt_openai/right_sidebar/imagePage.py
 pyqt_openai/test/__init__.py
-pyqt_openai/test/htmlformat.py
-pyqt_openai/test/sqlalchemy_example.py
+pyqt_openai/test/sqlalchemy_example.py
+pyqt_openai/util/__init__.py
+pyqt_openai/util/script.py
+pyqt_openai/util/version.py
```

### Comparing `pyqt-openai-0.1.61/setup.py` & `pyqt-openai-0.1.72/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-openai',
-    version='0.1.61',
+    version='0.1.72',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_openai.ico': ['close.svg', 'openai.svg', 'discord.svg', 'github.svg', 'help.svg', 'customize.svg', 'history.svg',
-                                      'user.svg', 'sidebar.svg', 'prompt.svg', 'save.svg', 'stackontop.svg',
+    package_data={'pyqt_openai.ico': ['close.svg', 'copy.svg', 'copy_light.svg', 'openai.svg', 'discord.svg', 'github.svg', 'help.svg', 'customize.svg', 'history.svg',
+                                      'user.svg', 'sidebar.svg', 'prompt.svg', 'save.svg', 'save_light.svg', 'stackontop.svg',
                                       'add.svg', 'delete.svg', 'setting.svg', 'search.svg',
                                       'vertical_three_dots.svg']},
     description='PyQt OpenAI example',
     url='https://github.com/yjg30737/pyqt-openai.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
         'qtpy',
         'aiohttp',
         'openai',
         'pyperclip',
-        'stability_sdk'
+        'stability_sdk',
+        'jinja2'
     ]
 )
```

