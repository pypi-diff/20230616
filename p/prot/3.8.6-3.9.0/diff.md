# Comparing `tmp/prot-3.8.6.tar.gz` & `tmp/prot-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prot-3.8.6.tar", last modified: Wed Jun 14 20:11:13 2023, max compression
+gzip compressed data, was "prot-3.9.0.tar", last modified: Fri Jun 16 11:49:10 2023, max compression
```

## Comparing `prot-3.8.6.tar` & `prot-3.9.0.tar`

### file list

```diff
@@ -1,298 +1,213 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2023-06-14 19:42:21.000000 prot-3.8.6/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2341 2023-06-14 20:11:13.394239 prot-3.8.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1444 2023-06-14 19:51:52.000000 prot-3.8.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-14 20:11:13.398239 prot-3.8.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1429 2023-06-14 20:08:19.000000 prot-3.8.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.170239 prot-3.8.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.190239 prot-3.8.6/src/prot/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38776 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2998 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot/__version__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.198239 prot-3.8.6/src/prot/bs/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      177 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5526 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2182 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsMap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      764 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsPro.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1236 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/bsSpaz.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.290239 prot-3.8.6/src/prot/bs/stdLib/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/alwaysLandLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4352 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bigGDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1568 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bridgitLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2261 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37874 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsAchievement.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8330 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsAssault.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34286 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsBomb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18154 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsCaptureTheFlag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11373 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsChosenOne.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9234 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsConquest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    96453 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsCoopGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5888 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsDeathMatch.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9248 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsEasterEggHunt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19687 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsElimination.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10709 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsFlag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27224 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsFootball.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   116735 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12498 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsHockey.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      172 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsInternal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7611 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsKeepAway.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsKingOfTheHill.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   155086 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageArabic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   158524 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageBelarussian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   127437 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageChinese.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   118386 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageCroatian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   135541 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageCzech.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    94441 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageDanish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141350 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageDutch.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   111226 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageEnglish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   105204 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageEsperanto.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   146287 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageFrench.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148309 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGerman.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141903 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGibberish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   187394 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageGreek.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   212586 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageHindi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   137372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageHungarian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   126188 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageIndonesian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144849 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageItalian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138448 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageKorean.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   162405 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePersian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   144892 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePolish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   145117 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguagePortuguese.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   121744 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageRomanian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   183660 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageRussian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   168786 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSerbian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   142925 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSpanish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   125252 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageSwedish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   129359 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageTurkish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   169058 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLanguageUkrainian.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34599 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsLobby.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37628 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMainMenu.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58253 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9381 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsMeteorShower.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6444 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsNinjaFight.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    48080 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsOnslaught.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11026 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsPowerup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24920 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsRace.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43185 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsRunaround.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12031 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsScoreBoard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12856 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsScoreSet.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18997 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsServerData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   141126 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsSpaz.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12571 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTargetPractice.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58723 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTeamGame.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10326 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTheLastStand.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    63826 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsTutorial.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1093681 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUI.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53124 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUI2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   188532 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsUtils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3224 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/bsVector.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3767 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/courtyardLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2120 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/cragCastleDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1635 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/doomShroomLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1513 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/footballStadiumDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1360 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/hockeyStadiumDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4179 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/lakeFrigidDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1674 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/monkeyFaceLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1448 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/rampageLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1491 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/roundaboutLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2377 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/stepRightUpLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1719 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/thePadLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2028 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/tipTopLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3284 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/towerDLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2234 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/bs/stdLib/zigZagLevelDefs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12398 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/code.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.294239 prot-3.8.6/src/prot/color/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      239 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2524 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/ansi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10462 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/ansitowin32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1915 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/initialise.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5404 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6438 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/color/winterm.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.294239 prot-3.8.6/src/prot/pip/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9136 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1827 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      755 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/extra.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  4056147 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/pip/packagesList.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.302239 prot-3.8.6/src/prot/progress/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4910 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2854 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/bar.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/counter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1380 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/progress/spinner.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.314239 prot-3.8.6/src/prot/prompt/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      872 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.318239 prot-3.8.6/src/prot/prompt/application/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      519 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44248 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/application.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5051 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/current.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1349 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/dummy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3699 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/application/run_in_terminal.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5919 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/auto_suggest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    70342 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/buffer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3768 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/cache.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.318239 prot-3.8.6/src/prot/prompt/clipboard/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      403 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2489 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/in_memory.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1147 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/clipboard/pyperclip.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.322239 prot-3.8.6/src/prot/prompt/completion/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      810 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11493 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3832 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/filesystem.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6945 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/fuzzy_completer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3885 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/nested.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2934 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/completion/word_completer.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.322239 prot-3.8.6/src/prot/prompt/contrib/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.6/src/prot/prompt/contrib/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.326239 prot-3.8.6/src/prot/prompt/contrib/completers/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       36 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/completers/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2012 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/completers/system.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.330239 prot-3.8.6/src/prot/prompt/contrib/regular_languages/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3220 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21889 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/compiler.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3239 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/completion.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3386 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/lexer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7827 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/regex_parser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/regular_languages/validation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.330239 prot-3.8.6/src/prot/prompt/contrib/ssh/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      138 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/ssh/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4365 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/ssh/server.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.334239 prot-3.8.6/src/prot/prompt/contrib/telnet/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       68 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4974 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/protocol.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9518 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/contrib/telnet/server.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      187 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/data_structures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    40593 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/document.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/enums.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.338239 prot-3.8.6/src/prot/prompt/eventloop/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4125 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/async_context_manager.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1711 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/async_generator.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1117 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/dummy_contextvars.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5514 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/inputhook.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3251 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2008 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/eventloop/win32.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.342239 prot-3.8.6/src/prot/prompt/filters/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9276 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/app.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5737 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1830 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      848 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/filters/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.346239 prot-3.8.6/src/prot/prompt/formatted_text/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8089 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/ansi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4881 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4328 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/html.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2747 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/formatted_text/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7131 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/history.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.354239 prot-3.8.6/src/prot/prompt/input/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      209 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13116 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/ansi_escape_sequences.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3275 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1522 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1835 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/posix_pipe.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3897 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/posix_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2538 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/typeahead.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10131 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/vt100.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8402 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/vt100_parser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22282 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4111 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/input/win32_pipe.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.358239 prot-3.8.6/src/prot/prompt/key_binding/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      335 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.366239 prot-3.8.6/src/prot/prompt/key_binding/bindings/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-14 19:42:40.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1736 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/auto_suggest.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7105 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/basic.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6841 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/completion.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      744 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/cpr.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19627 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/emacs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      468 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/focus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4946 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/mouse.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18371 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/named_commands.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1282 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/open_in_editor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2303 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/page_navigation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5573 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/scroll.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2583 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/search.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    75161 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/bindings/vi.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1917 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    32798 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/digraphs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      895 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/emacs_state.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19390 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/key_bindings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17631 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/key_processor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3316 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/key_binding/vi_state.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4885 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/keys.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.374239 prot-3.8.6/src/prot/prompt/layout/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97489 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/containers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34955 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/controls.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6941 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/dimension.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1001 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/dummy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14088 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10373 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/margins.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25365 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/menus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1043 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/mouse_handlers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34137 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/processors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9745 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/screen.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2259 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/layout/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.374239 prot-3.8.6/src/prot/prompt/lexers/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      372 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2322 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11940 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/lexers/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      116 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1339 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/mouse_events.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.378239 prot-3.8.6/src/prot/prompt/output/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      244 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6324 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2199 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/color_depth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1487 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/conemu.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1886 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21317 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/vt100.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21140 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/win32.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2794 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/output/windows10.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5155 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/patch_stdout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25735 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/renderer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6997 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/search.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1289 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/selection.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.382239 prot-3.8.6/src/prot/prompt/shortcuts/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      844 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8424 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/dialogs.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.386239 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      458 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14070 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11767 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/formatters.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57251 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/prompt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5707 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/shortcuts/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.390239 prot-3.8.6/src/prot/prompt/styles/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1603 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5062 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8363 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/defaults.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4355 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/named_colors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1952 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/pygments.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13023 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/style.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12437 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/styles/style_transformation.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/token.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8119 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5837 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/validation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.390239 prot-3.8.6/src/prot/prompt/widgets/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1181 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    28404 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3349 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/dialogs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12736 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/menus.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12193 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/widgets/toolbars.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4138 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/prompt/win32_types.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/src/prot/wcwidth/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      140 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8004 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/table_wide.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24250 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/table_zero.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.394239 prot-3.8.6/src/prot/wcwidth/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3891 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/tests/test_core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7831 2023-06-14 19:42:21.000000 prot-3.8.6/src/prot/wcwidth/wcwidth.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-14 20:11:13.194239 prot-3.8.6/src/prot.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2341 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9449 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2023-06-14 20:11:13.000000 prot-3.8.6/src/prot.egg-info/top_level.txt
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.644819 prot-3.9.0/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1069 2023-06-15 09:23:01.000000 prot-3.9.0/LICENSE
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 11:49:10.644819 prot-3.9.0/PKG-INFO
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1444 2023-06-15 09:23:01.000000 prot-3.9.0/README.md
+-rw-r--r--   0 u0_a269  (10269) u0_a269  (10269)       57 2023-06-15 09:29:23.000000 prot-3.9.0/pyproject.toml
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       38 2023-06-16 11:49:10.644819 prot-3.9.0/setup.cfg
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1429 2023-06-15 09:23:01.000000 prot-3.9.0/setup.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.580819 prot-3.9.0/src/
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    48198 2023-06-16 11:24:28.000000 prot-3.9.0/src/prot/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4568 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/__main__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       22 2023-06-16 11:48:00.000000 prot-3.9.0/src/prot/__version__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot/bs/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      177 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5599 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2190 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsMap.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      914 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsPro.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1300 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsSpaz.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    16217 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/code.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/color/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      239 2023-06-16 11:24:46.000000 prot-3.9.0/src/prot/color/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2299 2023-06-16 11:24:46.000000 prot-3.9.0/src/prot/color/ansi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10558 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/ansitowin32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1916 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/initialise.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5480 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6464 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/winterm.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/pip/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12222 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2354 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/__main__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      797 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/extra.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       18 2023-06-16 11:46:04.000000 prot-3.9.0/src/prot/pip/packagesList.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/progress/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4882 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2789 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/bar.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1372 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/counter.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1380 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/spinner.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      872 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/application/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      519 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    44227 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/application/application.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5050 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/application/current.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1349 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/dummy.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3699 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/run_in_terminal.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5918 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/auto_suggest.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    70320 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/buffer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3766 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/cache.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/clipboard/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      403 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/clipboard/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2488 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/clipboard/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1076 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/clipboard/in_memory.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1147 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/clipboard/pyperclip.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/completion/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      810 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/completion/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11486 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3831 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/filesystem.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6940 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/fuzzy_completer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3884 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/nested.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2931 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/word_completer.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/contrib/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/contrib/completers/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       36 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/completers/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2012 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/completers/system.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/regular_languages/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3220 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21888 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/compiler.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3238 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/completion.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3385 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/lexer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7825 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/regex_parser.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/validation.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/ssh/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      138 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/ssh/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4365 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/ssh/server.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/telnet/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       68 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      130 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/log.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4965 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/protocol.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9512 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/server.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      187 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/data_structures.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    40559 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/document.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      322 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/enums.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.608819 prot-3.9.0/src/prot/prompt/eventloop/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      636 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4125 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/async_context_manager.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1711 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/async_generator.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1117 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/dummy_contextvars.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5514 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/inputhook.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3251 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2008 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/win32.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.608819 prot-3.9.0/src/prot/prompt/filters/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1028 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9261 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/filters/app.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5733 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/filters/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1830 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/cli.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      848 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.612819 prot-3.9.0/src/prot/prompt/formatted_text/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1378 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8089 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/ansi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/formatted_text/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4324 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/formatted_text/html.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      756 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2747 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7129 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/history.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.616819 prot-3.9.0/src/prot/prompt/input/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      209 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    13116 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/ansi_escape_sequences.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3269 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1522 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1831 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/posix_pipe.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3897 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/posix_utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2538 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/typeahead.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10129 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/vt100.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8400 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/vt100_parser.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    22280 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/input/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4101 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/win32_pipe.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.620819 prot-3.9.0/src/prot/prompt/key_binding/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      335 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.624819 prot-3.9.0/src/prot/prompt/key_binding/bindings/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1736 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/auto_suggest.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7103 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/basic.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6965 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/completion.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      744 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/cpr.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    19603 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/emacs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      468 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/focus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4946 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/mouse.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    18366 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/named_commands.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1316 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/open_in_editor.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2349 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/page_navigation.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5573 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/scroll.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2583 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/search.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    75190 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/vi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1917 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    32798 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/digraphs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      889 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/emacs_state.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    19387 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/key_bindings.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    17624 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/key_binding/key_processor.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3312 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/vi_state.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/keys.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.628819 prot-3.9.0/src/prot/prompt/layout/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3462 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    97453 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/layout/containers.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    34933 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/controls.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6937 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/dimension.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1001 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/dummy.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    14081 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/layout.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10366 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/margins.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    25351 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/menus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1043 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/mouse_handlers.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    34123 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/layout/processors.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9744 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/screen.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2259 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.632819 prot-3.9.0/src/prot/prompt/lexers/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      372 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/lexers/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2320 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/lexers/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11933 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/lexers/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      116 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/log.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1339 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/mouse_events.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.632819 prot-3.9.0/src/prot/prompt/output/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      244 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6268 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/output/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2199 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/color_depth.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1487 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/conemu.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1886 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21307 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/output/vt100.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21122 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/output/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2794 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/windows10.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5154 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/patch_stdout.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    25802 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/renderer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6996 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/search.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1288 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/selection.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.636819 prot-3.9.0/src/prot/prompt/shortcuts/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      844 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8758 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/dialogs.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.636819 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      458 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    14068 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11758 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/formatters.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    57259 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/prompt/shortcuts/prompt.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5707 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/prompt/styles/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1603 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5062 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8409 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/styles/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4355 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/named_colors.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1952 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    13019 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/styles/style.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12433 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/styles/style_transformation.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       85 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/token.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8107 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5836 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/validation.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/prompt/widgets/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1181 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/widgets/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    28425 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/prompt/widgets/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3348 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/dialogs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12722 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/menus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12179 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/toolbars.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4138 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/win32_types.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/wcwidth/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      150 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10556 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/table_wide.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    31378 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/wcwidth/table_zero.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.644819 prot-3.9.0/src/prot/wcwidth/tests/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       42 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/wcwidth/tests/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3941 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/tests/test_core.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7908 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/wcwidth.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot.egg-info/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/PKG-INFO
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6360 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/SOURCES.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        1 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/dependency_links.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       59 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/entry_points.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        5 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/top_level.txt
```

### Comparing `prot-3.8.6/LICENSE` & `prot-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/PKG-INFO` & `prot-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prot
-Version: 3.8.6
+Version: 3.9.0
 Summary: A Simple Tool That Contains Advance Functions.
 Home-page: https://github.com/SAPTeamDEV/prot
 Author: Alireza Poodineh
 Author-email: itsaeliux@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prot-3.8.6/README.md` & `prot-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/setup.py` & `prot-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/bs/bs.py` & `prot-3.9.0/src/prot/bs/bs.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,165 +5,183 @@
 import shutil
 
 from base64 import b64encode
 from functools import partial
 
 treeCache = {}
 
+
 def getModel(file):
-    return file + '.bob'
+    return file + ".bob"
+
 
 def getCollideModel(file):
-    return file + '.cob'
+    return file + ".cob"
+
 
 def getTexture(file):
-    return file + '.texture'
+    return file + ".texture"
+
 
 def getSound(file):
-    return file + '.ogg'
+    return file + ".ogg"
+
+
+class Material(LoopBack):
+    pass
 
-class Material(LoopBack): pass
 
 class Factory(object):
     def __setattr__(self, key, value):
-        if key in ['dict', 'getcontents'] or key.startswith('_'):
+        if key in ["dict", "getcontents"] or key.startswith("_"):
             object.__setattr__(self, key, value)
-        if not hasattr(self, 'dict'):
+        if not hasattr(self, "dict"):
             self.dict = {}
         self.dict[key] = value
 
     def __getattribute__(self, key):
-        if key in ['dict', 'getcontents'] or key.startswith('_'):
+        if key in ["dict", "getcontents"] or key.startswith("_"):
             return object.__getattribute__(self, key, value)
-        if not hasattr(self, 'dict'):
+        if not hasattr(self, "dict"):
             self.dict = {}
         return self.dict[key]
 
-    def getcontents(self, path='.'):
+    def getcontents(self, path="."):
         files = []
         data = {self.__class__.__name__: files}
         for key, value in self.dict.items():
             if type(value) == str:
                 values = [value]
             elif type(value) in [list, tuple]:
                 values = list(value)
             else:
                 continue
             for fileName in values:
-                if fileName.endswith('.texture'):
-                    files += bs.getFiles(fileName.split('.')[0], path, ['ktx', 'dds'])
+                if fileName.endswith(".texture"):
+                    files += bs.getFiles(fileName.split(".")[0], path, ["ktx", "dds"])
                 else:
                     files.append(fileName)
         return data
 
+
 def md5sum(filename):
-    with open(filename, mode='rb') as f:
+    with open(filename, mode="rb") as f:
         d = hashlib.md5()
-        for buf in iter(partial(f.read, 128), b''):
+        for buf in iter(partial(f.read, 128), b""):
             d.update(buf)
     return d.hexdigest()
 
+
 def genPayloadInfo():
     files = []
     for root, subdirs, files_in_dir in os.walk(".", topdown=True, followlinks=False):
         for file in files_in_dir:
-            if file.startswith('.') or file == 'payload_info': continue
+            if file.startswith(".") or file == "payload_info":
+                continue
             files.append(os.path.join(root, file))
 
     payloadStr = "{}\n1\n".format(len(files))
     for file in files:
         payloadStr += "{} {}\n".format(file.strip("./"), md5sum(file))
 
-    with open('payload_info', 'w') as f:
+    with open("payload_info", "w") as f:
         f.write(payloadStr)
         f.close()
 
-def getFiles(file, path='.', formats=['ogg', 'ktx', 'dds', 'bob', 'cob', 'py', 'pyc']):
+
+def getFiles(file, path=".", formats=["ogg", "ktx", "dds", "bob", "cob", "py", "pyc"]):
     tree = makeTree(path)
     files = []
     for format in formats:
-        if file + '.' + format in tree:
-            files.append(file + '.' + format)
+        if file + "." + format in tree:
+            files.append(file + "." + format)
     return files
 
-def makeTree(source='.', ignoreCache=False):
+
+def makeTree(source=".", ignoreCache=False):
     if source in treeCache and not ignoreCache:
         return treeCache[source]
     tree = {}
     for p in os.listdir(source):
         if os.path.isdir(os.path.join(source, p)):
             for name, path in makeTree(os.path.join(source, p)).items():
                 tree[name] = path
         else:
             tree[p] = os.path.join(source, p)
     if not ignoreCache:
         treeCache[source] = tree
     return tree
 
+
 def encodeFile(source):
-    ff = open('coded-'+source,'wb')
-    ff.write('import base64;exec(base64.b64decode('+repr(b64encode(open(source).read()))+'))')
+    ff = open("coded-" + source, "wb")
+    ff.write(
+        "import base64;exec(base64.b64decode("
+        + repr(b64encode(open(source).read()))
+        + "))"
+    )
     ff.flush()
 
-def processMedia(data, path='.', divide=False, silent=False):
+
+def processMedia(data, path=".", divide=False, silent=False):
     tree = makeTree(path)
-    media = os.path.join(path, 'media')
+    media = os.path.join(path, "media")
     if not os.path.isdir(media):
         os.mkdir(media)
     for name, files in data.items():
         if divide:
             media = os.path.join(media, name)
             if not os.path.isdir(media):
-              os.mkdir(media)
+                os.mkdir(media)
 
-        audios = os.path.join(media, 'audios')
-        tex = os.path.join(media, 'textures')
-        texAndroid = os.path.join(tex, 'android')
-        texOther = os.path.join(tex, 'other')
-        models = os.path.join(media, 'models')
-        scripts = os.path.join(media, 'scripts')
+        audios = os.path.join(media, "audios")
+        tex = os.path.join(media, "textures")
+        texAndroid = os.path.join(tex, "android")
+        texOther = os.path.join(tex, "other")
+        models = os.path.join(media, "models")
+        scripts = os.path.join(media, "scripts")
 
         if not os.path.isdir(audios):
             os.mkdir(audios)
         if not os.path.isdir(tex):
             os.mkdir(tex)
         if not os.path.isdir(texAndroid):
             os.mkdir(texAndroid)
         if not os.path.isdir(texOther):
             os.mkdir(texOther)
         if not os.path.isdir(models):
             os.mkdir(models)
         if not os.path.isdir(scripts):
             os.mkdir(scripts)
 
-        audioFormats = ['ogg']
-        texFormats = ['dds', 'ktx']
-        modelFormats = ['bob', 'cob']
-        scriptFormats = ['py', 'pyc']
+        audioFormats = ["ogg"]
+        texFormats = ["dds", "ktx"]
+        modelFormats = ["bob", "cob"]
+        scriptFormats = ["py", "pyc"]
 
         for file in files:
             if file in tree:
                 if file.type in audioFormats:
                     if not silent:
-                        print(file + ' -> ' + audios)
+                        print(file + " -> " + audios)
                     shutil.copy(tree[file], audios)
                 elif file.type in texFormats:
-                    if file.type == 'ktx':
+                    if file.type == "ktx":
                         if not silent:
-                            print(file + ' -> ' + texAndroid)
+                            print(file + " -> " + texAndroid)
                         shutil.copy(tree[file], texAndroid)
                     else:
                         if not silent:
-                            print(file + ' -> ' + texOther)
+                            print(file + " -> " + texOther)
                         shutil.copy(tree[file], texOther)
                 elif file.type in modelFormats:
                     if not silent:
-                        print(file + ' -> ' + models)
+                        print(file + " -> " + models)
                     shutil.copy(tree[file], models)
                 elif file.type in scriptFormats:
                     if not silent:
-                        print(file + ' -> ' + scripts)
+                        print(file + " -> " + scripts)
                     shutil.copy(tree[file], scripts)
                 else:
-                   printWarn('type of file ' + file + ' is not supported')
+                    printWarn("type of file " + file + " is not supported")
             else:
-                printWarn('file ' + file + ' not found')
+                printWarn("file " + file + " not found")
```

### Comparing `prot-3.8.6/src/prot/bs/bsMap.py` & `prot-3.9.0/src/prot/bs/bsMap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from . import *
 
 import builtins as _builtins
 
 maps = {}
 depends = []
 
+
 class Map(object):
     name = "Map"
 
     @classmethod
     def getPreviewTextureName(cls):
         """
         Return the name of the preview texture for this map.
@@ -20,62 +21,68 @@
         """
         Called when the map is being preloaded;
         it should load any media it requires to
         class attributes on itself.
         """
         return None
 
+
 def registerMap(map):
     if not map.name in maps:
         maps[map.name] = map
     else:
-        raise Exception(repr(map.name) + 'already exists.')
+        raise Exception(repr(map.name) + "already exists.")
+
 
 def _import(*args, **kwargs):
     depends.append(args[0])
     if _import.redirect:
         return _builtins.__import(*args, **kwargs)
 
+
 def record(redirect=False):
     if redirect:
         _import.redirect = True
     else:
         _import.redirect = False
     _builtins.__import = _builtins.__import__
     _builtins.__import__ = _import
 
+
 def end():
     _builtins.__import__ = _builtins.__import
     del _builtins.__import
     del _import.redirect
 
+
 def clear():
     global maps
     global depends
     maps = {}
     depends = []
 
-def getMedia(path='.', divide=False, silent=False):
+
+def getMedia(path=".", divide=False, silent=False):
     tree = bs.makeTree(path)
     data = {}
     for name, obj in maps.items():
         medias = []
         preloads = []
         if obj.getPreviewTextureName() is not None:
-            medias += bs.getFiles(obj.getPreviewTextureName(), path, ['ktx', 'dds'])
+            medias += bs.getFiles(obj.getPreviewTextureName(), path, ["ktx", "dds"])
         if obj.onPreload() is not None:
             for key, value in obj.onPreload().items():
                 if type(value) == str:
                     preloads.append(value)
                 elif type(value) in [list, tuple]:
                     preloads += list(value)
         for preload in preloads:
-            if preload.endswith('.texture'):
-                medias += bs.getFiles(preload.split('.')[0], path, ['ktx', 'dds'])
+            if preload.endswith(".texture"):
+                medias += bs.getFiles(preload.split(".")[0], path, ["ktx", "dds"])
             else:
                 medias.append(preload)
         for depend in depends:
-            medias += bs.getFiles(depend, path, ['py', 'pyc'])
+            medias += bs.getFiles(depend, path, ["py", "pyc"])
         data[name] = [ProtString(media) for media in medias]
 
     if data:
-        bs.processMedia(data, path, divide, silent)
+        bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.8.6/src/prot/bs/bsSpaz.py` & `prot-3.9.0/src/prot/bs/bsSpaz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 from . import *
 
 import os
 import shutil
 
 appearances = {}
 
+
 class Appearance(Database):
     def __init__(self, name):
         Database.__init__(self)
         if not name in appearances:
             appearances[name] = self
         else:
-            raise Exception(repr(name) + 'already exists.')
+            raise Exception(repr(name) + "already exists.")
+
 
 def clear():
     global appearances
     appearances = {}
 
+
 def getOutput(file):
-    string = ''
+    string = ""
     for a in appearances:
-        string += 'addCharacter(' + repr(a) + ', cfg=' +str(appearances[a].dict) + ')\n'
-    
-    with open(file, 'w') as f:
+        string += (
+            "addCharacter(" + repr(a) + ", cfg=" + str(appearances[a].dict) + ")\n"
+        )
+
+    with open(file, "w") as f:
         f.write(string)
         f.flush()
 
-def getMedia(path='.', divide=False, silent=False):
+
+def getMedia(path=".", divide=False, silent=False):
     tree = bs.makeTree(path)
     data = {}
     for name, obj in appearances.items():
         medias = []
         for key, value in obj.dict.items():
             if type(value) == str:
                 values = [value]
             elif type(value) in [list, tuple]:
                 values = list(value)
             else:
                 continue
             for fileName in values:
-                medias += bs.getFiles(fileName, path, ['ogg', 'ktx', 'dds', 'bob', 'cob'])
+                medias += bs.getFiles(
+                    fileName, path, ["ogg", "ktx", "dds", "bob", "cob"]
+                )
         data[name] = [ProtString(media) for media in medias]
 
     if data:
-        bs.processMedia(data, path, divide, silent)
+        bs.processMedia(data, path, divide, silent)
```

### Comparing `prot-3.8.6/src/prot/bs/stdLib/bsRace.py` & `prot-3.9.0/src/prot/prompt/output/vt100.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,609 +1,683 @@
-import bs
-import random
-
-
-def bsGetAPIVersion():
-    # see bombsquadgame.com/apichanges
-    return 4
+"""
+Output for vt100 terminals.
 
+A lot of thanks, regarding outputting of colors, goes to the Pygments project:
+(We don't rely on Pygments anymore, because many things are very custom, and
+everything has been highly optimized.)
+http://pygments.org/
+"""
+import array
+import errno
+import sys
+from typing import (
+    IO,
+    Callable,
+    Dict,
+    Hashable,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    TextIO,
+    Tuple,
+)
+
+from prot.prompt.data_structures import Size
+from prot.prompt.output import Output
+from prot.prompt.styles import ANSI_COLOR_NAMES, Attrs
+
+from .color_depth import ColorDepth
+
+__all__ = [
+    "Vt100_Output",
+]
+
+
+FG_ANSI_COLORS = {
+    "ansidefault": 39,
+    # Low intensity.
+    "ansiblack": 30,
+    "ansired": 31,
+    "ansigreen": 32,
+    "ansiyellow": 33,
+    "ansiblue": 34,
+    "ansimagenta": 35,
+    "ansicyan": 36,
+    "ansigray": 37,
+    # High intensity.
+    "ansibrightblack": 90,
+    "ansibrightred": 91,
+    "ansibrightgreen": 92,
+    "ansibrightyellow": 93,
+    "ansibrightblue": 94,
+    "ansibrightmagenta": 95,
+    "ansibrightcyan": 96,
+    "ansiwhite": 97,
+}
+
+BG_ANSI_COLORS = {
+    "ansidefault": 49,
+    # Low intensity.
+    "ansiblack": 40,
+    "ansired": 41,
+    "ansigreen": 42,
+    "ansiyellow": 43,
+    "ansiblue": 44,
+    "ansimagenta": 45,
+    "ansicyan": 46,
+    "ansigray": 47,
+    # High intensity.
+    "ansibrightblack": 100,
+    "ansibrightred": 101,
+    "ansibrightgreen": 102,
+    "ansibrightyellow": 103,
+    "ansibrightblue": 104,
+    "ansibrightmagenta": 105,
+    "ansibrightcyan": 106,
+    "ansiwhite": 107,
+}
+
+
+ANSI_COLORS_TO_RGB = {
+    "ansidefault": (
+        0x00,
+        0x00,
+        0x00,
+    ),  # Don't use, 'default' doesn't really have a value.
+    "ansiblack": (0x00, 0x00, 0x00),
+    "ansigray": (0xE5, 0xE5, 0xE5),
+    "ansibrightblack": (0x7F, 0x7F, 0x7F),
+    "ansiwhite": (0xFF, 0xFF, 0xFF),
+    # Low intensity.
+    "ansired": (0xCD, 0x00, 0x00),
+    "ansigreen": (0x00, 0xCD, 0x00),
+    "ansiyellow": (0xCD, 0xCD, 0x00),
+    "ansiblue": (0x00, 0x00, 0xCD),
+    "ansimagenta": (0xCD, 0x00, 0xCD),
+    "ansicyan": (0x00, 0xCD, 0xCD),
+    # High intensity.
+    "ansibrightred": (0xFF, 0x00, 0x00),
+    "ansibrightgreen": (0x00, 0xFF, 0x00),
+    "ansibrightyellow": (0xFF, 0xFF, 0x00),
+    "ansibrightblue": (0x00, 0x00, 0xFF),
+    "ansibrightmagenta": (0xFF, 0x00, 0xFF),
+    "ansibrightcyan": (0x00, 0xFF, 0xFF),
+}
+
+
+assert set(FG_ANSI_COLORS) == set(ANSI_COLOR_NAMES)
+assert set(BG_ANSI_COLORS) == set(ANSI_COLOR_NAMES)
+assert set(ANSI_COLORS_TO_RGB) == set(ANSI_COLOR_NAMES)
+
+
+def _get_closest_ansi_color(r: int, g: int, b: int, exclude: Sequence[str] = ()) -> str:
+    """
+    Find closest ANSI color. Return it by name.
+
+    :param r: Red (Between 0 and 255.)
+    :param g: Green (Between 0 and 255.)
+    :param b: Blue (Between 0 and 255.)
+    :param exclude: A tuple of color names to exclude. (E.g. ``('ansired', )``.)
+    """
+    exclude = list(exclude)
+
+    # When we have a bit of saturation, avoid the gray-like colors, otherwise,
+    # too often the distance to the gray color is less.
+    saturation = abs(r - g) + abs(g - b) + abs(b - r)  # Between 0..510
+
+    if saturation > 30:
+        exclude.extend(["ansilightgray", "ansidarkgray", "ansiwhite", "ansiblack"])
+
+    # Take the closest color.
+    # (Thanks to Pygments for this part.)
+    distance = 257 * 257 * 3  # "infinity" (>distance from #000000 to #ffffff)
+    match = "ansidefault"
+
+    for name, (r2, g2, b2) in ANSI_COLORS_TO_RGB.items():
+        if name != "ansidefault" and name not in exclude:
+            d = (r - r2) ** 2 + (g - g2) ** 2 + (b - b2) ** 2
+
+            if d < distance:
+                match = name
+                distance = d
+
+    return match
+
+
+_ColorCodeAndName = Tuple[int, str]
+
+
+class _16ColorCache:
+    """
+    Cache which maps (r, g, b) tuples to 16 ansi colors.
+
+    :param bg: Cache for background colors, instead of foreground.
+    """
+
+    def __init__(self, bg: bool = False) -> None:
+        self.bg = bg
+        self._cache: Dict[Hashable, _ColorCodeAndName] = {}
+
+    def get_code(
+        self, value: Tuple[int, int, int], exclude: Sequence[str] = ()
+    ) -> _ColorCodeAndName:
+        """
+        Return a (ansi_code, ansi_name) tuple. (E.g. ``(44, 'ansiblue')``.) for
+        a given (r,g,b) value.
+        """
+        key: Hashable = (value, tuple(exclude))
+        cache = self._cache
+
+        if key not in cache:
+            cache[key] = self._get(value, exclude)
+
+        return cache[key]
+
+    def _get(
+        self, value: Tuple[int, int, int], exclude: Sequence[str] = ()
+    ) -> _ColorCodeAndName:
+        r, g, b = value
+        match = _get_closest_ansi_color(r, g, b, exclude=exclude)
+
+        # Turn color name into code.
+        if self.bg:
+            code = BG_ANSI_COLORS[match]
+        else:
+            code = FG_ANSI_COLORS[match]
 
-def bsGetGames():
-    return [RaceGame]
+        return code, match
 
 
-class RaceRegion(bs.Actor):
-    def __init__(self, pt, index):
-        bs.Actor.__init__(self)
-        activity = self.getActivity()
-        self._pt = pt
-        self._index = index
-        self.node = bs.newNode(
-            "region", owner=self, delegate=self,
-            attrs={'position': pt[: 3],
-                   'scale': (pt[3] * 2.0, pt[4] * 2.0, pt[5] * 2.0),
-                   'type': "box", 'materials': [activity._raceRegionMaterial]})
+class _256ColorCache(Dict[Tuple[int, int, int], int]):
+    """
+    Cache which maps (r, g, b) tuples to 256 colors.
+    """
+
+    def __init__(self) -> None:
+        # Build color table.
+        colors: List[Tuple[int, int, int]] = []
+
+        # colors 0..15: 16 basic colors
+        colors.append((0x00, 0x00, 0x00))  # 0
+        colors.append((0xCD, 0x00, 0x00))  # 1
+        colors.append((0x00, 0xCD, 0x00))  # 2
+        colors.append((0xCD, 0xCD, 0x00))  # 3
+        colors.append((0x00, 0x00, 0xEE))  # 4
+        colors.append((0xCD, 0x00, 0xCD))  # 5
+        colors.append((0x00, 0xCD, 0xCD))  # 6
+        colors.append((0xE5, 0xE5, 0xE5))  # 7
+        colors.append((0x7F, 0x7F, 0x7F))  # 8
+        colors.append((0xFF, 0x00, 0x00))  # 9
+        colors.append((0x00, 0xFF, 0x00))  # 10
+        colors.append((0xFF, 0xFF, 0x00))  # 11
+        colors.append((0x5C, 0x5C, 0xFF))  # 12
+        colors.append((0xFF, 0x00, 0xFF))  # 13
+        colors.append((0x00, 0xFF, 0xFF))  # 14
+        colors.append((0xFF, 0xFF, 0xFF))  # 15
+
+        # colors 16..232: the 6x6x6 color cube
+        valuerange = (0x00, 0x5F, 0x87, 0xAF, 0xD7, 0xFF)
+
+        for i in range(217):
+            r = valuerange[(i // 36) % 6]
+            g = valuerange[(i // 6) % 6]
+            b = valuerange[i % 6]
+            colors.append((r, g, b))
+
+        # colors 233..253: grayscale
+        for i in range(1, 22):
+            v = 8 + i * 10
+            colors.append((v, v, v))
+
+        self.colors = colors
+
+    def __missing__(self, value: Tuple[int, int, int]) -> int:
+        r, g, b = value
+
+        # Find closest color.
+        # (Thanks to Pygments for this!)
+        distance = 257 * 257 * 3  # "infinity" (>distance from #000000 to #ffffff)
+        match = 0
+
+        for i, (r2, g2, b2) in enumerate(self.colors):
+            if i >= 16:  # XXX: We ignore the 16 ANSI colors when mapping RGB
+                # to the 256 colors, because these highly depend on
+                # the color scheme of the terminal.
+                d = (r - r2) ** 2 + (g - g2) ** 2 + (b - b2) ** 2
+
+                if d < distance:
+                    match = i
+                    distance = d
+
+        # Turn color name into code.
+        self[value] = match
+        return match
+
+
+_16_fg_colors = _16ColorCache(bg=False)
+_16_bg_colors = _16ColorCache(bg=True)
+_256_colors = _256ColorCache()
+
+
+class _EscapeCodeCache(Dict[Attrs, str]):
+    """
+    Cache for VT100 escape codes. It maps
+    (fgcolor, bgcolor, bold, underline, reverse) tuples to VT100 escape sequences.
+
+    :param true_color: When True, use 24bit colors instead of 256 colors.
+    """
+
+    def __init__(self, color_depth: ColorDepth) -> None:
+        self.color_depth = color_depth
+
+    def __missing__(self, attrs: Attrs) -> str:
+        fgcolor, bgcolor, bold, underline, italic, blink, reverse, hidden = attrs
+        parts: List[str] = []
+
+        parts.extend(self._colors_to_code(fgcolor or "", bgcolor or ""))
+
+        if bold:
+            parts.append("1")
+        if italic:
+            parts.append("3")
+        if blink:
+            parts.append("5")
+        if underline:
+            parts.append("4")
+        if reverse:
+            parts.append("7")
+        if hidden:
+            parts.append("8")
 
+        if parts:
+            result = "\x1b[0;" + ";".join(parts) + "m"
+        else:
+            result = "\x1b[0m"
 
-class RaceGame(bs.TeamGameActivity):
+        self[attrs] = result
+        return result
 
-    @classmethod
-    def getName(cls):
-        return 'Race'
+    def _color_name_to_rgb(self, color: str) -> Tuple[int, int, int]:
+        "Turn 'ffffff', into (0xff, 0xff, 0xff)."
+        try:
+            rgb = int(color, 16)
+        except ValueError:
+            raise
+        else:
+            r = (rgb >> 16) & 0xFF
+            g = (rgb >> 8) & 0xFF
+            b = rgb & 0xFF
+            return r, g, b
+
+    def _colors_to_code(self, fg_color: str, bg_color: str) -> Iterable[str]:
+        """
+        Return a tuple with the vt100 values  that represent this color.
+        """
+        # When requesting ANSI colors only, and both fg/bg color were converted
+        # to ANSI, ensure that the foreground and background color are not the
+        # same. (Unless they were explicitly defined to be the same color.)
+        fg_ansi = ""
+
+        def get(color: str, bg: bool) -> List[int]:
+            nonlocal fg_ansi
+
+            table = BG_ANSI_COLORS if bg else FG_ANSI_COLORS
+
+            if not color or self.color_depth == ColorDepth.DEPTH_1_BIT:
+                return []
+
+            # 16 ANSI colors. (Given by name.)
+            elif color in table:
+                return [table[color]]
 
-    @classmethod
-    def getDescription(cls, sessionType):
-        return 'Run real fast!'
+            # RGB colors. (Defined as 'ffffff'.)
+            else:
+                try:
+                    rgb = self._color_name_to_rgb(color)
+                except ValueError:
+                    return []
+
+                # When only 16 colors are supported, use that.
+                if self.color_depth == ColorDepth.DEPTH_4_BIT:
+                    if bg:  # Background.
+                        if fg_color != bg_color:
+                            exclude = [fg_ansi]
+                        else:
+                            exclude = []
+                        code, name = _16_bg_colors.get_code(rgb, exclude=exclude)
+                        return [code]
+                    else:  # Foreground.
+                        code, name = _16_fg_colors.get_code(rgb)
+                        fg_ansi = name
+                        return [code]
+
+                # True colors. (Only when this feature is enabled.)
+                elif self.color_depth == ColorDepth.DEPTH_24_BIT:
+                    r, g, b = rgb
+                    return [(48 if bg else 38), 2, r, g, b]
 
-    @classmethod
-    def getScoreInfo(cls):
-        return {'scoreName': 'Time',
-                'lowerIsBetter': True,
-                'scoreType': 'milliseconds'}
+                # 256 RGB colors.
+                else:
+                    return [(48 if bg else 38), 5, _256_colors[rgb]]
 
-    @classmethod
-    def supportsSessionType(cls, sessionType):
-        return True if(
-            issubclass(sessionType, bs.TeamsSession)
-            or issubclass(sessionType, bs.FreeForAllSession)) else False
+        result: List[int] = []
+        result.extend(get(fg_color, False))
+        result.extend(get(bg_color, True))
+
+        return map(str, result)
+
+
+def _get_size(fileno: int) -> Tuple[int, int]:
+    # Thanks to fabric (fabfile.org), and
+    # http://sqizit.bartletts.id.au/2011/02/14/pseudo-terminals-in-python/
+    """
+    Get the size of this pseudo terminal.
+
+    :param fileno: stdout.fileno()
+    :returns: A (rows, cols) tuple.
+    """
+    # Inline imports, because these modules are not available on Windows.
+    # (This file is used by ConEmuOutput, which is used on Windows.)
+    import fcntl
+    import termios
+
+    # Buffer for the C call
+    buf = array.array("h", [0, 0, 0, 0])
+
+    # Do TIOCGWINSZ (Get)
+    # Note: We should not pass 'True' as a fourth parameter to 'ioctl'. (True
+    #       is the default.) This causes segmentation faults on some systems.
+    #       See: https://github.com/jonathanslenders/python-prompt-toolkit/pull/364
+    fcntl.ioctl(fileno, termios.TIOCGWINSZ, buf)  # type: ignore
+
+    # Return rows, cols
+    return buf[0], buf[1]
+
+
+class Vt100_Output(Output):
+    """
+    :param get_size: A callable which returns the `Size` of the output terminal.
+    :param stdout: Any object with has a `write` and `flush` method + an 'encoding' property.
+    :param term: The terminal environment variable. (xterm, xterm-256color, linux, ...)
+    :param write_binary: Encode the output before writing it. If `True` (the
+        default), the `stdout` object is supposed to expose an `encoding` attribute.
+    """
+
+    # For the error messages. Only display "Output is not a terminal" once per
+    # file descriptor.
+    _fds_not_a_terminal: Set[int] = set()
+
+    def __init__(
+        self,
+        stdout: TextIO,
+        get_size: Callable[[], Size],
+        term: Optional[str] = None,
+        write_binary: bool = True,
+    ) -> None:
+        assert all(hasattr(stdout, a) for a in ("write", "flush"))
+
+        if write_binary:
+            assert hasattr(stdout, "encoding")
+
+        self._buffer: List[str] = []
+        self.stdout = stdout
+        self.write_binary = write_binary
+        self._get_size = get_size
+        self.term = term or "xterm"
+
+        # Cache for escape codes.
+        self._escape_code_caches: Dict[ColorDepth, _EscapeCodeCache] = {
+            ColorDepth.DEPTH_1_BIT: _EscapeCodeCache(ColorDepth.DEPTH_1_BIT),
+            ColorDepth.DEPTH_4_BIT: _EscapeCodeCache(ColorDepth.DEPTH_4_BIT),
+            ColorDepth.DEPTH_8_BIT: _EscapeCodeCache(ColorDepth.DEPTH_8_BIT),
+            ColorDepth.DEPTH_24_BIT: _EscapeCodeCache(ColorDepth.DEPTH_24_BIT),
+        }
 
     @classmethod
-    def getSupportedMaps(cls, sessionType):
-        return bs.getMapsSupportingPlayType("race")
+    def from_pty(cls, stdout: TextIO, term: Optional[str] = None) -> "Vt100_Output":
+        """
+        Create an Output class from a pseudo terminal.
+        (This will take the dimensions by reading the pseudo
+        terminal attributes.)
+        """
+        # Normally, this requires a real TTY device, but people instantiate
+        # this class often during unit tests as well. For convenience, we print
+        # an error message, use standard dimensions, and go on.
+        fd = stdout.fileno()
+
+        if not stdout.isatty() and fd not in cls._fds_not_a_terminal:
+            msg = "Warning: Output is not a terminal (fd=%r).\n"
+            sys.stderr.write(msg % fd)
+            sys.stderr.flush()
+            cls._fds_not_a_terminal.add(fd)
+
+        def get_size() -> Size:
+            # If terminal (incorrectly) reports its size as 0, pick a
+            # reasonable default.  See
+            # https://github.com/ipython/ipython/issues/10071
+            rows, columns = (None, None)
+
+            # It is possible that `stdout` is no longer a TTY device at this
+            # point. In that case we get an `OSError` in the ioctl call in
+            # `get_size`. See:
+            # https://github.com/prompt-toolkit/python-prompt-toolkit/pull/1021
+            try:
+                rows, columns = _get_size(stdout.fileno())
+            except OSError:
+                pass
+            return Size(rows=rows or 24, columns=columns or 80)
+
+        return cls(stdout, get_size, term=term)
+
+    def get_size(self) -> Size:
+        return self._get_size()
+
+    def fileno(self) -> int:
+        "Return file descriptor."
+        return self.stdout.fileno()
+
+    def encoding(self) -> str:
+        "Return encoding used for stdout."
+        return self.stdout.encoding
+
+    def write_raw(self, data: str) -> None:
+        """
+        Write raw data to output.
+        """
+        self._buffer.append(data)
+
+    def write(self, data: str) -> None:
+        """
+        Write text to output.
+        (Removes vt100 escape codes. -- used for safely writing text.)
+        """
+        self._buffer.append(data.replace("\x1b", "?"))
+
+    def set_title(self, title: str) -> None:
+        """
+        Set terminal title.
+        """
+        if self.term not in (
+            "linux",
+            "eterm-color",
+        ):  # Not supported by the Linux console.
+            self.write_raw(
+                "\x1b]2;%s\x07" % title.replace("\x1b", "").replace("\x07", "")
+            )
+
+    def clear_title(self) -> None:
+        self.set_title("")
+
+    def erase_screen(self) -> None:
+        """
+        Erases the screen with the background colour and moves the cursor to
+        home.
+        """
+        self.write_raw("\x1b[2J")
+
+    def enter_alternate_screen(self) -> None:
+        self.write_raw("\x1b[?1049h\x1b[H")
+
+    def quit_alternate_screen(self) -> None:
+        self.write_raw("\x1b[?1049l")
+
+    def enable_mouse_support(self) -> None:
+        self.write_raw("\x1b[?1000h")
+
+        # Enable urxvt Mouse mode. (For terminals that understand this.)
+        self.write_raw("\x1b[?1015h")
+
+        # Also enable Xterm SGR mouse mode. (For terminals that understand this.)
+        self.write_raw("\x1b[?1006h")
+
+        # Note: E.g. lxterminal understands 1000h, but not the urxvt or sgr
+        #       extensions.
+
+    def disable_mouse_support(self) -> None:
+        self.write_raw("\x1b[?1000l")
+        self.write_raw("\x1b[?1015l")
+        self.write_raw("\x1b[?1006l")
+
+    def erase_end_of_line(self) -> None:
+        """
+        Erases from the current cursor position to the end of the current line.
+        """
+        self.write_raw("\x1b[K")
+
+    def erase_down(self) -> None:
+        """
+        Erases the screen from the current line down to the bottom of the
+        screen.
+        """
+        self.write_raw("\x1b[J")
+
+    def reset_attributes(self) -> None:
+        self.write_raw("\x1b[0m")
+
+    def set_attributes(self, attrs: Attrs, color_depth: ColorDepth) -> None:
+        """
+        Create new style and output.
+
+        :param attrs: `Attrs` instance.
+        """
+        # Get current depth.
+        escape_code_cache = self._escape_code_caches[color_depth]
+
+        # Write escape character.
+        self.write_raw(escape_code_cache[attrs])
+
+    def disable_autowrap(self) -> None:
+        self.write_raw("\x1b[?7l")
+
+    def enable_autowrap(self) -> None:
+        self.write_raw("\x1b[?7h")
+
+    def enable_bracketed_paste(self) -> None:
+        self.write_raw("\x1b[?2004h")
+
+    def disable_bracketed_paste(self) -> None:
+        self.write_raw("\x1b[?2004l")
+
+    def cursor_goto(self, row: int = 0, column: int = 0) -> None:
+        """
+        Move cursor position.
+        """
+        self.write_raw("\x1b[%i;%iH" % (row, column))
+
+    def cursor_up(self, amount: int) -> None:
+        if amount == 0:
+            pass
+        elif amount == 1:
+            self.write_raw("\x1b[A")
+        else:
+            self.write_raw("\x1b[%iA" % amount)
 
-    @classmethod
-    def getSettings(cls, sessionType):
-        settings = [("Laps", {'minValue': 1, "default": 3, "increment": 1}),
-                    ("Time Limit", {'choices': [('None', 0),
-                                                ('1 Minute', 60),
-                                                ('2 Minutes', 120),
-                                                ('5 Minutes', 300),
-                                                ('10 Minutes', 600),
-                                                ('20 Minutes', 1200)],
-                                    'default':0}),
-                    ("Mine Spawning", {'choices': [('No Mines', 0),
-                                                   ('8 Seconds', 8000),
-                                                   ('4 Seconds', 4000),
-                                                   ('2 Seconds', 2000)],
-                                       'default':4000}),
-                    ("Bomb Spawning", {'choices': [('None', 0),
-                                                   ('8 Seconds', 8000),
-                                                   ('4 Seconds', 4000),
-                                                   ('2 Seconds', 2000),
-                                                   ('1 Second', 1000)],
-                                       'default':2000}),
-                    ("Epic Mode", {'default': False})]
-
-        if issubclass(sessionType, bs.TeamsSession):
-            settings.append(("Entire Team Must Finish", {'default': False}))
-        return settings
-
-    def __init__(self, settings):
-        self._raceStarted = False
-        bs.TeamGameActivity.__init__(self, settings)
-        self._scoreBoard = bs.ScoreBoard()
-        if self.settings['Epic Mode']:
-            self._isSlowMotion = True
-        self._scoreSound = bs.getSound("score")
-        self._swipSound = bs.getSound("swip")
-        self._lastTeamTime = None
-        self._frontRaceRegion = None
-
-    def getInstanceDescription(self):
-        if isinstance(
-                self.getSession(),
-                bs.TeamsSession) and self.settings.get(
-                'Entire Team Must Finish', False):
-            tStr = ' Your entire team has to finish.'
+    def cursor_down(self, amount: int) -> None:
+        if amount == 0:
+            pass
+        elif amount == 1:
+            # Note: Not the same as '\n', '\n' can cause the window content to
+            #       scroll.
+            self.write_raw("\x1b[B")
         else:
-            tStr = ''
+            self.write_raw("\x1b[%iB" % amount)
 
-        if self.settings['Laps'] > 1:
-            s = ('Run ${ARG1} laps.'+tStr, self.settings['Laps'])
+    def cursor_forward(self, amount: int) -> None:
+        if amount == 0:
+            pass
+        elif amount == 1:
+            self.write_raw("\x1b[C")
         else:
-            s = 'Run 1 lap.'+tStr
-        return s
+            self.write_raw("\x1b[%iC" % amount)
 
-    def getInstanceScoreBoardDescription(self):
-        if self.settings['Laps'] > 1:
-            s = ('run ${ARG1} laps', self.settings['Laps'])
+    def cursor_backward(self, amount: int) -> None:
+        if amount == 0:
+            pass
+        elif amount == 1:
+            self.write_raw("\b")  # '\x1b[D'
         else:
-            s = 'run 1 lap'
-        return s
+            self.write_raw("\x1b[%iD" % amount)
 
-    def onTransitionIn(self):
-        bs.TeamGameActivity.onTransitionIn(
-            self, music='Epic Race' if self.settings['Epic Mode'] else 'Race')
-
-        self._nubTex = bs.getTexture('nub')
-        self._beep1Sound = bs.getSound('raceBeep1')
-        self._beep2Sound = bs.getSound('raceBeep2')
-
-        pts = self.getMap().getDefPoints('racePoint')
-
-        m = self._raceRegionMaterial = bs.Material()
-        m.addActions(
-            conditions=("theyHaveMaterial",
-                        bs.getSharedObject('playerMaterial')),
-            actions=(("modifyPartCollision", "collide", True),
-                     ("modifyPartCollision", "physical", False),
-                     ("call", "atConnect", self._handleRacePointCollide)))
-
-        self._regions = []
-        for pt in pts:
-            self._regions.append(RaceRegion(pt, len(self._regions)))
-
-    def _flashPlayer(self, player, scale):
-        pos = player.actor.node.position
-        light = bs.newNode('light',
-                           attrs={'position': pos,
-                                  'color': (1, 1, 0),
-                                  'heightAttenuated': False,
-                                  'radius': 0.4})
-        bs.gameTimer(500, light.delete)
-        bs.animate(light, 'intensity', {0: 0, 100: 1.0*scale, 500: 0})
+    def hide_cursor(self) -> None:
+        self.write_raw("\x1b[?25l")
 
-    def _handleRacePointCollide(self):
+    def show_cursor(self) -> None:
+        self.write_raw("\x1b[?12l\x1b[?25h")  # Stop blinking cursor and show.
 
-        regionNode, playerNode = bs.getCollisionInfo(
-            'sourceNode', 'opposingNode')
-        try:
-            player = playerNode.getDelegate().getPlayer()
-        except Exception:
-            player = None
-        region = regionNode.getDelegate()
-        if player is None or not player.exists() or region is None:
+    def flush(self) -> None:
+        """
+        Write to output stream and flush.
+        """
+        if not self._buffer:
             return
 
-        lastRegion = player.gameData['lastRegion']
-        thisRegion = region._index
+        data = "".join(self._buffer)
 
-        if lastRegion != thisRegion:
-
-            # if a player tries to skip regions, smite them
-            # ..allow a one region leeway though (its plausable players can get
-            # blown over a region, etc)
-            if thisRegion > lastRegion + 2:
-                if player.isAlive():
-                    player.actor.handleMessage(bs.DieMessage())
-                    bs.screenMessage(
-                        bs.Lstr(translate=(
-                            'statements',
-                            "Killing ${NAME} for skipping part of the track!"),
-                            subs=[('${NAME}', player.getName(full=True))]),
-                        color=(1, 0, 0))
+        try:
+            # (We try to encode ourself, because that way we can replace
+            # characters that don't exist in the character set, avoiding
+            # UnicodeEncodeError crashes. E.g. u'\xb7' does not appear in 'ascii'.)
+            # My Arch Linux installation of july 2015 reported 'ANSI_X3.4-1968'
+            # for sys.stdout.encoding in xterm.
+            out: IO
+            if self.write_binary:
+                if hasattr(self.stdout, "buffer"):
+                    out = self.stdout.buffer  # Py3.
+                else:
+                    out = self.stdout
+                out.write(data.encode(self.stdout.encoding or "utf-8", "replace"))
             else:
-                # if this player is in first, note that this is the
-                # front-most race-point
-                if player.gameData['rank'] == 0:
-                    self._frontRaceRegion = thisRegion
-
-                player.gameData['lastRegion'] = thisRegion
-                if lastRegion >= len(self._regions)-2 and thisRegion == 0:
-                    team = player.getTeam()
-                    player.gameData['lap'] = min(
-                        self.settings['Laps'],
-                        player.gameData['lap'] + 1)
-
-                    # in teams mode with all-must-finish on, the team lap
-                    # value is the min of all team players
-                    # ..otherwise its the max
-                    if isinstance(
-                            self.getSession(),
-                            bs.TeamsSession) and self.settings.get(
-                            'Entire Team Must Finish'):
-                        team.gameData['lap'] = min(
-                            [p.gameData['lap'] for p in team.players])
-                    else:
-                        team.gameData['lap'] = max(
-                            [p.gameData['lap'] for p in team.players])
-
-                    # a player is finishing
-                    if player.gameData['lap'] == self.settings['Laps']:
-
-                        # in teams mode, hand out points based on the order
-                        # players come in
-                        if isinstance(self.getSession(), bs.TeamsSession):
-                            if self._teamFinishPts > 0:
-                                self.scoreSet.playerScored(
-                                    player, self._teamFinishPts,
-                                    screenMessage=False)
-                            self._teamFinishPts -= 25
-
-                        # flash where the player is
-                        self._flashPlayer(player, 1.0)
-                        player.gameData['finished'] = True
-                        player.actor.handleMessage(
-                            bs.DieMessage(immediate=True))
-
-                        # makes sure noone behind them passes them in rank
-                        # while finishing..
-                        player.gameData['distance'] = 9999.0
-
-                        # if the whole team has finished the race..
-                        if team.gameData['lap'] == self.settings['Laps']:
-                            bs.playSound(self._scoreSound)
-                            player.getTeam().gameData['finished'] = True
-                            self._lastTeamTime = player.getTeam(
-                            ).gameData['time'] = \
-                                bs.getGameTime()-self._timer.getStartTime()
-                            self._checkEndGame()
-
-                        # team has yet to finish..
-                        else:
-                            bs.playSound(self._swipSound)
+                self.stdout.write(data)
 
-                    # they've just finished a lap but not the race..
-                    else:
-                        bs.playSound(self._swipSound)
-                        self._flashPlayer(player, 0.3)
-
-                        # print their lap number over their head..
-                        try:
-                            m = bs.newNode('math', owner=player.actor.node,
-                                           attrs={'input1': (0, 1.9, 0),
-                                                  'operation': 'add'})
-                            player.actor.node.connectAttr(
-                                'torsoPosition', m, 'input2')
-                            t = bs.newNode('text', owner=m, attrs={
-                                'text': bs.Lstr(
-                                    resource='lapNumberText',
-                                    subs=[('${CURRENT}',
-                                           str(player.gameData['lap']+1)),
-                                          ('${TOTAL}',
-                                           str(self.settings['Laps']))]),
-                                'inWorld': True,
-                                'color': (1, 1, 0, 1),
-                                'scale': 0.015,
-                                'hAlign': 'center'})
-                            m.connectAttr('output', t, 'position')
-                            bs.animate(
-                                t, 'scale',
-                                {0: 0, 200: 0.019, 2000: 0.019, 2200: 0})
-                            bs.gameTimer(2300, m.delete)
-                        except Exception, e:
-                            print 'Exception printing lap:', e
-
-    def onTeamJoin(self, team):
-        team.gameData['time'] = None
-        team.gameData['lap'] = 0
-        team.gameData['finished'] = False
-        self._updateScoreBoard()
-
-    def onPlayerJoin(self, player):
-        player.gameData['lastRegion'] = 0
-        player.gameData['lap'] = 0
-        player.gameData['distance'] = 0.0
-        player.gameData['finished'] = False
-        player.gameData['rank'] = None
-        bs.TeamGameActivity.onPlayerJoin(self, player)
-
-    def onPlayerLeave(self, player):
-        bs.TeamGameActivity.onPlayerLeave(self, player)
-
-        # a player leaving disqualifies the team if 'Entire Team Must Finish'
-        # is on (otherwise in teams mode everyone could just leave except the
-        # leading player to win)
-        if isinstance(self.getSession(),
-                      bs.TeamsSession) and self.settings.get(
-                'Entire Team Must Finish'):
-            # FIXME translate this
-            bs.screenMessage(
-                bs.Lstr(
-                    translate=(
-                        'statements',
-                        '${TEAM} is disqualified because ${PLAYER} left'),
-                    subs=[('${TEAM}', player.getTeam().name),
-                          ('${PLAYER}', player.getName(full=True))]),
-                color=(1, 1, 0))
-            player.getTeam().gameData['finished'] = True
-            player.getTeam().gameData['time'] = None
-            player.getTeam().gameData['lap'] = 0
-            bs.playSound(bs.getSound("boo"))
-            for player in player.getTeam().players:
-                player.gameData['lap'] = 0
-                player.gameData['finished'] = True
-                try:
-                    player.actor.handleMessage(bs.DieMessage())
-                except Exception:
-                    pass
-
-        # delay by one tick so team/player lists will be updated
-        bs.gameTimer(1, self._checkEndGame)
-
-    def _updateScoreBoard(self):
-        for team in self.teams:
-            distances = [player.gameData['distance'] for player in team.players]
-            if len(distances) == 0:
-                teamDist = 0
+            self.stdout.flush()
+        except IOError as e:
+            if e.args and e.args[0] == errno.EINTR:
+                # Interrupted system call. Can happen in case of a window
+                # resize signal. (Just ignore. The resize handler will render
+                # again anyway.)
+                pass
+            elif e.args and e.args[0] == 0:
+                # This can happen when there is a lot of output and the user
+                # sends a KeyboardInterrupt by pressing Control-C. E.g. in
+                # a Python REPL when we execute "while True: print('test')".
+                # (The `ptpython` REPL uses this `Output` class instead of
+                # `stdout` directly -- in order to be network transparent.)
+                # So, just ignore.
+                pass
             else:
-                if isinstance(
-                        self.getSession(),
-                        bs.TeamsSession) and self.settings.get(
-                        'Entire Team Must Finish'):
-                    teamDist = min(distances)
-                else:
-                    teamDist = max(distances)
-            self._scoreBoard.setTeamValue(
-                team, teamDist, self.settings['Laps'],
-                flash=(teamDist >= float(self.settings['Laps'])),
-                showValue=False)
-
-    def onBegin(self):
-        bs.TeamGameActivity.onBegin(self)
-        self.setupStandardTimeLimit(self.settings['Time Limit'])
-        self.setupStandardPowerupDrops()
-        self._teamFinishPts = 100
-
-        # throw a timer up on-screen
-        self._timeText = bs.NodeActor(
-            bs.newNode(
-                'text',
-                attrs={'vAttach': 'top', 'hAttach': 'center',
-                       'hAlign': 'center', 'color': (1, 1, 0.5, 1),
-                       'flatness': 0.5, 'shadow': 0.5, 'position': (0, -50),
-                       'scale': 1.4, 'text': ''}))
-        self._timer = bs.OnScreenTimer()
-
-        if self.settings['Mine Spawning'] != 0:
-            self._raceMines = [
-                {'point': p, 'mine': None}
-                for p in self.getMap().getDefPoints('raceMine')]
-            if len(self._raceMines) > 0:
-                self._raceMineTimer = bs.Timer(
-                    self.settings['Mine Spawning'],
-                    self._updateRaceMine, repeat=True)
-
-        self._scoreBoardTimer = bs.Timer(
-            250, self._updateScoreBoard, repeat=True)
-        self._playerOrderUpdateTimer = bs.Timer(
-            250, self._updatePlayerOrder, repeat=True)
-
-        if self._isSlowMotion:
-            tScale = 0.4
-            lightY = 50
-        else:
-            tScale = 1.0
-            lightY = 150
-        lStart = int(7100*tScale)
-        inc = int(1250*tScale)
-
-        bs.gameTimer(lStart, self._doLight1)
-        bs.gameTimer(lStart+inc, self._doLight2)
-        bs.gameTimer(lStart+2*inc, self._doLight3)
-        bs.gameTimer(lStart+3*inc, self._startRace)
-
-        self._startLights = []
-        for i in range(4):
-            l = bs.newNode('image',
-                           attrs={'texture': bs.getTexture('nub'),
-                                  'opacity': 1.0,
-                                  'absoluteScale': True,
-                                  'position': (-75+i*50, lightY),
-                                  'scale': (50, 50),
-                                  'attach': 'center'})
-            bs.animate(
-                l, 'opacity',
-                {4000 * tScale: 0, 5000 * tScale: 1.0, 12000 * tScale: 1.0,
-                 12500 * tScale: 0.0})
-            bs.gameTimer(int(13000*tScale), l.delete)
-            self._startLights.append(l)
-
-        self._startLights[0].color = (0.2, 0, 0)
-        self._startLights[1].color = (0.2, 0, 0)
-        self._startLights[2].color = (0.2, 0.05, 0)
-        self._startLights[3].color = (0.0, 0.3, 0)
-
-    def _doLight1(self):
-        self._startLights[0].color = (1.0, 0, 0)
-        bs.playSound(self._beep1Sound)
-
-    def _doLight2(self):
-        self._startLights[1].color = (1.0, 0, 0)
-        bs.playSound(self._beep1Sound)
-
-    def _doLight3(self):
-        self._startLights[2].color = (1.0, 0.3, 0)
-        bs.playSound(self._beep1Sound)
-
-    def _startRace(self):
-        self._startLights[3].color = (0.0, 1.0, 0)
-        bs.playSound(self._beep2Sound)
-        for player in self.players:
-            if player.actor is not None:
-                try:
-                    player.actor.connectControlsToPlayer()
-                except Exception, e:
-                    print 'Exception in race player connects:', e
-        self._timer.start()
-
-        if self.settings['Bomb Spawning'] != 0:
-            self._bombSpawnTimer = bs.Timer(
-                self.settings['Bomb Spawning'],
-                self._spawnBomb, repeat=True)
-
-        self._raceStarted = True
-
-    def _updatePlayerOrder(self):
-
-        # calc all player distances
-        for player in self.players:
-            try:
-                pos = bs.Vector(*player.actor.node.position)
-            except Exception:
-                pos = None
-            if pos is not None:
-                rIndex = player.gameData['lastRegion']
-                r1 = self._regions[rIndex]
-                r1Pt = bs.Vector(*r1._pt[:3])
-                r2 = self._regions[0] if rIndex == len(
-                    self._regions)-1 else self._regions[rIndex+1]
-                r2Pt = bs.Vector(*r2._pt[:3])
-                r1Dist = (pos-r1Pt).length()
-                r2Dist = (pos-r2Pt).length()
-                amt = 1.0-(r2Dist/(r2Pt-r1Pt).length())
-                amt = player.gameData['lap'] + (
-                    rIndex+amt) * (1.0/len(self._regions))
-                player.gameData['distance'] = amt
-
-        # sort players by distance and update their ranks
-        pList = [[player.gameData['distance'], player]
-                 for player in self.players]
-        pList.sort(reverse=True)
-        for i, p in enumerate(pList):
-            try:
-                p[1].gameData['rank'] = i
-                if p[1].actor is not None:
-                    n = p[1].actor.distanceTxt
-                    if n.exists():
-                        n.text = str(i+1) if p[1].isAlive() else ''
-            except Exception:
-                bs.printException('error updating player orders')
-
-    def _spawnBomb(self):
-        if self._frontRaceRegion is None:
-            return
-        region = (self._frontRaceRegion+(3)) % len(self._regions)
-        #print 'WOULD SPAWN BOMB AT',bs.getGameTime(),'AT REGION',region
-        pt = self._regions[region]._pt
-        # dont use the full region so we're less likely to spawn off a cliff
-        regionScale = 0.8
-        xRange = ((-0.5, 0.5) if pt[3] == 0
-                  else (-regionScale*pt[3], regionScale*pt[3]))
-        zRange = ((-0.5, 0.5) if pt[5] == 0
-                  else (-regionScale*pt[5], regionScale*pt[5]))
-        pt = (pt[0]+random.uniform(*xRange),
-              pt[1]+1.0, pt[2]+random.uniform(*zRange))
-        bs.gameTimer(
-            random.randrange(2000),
-            bs.WeakCall(self._spawnBombAtPt, pt))
+                raise
 
-    def _spawnBombAtPt(self, pt):
-        if self.hasEnded():
-            return
-        bs.Bomb(position=pt, bombType='normal').autoRetain()
-
-    def _makeMine(self, i):
-        m = self._raceMines[i]
-        m['mine'] = bs.Bomb(position=m['point'][:3], bombType='landMine')
-        m['mine'].arm()
-
-    def _flashMine(self, i):
-        m = self._raceMines[i]
-        light = bs.newNode("light",
-                           attrs={'position': m['point'][:3],
-                                  'color': (1, 0.2, 0.2),
-                                  'radius': 0.1,
-                                  'heightAttenuated': False})
-        bs.animate(light, "intensity", {0: 0, 100: 1.0, 200: 0}, loop=True)
-        bs.gameTimer(1000, light.delete)
-
-    def _updateRaceMine(self):
-        for i in range(3):
-            mIndex = random.randrange(len(self._raceMines))
-            m = self._raceMines[mIndex]
-            if m['mine'] is None or not m['mine'].exists():
-                break
-        if m['mine'] is None or not m['mine'].exists():
-            self._flashMine(mIndex)
-            bs.gameTimer(950, bs.Call(self._makeMine, mIndex))
-
-    def spawnPlayer(self, player):
+        self._buffer = []
 
-        # dont allow spawning if this team is done
-        if player.getTeam().gameData['finished']:
-            return
-
-        pt = self._regions[player.gameData['lastRegion']]._pt
-        # dont use the full region so we're less likely to spawn off a cliff
-        regionScale = 0.8 
-        xRange = ((-0.5, 0.5) if pt[3] == 0
-                  else (-regionScale*pt[3], regionScale*pt[3]))
-        zRange = ((-0.5, 0.5) if pt[5] == 0
-                  else (-regionScale*pt[5], regionScale*pt[5]))
-        pt = (pt[0]+random.uniform(*xRange),
-              pt[1], pt[2]+random.uniform(*zRange))
-        spaz = self.spawnPlayerSpaz(
-            player, position=pt, angle=90 if not self._raceStarted else None)
-
-        # prevent controlling of characters before the start of the race
-        if not self._raceStarted:
-            spaz.disconnectControlsFromPlayer()
-
-        m = bs.newNode('math', owner=spaz.node, attrs={
-                       'input1': (0, 1.4, 0), 'operation': 'add'})
-        spaz.node.connectAttr('torsoPosition', m, 'input2')
-        spaz.distanceTxt = bs.newNode('text',
-                                      owner=spaz.node,
-                                      attrs={'text': '',
-                                             'inWorld': True,
-                                             'color': (1, 1, 0.4),
-                                             'scale': 0.02,
-                                             'hAlign': 'center'})
-        m.connectAttr('output', spaz.distanceTxt, 'position')
-
-    def _checkEndGame(self):
-
-        # if there's no teams left racing, finish
-        teamsStillIn = len(
-            [t for t in self.teams if not t.gameData['finished']])
-        if teamsStillIn == 0:
-            self.endGame()
-            return
-
-        # count the number of teams that have completed the race
-        teamsCompleted = len(
-            [t for t in self.teams
-             if t.gameData['finished'] == True and t.gameData['time'] is not
-             None])
-
-        if teamsCompleted > 0:
-            # in teams mode its over as soon as any team finishes the race
-            if isinstance(self.getSession(), bs.TeamsSession):
-                self.endGame()
-            else:
-                # in ffa we keep the race going while there's still any points
-                # to be handed out. find out how many points we have to award
-                # and how many teams have finished, and once that matches
-                # we're done
-                pointsToAward = len(self.getSession()._getFFAPointAwards())
-                if teamsCompleted >= pointsToAward-teamsCompleted:
-                    self.endGame()
-                    return
-
-    def endGame(self):
-
-        # stop updating our time text, and set it to show the exact last
-        # finish time if we have one.. (so users dont get upset if their
-        # final time differs from what they see onscreen by a tiny bit)
-        if self._timer.hasStarted():
-            self._timer.stop(endTime=None if self._lastTeamTime is None else (
-                self._timer.getStartTime()+self._lastTeamTime))
-
-        results = bs.TeamGameResults()
-
-        for t in self.teams:
-            results.setTeamScore(t, t.gameData['time'])
-        # we don't announce a winner in ffa mode since its probably been a
-        # while since the first place guy crossed the finish line so it seems
-        # odd to be announcing that now..
-        self.end(results=results, announceWinningTeam=True if isinstance(
-            self.getSession(), bs.TeamsSession) else False)
-
-    def handleMessage(self, m):
-        if isinstance(m, bs.PlayerSpazDeathMessage):
-            bs.TeamGameActivity.handleMessage(self, m)  # augment default
-            try:
-                player = m.spaz.getPlayer()
-                if player is None:
-                    bs.printError('FIXME: getPlayer() should no '
-                                  'longer ever be returning None')
-                else:
-                    if not player.exists():
-                        raise Exception()
-                team = player.getTeam()
-            except Exception:
-                return
-            if not player.gameData['finished']:
-                self.respawnPlayer(player, respawnTime=1000)
-        else:
-            bs.TeamGameActivity.handleMessage(self, m)
+    def ask_for_cpr(self) -> None:
+        """
+        Asks for a cursor position report (CPR).
+        """
+        self.write_raw("\x1b[6n")
+        self.flush()
+
+    def bell(self) -> None:
+        "Sound bell."
+        self.write_raw("\a")
+        self.flush()
```

### Comparing `prot-3.8.6/src/prot/color/ansi.py` & `prot-3.9.0/src/prot/color/ansi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,110 @@
 # Copyright Jonathan Hartley 2013. BSD 3-Clause license, see LICENSE file.
-'''
+"""
 This module generates ANSI character codes to printing colors to terminals.
 See: http://en.wikipedia.org/wiki/ANSI_escape_code
-'''
+"""
 
-CSI = '\033['
-OSC = '\033]'
-BEL = '\007'
+CSI = "\033["
+OSC = "\033]"
+BEL = "\007"
 
 
 def code_to_chars(code):
-    return CSI + str(code) + 'm'
+    return CSI + str(code) + "m"
+
 
 def set_title(title):
-    return OSC + '2;' + title + BEL
+    return OSC + "2;" + title + BEL
+
 
 def clear_screen(mode=2):
-    return CSI + str(mode) + 'J'
+    return CSI + str(mode) + "J"
+
 
 def clear_line(mode=2):
-    return CSI + str(mode) + 'K'
+    return CSI + str(mode) + "K"
 
 
 class AnsiCodes(object):
     def __init__(self):
         # the subclasses declare class attributes which are numbers.
         # Upon instantiation we define instance attributes, which are the same
         # as the class attributes but wrapped with the ANSI escape sequence
         for name in dir(self):
-            if not name.startswith('_'):
+            if not name.startswith("_"):
                 value = getattr(self, name)
                 setattr(self, name, code_to_chars(value))
 
 
 class AnsiCursor(object):
     def UP(self, n=1):
-        return CSI + str(n) + 'A'
+        return CSI + str(n) + "A"
+
     def DOWN(self, n=1):
-        return CSI + str(n) + 'B'
+        return CSI + str(n) + "B"
+
     def FORWARD(self, n=1):
-        return CSI + str(n) + 'C'
+        return CSI + str(n) + "C"
+
     def BACK(self, n=1):
-        return CSI + str(n) + 'D'
+        return CSI + str(n) + "D"
+
     def POS(self, x=1, y=1):
-        return CSI + str(y) + ';' + str(x) + 'H'
+        return CSI + str(y) + ";" + str(x) + "H"
 
 
 class AnsiFore(AnsiCodes):
-    BLACK           = 30
-    RED             = 31
-    GREEN           = 32
-    YELLOW          = 33
-    BLUE            = 34
-    MAGENTA         = 35
-    CYAN            = 36
-    WHITE           = 37
-    RESET           = 39
+    BLACK = 30
+    RED = 31
+    GREEN = 32
+    YELLOW = 33
+    BLUE = 34
+    MAGENTA = 35
+    CYAN = 36
+    WHITE = 37
+    RESET = 39
 
     # These are fairly well supported, but not part of the standard.
-    LIGHTBLACK_EX   = 90
-    LIGHTRED_EX     = 91
-    LIGHTGREEN_EX   = 92
-    LIGHTYELLOW_EX  = 93
-    LIGHTBLUE_EX    = 94
+    LIGHTBLACK_EX = 90
+    LIGHTRED_EX = 91
+    LIGHTGREEN_EX = 92
+    LIGHTYELLOW_EX = 93
+    LIGHTBLUE_EX = 94
     LIGHTMAGENTA_EX = 95
-    LIGHTCYAN_EX    = 96
-    LIGHTWHITE_EX   = 97
+    LIGHTCYAN_EX = 96
+    LIGHTWHITE_EX = 97
 
 
 class AnsiBack(AnsiCodes):
-    BLACK           = 40
-    RED             = 41
-    GREEN           = 42
-    YELLOW          = 43
-    BLUE            = 44
-    MAGENTA         = 45
-    CYAN            = 46
-    WHITE           = 47
-    RESET           = 49
+    BLACK = 40
+    RED = 41
+    GREEN = 42
+    YELLOW = 43
+    BLUE = 44
+    MAGENTA = 45
+    CYAN = 46
+    WHITE = 47
+    RESET = 49
 
     # These are fairly well supported, but not part of the standard.
-    LIGHTBLACK_EX   = 100
-    LIGHTRED_EX     = 101
-    LIGHTGREEN_EX   = 102
-    LIGHTYELLOW_EX  = 103
-    LIGHTBLUE_EX    = 104
+    LIGHTBLACK_EX = 100
+    LIGHTRED_EX = 101
+    LIGHTGREEN_EX = 102
+    LIGHTYELLOW_EX = 103
+    LIGHTBLUE_EX = 104
     LIGHTMAGENTA_EX = 105
-    LIGHTCYAN_EX    = 106
-    LIGHTWHITE_EX   = 107
+    LIGHTCYAN_EX = 106
+    LIGHTWHITE_EX = 107
 
 
 class AnsiStyle(AnsiCodes):
-    BRIGHT    = 1
-    DIM       = 2
-    NORMAL    = 22
+    BRIGHT = 1
+    DIM = 2
+    NORMAL = 22
     RESET_ALL = 0
 
-Fore   = AnsiFore()
-Back   = AnsiBack()
-Style  = AnsiStyle()
+
+Fore = AnsiFore()
+Back = AnsiBack()
+Style = AnsiStyle()
 Cursor = AnsiCursor()
```

### Comparing `prot-3.8.6/src/prot/color/ansitowin32.py` & `prot-3.9.0/src/prot/color/ansitowin32.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 
 winterm = None
 if windll is not None:
     winterm = WinTerm()
 
 
 class StreamWrapper(object):
-    '''
+    """
     Wraps a stream (such as stdout), acting as a transparent proxy for all
     attribute access apart from method 'write()', which is delegated to our
     Converter instance.
-    '''
+    """
+
     def __init__(self, wrapped, converter):
         # double-underscore everything to prevent clashes with names of
         # attributes on the wrapped stream object.
         self.__wrapped = wrapped
         self.__convertor = converter
 
     def __getattr__(self, name):
@@ -38,16 +39,18 @@
         return self.__wrapped.__exit__(*args, **kwargs)
 
     def write(self, text):
         self.__convertor.write(text)
 
     def isatty(self):
         stream = self.__wrapped
-        if 'PYCHARM_HOSTED' in os.environ:
-            if stream is not None and (stream is sys.__stdout__ or stream is sys.__stderr__):
+        if "PYCHARM_HOSTED" in os.environ:
+            if stream is not None and (
+                stream is sys.__stdout__ or stream is sys.__stderr__
+            ):
                 return True
         try:
             stream_isatty = stream.isatty
         except AttributeError:
             return False
         else:
             return stream_isatty()
@@ -58,81 +61,90 @@
         try:
             return stream.closed
         except AttributeError:
             return True
 
 
 class AnsiToWin32(object):
-    '''
+    """
     Implements a 'write()' method which, on Windows, will strip ANSI character
     sequences from the text, and if outputting to a tty, will convert them into
     win32 function calls.
-    '''
-    ANSI_CSI_RE = re.compile('\001?\033\\[((?:\\d|;)*)([a-zA-Z])\002?')   # Control Sequence Introducer
-    ANSI_OSC_RE = re.compile('\001?\033\\]((?:.|;)*?)(\x07)\002?')        # Operating System Command
+    """
+
+    ANSI_CSI_RE = re.compile(
+        "\001?\033\\[((?:\\d|;)*)([a-zA-Z])\002?"
+    )  # Control Sequence Introducer
+    ANSI_OSC_RE = re.compile(
+        "\001?\033\\]((?:.|;)*?)(\x07)\002?"
+    )  # Operating System Command
 
     def __init__(self, wrapped, convert=None, strip=None, autoreset=False):
         # The wrapped stream (normally sys.stdout or sys.stderr)
         self.wrapped = wrapped
 
         # should we reset colors to defaults after every .write()
         self.autoreset = autoreset
 
         # create the proxy wrapping our output stream
         self.stream = StreamWrapper(wrapped, self)
 
-        on_windows = os.name == 'nt'
+        on_windows = os.name == "nt"
         # We test if the WinAPI works, because even if we are on Windows
         # we may be using a terminal that doesn't support the WinAPI
         # (e.g. Cygwin Terminal). In this case it's up to the terminal
         # to support the ANSI codes.
         conversion_supported = on_windows and winapi_test()
 
         # should we strip ANSI sequences from our output?
         if strip is None:
-            strip = conversion_supported or (not self.stream.closed and not self.stream.isatty())
+            strip = conversion_supported or (
+                not self.stream.closed and not self.stream.isatty()
+            )
         self.strip = strip
 
         # should we should convert ANSI sequences into win32 calls?
         if convert is None:
-            convert = conversion_supported and not self.stream.closed and self.stream.isatty()
+            convert = (
+                conversion_supported and not self.stream.closed and self.stream.isatty()
+            )
         self.convert = convert
 
         # dict of ansi codes to win32 functions and parameters
         self.win32_calls = self.get_win32_calls()
 
         # are we wrapping stderr?
         self.on_stderr = self.wrapped is sys.stderr
 
     def should_wrap(self):
-        '''
+        """
         True if this class is actually needed. If false, then the output
         stream will not be affected, nor will win32 calls be issued, so
         wrapping stdout is not actually required. This will generally be
         False on non-Windows platforms, unless optional functionality like
         autoreset has been requested using kwargs to init()
-        '''
+        """
         return self.convert or self.strip or self.autoreset
 
     def get_win32_calls(self):
         if self.convert and winterm:
             return {
-                AnsiStyle.RESET_ALL: (winterm.reset_all, ),
+                AnsiStyle.RESET_ALL: (winterm.reset_all,),
                 AnsiStyle.BRIGHT: (winterm.style, WinStyle.BRIGHT),
                 AnsiStyle.DIM: (winterm.style, WinStyle.NORMAL),
                 AnsiStyle.NORMAL: (winterm.style, WinStyle.NORMAL),
                 AnsiFore.BLACK: (winterm.fore, WinColor.BLACK),
                 AnsiFore.RED: (winterm.fore, WinColor.RED),
                 AnsiFore.GREEN: (winterm.fore, WinColor.GREEN),
                 AnsiFore.YELLOW: (winterm.fore, WinColor.YELLOW),
                 AnsiFore.BLUE: (winterm.fore, WinColor.BLUE),
                 AnsiFore.MAGENTA: (winterm.fore, WinColor.MAGENTA),
                 AnsiFore.CYAN: (winterm.fore, WinColor.CYAN),
                 AnsiFore.WHITE: (winterm.fore, WinColor.GREY),
-                AnsiFore.RESET: (winterm.fore, ),
+                AnsiFore.RESET: (winterm.fore,),
                 AnsiFore.LIGHTBLACK_EX: (winterm.fore, WinColor.BLACK, True),
                 AnsiFore.LIGHTRED_EX: (winterm.fore, WinColor.RED, True),
                 AnsiFore.LIGHTGREEN_EX: (winterm.fore, WinColor.GREEN, True),
                 AnsiFore.LIGHTYELLOW_EX: (winterm.fore, WinColor.YELLOW, True),
                 AnsiFore.LIGHTBLUE_EX: (winterm.fore, WinColor.BLUE, True),
                 AnsiFore.LIGHTMAGENTA_EX: (winterm.fore, WinColor.MAGENTA, True),
                 AnsiFore.LIGHTCYAN_EX: (winterm.fore, WinColor.CYAN, True),
@@ -141,15 +153,15 @@
                 AnsiBack.RED: (winterm.back, WinColor.RED),
                 AnsiBack.GREEN: (winterm.back, WinColor.GREEN),
                 AnsiBack.YELLOW: (winterm.back, WinColor.YELLOW),
                 AnsiBack.BLUE: (winterm.back, WinColor.BLUE),
                 AnsiBack.MAGENTA: (winterm.back, WinColor.MAGENTA),
                 AnsiBack.CYAN: (winterm.back, WinColor.CYAN),
                 AnsiBack.WHITE: (winterm.back, WinColor.GREY),
-                AnsiBack.RESET: (winterm.back, ),
+                AnsiBack.RESET: (winterm.back,),
                 AnsiBack.LIGHTBLACK_EX: (winterm.back, WinColor.BLACK, True),
                 AnsiBack.LIGHTRED_EX: (winterm.back, WinColor.RED, True),
                 AnsiBack.LIGHTGREEN_EX: (winterm.back, WinColor.GREEN, True),
                 AnsiBack.LIGHTYELLOW_EX: (winterm.back, WinColor.YELLOW, True),
                 AnsiBack.LIGHTBLUE_EX: (winterm.back, WinColor.BLUE, True),
                 AnsiBack.LIGHTMAGENTA_EX: (winterm.back, WinColor.MAGENTA, True),
                 AnsiBack.LIGHTCYAN_EX: (winterm.back, WinColor.CYAN, True),
@@ -162,96 +174,89 @@
             self.write_and_convert(text)
         else:
             self.wrapped.write(text)
             self.wrapped.flush()
         if self.autoreset:
             self.reset_all()
 
-
     def reset_all(self):
         if self.convert:
-            self.call_win32('m', (0,))
+            self.call_win32("m", (0,))
         elif not self.strip and not self.stream.closed:
             self.wrapped.write(Style.RESET_ALL)
 
-
     def write_and_convert(self, text):
-        '''
+        """
         Write the given text to our wrapped stream, stripping any ANSI
         sequences from the text, and optionally converting them into win32
         calls.
-        '''
+        """
         cursor = 0
         text = self.convert_osc(text)
         for match in self.ANSI_CSI_RE.finditer(text):
             start, end = match.span()
             self.write_plain_text(text, cursor, start)
             self.convert_ansi(*match.groups())
             cursor = end
         self.write_plain_text(text, cursor, len(text))
 
-
     def write_plain_text(self, text, start, end):
         if start < end:
             self.wrapped.write(text[start:end])
             self.wrapped.flush()
 
-
     def convert_ansi(self, paramstring, command):
         if self.convert:
             params = self.extract_params(command, paramstring)
             self.call_win32(command, params)
 
-
     def extract_params(self, command, paramstring):
-        if command in 'Hf':
-            params = tuple(int(p) if len(p) != 0 else 1 for p in paramstring.split(';'))
+        if command in "Hf":
+            params = tuple(int(p) if len(p) != 0 else 1 for p in paramstring.split(";"))
             while len(params) < 2:
                 # defaults:
                 params = params + (1,)
         else:
-            params = tuple(int(p) for p in paramstring.split(';') if len(p) != 0)
+            params = tuple(int(p) for p in paramstring.split(";") if len(p) != 0)
             if len(params) == 0:
                 # defaults:
-                if command in 'JKm':
+                if command in "JKm":
                     params = (0,)
-                elif command in 'ABCD':
+                elif command in "ABCD":
                     params = (1,)
 
         return params
 
-
     def call_win32(self, command, params):
-        if command == 'm':
+        if command == "m":
             for param in params:
                 if param in self.win32_calls:
                     func_args = self.win32_calls[param]
                     func = func_args[0]
                     args = func_args[1:]
                     kwargs = dict(on_stderr=self.on_stderr)
                     func(*args, **kwargs)
-        elif command in 'J':
+        elif command in "J":
             winterm.erase_screen(params[0], on_stderr=self.on_stderr)
-        elif command in 'K':
+        elif command in "K":
             winterm.erase_line(params[0], on_stderr=self.on_stderr)
-        elif command in 'Hf':     # cursor position - absolute
+        elif command in "Hf":  # cursor position - absolute
             winterm.set_cursor_position(params, on_stderr=self.on_stderr)
-        elif command in 'ABCD':   # cursor position - relative
+        elif command in "ABCD":  # cursor position - relative
             n = params[0]
             # A - up, B - down, C - forward, D - back
-            x, y = {'A': (0, -n), 'B': (0, n), 'C': (n, 0), 'D': (-n, 0)}[command]
+            x, y = {"A": (0, -n), "B": (0, n), "C": (n, 0), "D": (-n, 0)}[command]
             winterm.cursor_adjust(x, y, on_stderr=self.on_stderr)
 
-
     def convert_osc(self, text):
         for match in self.ANSI_OSC_RE.finditer(text):
             start, end = match.span()
             text = text[:start] + text[end:]
             paramstring, command = match.groups()
-            if command in '\x07':       # \x07 = BEL
+            if command in "\x07":  # \x07 = BEL
                 params = paramstring.split(";")
                 # 0 - change title and icon (we will only change title)
                 # 1 - change icon (we don't support this)
                 # 2 - change title
-                if params[0] in '02':
+                if params[0] in "02":
                     winterm.set_title(params[1])
         return text
```

### Comparing `prot-3.8.6/src/prot/color/initialise.py` & `prot-3.9.0/src/prot/color/initialise.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 wrapped_stdout = None
 wrapped_stderr = None
 
 atexit_done = False
 
 
 def reset_all():
-    if AnsiToWin32 is not None:    # Issue #74: objects might become None at exit
+    if AnsiToWin32 is not None:  # Issue #74: objects might become None at exit
         AnsiToWin32(orig_stdout).reset_all()
 
 
 def init(autoreset=False, convert=None, strip=None, wrap=True):
-
     if not wrap and any([autoreset, convert, strip]):
-        raise ValueError('wrap=False conflicts with any other arg=True')
+        raise ValueError("wrap=False conflicts with any other arg=True")
 
     global wrapped_stdout, wrapped_stderr
     global orig_stdout, orig_stderr
 
     orig_stdout = sys.stdout
     orig_stderr = sys.stderr
 
     if sys.stdout is None:
         wrapped_stdout = None
     else:
-        sys.stdout = wrapped_stdout = \
-            wrap_stream(orig_stdout, convert, strip, autoreset, wrap)
+        sys.stdout = wrapped_stdout = wrap_stream(
+            orig_stdout, convert, strip, autoreset, wrap
+        )
     if sys.stderr is None:
         wrapped_stderr = None
     else:
-        sys.stderr = wrapped_stderr = \
-            wrap_stream(orig_stderr, convert, strip, autoreset, wrap)
+        sys.stderr = wrapped_stderr = wrap_stream(
+            orig_stderr, convert, strip, autoreset, wrap
+        )
 
     global atexit_done
     if not atexit_done:
         atexit.register(reset_all)
         atexit_done = True
 
 
@@ -69,12 +70,11 @@
         sys.stdout = wrapped_stdout
     if wrapped_stderr is not None:
         sys.stderr = wrapped_stderr
 
 
 def wrap_stream(stream, convert, strip, autoreset, wrap):
     if wrap:
-        wrapper = AnsiToWin32(stream,
-            convert=convert, strip=strip, autoreset=autoreset)
+        wrapper = AnsiToWin32(stream, convert=convert, strip=strip, autoreset=autoreset)
         if wrapper.should_wrap():
             stream = wrapper.stream
     return stream
```

### Comparing `prot-3.8.6/src/prot/color/win32.py` & `prot-3.9.0/src/prot/color/win32.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,50 @@
 # from winbase.h
 STDOUT = -11
 STDERR = -12
 
 try:
     import ctypes
     from ctypes import LibraryLoader
+
     windll = LibraryLoader(ctypes.WinDLL)
     from ctypes import wintypes
 except (AttributeError, ImportError):
     windll = None
     SetConsoleTextAttribute = lambda *_: None
     winapi_test = lambda *_: None
 else:
     from ctypes import byref, Structure, c_char, POINTER
 
     COORD = wintypes._COORD
 
     class CONSOLE_SCREEN_BUFFER_INFO(Structure):
         """struct in wincon.h."""
+
         _fields_ = [
             ("dwSize", COORD),
             ("dwCursorPosition", COORD),
             ("wAttributes", wintypes.WORD),
             ("srWindow", wintypes.SMALL_RECT),
             ("dwMaximumWindowSize", COORD),
         ]
+
         def __str__(self):
-            return '(%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d)' % (
-                self.dwSize.Y, self.dwSize.X
-                , self.dwCursorPosition.Y, self.dwCursorPosition.X
-                , self.wAttributes
-                , self.srWindow.Top, self.srWindow.Left, self.srWindow.Bottom, self.srWindow.Right
-                , self.dwMaximumWindowSize.Y, self.dwMaximumWindowSize.X
+            return "(%d,%d,%d,%d,%d,%d,%d,%d,%d,%d,%d)" % (
+                self.dwSize.Y,
+                self.dwSize.X,
+                self.dwCursorPosition.Y,
+                self.dwCursorPosition.X,
+                self.wAttributes,
+                self.srWindow.Top,
+                self.srWindow.Left,
+                self.srWindow.Bottom,
+                self.srWindow.Right,
+                self.dwMaximumWindowSize.Y,
+                self.dwMaximumWindowSize.X,
             )
 
     _GetStdHandle = windll.kernel32.GetStdHandle
     _GetStdHandle.argtypes = [
         wintypes.DWORD,
     ]
     _GetStdHandle.restype = wintypes.HANDLE
@@ -80,34 +89,31 @@
         wintypes.DWORD,
         COORD,
         POINTER(wintypes.DWORD),
     ]
     _FillConsoleOutputAttribute.restype = wintypes.BOOL
 
     _SetConsoleTitleW = windll.kernel32.SetConsoleTitleW
-    _SetConsoleTitleW.argtypes = [
-        wintypes.LPCWSTR
-    ]
+    _SetConsoleTitleW.argtypes = [wintypes.LPCWSTR]
     _SetConsoleTitleW.restype = wintypes.BOOL
 
     def _winapi_test(handle):
         csbi = CONSOLE_SCREEN_BUFFER_INFO()
-        success = _GetConsoleScreenBufferInfo(
-            handle, byref(csbi))
+        success = _GetConsoleScreenBufferInfo(handle, byref(csbi))
         return bool(success)
 
     def winapi_test():
-        return any(_winapi_test(h) for h in
-                   (_GetStdHandle(STDOUT), _GetStdHandle(STDERR)))
+        return any(
+            _winapi_test(h) for h in (_GetStdHandle(STDOUT), _GetStdHandle(STDERR))
+        )
 
     def GetConsoleScreenBufferInfo(stream_id=STDOUT):
         handle = _GetStdHandle(stream_id)
         csbi = CONSOLE_SCREEN_BUFFER_INFO()
-        success = _GetConsoleScreenBufferInfo(
-            handle, byref(csbi))
+        success = _GetConsoleScreenBufferInfo(handle, byref(csbi))
         return csbi
 
     def SetConsoleTextAttribute(stream_id, attrs):
         handle = _GetStdHandle(stream_id)
         return _SetConsoleTextAttribute(handle, attrs)
 
     def SetConsoleCursorPosition(stream_id, position, adjust=True):
@@ -131,22 +137,24 @@
     def FillConsoleOutputCharacter(stream_id, char, length, start):
         handle = _GetStdHandle(stream_id)
         char = c_char(char.encode())
         length = wintypes.DWORD(length)
         num_written = wintypes.DWORD(0)
         # Note that this is hard-coded for ANSI (vs wide) bytes.
         success = _FillConsoleOutputCharacterA(
-            handle, char, length, start, byref(num_written))
+            handle, char, length, start, byref(num_written)
+        )
         return num_written.value
 
     def FillConsoleOutputAttribute(stream_id, attr, length, start):
-        ''' FillConsoleOutputAttribute( hConsole, csbi.wAttributes, dwConSize, coordScreen, &cCharsWritten )'''
+        """FillConsoleOutputAttribute( hConsole, csbi.wAttributes, dwConSize, coordScreen, &cCharsWritten )"""
         handle = _GetStdHandle(stream_id)
         attribute = wintypes.WORD(attr)
         length = wintypes.DWORD(length)
         num_written = wintypes.DWORD(0)
         # Note that this is hard-coded for ANSI (vs wide) bytes.
         return _FillConsoleOutputAttribute(
-            handle, attribute, length, start, byref(num_written))
+            handle, attribute, length, start, byref(num_written)
+        )
 
     def SetConsoleTitle(title):
         return _SetConsoleTitleW(title)
```

### Comparing `prot-3.8.6/src/prot/color/winterm.py` & `prot-3.9.0/src/prot/color/winterm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # Copyright Jonathan Hartley 2013. BSD 3-Clause license, see LICENSE file.
 from . import win32
 
 
 # from wincon.h
 class WinColor(object):
-    BLACK   = 0
-    BLUE    = 1
-    GREEN   = 2
-    CYAN    = 3
-    RED     = 4
+    BLACK = 0
+    BLUE = 1
+    GREEN = 2
+    CYAN = 3
+    RED = 4
     MAGENTA = 5
-    YELLOW  = 6
-    GREY    = 7
+    YELLOW = 6
+    GREY = 7
+
 
 # from wincon.h
 class WinStyle(object):
-    NORMAL              = 0x00 # dim text, dim background
-    BRIGHT              = 0x08 # bright text, dim background
-    BRIGHT_BACKGROUND   = 0x80 # dim text, bright background
+    NORMAL = 0x00  # dim text, dim background
+    BRIGHT = 0x08  # bright text, dim background
+    BRIGHT_BACKGROUND = 0x80  # dim text, bright background
 
-class WinTerm(object):
 
+class WinTerm(object):
     def __init__(self):
         self._default = win32.GetConsoleScreenBufferInfo(win32.STDOUT).wAttributes
         self.set_attrs(self._default)
         self._default_fore = self._fore
         self._default_back = self._back
         self._default_style = self._style
         # In order to emulate LIGHT_EX in windows, we borrow the BRIGHT style.
@@ -115,31 +116,35 @@
         handle = win32.STDOUT
         if on_stderr:
             handle = win32.STDERR
         csbi = win32.GetConsoleScreenBufferInfo(handle)
         # get the number of character cells in the current buffer
         cells_in_screen = csbi.dwSize.X * csbi.dwSize.Y
         # get number of character cells before current cursor position
-        cells_before_cursor = csbi.dwSize.X * csbi.dwCursorPosition.Y + csbi.dwCursorPosition.X
+        cells_before_cursor = (
+            csbi.dwSize.X * csbi.dwCursorPosition.Y + csbi.dwCursorPosition.X
+        )
         if mode == 0:
             from_coord = csbi.dwCursorPosition
             cells_to_erase = cells_in_screen - cells_before_cursor
         elif mode == 1:
             from_coord = win32.COORD(0, 0)
             cells_to_erase = cells_before_cursor
         elif mode == 2:
             from_coord = win32.COORD(0, 0)
             cells_to_erase = cells_in_screen
         else:
             # invalid mode
             return
         # fill the entire screen with blanks
-        win32.FillConsoleOutputCharacter(handle, ' ', cells_to_erase, from_coord)
+        win32.FillConsoleOutputCharacter(handle, " ", cells_to_erase, from_coord)
         # now set the buffer's attributes accordingly
-        win32.FillConsoleOutputAttribute(handle, self.get_attrs(), cells_to_erase, from_coord)
+        win32.FillConsoleOutputAttribute(
+            handle, self.get_attrs(), cells_to_erase, from_coord
+        )
         if mode == 2:
             # put the cursor where needed
             win32.SetConsoleCursorPosition(handle, (1, 1))
 
     def erase_line(self, mode=0, on_stderr=False):
         # 0 should clear from the cursor to the end of the line.
         # 1 should clear from the cursor to the beginning of the line.
@@ -157,13 +162,15 @@
         elif mode == 2:
             from_coord = win32.COORD(0, csbi.dwCursorPosition.Y)
             cells_to_erase = csbi.dwSize.X
         else:
             # invalid mode
             return
         # fill the entire screen with blanks
-        win32.FillConsoleOutputCharacter(handle, ' ', cells_to_erase, from_coord)
+        win32.FillConsoleOutputCharacter(handle, " ", cells_to_erase, from_coord)
         # now set the buffer's attributes accordingly
-        win32.FillConsoleOutputAttribute(handle, self.get_attrs(), cells_to_erase, from_coord)
+        win32.FillConsoleOutputAttribute(
+            handle, self.get_attrs(), cells_to_erase, from_coord
+        )
 
     def set_title(self, title):
         win32.SetConsoleTitle(title)
```

### Comparing `prot-3.8.6/src/prot/pip/extra.py` & `prot-3.9.0/src/prot/pip/extra.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import xmlrpc.client as xmlrpclib
 
-pypi = xmlrpclib.ServerProxy('https://pypi.org/pypi', allow_none=True)
+pypi = xmlrpclib.ServerProxy("https://pypi.org/pypi", allow_none=True)
+
 
 def allPackages():
-	"""return a list of all server packages"""
-	return pypi.list_packages()
+    """return a list of all server packages"""
+    return pypi.list_packages()
+
 
 def userPackages(user):
-	"""return a list of user packages"""
-	return pypi.user_packages(user)
+    """return a list of user packages"""
+    return pypi.user_packages(user)
+
 
 def releaseUrls(name, version):
-	"""return a list of release urls"""
-	return pypi.release_urls(name, version)
+    """return a list of release urls"""
+    return pypi.release_urls(name, version)
+
 
 def packageRoles(name):
-	"""return a list of package roles"""
-	return pypi.package_roles(name)
+    """return a list of package roles"""
+    return pypi.package_roles(name)
+
 
 def packageReleases(name, show_hidden=True):
-	"""return a list of package releases"""
-	return pypi.package_releases(name, show_hidden)
+    """return a list of package releases"""
+    return pypi.package_releases(name, show_hidden)
+
 
 def releaseData(name, version):
-	"""return dictionary with release data"""
-	return pypi.release_data(name, version)
+    """return dictionary with release data"""
+    return pypi.release_data(name, version)
```

### Comparing `prot-3.8.6/src/prot/progress/__init__.py` & `prot-3.9.0/src/prot/progress/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,53 +15,54 @@
 from __future__ import division, print_function
 
 from .. import printMsg
 from collections import deque
 from datetime import timedelta
 from math import ceil
 from sys import stderr, stdout
+
 try:
     from time import monotonic
 except ImportError:
     from time import time as monotonic
 
 
-__version__ = '1.5'
+__version__ = "1.5"
 
-HIDE_CURSOR = '\x1b[?25l'
-SHOW_CURSOR = '\x1b[?25h'
+HIDE_CURSOR = "\x1b[?25l"
+SHOW_CURSOR = "\x1b[?25h"
 
 
 class Infinite(object):
     file = stdout
-    sma_window = 10         # Simple Moving Average window
+    sma_window = 10  # Simple Moving Average window
     check_tty = True
     hide_cursor = True
 
-    def __init__(self, message='', **kwargs):
+    def __init__(self, message="", **kwargs):
         self.index = 0
         self.start_ts = monotonic()
         self.avg = 0
         self._avg_update_ts = self.start_ts
         self._ts = self.start_ts
         self._xput = deque(maxlen=self.sma_window)
         for key, val in kwargs.items():
             setattr(self, key, val)
 
         self._width = 0
         self.message = message
 
         if self.file and self.is_tty():
             if self.hide_cursor:
-                printMsg(HIDE_CURSOR, end='', file=self.file)
-            printMsg(self.message, end='', file=self.file)
+                printMsg(HIDE_CURSOR, end="", file=self.file)
+            printMsg(self.message, end="", file=self.file)
             self.file.flush()
 
     def __getitem__(self, key):
-        if key.startswith('_'):
+        if key.startswith("_"):
             return None
         return getattr(self, key, None)
 
     @property
     def elapsed(self):
         return int(monotonic() - self.start_ts)
 
@@ -71,47 +72,46 @@
 
     def update_avg(self, n, dt):
         if n > 0:
             xput_len = len(self._xput)
             self._xput.append(dt / n)
             now = monotonic()
             # update when we're still filling _xput, then after every second
-            if (xput_len < self.sma_window or
-                    now - self._avg_update_ts > 1):
+            if xput_len < self.sma_window or now - self._avg_update_ts > 1:
                 self.avg = sum(self._xput) / len(self._xput)
                 self._avg_update_ts = now
 
     def update(self):
         pass
 
     def start(self):
         pass
 
     def clearln(self):
         if self.file and self.is_tty():
-            printMsg('\r\x1b[K', end='', file=self.file)
+            printMsg("\r\x1b[K", end="", file=self.file)
 
     def write(self, s):
         if self.file and self.is_tty():
             line = self.message + s.ljust(self._width)
-            printMsg('\r' + line, end='', file=self.file)
+            printMsg("\r" + line, end="", file=self.file)
             self._width = max(self._width, len(s))
             self.file.flush()
 
     def writeln(self, line):
         if self.file and self.is_tty():
             self.clearln()
-            printMsg(line, end='', file=self.file)
+            printMsg(line, end="", file=self.file)
             self.file.flush()
 
     def finish(self):
         if self.file and self.is_tty():
             printMsg(file=self.file)
             if self.hide_cursor:
-                printMsg(SHOW_CURSOR, end='', file=self.file)
+                printMsg(SHOW_CURSOR, end="", file=self.file)
 
     def is_tty(self):
         return self.file.isatty() if self.check_tty else True
 
     def next(self, n=1):
         now = monotonic()
         dt = now - self._ts
@@ -133,15 +133,15 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.finish()
 
 
 class Progress(Infinite):
     def __init__(self, *args, **kwargs):
         super(Progress, self).__init__(*args, **kwargs)
-        self.max = kwargs.get('max', 100)
+        self.max = kwargs.get("max", 100)
 
     @property
     def eta(self):
         return int(ceil(self.avg * self.remaining))
 
     @property
     def eta_td(self):
```

### Comparing `prot-3.8.6/src/prot/progress/bar.py` & `prot-3.9.0/src/prot/progress/bar.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,73 +19,73 @@
 import sys
 
 from . import Progress
 
 
 class Bar(Progress):
     width = 32
-    suffix = '%(index)d/%(max)d'
-    bar_prefix = ' |'
-    bar_suffix = '| '
-    empty_fill = ' '
-    fill = '#'
+    suffix = "%(index)d/%(max)d"
+    bar_prefix = " |"
+    bar_suffix = "| "
+    empty_fill = " "
+    fill = "#"
 
     def update(self):
         filled_length = int(self.width * self.progress)
         empty_length = self.width - filled_length
 
         message = self.message % self
         bar = self.fill * filled_length
         empty = self.empty_fill * empty_length
         suffix = self.suffix % self
-        line = ''.join([message, self.bar_prefix, bar, empty, self.bar_suffix,
-                        suffix])
+        line = "".join([message, self.bar_prefix, bar, empty, self.bar_suffix, suffix])
         self.writeln(line)
 
 
 class ChargingBar(Bar):
-    suffix = '%(percent)d%%'
-    bar_prefix = ' '
-    bar_suffix = ' '
-    empty_fill = '∙'
-    fill = '█'
+    suffix = "%(percent)d%%"
+    bar_prefix = " "
+    bar_suffix = " "
+    empty_fill = "∙"
+    fill = "█"
 
 
 class FillingSquaresBar(ChargingBar):
-    empty_fill = '▢'
-    fill = '▣'
+    empty_fill = "▢"
+    fill = "▣"
 
 
 class FillingCirclesBar(ChargingBar):
-    empty_fill = '◯'
-    fill = '◉'
+    empty_fill = "◯"
+    fill = "◉"
 
 
 class IncrementalBar(Bar):
-    if sys.platform.startswith('win'):
-        phases = (u' ', u'▌', u'█')
+    if sys.platform.startswith("win"):
+        phases = (" ", "▌", "█")
     else:
-        phases = (' ', '▏', '▎', '▍', '▌', '▋', '▊', '▉', '█')
+        phases = (" ", "▏", "▎", "▍", "▌", "▋", "▊", "▉", "█")
 
     def update(self):
         nphases = len(self.phases)
         filled_len = self.width * self.progress
-        nfull = int(filled_len)                      # Number of full chars
+        nfull = int(filled_len)  # Number of full chars
         phase = int((filled_len - nfull) * nphases)  # Phase of last char
-        nempty = self.width - nfull                  # Number of empty chars
+        nempty = self.width - nfull  # Number of empty chars
 
         message = self.message % self
         bar = self.phases[-1] * nfull
-        current = self.phases[phase] if phase > 0 else ''
+        current = self.phases[phase] if phase > 0 else ""
         empty = self.empty_fill * max(0, nempty - len(current))
         suffix = self.suffix % self
-        line = ''.join([message, self.bar_prefix, bar, current, empty,
-                        self.bar_suffix, suffix])
+        line = "".join(
+            [message, self.bar_prefix, bar, current, empty, self.bar_suffix, suffix]
+        )
         self.writeln(line)
 
 
 class PixelBar(IncrementalBar):
-    phases = ('⡀', '⡄', '⡆', '⡇', '⣇', '⣧', '⣷', '⣿')
+    phases = ("⡀", "⡄", "⡆", "⡇", "⣇", "⣧", "⣷", "⣿")
 
 
 class ShadyBar(IncrementalBar):
-    phases = (' ', '░', '▒', '▓', '█')
+    phases = (" ", "░", "▒", "▓", "█")
```

### Comparing `prot-3.8.6/src/prot/progress/counter.py` & `prot-3.9.0/src/prot/progress/counter.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 class Countdown(Progress):
     def update(self):
         self.write(str(self.remaining))
 
 
 class Stack(Progress):
-    phases = (' ', '▁', '▂', '▃', '▄', '▅', '▆', '▇', '█')
+    phases = (" ", "▁", "▂", "▃", "▄", "▅", "▆", "▇", "█")
 
     def update(self):
         nphases = len(self.phases)
         i = min(nphases - 1, int(self.progress * nphases))
         self.write(self.phases[i])
 
 
 class Pie(Stack):
-    phases = ('○', '◔', '◑', '◕', '●')
+    phases = ("○", "◔", "◑", "◕", "●")
```

### Comparing `prot-3.8.6/src/prot/progress/spinner.py` & `prot-3.9.0/src/prot/progress/spinner.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from __future__ import unicode_literals
 from . import Infinite
 
 
 class Spinner(Infinite):
-    phases = ('-', '\\', '|', '/')
+    phases = ("-", "\\", "|", "/")
     hide_cursor = True
 
     def update(self):
         i = self.index % len(self.phases)
         self.write(self.phases[i])
 
 
 class PieSpinner(Spinner):
-    phases = ['◷', '◶', '◵', '◴']
+    phases = ["◷", "◶", "◵", "◴"]
 
 
 class MoonSpinner(Spinner):
-    phases = ['◑', '◒', '◐', '◓']
+    phases = ["◑", "◒", "◐", "◓"]
 
 
 class LineSpinner(Spinner):
-    phases = ['⎺', '⎻', '⎼', '⎽', '⎼', '⎻']
+    phases = ["⎺", "⎻", "⎼", "⎽", "⎼", "⎻"]
 
 
 class PixelSpinner(Spinner):
-    phases = ['⣾', '⣷', '⣯', '⣟', '⡿', '⢿', '⣻', '⣽']
+    phases = ["⣾", "⣷", "⣯", "⣟", "⡿", "⢿", "⣻", "⣽"]
```

### Comparing `prot-3.8.6/src/prot/prompt/__init__.py` & `prot-3.9.0/src/prot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/application/__init__.py` & `prot-3.9.0/src/prot/prompt/application/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/application/application.py` & `prot-3.9.0/src/prot/prompt/application/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         on_invalidate: Optional[ApplicationEventHandler] = None,
         before_render: Optional[ApplicationEventHandler] = None,
         after_render: Optional[ApplicationEventHandler] = None,
         # I/O.
         input: Optional[Input] = None,
         output: Optional[Output] = None,
     ):
-
         # If `enable_page_navigation_bindings` is not specified, enable it in
         # case of full screen applications only. This can be overridden by the user.
         if enable_page_navigation_bindings is None:
             enable_page_navigation_bindings = Condition(lambda: self.full_screen)
 
         paste_mode = to_filter(paste_mode)
         mouse_support = to_filter(mouse_support)
@@ -475,15 +474,15 @@
             else:
                 schedule_redraw()
         else:
             schedule_redraw()
 
     @property
     def invalidated(self) -> bool:
-        " True when a redraw operation has been scheduled. "
+        "True when a redraw operation has been scheduled."
         return self._invalidated
 
     def _redraw(self, render_as_done: bool = False) -> None:
         """
         Render the command line again. (Not thread safe!) (From other threads,
         or if unsure, use :meth:`.Application.invalidate`.)
 
@@ -578,15 +577,15 @@
         # Erase, request position (when cursor is at the start position)
         # and redraw again. -- The order is important.
         self.renderer.erase(leave_alternate_screen=False)
         self._request_absolute_cursor_position()
         self._redraw()
 
     def _pre_run(self, pre_run: Optional[Callable[[], None]] = None) -> None:
-        " Called during `run`. "
+        "Called during `run`."
         if pre_run:
             pre_run()
 
         # Process registered "pre_run_callables" and clear list.
         for c in self.pre_run_callables:
             c()
         del self.pre_run_callables[:]
@@ -611,15 +610,15 @@
         :param set_exception_handler: When set, in case of an exception, go out
             of the alternate screen and hide the application, display the
             exception, and wait for the user to press ENTER.
         """
         assert not self._is_running, "Application is already running."
 
         async def _run_async() -> _AppResult:
-            " Coroutine. "
+            "Coroutine."
             loop = get_event_loop()
             f = loop.create_future()
             self.future = f  # XXX: make sure to set this before calling '_redraw'.
             self.loop = loop
             self.context = contextvars.copy_context()
 
             # Counter for cancelling 'flush' timeouts. Every time when a key is
@@ -880,25 +879,25 @@
             )
             self.output.flush()
 
         run_in_terminal(in_terminal)
 
     @overload
     def exit(self) -> None:
-        " Exit without arguments. "
+        "Exit without arguments."
 
     @overload
     def exit(self, *, result: _AppResult, style: str = "") -> None:
-        " Exit with `_AppResult`. "
+        "Exit with `_AppResult`."
 
     @overload
     def exit(
         self, *, exception: Union[BaseException, Type[BaseException]], style: str = ""
     ) -> None:
-        " Exit with exception. "
+        "Exit with exception."
 
     def exit(
         self,
         result: Optional[_AppResult] = None,
         exception: Optional[Union[BaseException, Type[BaseException]]] = None,
         style: str = "",
     ) -> None:
@@ -1021,15 +1020,15 @@
             style=style or self._merged_style,
             color_depth=self.color_depth,
             style_transformation=self.style_transformation,
         )
 
     @property
     def is_running(self) -> bool:
-        " `True` when the application is currently active/running. "
+        "`True` when the application is currently active/running."
         return self._is_running
 
     @property
     def is_done(self) -> bool:
         if self.future:
             return self.future.done()
         return False
@@ -1063,21 +1062,21 @@
         self.app = app
         self._cache: SimpleCache[
             Tuple[Window, FrozenSet[UIControl]], KeyBindingsBase
         ] = SimpleCache()
 
     @property
     def _version(self) -> Hashable:
-        """ Not needed - this object is not going to be wrapped in another
-        KeyBindings object. """
+        """Not needed - this object is not going to be wrapped in another
+        KeyBindings object."""
         raise NotImplementedError
 
     def bindings(self) -> List[Binding]:
-        """ Not needed - this object is not going to be wrapped in another
-        KeyBindings object. """
+        """Not needed - this object is not going to be wrapped in another
+        KeyBindings object."""
         raise NotImplementedError
 
     def _create_key_bindings(
         self, current_window: Window, other_controls: List[UIControl]
     ) -> KeyBindingsBase:
         """
         Create a `KeyBindings` object that merges the `KeyBindings` from the
@@ -1160,14 +1159,14 @@
 
     @key_bindings.add("enter")
     def _ok(event: E) -> None:
         event.app.exit()
 
     @key_bindings.add(Keys.Any)
     def _ignore(event: E) -> None:
-        " Disallow typing. "
+        "Disallow typing."
         pass
 
     session: PromptSession[None] = PromptSession(
         message=wait_text, key_bindings=key_bindings
     )
     await session.app.run_async()
```

### Comparing `prot-3.8.6/src/prot/prompt/application/current.py` & `prot-3.9.0/src/prot/prompt/application/current.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         explicitely.
     :param output: Use this as a default output.
     """
 
     def __init__(
         self, input: Optional["Input"] = None, output: Optional["Output"] = None
     ) -> None:
-
         self._input = input
         self._output = output
 
         # The application will be set dynamically by the `set_app` context
         # manager. This is called in the application itself.
         self.app: Optional["Application[Any]"] = None
```

### Comparing `prot-3.8.6/src/prot/prompt/application/dummy.py` & `prot-3.9.0/src/prot/prompt/application/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/application/run_in_terminal.py` & `prot-3.9.0/src/prot/prompt/application/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/auto_suggest.py` & `prot-3.9.0/src/prot/prompt/auto_suggest.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
 
 class ConditionalAutoSuggest(AutoSuggest):
     """
     Auto suggest that can be turned on and of according to a certain condition.
     """
 
     def __init__(self, auto_suggest: AutoSuggest, filter: Union[bool, Filter]) -> None:
-
         self.auto_suggest = auto_suggest
         self.filter = to_filter(filter)
 
     def get_suggestion(
         self, buffer: "Buffer", document: Document
     ) -> Optional[Suggestion]:
         if self.filter():
```

### Comparing `prot-3.8.6/src/prot/prompt/buffer.py` & `prot-3.9.0/src/prot/prompt/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     "indent",
     "unindent",
     "reshape_text",
 ]
 
 
 class EditReadOnlyBuffer(Exception):
-    " Attempt editing of read-only :class:`.Buffer`. "
+    "Attempt editing of read-only :class:`.Buffer`."
 
 
 class ValidationState(Enum):
-    " The validation state of a buffer. This is set after the validation. "
+    "The validation state of a buffer. This is set after the validation."
     VALID = "VALID"
     INVALID = "INVALID"
     UNKNOWN = "UNKNOWN"
 
 
 class CompletionState:
     """
@@ -73,15 +73,14 @@
 
     def __init__(
         self,
         original_document: "Document",
         completions: Optional[List["Completion"]] = None,
         complete_index: Optional[int] = None,
     ):
-
         #: Document as it was when the completion started.
         self.original_document = original_document
 
         #: List of all the current Completion instances which are possible at
         #: this point.
         self.completions = completions or []
 
@@ -145,15 +144,14 @@
     """
     For yank-last-arg/yank-nth-arg: Keep track of where we are in the history.
     """
 
     def __init__(
         self, history_position: int = 0, n: int = -1, previous_inserted_word: str = ""
     ):
-
         self.history_position = history_position
         self.previous_inserted_word = previous_inserted_word
         self.n = n
 
     def __repr__(self) -> str:
         return "%s(history_position=%r, n=%r, previous_inserted_word=%r)" % (
             self.__class__.__name__,
@@ -242,15 +240,14 @@
         multiline: FilterOrBool = True,
         on_text_changed: Optional[BufferEventHandler] = None,
         on_text_insert: Optional[BufferEventHandler] = None,
         on_cursor_position_changed: Optional[BufferEventHandler] = None,
         on_completions_changed: Optional[BufferEventHandler] = None,
         on_suggestion_set: Optional[BufferEventHandler] = None,
     ):
-
         # Accept both filters and booleans as input.
         enable_history_search = to_filter(enable_history_search)
         complete_while_typing = to_filter(complete_while_typing)
         validate_while_typing = to_filter(validate_while_typing)
         read_only = to_filter(read_only)
         multiline = to_filter(multiline)
 
@@ -381,15 +378,15 @@
         self._working_lines = self.history.get_strings()[:]
         self._working_lines.append(document.text)
         self.__working_index = len(self._working_lines) - 1
 
     # <getters/setters>
 
     def _set_text(self, value: str) -> bool:
-        """ set text at current working_index. Return whether it changed. """
+        """set text at current working_index. Return whether it changed."""
         working_index = self.working_index
         working_lines = self._working_lines
 
         original_value = working_lines[working_index]
         working_lines[working_index] = value
 
         # Return True when this text has been changed.
@@ -401,15 +398,15 @@
             # documents. >100,000 of lines.)
             return True
         elif value != original_value:
             return True
         return False
 
     def _set_cursor_position(self, value: int) -> bool:
-        """ Set cursor position. Return whether it changed. """
+        """Set cursor position. Return whether it changed."""
         original_position = self.__cursor_position
         self.__cursor_position = max(0, value)
 
         return value != original_position
 
     @property
     def text(self) -> str:
@@ -666,25 +663,25 @@
     def cursor_left(self, count: int = 1) -> None:
         self.cursor_position += self.document.get_cursor_left_position(count=count)
 
     def cursor_right(self, count: int = 1) -> None:
         self.cursor_position += self.document.get_cursor_right_position(count=count)
 
     def cursor_up(self, count: int = 1) -> None:
-        """ (for multiline edit). Move cursor to the previous line.  """
+        """(for multiline edit). Move cursor to the previous line."""
         original_column = self.preferred_column or self.document.cursor_position_col
         self.cursor_position += self.document.get_cursor_up_position(
             count=count, preferred_column=original_column
         )
 
         # Remember the original column for the next up/down movement.
         self.preferred_column = original_column
 
     def cursor_down(self, count: int = 1) -> None:
-        """ (for multiline edit). Move cursor to the next line.  """
+        """(for multiline edit). Move cursor to the next line."""
         original_column = self.preferred_column or self.document.cursor_position_col
         self.cursor_position += self.document.get_cursor_down_position(
             count=count, preferred_column=original_column
         )
 
         # Remember the original column for the next up/down movement.
         self.preferred_column = original_column
@@ -1659,29 +1656,28 @@
         @_only_one_at_a_time
         async def async_completer(
             select_first: bool = False,
             select_last: bool = False,
             insert_common_part: bool = False,
             complete_event: Optional[CompleteEvent] = None,
         ) -> None:
-
             document = self.document
             complete_event = complete_event or CompleteEvent(text_inserted=True)
 
             # Don't complete when we already have completions.
             if self.complete_state or not self.completer:
                 return
 
             # Create an empty CompletionState.
             complete_state = CompletionState(original_document=self.document)
             self.complete_state = complete_state
 
             def proceed() -> bool:
-                """ Keep retrieving completions. Input text has not yet changed
-                while generating completions. """
+                """Keep retrieving completions. Input text has not yet changed
+                while generating completions."""
                 return self.complete_state == complete_state
 
             async for completion in self.completer.get_completions_async(
                 document, complete_event
             ):
                 complete_state.completions.append(completion)
                 self.on_completions_changed.fire()
@@ -1859,15 +1855,15 @@
         finally:
             running = False
 
     return cast(_T, new_coroutine)
 
 
 class _Retry(Exception):
-    " Retry in `_only_one_at_a_time`. "
+    "Retry in `_only_one_at_a_time`."
 
 
 def indent(buffer: Buffer, from_row: int, to_row: int, count: int = 1) -> None:
     """
     Indent text of a :class:`.Buffer` object.
     """
     current_row = buffer.document.cursor_position_row
```

### Comparing `prot-3.8.6/src/prot/prompt/cache.py` & `prot-3.9.0/src/prot/prompt/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 key_to_remove = self._keys.popleft()
                 if key_to_remove in self._data:
                     del self._data[key_to_remove]
 
             return value
 
     def clear(self) -> None:
-        " Clear cache. "
+        "Clear cache."
         self._data = {}
         self._keys = deque()
 
 
 _K = TypeVar("_K", bound=Tuple)
 _V = TypeVar("_V")
```

### Comparing `prot-3.8.6/src/prot/prompt/clipboard/base.py` & `prot-3.9.0/src/prot/prompt/clipboard/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     :param text: string
     :param type: :class:`~prompt_toolkit.selection.SelectionType`
     """
 
     def __init__(
         self, text: str = "", type: SelectionType = SelectionType.CHARACTERS
     ) -> None:
-
         self.text = text
         self.type = type
 
 
 class Clipboard(metaclass=ABCMeta):
     """
     Abstract baseclass for clipboards.
```

### Comparing `prot-3.8.6/src/prot/prompt/clipboard/in_memory.py` & `prot-3.9.0/src/prot/prompt/clipboard/in_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     This implements a kill-ring, for Emacs mode.
     """
 
     def __init__(
         self, data: Optional[ClipboardData] = None, max_size: int = 60
     ) -> None:
-
         assert max_size >= 1
 
         self.max_size = max_size
         self._ring: Deque[ClipboardData] = deque()
 
         if data is not None:
             self.set_data(data)
```

### Comparing `prot-3.8.6/src/prot/prompt/clipboard/pyperclip.py` & `prot-3.9.0/src/prot/prompt/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/completion/__init__.py` & `prot-3.9.0/src/prot/prompt/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/completion/base.py` & `prot-3.9.0/src/prot/prompt/completion/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         text: str,
         start_position: int = 0,
         display: Optional[AnyFormattedText] = None,
         display_meta: Optional[AnyFormattedText] = None,
         style: str = "",
         selected_style: str = "",
     ) -> None:
-
         from prot.prompt.formatted_text import to_formatted_text
 
         self.text = text
         self.start_position = start_position
         self._display_meta = display_meta
 
         if display is None:
@@ -87,29 +86,29 @@
         )
 
     def __hash__(self) -> int:
         return hash((self.text, self.start_position, self.display, self._display_meta))
 
     @property
     def display_text(self) -> str:
-        " The 'display' field as plain text. "
+        "The 'display' field as plain text."
         from prot.prompt.formatted_text import fragment_list_to_text
 
         return fragment_list_to_text(self.display)
 
     @property
     def display_meta(self) -> StyleAndTextTuples:
-        " Return meta-text. (This is lazy when using a callable). "
+        "Return meta-text. (This is lazy when using a callable)."
         from prot.prompt.formatted_text import to_formatted_text
 
         return to_formatted_text(self._display_meta or "")
 
     @property
     def display_meta_text(self) -> str:
-        " The 'meta' field as plain text. "
+        "The 'meta' field as plain text."
         from prot.prompt.formatted_text import fragment_list_to_text
 
         return fragment_list_to_text(self.display_meta)
 
     def new_completion_from_position(self, position: int) -> "Completion":
         """
         (Only for internal use!)
@@ -290,15 +289,14 @@
         for completer in self.completers:
             for c in completer.get_completions(document, complete_event):
                 yield c
 
     async def get_completions_async(
         self, document: Document, complete_event: CompleteEvent
     ) -> AsyncGenerator[Completion, None]:
-
         # Get all completions from the other completers in a blocking way.
         for completer in self.completers:
             async for item in completer.get_completions_async(document, complete_event):
                 yield item
 
 
 def merge_completers(completers: Sequence[Completer]) -> _MergedCompleter:
@@ -310,14 +308,15 @@
 
 def get_common_complete_suffix(
     document: Document, completions: Sequence[Completion]
 ) -> str:
     """
     Return the common prefix for all completions.
     """
+
     # Take only completions that don't change the text before the cursor.
     def doesnt_change_before_cursor(completion: Completion) -> bool:
         end = completion.text[: -completion.start_position]
         return document.text_before_cursor.endswith(end)
 
     completions2 = [c for c in completions if doesnt_change_before_cursor(c)]
```

### Comparing `prot-3.8.6/src/prot/prompt/completion/filesystem.py` & `prot-3.9.0/src/prot/prompt/completion/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self,
         only_directories: bool = False,
         get_paths: Optional[Callable[[], List[str]]] = None,
         file_filter: Optional[Callable[[str], bool]] = None,
         min_input_len: int = 0,
         expanduser: bool = False,
     ) -> None:
-
         self.only_directories = only_directories
         self.get_paths = get_paths or (lambda: ["."])
         self.file_filter = file_filter or (lambda _: True)
         self.min_input_len = min_input_len
         self.expanduser = expanduser
 
     def get_completions(
```

### Comparing `prot-3.8.6/src/prot/prompt/completion/fuzzy_completer.py` & `prot-3.9.0/src/prot/prompt/completion/fuzzy_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     def __init__(
         self,
         completer: Completer,
         WORD: bool = False,
         pattern: Optional[str] = None,
         enable_fuzzy: FilterOrBool = True,
     ):
-
         assert pattern is None or pattern.startswith("^")
 
         self.completer = completer
         self.pattern = pattern
         self.WORD = WORD
         self.pattern = pattern
         self.enable_fuzzy = to_filter(enable_fuzzy)
@@ -73,15 +72,14 @@
         if self.WORD:
             return r"[^\s]+"
         return "^[a-zA-Z0-9_]*"
 
     def _get_fuzzy_completions(
         self, document: Document, complete_event: CompleteEvent
     ) -> Iterable[Completion]:
-
         word_before_cursor = document.get_word_before_cursor(
             pattern=re.compile(self._get_pattern())
         )
 
         # Get completions
         document2 = Document(
             text=document.text[: document.cursor_position - len(word_before_cursor)],
@@ -101,15 +99,15 @@
                 # Prefer the match, closest to the left, then shortest.
                 best = min(matches, key=lambda m: (m.start(), len(m.group(1))))
                 fuzzy_matches.append(
                     _FuzzyMatch(len(best.group(1)), best.start(), compl)
                 )
 
         def sort_key(fuzzy_match: "_FuzzyMatch") -> Tuple[int, int]:
-            " Sort by start position, then by the length of the match. "
+            "Sort by start position, then by the length of the match."
             return fuzzy_match.start_pos, fuzzy_match.match_length
 
         fuzzy_matches = sorted(fuzzy_matches, key=sort_key)
 
         for match in fuzzy_matches:
             # Include these completions, but set the correct `display`
             # attribute and `start_position`.
@@ -172,15 +170,14 @@
 
     def __init__(
         self,
         words: Union[List[str], Callable[[], List[str]]],
         meta_dict: Optional[Dict[str, str]] = None,
         WORD: bool = False,
     ) -> None:
-
         self.words = words
         self.meta_dict = meta_dict or {}
         self.WORD = WORD
 
         self.word_completer = WordCompleter(
             words=self.words, WORD=self.WORD, meta_dict=self.meta_dict
         )
```

### Comparing `prot-3.8.6/src/prot/prompt/completion/nested.py` & `prot-3.9.0/src/prot/prompt/completion/nested.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     If you need multiple levels, check out the `from_nested_dict` classmethod.
     """
 
     def __init__(
         self, options: Dict[str, Optional[Completer]], ignore_case: bool = True
     ) -> None:
-
         self.options = options
         self.ignore_case = ignore_case
 
     def __repr__(self) -> str:
         return "NestedCompleter(%r, ignore_case=%r)" % (self.options, self.ignore_case)
 
     @classmethod
```

### Comparing `prot-3.8.6/src/prot/prompt/completion/word_completer.py` & `prot-3.9.0/src/prot/prompt/completion/word_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         ignore_case: bool = False,
         meta_dict: Optional[Dict[str, str]] = None,
         WORD: bool = False,
         sentence: bool = False,
         match_middle: bool = False,
         pattern: Optional[Pattern[str]] = None,
     ) -> None:
-
         assert not (WORD and sentence)
 
         self.words = words
         self.ignore_case = ignore_case
         self.meta_dict = meta_dict or {}
         self.WORD = WORD
         self.sentence = sentence
@@ -64,15 +63,15 @@
                 WORD=self.WORD, pattern=self.pattern
             )
 
         if self.ignore_case:
             word_before_cursor = word_before_cursor.lower()
 
         def word_matches(word: str) -> bool:
-            """ True when the word before the cursor matches. """
+            """True when the word before the cursor matches."""
             if self.ignore_case:
                 word = word.lower()
 
             if self.match_middle:
                 return word_before_cursor in word
             else:
                 return word.startswith(word_before_cursor)
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/completers/system.py` & `prot-3.9.0/src/prot/prompt/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/__init__.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/compiler.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
     def __init__(
         self,
         root_node: Node,
         escape_funcs: Optional[EscapeFuncDict] = None,
         unescape_funcs: Optional[EscapeFuncDict] = None,
     ) -> None:
-
         self.root_node = root_node
         self.escape_funcs = escape_funcs or {}
         self.unescape_funcs = unescape_funcs or {}
 
         #: Dictionary that will map the regex names to Node instances.
         self._group_names_to_nodes: Dict[
             str, str
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/completion.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     :param completers: `dict` mapping variable names of the grammar to the
                        `Completer` instances to be used for each variable.
     """
 
     def __init__(
         self, compiled_grammar: _CompiledGrammar, completers: Dict[str, Completer]
     ) -> None:
-
         self.compiled_grammar = compiled_grammar
         self.completers = completers
 
     def get_completions(
         self, document: Document, complete_event: CompleteEvent
     ) -> Iterable[Completion]:
         m = self.compiled_grammar.match_prefix(document.text_before_cursor)
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/lexer.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     def __init__(
         self,
         compiled_grammar: _CompiledGrammar,
         default_style: str = "",
         lexers: Optional[Dict[str, Lexer]] = None,
     ) -> None:
-
         self.compiled_grammar = compiled_grammar
         self.default_style = default_style
         self.lexers = lexers or {}
 
     def _get_text_fragments(self, text: str) -> StyleAndTextTuples:
         m = self.compiled_grammar.match_prefix(text)
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/regex_parser.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/regex_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     """
     Takes a list of tokens from the tokenizer, and returns a parse tree.
     """
     # We add a closing brace because that represents the final pop of the stack.
     tokens: List[str] = [")"] + regex_tokens[::-1]
 
     def wrap(lst: List[Node]) -> Node:
-        """ Turn list into sequence when it contains several items. """
+        """Turn list into sequence when it contains several items."""
         if len(lst) == 1:
             return lst[0]
         else:
             return NodeSequence(lst)
 
     def _parse() -> Node:
         or_list: List[List[Node]] = []
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/regular_languages/validation.py` & `prot-3.9.0/src/prot/prompt/contrib/regular_languages/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     :param validators: `dict` mapping variable names of the grammar to the
                        `Validator` instances to be used for each variable.
     """
 
     def __init__(
         self, compiled_grammar: _CompiledGrammar, validators: Dict[str, Validator]
     ) -> None:
-
         self.compiled_grammar = compiled_grammar
         self.validators = validators
 
     def validate(self, document: Document) -> None:
         # Parse input document.
         # We use `match`, not `match_prefix`, because for validation, we want
         # the actual, unambiguous interpretation of the input.
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/ssh/server.py` & `prot-3.9.0/src/prot/prompt/contrib/ssh/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/contrib/telnet/protocol.py` & `prot-3.9.0/src/prot/prompt/contrib/telnet/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,38 +62,37 @@
     """
 
     def __init__(
         self,
         data_received_callback: Callable[[bytes], None],
         size_received_callback: Callable[[int, int], None],
     ) -> None:
-
         self.data_received_callback = data_received_callback
         self.size_received_callback = size_received_callback
 
         self._parser = self._parse_coroutine()
         self._parser.send(None)  # type: ignore
 
     def received_data(self, data: bytes) -> None:
         self.data_received_callback(data)
 
     def do_received(self, data: bytes) -> None:
-        """ Received telnet DO command. """
+        """Received telnet DO command."""
         logger.info("DO %r", data)
 
     def dont_received(self, data: bytes) -> None:
-        """ Received telnet DONT command. """
+        """Received telnet DONT command."""
         logger.info("DONT %r", data)
 
     def will_received(self, data: bytes) -> None:
-        """ Received telnet WILL command. """
+        """Received telnet WILL command."""
         logger.info("WILL %r", data)
 
     def wont_received(self, data: bytes) -> None:
-        """ Received telnet WONT command. """
+        """Received telnet WONT command."""
         logger.info("WONT %r", data)
 
     def command_received(self, command: bytes, data: bytes) -> None:
         if command == DO:
             self.do_received(data)
 
         elif command == DONT:
```

### Comparing `prot-3.8.6/src/prot/prompt/contrib/telnet/server.py` & `prot-3.9.0/src/prot/prompt/contrib/telnet/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         conn: socket.socket,
         addr: Tuple[str, int],
         interact: Callable[["TelnetConnection"], Awaitable[None]],
         server: "TelnetServer",
         encoding: str,
         style: Optional[BaseStyle],
     ) -> None:
-
         self.conn = conn
         self.addr = addr
         self.interact = interact
         self.server = server
         self.encoding = encoding
         self.style = style
         self._closed = False
@@ -130,19 +129,19 @@
         def get_size() -> Size:
             return self.size
 
         self.stdout = cast(TextIO, _ConnectionStdout(conn, encoding=encoding))
         self.vt100_output = Vt100_Output(self.stdout, get_size, write_binary=False)
 
         def data_received(data: bytes) -> None:
-            """ TelnetProtocolParser 'data_received' callback """
+            """TelnetProtocolParser 'data_received' callback"""
             self.vt100_input.send_bytes(data)
 
         def size_received(rows: int, columns: int) -> None:
-            """ TelnetProtocolParser 'size_received' callback """
+            """TelnetProtocolParser 'size_received' callback"""
             self.size = Size(rows=rows, columns=columns)
             get_app()._on_resize()
 
         self.parser = TelnetProtocolParser(data_received, size_received)
         self.context: Optional[contextvars.Context] = None
 
     async def run_application(self) -> None:
@@ -243,15 +242,14 @@
         self,
         host: str = "127.0.0.1",
         port: int = 23,
         interact: Callable[[TelnetConnection], Awaitable[None]] = _dummy_interact,
         encoding: str = "utf-8",
         style: Optional[BaseStyle] = None,
     ) -> None:
-
         self.host = host
         self.port = port
         self.interact = interact
         self.encoding = encoding
         self.style = style
         self._application_tasks: List[asyncio.Task] = []
```

### Comparing `prot-3.8.6/src/prot/prompt/document.py` & `prot-3.9.0/src/prot/prompt/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
     def __init__(
         self,
         text: str = "",
         cursor_position: Optional[int] = None,
         selection: Optional[SelectionState] = None,
     ) -> None:
-
         # Check cursor position. It can also be right after the end. (Where we
         # insert text.)
         assert cursor_position is None or cursor_position <= len(text), AssertionError(
             "cursor_position=%r, len_text=%r" % (cursor_position, len(text))
         )
 
         # By default, if no cursor position was given, make sure to put the
@@ -137,54 +136,54 @@
             self.text == other.text
             and self.cursor_position == other.cursor_position
             and self.selection == other.selection
         )
 
     @property
     def text(self) -> str:
-        " The document text. "
+        "The document text."
         return self._text
 
     @property
     def cursor_position(self) -> int:
-        " The document cursor position. "
+        "The document cursor position."
         return self._cursor_position
 
     @property
     def selection(self) -> Optional[SelectionState]:
-        " :class:`.SelectionState` object. "
+        ":class:`.SelectionState` object."
         return self._selection
 
     @property
     def current_char(self) -> str:
-        """ Return character under cursor or an empty string. """
+        """Return character under cursor or an empty string."""
         return self._get_char_relative_to_cursor(0) or ""
 
     @property
     def char_before_cursor(self) -> str:
-        """ Return character before the cursor or an empty string. """
+        """Return character before the cursor or an empty string."""
         return self._get_char_relative_to_cursor(-1) or ""
 
     @property
     def text_before_cursor(self) -> str:
         return self.text[: self.cursor_position :]
 
     @property
     def text_after_cursor(self) -> str:
         return self.text[self.cursor_position :]
 
     @property
     def current_line_before_cursor(self) -> str:
-        """ Text from the start of the line until the cursor. """
+        """Text from the start of the line until the cursor."""
         _, _, text = self.text_before_cursor.rpartition("\n")
         return text
 
     @property
     def current_line_after_cursor(self) -> str:
-        """ Text from the cursor until the end of the line. """
+        """Text from the cursor until the end of the line."""
         text, _, _ = self.text_after_cursor.partition("\n")
         return text
 
     @property
     def lines(self) -> List[str]:
         """
         Array of all the lines.
@@ -228,27 +227,27 @@
         """
         Array of the lines starting from the current line, until the last line.
         """
         return self.lines[self.cursor_position_row :]
 
     @property
     def line_count(self) -> int:
-        r""" Return the number of lines in this document. If the document ends
-        with a trailing \n, that counts as the beginning of a new line. """
+        r"""Return the number of lines in this document. If the document ends
+        with a trailing \n, that counts as the beginning of a new line."""
         return len(self.lines)
 
     @property
     def current_line(self) -> str:
-        """ Return the text on the line where the cursor is. (when the input
-        consists of just one line, it equals `text`. """
+        """Return the text on the line where the cursor is. (when the input
+        consists of just one line, it equals `text`."""
         return self.current_line_before_cursor + self.current_line_after_cursor
 
     @property
     def leading_whitespace_in_current_line(self) -> str:
-        """ The leading whitespace in the left margin of the current line.  """
+        """The leading whitespace in the left margin of the current line."""
         current_line = self.current_line
         length = len(current_line) - len(current_line.lstrip())
         return current_line[:length]
 
     def _get_char_relative_to_cursor(self, offset: int = 0) -> str:
         """
         Return character relative to cursor position, or empty string
@@ -337,20 +336,20 @@
         # Keep in range. (len(self.text) is included, because the cursor can be
         # right after the end of the text as well.)
         result = max(0, min(result, len(self.text)))
         return result
 
     @property
     def is_cursor_at_the_end(self) -> bool:
-        """ True when the cursor is at the end of the text. """
+        """True when the cursor is at the end of the text."""
         return self.cursor_position == len(self.text)
 
     @property
     def is_cursor_at_the_end_of_line(self) -> bool:
-        """ True when the cursor is at the end of this line. """
+        """True when the cursor is at the end of this line."""
         return self.current_char in ("\n", "")
 
     def has_match_at_current_position(self, sub: str) -> bool:
         """
         `True` when this substring is found at the cursor position.
         """
         return self.text.find(sub, self.cursor_position) == self.cursor_position
@@ -830,35 +829,35 @@
                 return self.find_enclosing_bracket_right(A, B, end_pos=end_pos) or 0
             elif self.current_char == B:
                 return self.find_enclosing_bracket_left(A, B, start_pos=start_pos) or 0
 
         return 0
 
     def get_start_of_document_position(self) -> int:
-        """ Relative position for the start of the document. """
+        """Relative position for the start of the document."""
         return -self.cursor_position
 
     def get_end_of_document_position(self) -> int:
-        """ Relative position for the end of the document. """
+        """Relative position for the end of the document."""
         return len(self.text) - self.cursor_position
 
     def get_start_of_line_position(self, after_whitespace: bool = False) -> int:
-        """ Relative position for the start of this line. """
+        """Relative position for the start of this line."""
         if after_whitespace:
             current_line = self.current_line
             return (
                 len(current_line)
                 - len(current_line.lstrip())
                 - self.cursor_position_col
             )
         else:
             return -len(self.current_line_before_cursor)
 
     def get_end_of_line_position(self) -> int:
-        """ Relative position for the end of this line. """
+        """Relative position for the end of this line."""
         return len(self.current_line_after_cursor)
 
     def last_non_blank_of_current_line_position(self) -> int:
         """
         Relative position for the last non blank character of this line.
         """
         return len(self.current_line.rstrip()) - self.cursor_position_col - 1
```

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/__init__.py` & `prot-3.9.0/src/prot/prompt/eventloop/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/async_context_manager.py` & `prot-3.9.0/src/prot/prompt/eventloop/async_context_manager.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/async_generator.py` & `prot-3.9.0/src/prot/prompt/eventloop/async_generator.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/dummy_contextvars.py` & `prot-3.9.0/src/prot/prompt/eventloop/dummy_contextvars.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/inputhook.py` & `prot-3.9.0/src/prot/prompt/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/utils.py` & `prot-3.9.0/src/prot/prompt/eventloop/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/eventloop/win32.py` & `prot-3.9.0/src/prot/prompt/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/filters/__init__.py` & `prot-3.9.0/src/prot/prompt/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/filters/app.py` & `prot-3.9.0/src/prot/prompt/filters/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,21 +146,21 @@
     True when the current buffer has been marked as multiline.
     """
     return get_app().current_buffer.multiline()
 
 
 @Condition
 def has_validation_error() -> bool:
-    " Current buffer has validation error.  "
+    "Current buffer has validation error."
     return get_app().current_buffer.validation_error is not None
 
 
 @Condition
 def has_arg() -> bool:
-    " Enable when the input processor has an 'arg'. "
+    "Enable when the input processor has an 'arg'."
     return get_app().key_processor.arg is not None
 
 
 @Condition
 def is_done() -> bool:
     """
     True when the CLI is returning, aborting or exiting.
@@ -311,25 +311,25 @@
         return False
 
     return app.vi_state.waiting_for_digraph
 
 
 @Condition
 def vi_recording_macro() -> bool:
-    " When recording a Vi macro. "
+    "When recording a Vi macro."
     app = get_app()
     if app.editing_mode != EditingMode.VI:
         return False
 
     return app.vi_state.recording_register is not None
 
 
 @Condition
 def emacs_mode() -> bool:
-    " When the Emacs bindings are active. "
+    "When the Emacs bindings are active."
     return get_app().editing_mode == EditingMode.EMACS
 
 
 @Condition
 def emacs_insert_mode() -> bool:
     app = get_app()
     if (
@@ -356,28 +356,28 @@
         app.current_buffer.selection_state
         and app.current_buffer.selection_state.shift_mode
     )
 
 
 @Condition
 def is_searching() -> bool:
-    " When we are searching. "
+    "When we are searching."
     app = get_app()
     return app.layout.is_searching
 
 
 @Condition
 def control_is_searchable() -> bool:
-    " When the current UIControl is searchable. "
+    "When the current UIControl is searchable."
     from prot.prompt.layout.controls import BufferControl
 
     control = get_app().layout.current_control
 
     return (
         isinstance(control, BufferControl) and control.search_buffer_control is not None
     )
 
 
 @Condition
 def vi_search_direction_reversed() -> bool:
-    " When the '/' and '?' key bindings for Vi-style searching have been reversed. "
+    "When the '/' and '?' key bindings for Vi-style searching have been reversed."
     return get_app().reverse_vi_search_direction()
```

### Comparing `prot-3.8.6/src/prot/prompt/filters/base.py` & `prot-3.9.0/src/prot/prompt/filters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         result = _AndList(filters)
         self[filters] = result
         return result
 
 
 class _OrCache(Dict[Tuple[Filter, Filter], "_OrList"]):
-    """ Cache for Or operation between filters. """
+    """Cache for Or operation between filters."""
 
     def __missing__(self, filters: Tuple[Filter, Filter]) -> Filter:
         a, b = filters
         assert isinstance(b, Filter), "Expecting filter, got %r" % b
 
         if isinstance(b, Always) or isinstance(a, Never):
             return b
@@ -91,15 +91,15 @@
 
         result = _OrList(filters)
         self[filters] = result
         return result
 
 
 class _InvertCache(Dict[Filter, "_Invert"]):
-    """ Cache for inversion operator. """
+    """Cache for inversion operator."""
 
     def __missing__(self, filter: Filter) -> Filter:
         result = _Invert(filter)
         self[filter] = result
         return result
```

### Comparing `prot-3.8.6/src/prot/prompt/filters/cli.py` & `prot-3.9.0/src/prot/prompt/filters/cli.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/filters/utils.py` & `prot-3.9.0/src/prot/prompt/filters/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/__init__.py` & `prot-3.9.0/src/prot/prompt/formatted_text/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/ansi.py` & `prot-3.9.0/src/prot/prompt/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/base.py` & `prot-3.9.0/src/prot/prompt/formatted_text/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     "is_formatted_text",
     "Template",
     "merge_formatted_text",
     "FormattedText",
 ]
 
 OneStyleAndTextTuple = Union[
-    Tuple[str, str], Tuple[str, str, Callable[[MouseEvent], None]],
+    Tuple[str, str],
+    Tuple[str, str, Callable[[MouseEvent], None]],
 ]
 
 # List of (style, text) tuples.
 StyleAndTextTuples = List[OneStyleAndTextTuple]
 
 
 if TYPE_CHECKING:
```

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/html.py` & `prot-3.9.0/src/prot/prompt/formatted_text/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 
         result: StyleAndTextTuples = []
         name_stack: List[str] = []
         fg_stack: List[str] = []
         bg_stack: List[str] = []
 
         def get_current_style() -> str:
-            " Build style string for current node. "
+            "Build style string for current node."
             parts = []
             if name_stack:
                 parts.append("class:" + ",".join(name_stack))
 
             if fg_stack:
                 parts.append("fg:" + fg_stack[-1])
             if bg_stack:
                 parts.append("bg:" + bg_stack[-1])
             return " ".join(parts)
 
         def process_node(node: Any) -> None:
-            " Process node recursively. "
+            "Process node recursively."
             for child in node.childNodes:
                 if child.nodeType == child.TEXT_NODE:
                     result.append((get_current_style(), child.data))
                 else:
                     add_to_name_stack = child.nodeName not in (
                         "#document",
                         "html-root",
```

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/pygments.py` & `prot-3.9.0/src/prot/prompt/formatted_text/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/formatted_text/utils.py` & `prot-3.9.0/src/prot/prompt/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/history.py` & `prot-3.9.0/src/prot/prompt/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def get_strings(self) -> List[str]:
         """
         Get the strings from the history that are loaded so far.
         """
         return self._loaded_strings
 
     def append_string(self, string: str) -> None:
-        " Add string to the history. "
+        "Add string to the history."
         self._loaded_strings.append(string)
         self.store_string(string)
 
     #
     # Implementation for specific backends.
     #
```

### Comparing `prot-3.8.6/src/prot/prompt/input/ansi_escape_sequences.py` & `prot-3.9.0/src/prot/prompt/input/ansi_escape_sequences.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/input/base.py` & `prot-3.9.0/src/prot/prompt/input/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,28 +44,28 @@
         """
         Flush the underlying parser. and return the pending keys.
         (Used for vt100 input.)
         """
         return []
 
     def flush(self) -> None:
-        " The event loop can call this when the input has to be flushed. "
+        "The event loop can call this when the input has to be flushed."
         pass
 
     @property
     def responds_to_cpr(self) -> bool:
         """
         `True` if the `Application` can expect to receive a CPR response from
         here.
         """
         return False
 
     @abstractproperty
     def closed(self) -> bool:
-        " Should be true when the input stream is closed. "
+        "Should be true when the input stream is closed."
         return False
 
     @abstractmethod
     def raw_mode(self) -> ContextManager[None]:
         """
         Context manager that turns the input into raw mode.
         """
@@ -87,15 +87,15 @@
     def detach(self) -> ContextManager[None]:
         """
         Return a context manager that makes sure that this input is not active
         in the current event loop.
         """
 
     def close(self) -> None:
-        " Close input. "
+        "Close input."
         pass
 
 
 class DummyInput(Input):
     """
     Input for use in a `DummyApplication`
     """
```

### Comparing `prot-3.8.6/src/prot/prompt/input/defaults.py` & `prot-3.9.0/src/prot/prompt/input/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/input/posix_pipe.py` & `prot-3.9.0/src/prot/prompt/input/posix_pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,25 +44,25 @@
     def responds_to_cpr(self) -> bool:
         return False
 
     def send_bytes(self, data: bytes) -> None:
         os.write(self._w, data)
 
     def send_text(self, data: str) -> None:
-        " Send text to the input. "
+        "Send text to the input."
         os.write(self._w, data.encode("utf-8"))
 
     def raw_mode(self) -> ContextManager[None]:
         return DummyContext()
 
     def cooked_mode(self) -> ContextManager[None]:
         return DummyContext()
 
     def close(self) -> None:
-        " Close pipe fds. "
+        "Close pipe fds."
         os.close(self._r)
         os.close(self._w)
 
         # We should assign `None` to 'self._r` and 'self._w',
         # The event loop still needs to know the the fileno for this input in order
         # to properly remove it from the selectors.
```

### Comparing `prot-3.8.6/src/prot/prompt/input/posix_utils.py` & `prot-3.9.0/src/prot/prompt/input/posix_utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/input/typeahead.py` & `prot-3.9.0/src/prot/prompt/input/typeahead.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/input/vt100.py` & `prot-3.9.0/src/prot/prompt/input/vt100.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         """
         Return a context manager that makes sure that this input is not active
         in the current event loop.
         """
         return _detached_input(self)
 
     def read_keys(self) -> List[KeyPress]:
-        " Read list of KeyPress. "
+        "Read list of KeyPress."
         # Read text from stdin.
         data = self.stdin_reader.read()
 
         # Pass it through our vt100 parser.
         self.vt100_parser.feed(data)
 
         # Return result.
```

### Comparing `prot-3.8.6/src/prot/prompt/input/vt100_parser.py` & `prot-3.9.0/src/prot/prompt/input/vt100_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # be shorter.)
 _cpr_response_prefix_re = re.compile("^" + re.escape("\x1b[") + r"[\d;]*\Z")
 
 _mouse_event_prefix_re = re.compile("^" + re.escape("\x1b[") + r"(<?[\d;]*|M.{0,2})\Z")
 
 
 class _Flush:
-    """ Helper object to indicate flush operation to the parser. """
+    """Helper object to indicate flush operation to the parser."""
 
     pass
 
 
 class _IsPrefixOfLongerMatchCache(Dict[str, bool]):
     """
     Dictionary that maps input sequences to a boolean indicating whether there is
```

### Comparing `prot-3.8.6/src/prot/prompt/input/win32.py` & `prot-3.9.0/src/prot/prompt/input/win32.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         if sys.stdin.isatty():
             self.handle = HANDLE(windll.kernel32.GetStdHandle(STD_INPUT_HANDLE))
         else:
             self._fdcon = os.open("CONIN$", os.O_RDWR | os.O_BINARY)
             self.handle = HANDLE(msvcrt.get_osfhandle(self._fdcon))
 
     def close(self) -> None:
-        " Close fdcon. "
+        "Close fdcon."
         if self._fdcon is not None:
             os.close(self._fdcon)
 
     def read(self) -> Iterable[KeyPress]:
         """
         Return a list of `KeyPress` instances. It won't return anything when
         there was nothing to read.  (This function doesn't block.)
```

### Comparing `prot-3.8.6/src/prot/prompt/input/win32_pipe.py` & `prot-3.9.0/src/prot/prompt/input/win32_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """
         The windows pipe doesn't depend on the file handle.
         """
         raise NotImplementedError
 
     @property
     def handle(self):
-        " The handle used for registering this pipe in the event loop. "
+        "The handle used for registering this pipe in the event loop."
         return self._event
 
     def attach(self, input_ready_callback: Callable) -> ContextManager[None]:
         """
         Return a context manager that makes this input active in the current
         event loop.
         """
@@ -74,15 +74,15 @@
         """
         Return a context manager that makes sure that this input is not active
         in the current event loop.
         """
         return detach_win32_input(self)
 
     def read_keys(self) -> List[KeyPress]:
-        " Read list of KeyPress. "
+        "Read list of KeyPress."
 
         # Return result.
         result = self._buffer
         self._buffer = []
 
         # Reset event.
         windll.kernel32.ResetEvent(self._event)
@@ -104,33 +104,33 @@
         return result
 
     @property
     def responds_to_cpr(self) -> bool:
         return False
 
     def send_bytes(self, data: bytes) -> None:
-        " Send bytes to the input. "
+        "Send bytes to the input."
         self.send_text(data.decode("utf-8", "ignore"))
 
     def send_text(self, text: str) -> None:
-        " Send text to the input. "
+        "Send text to the input."
         # Pass it through our vt100 parser.
         self.vt100_parser.feed(text)
 
         # Set event.
         windll.kernel32.SetEvent(self._event)
 
     def raw_mode(self) -> ContextManager[None]:
         return DummyContext()
 
     def cooked_mode(self) -> ContextManager[None]:
         return DummyContext()
 
     def close(self) -> None:
-        " Close pipe handles. "
+        "Close pipe handles."
         windll.kernel32.CloseHandle(self._event)
         self._closed = True
 
     def typeahead_hash(self) -> str:
         """
         This needs to be unique for every `PipeInput`.
         """
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/auto_suggest.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/basic.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     "load_basic_bindings",
 ]
 
 E = KeyPressEvent
 
 
 def if_no_repeat(event: E) -> bool:
-    """ Callable that returns True when the previous event was delivered to
-    another handler. """
+    """Callable that returns True when the previous event was delivered to
+    another handler."""
     return not event.is_repeat
 
 
 def load_basic_bindings() -> KeyBindings:
     key_bindings = KeyBindings()
     insert_mode = vi_insert_mode | emacs_insert_mode
     handle = key_bindings.add
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/completion.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,24 +128,29 @@
                         completion.style or ""
                     )
 
                     result.extend(to_formatted_text(completion.display, style=style))
 
                     # Add padding.
                     padding = max_compl_width - get_cwidth(completion.display_text)
-                    result.append((completion.style, " " * padding,))
+                    result.append(
+                        (
+                            completion.style,
+                            " " * padding,
+                        )
+                    )
                 except IndexError:
                     pass
             result.append(("", "\n"))
 
         app.print_text(to_formatted_text(result, "class:readline-like-completions"))
 
     # User interaction through an application generator function.
     async def run_compl() -> None:
-        " Coroutine. "
+        "Coroutine."
         async with in_terminal(render_cli_done=True):
             if len(completions) > completions_per_page:
                 # Ask confirmation if it doesn't fit on the screen.
                 confirm = await create_confirm_session(
                     "Display all {} possibilities?".format(len(completions)),
                 ).prompt_async()
 
@@ -194,10 +199,10 @@
     @bindings.add("Q")
     @bindings.add(Keys.ControlC)
     def _no(event: E) -> None:
         event.app.exit(result=False)
 
     @bindings.add(Keys.Any)
     def _ignore(event: E) -> None:
-        " Disable inserting of text. "
+        "Disable inserting of text."
 
     return PromptSession(message, key_bindings=bindings, erase_when_done=True)
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/cpr.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/cpr.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/emacs.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/emacs.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,20 +101,20 @@
 
     handle("c-x", "(")(get_by_name("start-kbd-macro"))
     handle("c-x", ")")(get_by_name("end-kbd-macro"))
     handle("c-x", "e")(get_by_name("call-last-kbd-macro"))
 
     @handle("c-n")
     def _next(event: E) -> None:
-        " Next line. "
+        "Next line."
         event.current_buffer.auto_down()
 
     @handle("c-p")
     def _prev(event: E) -> None:
-        " Previous line. "
+        "Previous line."
         event.current_buffer.auto_up(count=event.arg)
 
     def handle_digit(c: str) -> None:
         """
         Handle input of arguments.
         The first number needs to be preceded by escape.
         """
@@ -125,16 +125,15 @@
             event.append_to_arg_count(c)
 
     for c in "0123456789":
         handle_digit(c)
 
     @handle("escape", "-", filter=~has_arg)
     def _meta_dash(event: E) -> None:
-        """
-        """
+        """ """
         if event._arg is None:
             event.append_to_arg_count("-")
 
     @handle("-", filter=Condition(lambda: get_app().key_processor.arg == "-"))
     def _dash(event: E) -> None:
         """
         When '-' is typed again, after exactly '-' has been given as an
@@ -165,32 +164,32 @@
             match = buff.document.find(char, in_current_line=True, count=count)
 
         if match is not None:
             buff.cursor_position += match
 
     @handle("c-]", Keys.Any)
     def _goto_char(event: E) -> None:
-        " When Ctl-] + a character is pressed. go to that character. "
+        "When Ctl-] + a character is pressed. go to that character."
         # Also named 'character-search'
         character_search(event.current_buffer, event.data, event.arg)
 
     @handle("escape", "c-]", Keys.Any)
     def _goto_char_backwards(event: E) -> None:
-        " Like Ctl-], but backwards. "
+        "Like Ctl-], but backwards."
         # Also named 'character-search-backward'
         character_search(event.current_buffer, event.data, -event.arg)
 
     @handle("escape", "a")
     def _prev_sentence(event: E) -> None:
-        " Previous sentence. "
+        "Previous sentence."
         # TODO:
 
     @handle("escape", "e")
     def _end_of_sentence(event: E) -> None:
-        " Move to end of sentence. "
+        "Move to end of sentence."
         # TODO:
 
     @handle("escape", "t", filter=insert_mode)
     def _swap_characters(event: E) -> None:
         """
         Swap the last two words before the cursor.
         """
@@ -378,24 +377,24 @@
     )
     handle("/", filter=is_read_only & vi_search_direction_reversed)(
         search.start_reverse_incremental_search
     )
 
     @handle("n", filter=is_read_only)
     def _jump_next(event: E) -> None:
-        " Jump to next match. "
+        "Jump to next match."
         event.current_buffer.apply_search(
             event.app.current_search_state,
             include_current_position=False,
             count=event.arg,
         )
 
     @handle("N", filter=is_read_only)
     def _jump_prev(event: E) -> None:
-        " Jump to previous match. "
+        "Jump to previous match."
         event.current_buffer.apply_search(
             ~event.app.current_search_state,
             include_current_position=False,
             count=event.arg,
         )
 
     return ConditionalKeyBindings(key_bindings, emacs_mode)
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/mouse.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/named_commands.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/named_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 def register(name: str) -> Callable[[_T], _T]:
     """
     Store handler in the `_readline_commands` dictionary.
     """
 
     def decorator(handler: _T) -> _T:
-        " `handler` is a callable or Binding. "
+        "`handler` is a callable or Binding."
         if isinstance(handler, Binding):
             _readline_commands[name] = handler
         else:
             _readline_commands[name] = key_binding()(cast(_Handler, handler))
 
         return handler
 
@@ -111,15 +111,15 @@
     """
     buff = event.current_buffer
     buff.cursor_position += buff.document.get_cursor_right_position(count=event.arg)
 
 
 @register("backward-char")
 def backward_char(event: E) -> None:
-    " Move back a character. "
+    "Move back a character."
     buff = event.current_buffer
     buff.cursor_position += buff.document.get_cursor_left_position(count=event.arg)
 
 
 @register("forward-word")
 def forward_word(event: E) -> None:
     """
@@ -202,15 +202,15 @@
 
 
 @register("end-of-history")
 def end_of_history(event: E) -> None:
     """
     Move to the end of the input history, i.e., the line currently being entered.
     """
-    event.current_buffer.history_forward(count=10 ** 100)
+    event.current_buffer.history_forward(count=10**100)
     buff = event.current_buffer
     buff.go_to_history(len(buff._working_lines) - 1)
 
 
 @register("reverse-search-history")
 def reverse_search_history(event: E) -> None:
     """
@@ -571,14 +571,15 @@
 
 
 @register("print-last-kbd-macro")
 def print_last_kbd_macro(event: E) -> None:
     """
     Print the last keyboard macro.
     """
+
     # TODO: Make the format suitable for the inputrc file.
     def print_macro() -> None:
         macro = event.app.emacs_state.macro
         if macro:
             for k in macro:
                 printMsg(k)
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/open_in_editor.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/open_in_editor.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 
 def load_open_in_editor_bindings() -> KeyBindingsBase:
     """
     Load both the Vi and emacs key bindings for handling edit-and-execute-command.
     """
     return merge_key_bindings(
-        [load_emacs_open_in_editor_bindings(), load_vi_open_in_editor_bindings(),]
+        [
+            load_emacs_open_in_editor_bindings(),
+            load_vi_open_in_editor_bindings(),
+        ]
     )
 
 
 def load_emacs_open_in_editor_bindings() -> KeyBindings:
     """
     Pressing C-X C-E will open the buffer in an external editor.
     """
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/page_navigation.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/page_navigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     Load both the Vi and Emacs bindings for page navigation.
     """
     # Only enable when a `Buffer` is focused, otherwise, we would catch keys
     # when another widget is focused (like for instance `c-d` in a
     # ptterm.Terminal).
     return ConditionalKeyBindings(
         merge_key_bindings(
-            [load_emacs_page_navigation_bindings(), load_vi_page_navigation_bindings(),]
+            [
+                load_emacs_page_navigation_bindings(),
+                load_vi_page_navigation_bindings(),
+            ]
         ),
         buffer_has_focus,
     )
 
 
 def load_emacs_page_navigation_bindings() -> KeyBindingsBase:
     """
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/scroll.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/search.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/bindings/vi.py` & `prot-3.9.0/src/prot/prompt/key_binding/bindings/vi.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     Return struct for functions wrapped in ``text_object``.
     Both `start` and `end` are relative to the current cursor position.
     """
 
     def __init__(
         self, start: int, end: int = 0, type: TextObjectType = TextObjectType.EXCLUSIVE
     ):
-
         self.start = start
         self.end = end
         self.type = type
 
     @property
     def selection_type(self) -> SelectionType:
         if self.type == TextObjectType.LINEWISE:
@@ -482,16 +481,16 @@
         )
 
     @handle("backspace", filter=vi_navigation_mode)
     def _go_left(event: E) -> None:
         """
         In navigation-mode, move cursor.
         """
-        event.current_buffer.cursor_position += event.current_buffer.document.get_cursor_left_position(
-            count=event.arg
+        event.current_buffer.cursor_position += (
+            event.current_buffer.document.get_cursor_left_position(count=event.arg)
         )
 
     @handle("c-n", filter=vi_insert_mode)
     def _complete_next(event: E) -> None:
         b = event.current_buffer
 
         if b.complete_state:
@@ -669,16 +668,18 @@
     @handle("i", filter=vi_navigation_mode & ~is_read_only)
     def _i(event: E) -> None:
         event.app.vi_state.input_mode = InputMode.INSERT
 
     @handle("I", filter=vi_navigation_mode & ~is_read_only)
     def _I(event: E) -> None:
         event.app.vi_state.input_mode = InputMode.INSERT
-        event.current_buffer.cursor_position += event.current_buffer.document.get_start_of_line_position(
-            after_whitespace=True
+        event.current_buffer.cursor_position += (
+            event.current_buffer.document.get_start_of_line_position(
+                after_whitespace=True
+            )
         )
 
     @Condition
     def in_block_selection() -> bool:
         buff = get_app().current_buffer
         return bool(
             buff.selection_state and buff.selection_state.type == SelectionType.BLOCK
@@ -1309,15 +1310,15 @@
         """
         start = event.current_buffer.document.start_of_paragraph()
         end = event.current_buffer.document.end_of_paragraph(count=event.arg)
         return TextObject(start, end)
 
     @text_object("^")
     def _start_of_line(event: E) -> TextObject:
-        """ 'c^', 'd^' and '^': Soft start of line, after whitespace. """
+        """'c^', 'd^' and '^': Soft start of line, after whitespace."""
         return TextObject(
             event.current_buffer.document.get_start_of_line_position(
                 after_whitespace=True
             )
         )
 
     @text_object("0")
@@ -2164,15 +2165,15 @@
 def load_vi_search_bindings() -> KeyBindingsBase:
     key_bindings = KeyBindings()
     handle = key_bindings.add
     from . import search
 
     @Condition
     def search_buffer_is_empty() -> bool:
-        " Returns True when the search buffer is empty. "
+        "Returns True when the search buffer is empty."
         return get_app().current_buffer.text == ""
 
     # Vi-style forward search.
     handle(
         "/",
         filter=(vi_navigation_mode | vi_selection_mode) & ~vi_search_direction_reversed,
     )(search.start_forward_incremental_search)
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/defaults.py` & `prot-3.9.0/src/prot/prompt/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/digraphs.py` & `prot-3.9.0/src/prot/prompt/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/emacs_state.py` & `prot-3.9.0/src/prot/prompt/key_binding/emacs_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         self.current_recording: Optional[List[KeyPress]] = None
 
     def reset(self) -> None:
         self.current_recording = None
 
     @property
     def is_recording(self) -> bool:
-        " Tell whether we are recording a macro. "
+        "Tell whether we are recording a macro."
         return self.current_recording is not None
 
     def start_macro(self) -> None:
-        " Start recording macro. "
+        "Start recording macro."
         self.current_recording = []
 
     def end_macro(self) -> None:
-        " End recording macro. "
+        "End recording macro."
         self.macro = self.current_recording
         self.current_recording = None
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/key_bindings.py` & `prot-3.9.0/src/prot/prompt/key_binding/key_bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,22 +506,21 @@
     :param registries: List of :class:`.KeyBindings` objects.
     :param filter: :class:`~prompt_toolkit.filters.Filter` object.
     """
 
     def __init__(
         self, key_bindings: KeyBindingsBase, filter: FilterOrBool = True
     ) -> None:
-
         _Proxy.__init__(self)
 
         self.key_bindings = key_bindings
         self.filter = to_filter(filter)
 
     def _update_cache(self) -> None:
-        " If the original key bindings was changed. Update our copy version. "
+        "If the original key bindings was changed. Update our copy version."
         expected_version = self.key_bindings._version
 
         if self._last_version != expected_version:
             bindings2 = KeyBindings()
 
             # Copy all bindings from `self.key_bindings`, adding our condition.
             for b in self.key_bindings.bindings:
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/key_processor.py` & `prot-3.9.0/src/prot/prompt/key_binding/key_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,24 +397,24 @@
         app = get_app()
         timeout = app.timeoutlen
 
         if timeout is None:
             return
 
         async def wait() -> None:
-            " Wait for timeout. "
+            "Wait for timeout."
             # This sleep can be cancelled. In that case we don't flush.
             await sleep(timeout)
 
             if len(self.key_buffer) > 0:
                 # (No keys pressed in the meantime.)
                 flush_keys()
 
         def flush_keys() -> None:
-            " Flush keys. "
+            "Flush keys."
             self.feed(_Flush)
             self.process_keys()
 
         # Automatically flush keys.
         if self._flush_wait_task:
             self._flush_wait_task.cancel()
         self._flush_wait_task = app.create_background_task(wait())
@@ -435,15 +435,14 @@
         self,
         key_processor_ref: "weakref.ReferenceType[KeyProcessor]",
         arg: Optional[str],
         key_sequence: List[KeyPress],
         previous_key_sequence: List[KeyPress],
         is_repeat: bool,
     ) -> None:
-
         self._key_processor_ref = key_processor_ref
         self.key_sequence = key_sequence
         self.previous_key_sequence = previous_key_sequence
 
         #: True when the previous key sequence was handled by the same handler.
         self.is_repeat = is_repeat
 
@@ -522,9 +521,9 @@
         else:
             result = "%s%s" % (current, data)
 
         self.key_processor.arg = result
 
     @property
     def cli(self) -> "Application":
-        " For backward-compatibility. "
+        "For backward-compatibility."
         return self.app
```

### Comparing `prot-3.8.6/src/prot/prompt/key_binding/vi_state.py` & `prot-3.9.0/src/prot/prompt/key_binding/vi_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,20 @@
         # This happens when control-o has been pressed in insert or replace
         # mode. The user can now do one navigation action and we'll return back
         # to insert/replace.
         self.temporary_navigation_mode = False
 
     @property
     def input_mode(self) -> InputMode:
-        " Get `InputMode`. "
+        "Get `InputMode`."
         return self.__input_mode
 
     @input_mode.setter
     def input_mode(self, value: InputMode) -> None:
-        " Set `InputMode`. "
+        "Set `InputMode`."
         if value == InputMode.NAVIGATION:
             self.waiting_for_digraph = False
             self.operator_func = None
             self.operator_arg = None
 
         self.__input_mode = value
```

### Comparing `prot-3.8.6/src/prot/prompt/keys.py` & `prot-3.9.0/src/prot/prompt/keys.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/layout/__init__.py` & `prot-3.9.0/src/prot/prompt/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/layout/containers.py` & `prot-3.9.0/src/prot/prompt/layout/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,30 +166,30 @@
             ...
 
 
 AnyContainer = Union[Container, "MagicContainer"]
 
 
 def _window_too_small() -> "Window":
-    " Create a `Window` that displays the 'Window too small' text. "
+    "Create a `Window` that displays the 'Window too small' text."
     return Window(
         FormattedTextControl(text=[("class:window-too-small", " Window too small... ")])
     )
 
 
 class VerticalAlign(Enum):
-    " Alignment for `HSplit`. "
+    "Alignment for `HSplit`."
     TOP = "TOP"
     CENTER = "CENTER"
     BOTTOM = "BOTTOM"
     JUSTIFY = "JUSTIFY"
 
 
 class HorizontalAlign(Enum):
-    " Alignment for `VSplit`. "
+    "Alignment for `VSplit`."
     LEFT = "LEFT"
     CENTER = "CENTER"
     RIGHT = "RIGHT"
     JUSTIFY = "JUSTIFY"
 
 
 class _Split(Container):
@@ -207,15 +207,14 @@
         width: AnyDimension = None,
         height: AnyDimension = None,
         z_index: Optional[int] = None,
         modal: bool = False,
         key_bindings: Optional[KeyBindingsBase] = None,
         style: Union[str, Callable[[], str]] = "",
     ) -> None:
-
         self.children = [to_container(c) for c in children]
         self.window_too_small = window_too_small or _window_too_small()
         self.padding = padding
         self.padding_char = padding_char
         self.padding_style = padding_style
 
         self.width = width
@@ -281,15 +280,14 @@
         width: AnyDimension = None,
         height: AnyDimension = None,
         z_index: Optional[int] = None,
         modal: bool = False,
         key_bindings: Optional[KeyBindingsBase] = None,
         style: Union[str, Callable[[], str]] = "",
     ) -> None:
-
         super().__init__(
             children=children,
             window_too_small=window_too_small,
             padding=padding,
             padding_char=padding_char,
             padding_style=padding_style,
             width=width,
@@ -518,15 +516,14 @@
         width: AnyDimension = None,
         height: AnyDimension = None,
         z_index: Optional[int] = None,
         modal: bool = False,
         key_bindings: Optional[KeyBindingsBase] = None,
         style: Union[str, Callable[[], str]] = "",
     ) -> None:
-
         super().__init__(
             children=children,
             window_too_small=window_too_small,
             padding=padding,
             padding_char=padding_char,
             padding_style=padding_style,
             width=width,
@@ -761,15 +758,14 @@
         content: AnyContainer,
         floats: List["Float"],
         modal: bool = False,
         key_bindings: Optional[KeyBindingsBase] = None,
         style: Union[str, Callable[[], str]] = "",
         z_index: Optional[int] = None,
     ) -> None:
-
         self.content = to_container(content)
         self.floats = floats
 
         self.modal = modal
         self.key_bindings = key_bindings
         self.style = style
         self.z_index = z_index
@@ -818,15 +814,15 @@
             # position is not drawn yet, because it's a Float itself, we have
             # to postpone this calculation. (This is a work-around, but good
             # enough for now.)
             postpone = fl.xcursor is not None or fl.ycursor is not None
 
             if postpone:
                 new_z_index = (
-                    number + 10 ** 8
+                    number + 10**8
                 )  # Draw as late as possible, but keep the order.
                 screen.draw_with_z_index(
                     z_index=new_z_index,
                     draw_func=partial(
                         self._draw_float,
                         fl,
                         screen,
@@ -854,15 +850,15 @@
         screen: Screen,
         mouse_handlers: MouseHandlers,
         write_position: WritePosition,
         style: str,
         erase_bg: bool,
         z_index: Optional[int],
     ) -> None:
-        " Draw a single Float. "
+        "Draw a single Float."
         # When a menu_position was given, use this instead of the cursor
         # position. (These cursor positions are absolute, translate again
         # relative to the write_position.)
         # Note: This should be inside the for-loop, because one float could
         #       set the cursor position to be used for the next one.
         cpos = screen.get_menu_position(
             fl.attach_to_window or get_app().layout.current_window
@@ -1061,15 +1057,14 @@
         ycursor: bool = False,
         attach_to_window: Optional[AnyContainer] = None,
         hide_when_covering_content: bool = False,
         allow_cover_cursor: bool = False,
         z_index: int = 1,
         transparent: bool = False,
     ):
-
         assert z_index >= 1
 
         self.left = left
         self.right = right
         self.top = top
         self.bottom = bottom
 
@@ -1141,15 +1136,14 @@
         configured_scroll_offsets: "ScrollOffsets",
         visible_line_to_row_col: Dict[int, Tuple[int, int]],
         rowcol_to_yx: Dict[Tuple[int, int], Tuple[int, int]],
         x_offset: int,
         y_offset: int,
         wrap_lines: bool,
     ) -> None:
-
         self.window = window
         self.ui_content = ui_content
         self.vertical_scroll = vertical_scroll
         self.window_width = window_width  # Width without margins.
         self.window_height = window_height
 
         self.configured_scroll_offsets = configured_scroll_offsets
@@ -1334,15 +1328,14 @@
     def __init__(
         self,
         top: Union[int, Callable[[], int]] = 0,
         bottom: Union[int, Callable[[], int]] = 0,
         left: Union[int, Callable[[], int]] = 0,
         right: Union[int, Callable[[], int]] = 0,
     ) -> None:
-
         self._top = top
         self._bottom = bottom
         self._left = left
         self._right = right
 
     @property
     def top(self) -> int:
@@ -1482,15 +1475,14 @@
             None, List[ColorColumn], Callable[[], List[ColorColumn]]
         ] = None,
         align: Union[WindowAlign, Callable[[], WindowAlign]] = WindowAlign.LEFT,
         style: Union[str, Callable[[], str]] = "",
         char: Union[None, str, Callable[[], str]] = None,
         get_line_prefix: Optional[GetLinePrefixCallable] = None,
     ) -> None:
-
         self.allow_scroll_beyond_bottom = to_filter(allow_scroll_beyond_bottom)
         self.always_hide_cursor = to_filter(always_hide_cursor)
         self.wrap_lines = to_filter(wrap_lines)
         self.cursorline = to_filter(cursorline)
         self.cursorcolumn = to_filter(cursorcolumn)
 
         self.content = content or DummyControl()
@@ -1543,14 +1535,15 @@
         self.render_info: Optional[WindowRenderInfo] = None
 
     def _get_margin_width(self, margin: Margin) -> int:
         """
         Return the width for this margin.
         (Calculate only once per render time.)
         """
+
         # Margin.get_width, needs to have a UIContent instance.
         def get_ui_content() -> UIContent:
             return self._get_ui_content(width=0, height=0)
 
         def get_width() -> int:
             return margin.get_width(get_ui_content)
 
@@ -1567,16 +1560,16 @@
 
     def preferred_width(self, max_available_width: int) -> Dimension:
         """
         Calculate the preferred width for this window.
         """
 
         def preferred_content_width() -> Optional[int]:
-            """ Content width: is only calculated if no exact width for the
-            window was given. """
+            """Content width: is only calculated if no exact width for the
+            window was given."""
             if self.ignore_content_width():
                 return None
 
             # Calculate the width of the margin.
             total_margin_width = self._get_total_margin_width()
 
             # Window of the content. (Can be `None`.)
@@ -1598,16 +1591,16 @@
 
     def preferred_height(self, width: int, max_available_height: int) -> Dimension:
         """
         Calculate the preferred height for this window.
         """
 
         def preferred_content_height() -> Optional[int]:
-            """ Content height: is only calculated if no exact height for the
-            window was given. """
+            """Content height: is only calculated if no exact height for the
+            window was given."""
             if self.ignore_content_height():
                 return None
 
             total_margin_width = self._get_total_margin_width()
             wrap_lines = self.wrap_lines()
 
             return self.content.preferred_height(
@@ -1680,15 +1673,15 @@
         def get_content() -> UIContent:
             return self.content.create_content(width=width, height=height)
 
         key = (get_app().render_counter, width, height)
         return self._ui_content_cache.get(key, get_content)
 
     def _get_digraph_char(self) -> Optional[str]:
-        " Return `False`, or the Digraph symbol to be used. "
+        "Return `False`, or the Digraph symbol to be used."
         app = get_app()
         if app.quoted_insert:
             return "^"
         if app.vi_state.waiting_for_digraph:
             if app.vi_state.digraph_symbol1:
                 return app.vi_state.digraph_symbol1
             return "?"
@@ -1797,16 +1790,16 @@
             y_offset=y_offset,
             wrap_lines=wrap_lines,
         )
         self.render_info = render_info
 
         # Set mouse handlers.
         def mouse_handler(mouse_event: MouseEvent) -> None:
-            """ Wrapper around the mouse_handler of the `UIControl` that turns
-            screen coordinates into line coordinates. """
+            """Wrapper around the mouse_handler of the `UIControl` that turns
+            screen coordinates into line coordinates."""
             # Don't handle mouse events outside of the current modal part of
             # the UI.
             if self not in get_app().layout.walk_through_modal_area():
                 return
 
             # Find row/col position first.
             yx_to_rowcol = {v: k for k, v in rowcol_to_yx.items()}
@@ -1858,15 +1851,15 @@
             handler=mouse_handler,
         )
 
         # Render and copy margins.
         move_x = 0
 
         def render_margin(m: Margin, width: int) -> UIContent:
-            " Render margin. Return `Screen`. "
+            "Render margin. Return `Screen`."
             # Retrieve margin fragments.
             fragments = m.create_margin(render_info, width, write_position.height)
 
             # Turn it into a UIContent object.
             # already rendered those fragments using this size.)
             return FormattedTextControl(fragments).create_content(
                 width + 1, write_position.height
@@ -2076,15 +2069,15 @@
                 lineno += 1
                 y += 1
             return y
 
         copy()
 
         def cursor_pos_to_screen_pos(row: int, col: int) -> Point:
-            " Translate row/col from UIContent to real Screen coordinates. "
+            "Translate row/col from UIContent to real Screen coordinates."
             try:
                 y, x = rowcol_to_yx[row, col]
             except KeyError:
                 # Normally this should never happen. (It is a bug, if it happens.)
                 # But to be sure, return (0, 0)
                 return Point(x=0, y=0)
 
@@ -2160,15 +2153,14 @@
                 row = screen.data_buffer[y]
                 for x in range(wp.xpos, wp.xpos + wp.width):
                     row[x] = char_obj
 
     def _apply_style(
         self, new_screen: Screen, write_position: WritePosition, parent_style: str
     ) -> None:
-
         # Apply `self.style`.
         style = parent_style + " " + to_str(self.style)
 
         new_screen.fill_area(write_position, style=style, after=False)
 
         # Apply the 'last-line' class to the last line of each Window. This can
         # be used to apply an 'underline' to the user control.
@@ -2440,15 +2432,15 @@
             current_scroll: int,
             scroll_offset_start: int,
             scroll_offset_end: int,
             cursor_pos: int,
             window_size: int,
             content_size: int,
         ) -> int:
-            " Scrolling algorithm. Used for both horizontal and vertical scrolling. "
+            "Scrolling algorithm. Used for both horizontal and vertical scrolling."
             # Calculate the scroll offset to apply.
             # This can obviously never be more than have the screen size. Also, when the
             # cursor appears at the top or bottom, we don't apply the offset.
             scroll_offset_start = int(
                 min(scroll_offset_start, window_size / 2, cursor_pos)
             )
             scroll_offset_end = int(
@@ -2524,28 +2516,28 @@
         """
         if mouse_event.event_type == MouseEventType.SCROLL_DOWN:
             self._scroll_down()
         elif mouse_event.event_type == MouseEventType.SCROLL_UP:
             self._scroll_up()
 
     def _scroll_down(self) -> None:
-        " Scroll window down. "
+        "Scroll window down."
         info = self.render_info
 
         if info is None:
             return
 
         if self.vertical_scroll < info.content_height - info.window_height:
             if info.cursor_position.y <= info.configured_scroll_offsets.top:
                 self.content.move_cursor_down()
 
             self.vertical_scroll += 1
 
     def _scroll_up(self) -> None:
-        " Scroll window up. "
+        "Scroll window up."
         info = self.render_info
 
         if info is None:
             return
 
         if info.vertical_scroll > 0:
             # TODO: not entirely correct yet in case of line wrapping and long lines.
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/controls.py` & `prot-3.9.0/src/prot/prompt/layout/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,26 +171,25 @@
         self,
         get_line: Callable[[int], StyleAndTextTuples] = (lambda i: []),
         line_count: int = 0,
         cursor_position: Optional[Point] = None,
         menu_position: Optional[Point] = None,
         show_cursor: bool = True,
     ):
-
         self.get_line = get_line
         self.line_count = line_count
         self.cursor_position = cursor_position or Point(x=0, y=0)
         self.menu_position = menu_position
         self.show_cursor = show_cursor
 
         # Cache for line heights. Maps cache key -> height
         self._line_heights_cache: Dict[Hashable, int] = {}
 
     def __getitem__(self, lineno: int) -> StyleAndTextTuples:
-        " Make it iterable (iterate line by line). "
+        "Make it iterable (iterate line by line)."
         if lineno < self.line_count:
             return self.get_line(lineno)
         else:
             raise IndexError
 
     def get_height_for_line(
         self,
@@ -215,15 +214,15 @@
         # the same, while the content would change over time.
         key = get_app().render_counter, lineno, width, slice_stop
 
         try:
             return self._line_heights_cache[key]
         except KeyError:
             if width == 0:
-                height = 10 ** 8
+                height = 10**8
             else:
                 # Calculate line width first.
                 line = fragment_list_to_text(self.get_line(lineno))[:slice_stop]
                 text_width = get_cwidth(line)
 
                 if get_line_prefix:
                     # Add prefix width.
@@ -242,24 +241,24 @@
 
                         fragments2 = to_formatted_text(
                             get_line_prefix(lineno, height - 1)
                         )
                         prefix_width = get_cwidth(fragment_list_to_text(fragments2))
 
                         if prefix_width >= width:  # Prefix doesn't fit.
-                            height = 10 ** 8
+                            height = 10**8
                             break
 
                         text_width += prefix_width
                 else:
                     # Fast path: compute height when there's no line prefix.
                     try:
                         quotient, remainder = divmod(text_width, width)
                     except ZeroDivisionError:
-                        height = 10 ** 8
+                        height = 10**8
                     else:
                         if remainder:
                             quotient += 1  # Like math.ceil.
                         height = max(1, quotient)
 
             # Cache and return
             self._line_heights_cache[key] = height
@@ -315,15 +314,14 @@
         style: str = "",
         focusable: FilterOrBool = False,
         key_bindings: Optional["KeyBindingsBase"] = None,
         show_cursor: bool = True,
         modal: bool = False,
         get_cursor_position: Optional[Callable[[], Optional[Point]]] = None,
     ) -> None:
-
         self.text = text  # No type check on 'text'. This is done dynamically.
         self.style = style
         self.focusable = to_filter(focusable)
 
         # Key bindings.
         self.key_bindings = key_bindings
         self.show_cursor = show_cursor
@@ -371,15 +369,14 @@
     def preferred_height(
         self,
         width: int,
         max_available_height: int,
         wrap_lines: bool,
         get_line_prefix: Optional[GetLinePrefixCallable],
     ) -> Optional[int]:
-
         content = self.create_content(width, None)
         return content.line_count
 
     def create_content(self, width: int, height: Optional[int]) -> UIContent:
         # Get fragments
         fragments_with_mouse_handlers = self._get_formatted_text_cached()
         fragment_lines_with_mouse_handlers = list(
@@ -485,15 +482,15 @@
     """
 
     def create_content(self, width: int, height: int) -> UIContent:
         def get_line(i: int) -> StyleAndTextTuples:
             return []
 
         return UIContent(
-            get_line=get_line, line_count=100 ** 100
+            get_line=get_line, line_count=100**100
         )  # Something very big.
 
     def is_focusable(self) -> bool:
         return False
 
 
 _ProcessedLine = NamedTuple(
@@ -537,15 +534,14 @@
         search_buffer_control: Union[
             None, "SearchBufferControl", Callable[[], "SearchBufferControl"]
         ] = None,
         menu_position: Optional[Callable] = None,
         focus_on_click: FilterOrBool = False,
         key_bindings: Optional["KeyBindingsBase"] = None,
     ):
-
         self.input_processors = input_processors
         self.include_default_input_processors = include_default_input_processors
 
         self.default_input_processors = [
             HighlightSearchProcessor(),
             HighlightIncrementalSearchProcessor(),
             HighlightSelectionProcessor(),
@@ -628,15 +624,14 @@
     def preferred_height(
         self,
         width: int,
         max_available_height: int,
         wrap_lines: bool,
         get_line_prefix: Optional[GetLinePrefixCallable],
     ) -> Optional[int]:
-
         # Calculate the content height, if it was drawn on a screen with the
         # given width.
         height = 0
         content = self.create_content(width, height=1)  # Pass a dummy '1' as height.
 
         # When line wrapping is off, the height should be equal to the amount
         # of lines.
@@ -658,14 +653,15 @@
 
     def _get_formatted_text_for_line_func(
         self, document: Document
     ) -> Callable[[int], StyleAndTextTuples]:
         """
         Create a function that returns the fragments for a given line.
         """
+
         # Cache using `document.text`.
         def get_formatted_text_for_line() -> Callable[[int], StyleAndTextTuples]:
             return self.lexer.lex_document(document)
 
         key = (document.text, self.lexer.invalidation_hash())
         return self._fragment_cache.get(key, get_formatted_text_for_line)
 
@@ -681,20 +677,21 @@
         input_processors = self.input_processors or []
         if self.include_default_input_processors:
             input_processors = self.default_input_processors + input_processors
 
         merged_processor = merge_processors(input_processors)
 
         def transform(lineno: int, fragments: StyleAndTextTuples) -> _ProcessedLine:
-            " Transform the fragments for a given line number. "
+            "Transform the fragments for a given line number."
+
             # Get cursor position at this line.
             def source_to_display(i: int) -> int:
-                """ X position from the buffer to the x position in the
+                """X position from the buffer to the x position in the
                 processed fragment list. By default, we start from the 'identity'
-                operation. """
+                operation."""
                 return i
 
             transformation = merged_processor.apply_transformation(
                 TransformationInput(
                     self, document, lineno, source_to_display, fragments, width, height
                 )
             )
@@ -762,19 +759,19 @@
 
         get_processed_line = self._create_get_processed_line_func(
             document, width, height
         )
         self._last_get_processed_line = get_processed_line
 
         def translate_rowcol(row: int, col: int) -> Point:
-            " Return the content column for this coordinate. "
+            "Return the content column for this coordinate."
             return Point(x=get_processed_line(row).source_to_display(col), y=row)
 
         def get_line(i: int) -> StyleAndTextTuples:
-            " Return the fragments for a given line number. "
+            "Return the fragments for a given line number."
             fragments = get_processed_line(i).fragments
 
             # Add a space at the end, because that is a possible cursor
             # position. (When inserting after the input.) We should do this on
             # all the lines, not just the line containing the cursor. (Because
             # otherwise, line wrapping/scrolling could change when moving the
             # cursor around.)
@@ -921,15 +918,14 @@
         buffer: Optional[Buffer] = None,
         input_processors: Optional[List[Processor]] = None,
         lexer: Optional[Lexer] = None,
         focus_on_click: FilterOrBool = False,
         key_bindings: Optional["KeyBindingsBase"] = None,
         ignore_case: FilterOrBool = False,
     ):
-
         super().__init__(
             buffer=buffer,
             input_processors=input_processors,
             lexer=lexer,
             focus_on_click=focus_on_click,
             key_bindings=key_bindings,
         )
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/dimension.py` & `prot-3.9.0/src/prot/prompt/layout/dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.max_specified = max is not None
         self.preferred_specified = preferred is not None
         self.weight_specified = weight is not None
 
         if min is None:
             min = 0  # Smallest possible value.
         if max is None:  # 0-values are allowed, so use "is None"
-            max = 1000 ** 10  # Something huge.
+            max = 1000**10  # Something huge.
         if preferred is None:
             preferred = min
         if weight is None:
             weight = 1
 
         self.min = min
         self.max = max
@@ -90,15 +90,15 @@
         """
         Create a dimension that represents a zero size. (Used for 'invisible'
         controls.)
         """
         return cls.exact(amount=0)
 
     def is_zero(self) -> bool:
-        " True if this `Dimension` represents a zero size. "
+        "True if this `Dimension` represents a zero size."
         return self.preferred == 0 or self.max == 0
 
     def __repr__(self) -> str:
         fields = []
         if self.min_specified:
             fields.append("min=%r" % self.min)
         if self.max_specified:
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/dummy.py` & `prot-3.9.0/src/prot/prompt/layout/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/layout/layout.py` & `prot-3.9.0/src/prot/prompt/layout/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     """
 
     def __init__(
         self,
         container: AnyContainer,
         focused_element: Optional[FocusableElement] = None,
     ):
-
         self.container = to_container(container)
         self._stack: List[Window] = []
 
         # Map search BufferControl back to the original BufferControl.
         # This is used to keep track of when exactly we are searching, and for
         # applying the search.
         # When a link exists in this dictionary, that means the search is
@@ -209,25 +208,25 @@
                 self.current_window = window
                 return
 
         raise ValueError("Control not found in the user interface.")
 
     @property
     def current_window(self) -> Window:
-        " Return the :class:`.Window` object that is currently focused. "
+        "Return the :class:`.Window` object that is currently focused."
         return self._stack[-1]
 
     @current_window.setter
     def current_window(self, value: Window):
-        " Set the :class:`.Window` object to be currently focused. "
+        "Set the :class:`.Window` object to be currently focused."
         self._stack.append(value)
 
     @property
     def is_searching(self) -> bool:
-        " True if we are searching right now. "
+        "True if we are searching right now."
         return self.current_control in self.search_links
 
     @property
     def search_target_buffer_control(self) -> Optional[BufferControl]:
         """
         Return the :class:`.BufferControl` in which we are searching or `None`.
         """
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/margins.py` & `prot-3.9.0/src/prot/prompt/layout/margins.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     :param display_tildes: Display tildes after the end of the document, just
         like Vi does.
     """
 
     def __init__(
         self, relative: FilterOrBool = False, display_tildes: FilterOrBool = False
     ) -> None:
-
         self.relative = to_filter(relative)
         self.display_tildes = to_filter(display_tildes)
 
     def get_width(self, get_ui_content: Callable[[], UIContent]) -> int:
         line_count = get_ui_content().line_count
         return max(3, len("%s" % line_count) + 1)
 
@@ -165,15 +164,14 @@
 
     def __init__(
         self,
         display_arrows: FilterOrBool = False,
         up_arrow_symbol: str = "^",
         down_arrow_symbol: str = "v",
     ) -> None:
-
         self.display_arrows = to_filter(display_arrows)
         self.up_arrow_symbol = up_arrow_symbol
         self.down_arrow_symbol = down_arrow_symbol
 
     def get_width(self, get_ui_content: Callable[[], UIContent]) -> int:
         return 1
 
@@ -198,15 +196,15 @@
             )
             scrollbar_top = int(window_height * fraction_above)
         except ZeroDivisionError:
             return []
         else:
 
             def is_scroll_button(row: int) -> bool:
-                " True if we should display a button on this row. "
+                "True if we should display a button on this row."
                 return scrollbar_top <= row <= scrollbar_top + scrollbar_height
 
             # Up arrow.
             result: StyleAndTextTuples = []
             if display_arrows:
                 result.extend(
                     [
@@ -268,20 +266,19 @@
     def __init__(
         self,
         get_prompt: Callable[[], StyleAndTextTuples],
         get_continuation: Optional[
             Callable[[int, int, bool], StyleAndTextTuples]
         ] = None,
     ) -> None:
-
         self.get_prompt = get_prompt
         self.get_continuation = get_continuation
 
     def get_width(self, get_ui_content: Callable[[], UIContent]) -> int:
-        " Width to report to the `Window`. "
+        "Width to report to the `Window`."
         # Take the width from the first line.
         text = fragment_list_to_text(self.get_prompt())
         return get_cwidth(text)
 
     def create_margin(
         self, window_render_info: "WindowRenderInfo", width: int, height: int
     ) -> StyleAndTextTuples:
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/menus.py` & `prot-3.9.0/src/prot/prompt/layout/menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     def preferred_height(
         self,
         width: int,
         max_available_height: int,
         wrap_lines: bool,
         get_line_prefix: Optional[GetLinePrefixCallable],
     ) -> Optional[int]:
-
         complete_state = get_app().current_buffer.complete_state
         if complete_state:
             return len(complete_state.completions)
         else:
             return 0
 
     def create_content(self, width: int, height: int) -> UIContent:
@@ -165,15 +164,14 @@
             )
         else:
             return 0
 
     def _get_menu_item_meta_fragments(
         self, completion: Completion, is_current_completion: bool, width: int
     ) -> StyleAndTextTuples:
-
         if is_current_completion:
             style_str = "class:completion-menu.meta.completion.current"
         else:
             style_str = "class:completion-menu.meta.completion"
 
         text, tw = _trim_formatted_text(completion.display_meta, width - 2)
         padding = " " * (width - 1 - tw)
@@ -271,17 +269,16 @@
     #       visible at the point where we draw this menu.
     def __init__(
         self,
         max_height: Optional[int] = None,
         scroll_offset: Union[int, Callable[[], int]] = 0,
         extra_filter: FilterOrBool = True,
         display_arrows: FilterOrBool = False,
-        z_index: int = 10 ** 8,
+        z_index: int = 10**8,
     ) -> None:
-
         extra_filter = to_filter(extra_filter)
         display_arrows = to_filter(display_arrows)
 
         super().__init__(
             content=Window(
                 content=CompletionsMenuControl(),
                 width=Dimension(min=8),
@@ -401,20 +398,20 @@
         self._render_pos_to_completion = {}
 
         _T = TypeVar("_T")
 
         def grouper(
             n: int, iterable: Iterable[_T], fillvalue: Optional[_T] = None
         ) -> Iterable[List[_T]]:
-            " grouper(3, 'ABCDEFG', 'x') --> ABC DEF Gxx "
+            "grouper(3, 'ABCDEFG', 'x') --> ABC DEF Gxx"
             args = [iter(iterable)] * n
             return zip_longest(fillvalue=fillvalue, *args)
 
         def is_current_completion(completion: Completion) -> bool:
-            " Returns True when this completion is the currently selected one. "
+            "Returns True when this completion is the currently selected one."
             return (
                 complete_state is not None
                 and complete_state.complete_index is not None
                 and c == complete_state.current_completion
             )
 
         # Space required outside of the regular columns, for displaying the
@@ -563,15 +560,15 @@
         """
         from prot.prompt.key_binding.key_bindings import KeyBindings
 
         kb = KeyBindings()
 
         @Condition
         def filter() -> bool:
-            " Only handle key bindings if this menu is visible. "
+            "Only handle key bindings if this menu is visible."
             app = get_app()
             complete_state = app.current_buffer.complete_state
 
             # There need to be completions, and one needs to be selected.
             if complete_state is None or complete_state.complete_index is None:
                 return False
 
@@ -616,17 +613,16 @@
 
     def __init__(
         self,
         min_rows: int = 3,
         suggested_max_column_width: int = 30,
         show_meta: FilterOrBool = True,
         extra_filter: FilterOrBool = True,
-        z_index: int = 10 ** 8,
+        z_index: int = 10**8,
     ) -> None:
-
         show_meta = to_filter(show_meta)
         extra_filter = to_filter(extra_filter)
 
         # Display filter: show when there are completions but not at the point
         # we are returning the input.
         full_filter = has_completions & ~is_done & extra_filter
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/mouse_handlers.py` & `prot-3.9.0/src/prot/prompt/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/layout/processors.py` & `prot-3.9.0/src/prot/prompt/layout/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         document: Document,
         lineno: int,
         source_to_display: SourceToDisplay,
         fragments: StyleAndTextTuples,
         width: int,
         height: int,
     ) -> None:
-
         self.buffer_control = buffer_control
         self.document = document
         self.lineno = lineno
         self.source_to_display = source_to_display
         self.fragments = fragments
         self.width = width
         self.height = height
@@ -147,15 +146,14 @@
 
     def __init__(
         self,
         fragments: StyleAndTextTuples,
         source_to_display: Optional[SourceToDisplay] = None,
         display_to_source: Optional[DisplayToSource] = None,
     ) -> None:
-
         self.fragments = fragments
         self.source_to_display = source_to_display or (lambda i: i)
         self.display_to_source = display_to_source or (lambda i: i)
 
 
 class DummyProcessor(Processor):
     """
@@ -185,15 +183,14 @@
         The text we are searching for.
         """
         return buffer_control.search_state.text
 
     def apply_transformation(
         self, transformation_input: TransformationInput
     ) -> Transformation:
-
         (
             buffer_control,
             document,
             lineno,
             source_to_display,
             fragments,
             _,
@@ -396,15 +393,14 @@
             ]
         else:
             return []
 
     def apply_transformation(
         self, transformation_input: TransformationInput
     ) -> Transformation:
-
         (
             buffer_control,
             document,
             lineno,
             source_to_display,
             fragments,
             _,
@@ -443,15 +439,14 @@
     """
     When we're in Vi block insert mode, display all the cursors.
     """
 
     def apply_transformation(
         self, transformation_input: TransformationInput
     ) -> Transformation:
-
         (
             buffer_control,
             document,
             lineno,
             source_to_display,
             fragments,
             _,
@@ -699,15 +694,14 @@
     def __init__(
         self,
         tabstop: Union[int, Callable[[], int]] = 4,
         char1: Union[str, Callable[[], str]] = "|",
         char2: Union[str, Callable[[], str]] = "\u2508",
         style: str = "class:tab",
     ) -> None:
-
         self.char1 = char1
         self.char2 = char2
         self.tabstop = tabstop
         self.style = style
 
     def apply_transformation(self, ti: TransformationInput) -> Transformation:
         tabstop = to_int(self.tabstop)
@@ -743,19 +737,19 @@
 
         position_mappings[len(fragments)] = pos
         # Add `pos+1` to mapping, because the cursor can be right after the
         # line as well.
         position_mappings[len(fragments) + 1] = pos + 1
 
         def source_to_display(from_position: int) -> int:
-            " Maps original cursor position to the new one. "
+            "Maps original cursor position to the new one."
             return position_mappings[from_position]
 
         def display_to_source(display_pos: int) -> int:
-            " Maps display cursor position to the original one. "
+            "Maps display cursor position to the original one."
             position_mappings_reversed = {v: k for k, v in position_mappings.items()}
 
             while display_pos >= 0:
                 try:
                     return position_mappings_reversed[display_pos]
                 except KeyError:
                     display_pos -= 1
@@ -803,16 +797,16 @@
         from prot.prompt.layout.controls import BufferControl
 
         # Emulate the BufferControl through which we are searching.
         # For this we filter out some of the input processors.
         excluded_processors = tuple(self._excluded_input_processors)
 
         def filter_processor(item: Processor) -> Optional[Processor]:
-            """ Filter processors from the main control that we want to disable
-            here. This returns either an accepted processor or None. """
+            """Filter processors from the main control that we want to disable
+            here. This returns either an accepted processor or None."""
             # For a `_MergedProcessor`, check each individual processor, recursively.
             if isinstance(item, _MergedProcessor):
                 accepted_processors = [filter_processor(p) for p in item.processors]
                 return merge_processors(
                     [p for p in accepted_processors if p is not None]
                 )
 
@@ -986,16 +980,16 @@
 
     def apply_transformation(self, ti: TransformationInput) -> Transformation:
         source_to_display_functions = [ti.source_to_display]
         display_to_source_functions = []
         fragments = ti.fragments
 
         def source_to_display(i: int) -> int:
-            """ Translate x position from the buffer to the x position in the
-            processor fragments list. """
+            """Translate x position from the buffer to the x position in the
+            processor fragments list."""
             for f in source_to_display_functions:
                 i = f(i)
             return i
 
         for p in self.processors:
             transformation = p.apply_transformation(
                 TransformationInput(
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/screen.py` & `prot-3.9.0/src/prot/prompt/layout/screen.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 
     def __init__(
         self,
         default_char: Optional[Char] = None,
         initial_width: int = 0,
         initial_height: int = 0,
     ) -> None:
-
         if default_char is None:
             default_char2 = _CHAR_CACHE[" ", Transparent]
         else:
             default_char2 = default_char
 
         self.data_buffer: DefaultDict[int, DefaultDict[int, Char]] = defaultdict(
             lambda: defaultdict(lambda: default_char2)
```

### Comparing `prot-3.8.6/src/prot/prompt/layout/utils.py` & `prot-3.9.0/src/prot/prompt/layout/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/lexers/base.py` & `prot-3.9.0/src/prot/prompt/lexers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def __init__(self, style: str = "") -> None:
         self.style = style
 
     def lex_document(self, document: Document) -> Callable[[int], StyleAndTextTuples]:
         lines = document.lines
 
         def get_line(lineno: int) -> StyleAndTextTuples:
-            " Return the tokens for the given line. "
+            "Return the tokens for the given line."
             try:
                 return [(self.style, lines[lineno])]
             except IndexError:
                 return []
 
         return get_line
```

### Comparing `prot-3.8.6/src/prot/prompt/lexers/pygments.py` & `prot-3.9.0/src/prot/prompt/lexers/pygments.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,14 @@
 
     def __init__(
         self,
         pygments_lexer_cls: Type["PygmentsLexerCls"],
         sync_from_start: FilterOrBool = True,
         syntax_sync: Optional[SyntaxSync] = None,
     ) -> None:
-
         self.pygments_lexer_cls = pygments_lexer_cls
         self.sync_from_start = to_filter(sync_from_start)
 
         # Instantiate the Pygments lexer.
         self.pygments_lexer = pygments_lexer_cls(
             stripnl=False, stripall=False, ensurenl=False
         )
@@ -232,22 +231,22 @@
         cache: Dict[int, StyleAndTextTuples] = {}
 
         # Pygments generators that are currently lexing.
         # Map lexer generator to the line number.
         line_generators: Dict[LineGenerator, int] = {}
 
         def get_syntax_sync() -> SyntaxSync:
-            " The Syntax synchronisation object that we currently use. "
+            "The Syntax synchronisation object that we currently use."
             if self.sync_from_start():
                 return SyncFromStart()
             else:
                 return self.syntax_sync
 
         def find_closest_generator(i: int) -> Optional[LineGenerator]:
-            " Return a generator close to line 'i', or None if none was found. "
+            "Return a generator close to line 'i', or None if none was found."
             for generator, lineno in line_generators.items():
                 if lineno < i and i - lineno < self.REUSE_GENERATOR_MAX_DISTANCE:
                     return generator
             return None
 
         def create_line_generator(start_lineno: int, column: int = 0) -> LineGenerator:
             """
@@ -305,15 +304,15 @@
                 next(generator)
                 row += 1
 
             line_generators[generator] = row
             return generator
 
         def get_line(i: int) -> StyleAndTextTuples:
-            " Return the tokens for a given line number. "
+            "Return the tokens for a given line number."
             try:
                 return cache[i]
             except KeyError:
                 generator = get_generator(i)
 
                 # Exhaust the generator, until we find the requested line.
                 for num, line in generator:
```

### Comparing `prot-3.8.6/src/prot/prompt/mouse_events.py` & `prot-3.9.0/src/prot/prompt/mouse_events.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/output/base.py` & `prot-3.9.0/src/prot/prompt/output/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,67 +22,67 @@
     Actual implementations are
     :class:`~prompt_toolkit.output.vt100.Vt100_Output` and
     :class:`~prompt_toolkit.output.win32.Win32Output`.
     """
 
     @abstractmethod
     def fileno(self) -> int:
-        " Return the file descriptor to which we can write for the output. "
+        "Return the file descriptor to which we can write for the output."
 
     @abstractmethod
     def encoding(self) -> str:
         """
         Return the encoding for this output, e.g. 'utf-8'.
         (This is used mainly to know which characters are supported by the
         output the data, so that the UI can provide alternatives, when
         required.)
         """
 
     @abstractmethod
     def write(self, data: str) -> None:
-        " Write text (Terminal escape sequences will be removed/escaped.) "
+        "Write text (Terminal escape sequences will be removed/escaped.)"
 
     @abstractmethod
     def write_raw(self, data: str) -> None:
-        " Write text. "
+        "Write text."
 
     @abstractmethod
     def set_title(self, title: str) -> None:
-        " Set terminal title. "
+        "Set terminal title."
 
     @abstractmethod
     def clear_title(self) -> None:
-        " Clear title again. (or restore previous title.) "
+        "Clear title again. (or restore previous title.)"
 
     @abstractmethod
     def flush(self) -> None:
-        " Write to output stream and flush. "
+        "Write to output stream and flush."
 
     @abstractmethod
     def erase_screen(self) -> None:
         """
         Erases the screen with the background colour and moves the cursor to
         home.
         """
 
     @abstractmethod
     def enter_alternate_screen(self) -> None:
-        " Go to the alternate screen buffer. (For full screen applications). "
+        "Go to the alternate screen buffer. (For full screen applications)."
 
     @abstractmethod
     def quit_alternate_screen(self) -> None:
-        " Leave the alternate screen buffer. "
+        "Leave the alternate screen buffer."
 
     @abstractmethod
     def enable_mouse_support(self) -> None:
-        " Enable mouse. "
+        "Enable mouse."
 
     @abstractmethod
     def disable_mouse_support(self) -> None:
-        " Disable mouse. "
+        "Disable mouse."
 
     @abstractmethod
     def erase_end_of_line(self) -> None:
         """
         Erases from the current cursor position to the end of the current line.
         """
 
@@ -91,90 +91,90 @@
         """
         Erases the screen from the current line down to the bottom of the
         screen.
         """
 
     @abstractmethod
     def reset_attributes(self) -> None:
-        " Reset color and styling attributes. "
+        "Reset color and styling attributes."
 
     @abstractmethod
     def set_attributes(self, attrs: Attrs, color_depth: ColorDepth) -> None:
-        " Set new color and styling attributes. "
+        "Set new color and styling attributes."
 
     @abstractmethod
     def disable_autowrap(self) -> None:
-        " Disable auto line wrapping. "
+        "Disable auto line wrapping."
 
     @abstractmethod
     def enable_autowrap(self) -> None:
-        " Enable auto line wrapping. "
+        "Enable auto line wrapping."
 
     @abstractmethod
     def cursor_goto(self, row: int = 0, column: int = 0) -> None:
-        " Move cursor position. "
+        "Move cursor position."
 
     @abstractmethod
     def cursor_up(self, amount: int) -> None:
-        " Move cursor `amount` place up. "
+        "Move cursor `amount` place up."
 
     @abstractmethod
     def cursor_down(self, amount: int) -> None:
-        " Move cursor `amount` place down. "
+        "Move cursor `amount` place down."
 
     @abstractmethod
     def cursor_forward(self, amount: int) -> None:
-        " Move cursor `amount` place forward. "
+        "Move cursor `amount` place forward."
 
     @abstractmethod
     def cursor_backward(self, amount: int) -> None:
-        " Move cursor `amount` place backward. "
+        "Move cursor `amount` place backward."
 
     @abstractmethod
     def hide_cursor(self) -> None:
-        " Hide cursor. "
+        "Hide cursor."
 
     @abstractmethod
     def show_cursor(self) -> None:
-        " Show cursor. "
+        "Show cursor."
 
     def ask_for_cpr(self) -> None:
         """
         Asks for a cursor position report (CPR).
         (VT100 only.)
         """
 
     @abstractmethod
     def get_size(self) -> Size:
-        " Return the size of the output window. "
+        "Return the size of the output window."
 
     def bell(self) -> None:
-        " Sound bell. "
+        "Sound bell."
 
     def enable_bracketed_paste(self) -> None:
-        " For vt100 only. "
+        "For vt100 only."
 
     def disable_bracketed_paste(self) -> None:
-        " For vt100 only. "
+        "For vt100 only."
 
     def scroll_buffer_to_prompt(self) -> None:
-        " For Win32 only. "
+        "For Win32 only."
 
     def get_rows_below_cursor_position(self) -> int:
-        " For Windows only. "
+        "For Windows only."
         raise NotImplementedError
 
 
 class DummyOutput(Output):
     """
     For testing. An output class that doesn't render anything.
     """
 
     def fileno(self) -> int:
-        " There is no sensible default for fileno(). "
+        "There is no sensible default for fileno()."
         raise NotImplementedError
 
     def encoding(self) -> str:
         return "utf-8"
 
     def write(self, data: str) -> None:
         pass
```

### Comparing `prot-3.8.6/src/prot/prompt/output/color_depth.py` & `prot-3.9.0/src/prot/prompt/output/color_depth.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/output/conemu.py` & `prot-3.9.0/src/prot/prompt/output/conemu.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/output/defaults.py` & `prot-3.9.0/src/prot/prompt/output/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/output/win32.py` & `prot-3.9.0/src/prot/prompt/output/win32.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,29 +101,29 @@
         info = self.get_win32_screen_buffer_info()
         self.default_attrs = info.wAttributes if info else 15
 
         if _DEBUG_RENDER_OUTPUT:
             self.LOG = open(_DEBUG_RENDER_OUTPUT_FILENAME, "ab")
 
     def fileno(self) -> int:
-        " Return file descriptor. "
+        "Return file descriptor."
         return self.stdout.fileno()
 
     def encoding(self) -> str:
-        " Return encoding used for stdout. "
+        "Return encoding used for stdout."
         return self.stdout.encoding
 
     def write(self, data: str) -> None:
         if self._hidden:
             data = " " * get_cwidth(data)
 
         self._buffer.append(data)
 
     def write_raw(self, data: str) -> None:
-        " For win32, there is no difference between write and write_raw. "
+        "For win32, there is no difference between write and write_raw."
         self.write(data)
 
     def get_size(self) -> Size:
         info = self.get_win32_screen_buffer_info()
 
         # We take the width of the *visible* region as the size. Not the width
         # of the complete screen buffer. (Unless use_complete_width has been
@@ -227,16 +227,15 @@
 
         start = sbinfo.dwCursorPosition
         length = (size.X - size.X) + size.X * (size.Y - sbinfo.dwCursorPosition.Y)
 
         self._erase(start, length)
 
     def erase_end_of_line(self) -> None:
-        """
-        """
+        """ """
         sbinfo = self.get_win32_screen_buffer_info()
         start = sbinfo.dwCursorPosition
         length = sbinfo.dwSize.X - sbinfo.dwCursorPosition.X
 
         self._erase(start, length)
 
     def _erase(self, start, length):
@@ -259,15 +258,15 @@
             sbinfo.wAttributes,
             length,
             _coord_byval(start),
             byref(chars_written),
         )
 
     def reset_attributes(self) -> None:
-        " Reset the console foreground/background color. "
+        "Reset the console foreground/background color."
         self._winapi(
             windll.kernel32.SetConsoleTextAttribute, self.hconsole, self.default_attrs
         )
         self._hidden = False
 
     def set_attributes(self, attrs: Attrs, color_depth: ColorDepth) -> None:
         fgcolor, bgcolor, bold, underline, italic, blink, reverse, hidden = attrs
@@ -501,15 +500,15 @@
     MAGENTA = 0x0050
     YELLOW = 0x0060
     GRAY = 0x0070
     INTENSITY = 0x0080  # Background color is intensified.
 
 
 def _create_ansi_color_dict(color_cls) -> Dict[str, int]:
-    " Create a table that maps the 16 named ansi colors to their Windows code. "
+    "Create a table that maps the 16 named ansi colors to their Windows code."
     return {
         "ansidefault": color_cls.BLACK,
         "ansiblack": color_cls.BLACK,
         "ansigray": color_cls.GRAY,
         "ansibrightblack": color_cls.BLACK | color_cls.INTENSITY,
         "ansiwhite": color_cls.GRAY | color_cls.INTENSITY,
         # Low intensity.
```

### Comparing `prot-3.8.6/src/prot/prompt/output/windows10.py` & `prot-3.9.0/src/prot/prompt/output/windows10.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/patch_stdout.py` & `prot-3.9.0/src/prot/prompt/patch_stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     Proxy object for stdout which captures everything and prints output above
     the current application.
     """
 
     def __init__(
         self, raw: bool = False, original_stdout: Optional[TextIO] = None
     ) -> None:
-
         original_stdout = original_stdout or sys.__stdout__
 
         self.original_stdout = original_stdout
 
         self._lock = threading.RLock()
         self._raw = raw
         self._buffer: List[str] = []
```

### Comparing `prot-3.8.6/src/prot/prompt/renderer.py` & `prot-3.9.0/src/prot/prompt/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,21 +81,21 @@
     _output_cursor_up = output.cursor_up
     _output_cursor_backward = output.cursor_backward
 
     # Hide cursor before rendering. (Avoid flickering.)
     output.hide_cursor()
 
     def reset_attributes() -> None:
-        " Wrapper around Output.reset_attributes. "
+        "Wrapper around Output.reset_attributes."
         nonlocal last_style
         _output_reset_attributes()
         last_style = None  # Forget last char after resetting attributes.
 
     def move_cursor(new: Point) -> Point:
-        " Move cursor to this `new` point. Returns the given Point. "
+        "Move cursor to this `new` point. Returns the given Point."
         current_x, current_y = current_pos.x, current_pos.y
 
         if new.y > current_y:
             # Use newlines instead of CURSOR_DOWN, because this might add new lines.
             # CURSOR_DOWN will never create new lines at the bottom.
             # Also reset attributes, otherwise the newline could draw a
             # background color.
@@ -240,42 +240,41 @@
     if screen.show_cursor or is_done:
         output.show_cursor()
 
     return current_pos, last_style
 
 
 class HeightIsUnknownError(Exception):
-    " Information unavailable. Did not yet receive the CPR response. "
+    "Information unavailable. Did not yet receive the CPR response."
 
 
 class _StyleStringToAttrsCache(Dict[str, Attrs]):
     """
     A cache structure that maps style strings to :class:`.Attr`.
     (This is an important speed up.)
     """
 
     def __init__(
         self,
         get_attrs_for_style_str: Callable[["str"], Attrs],
         style_transformation: StyleTransformation,
     ) -> None:
-
         self.get_attrs_for_style_str = get_attrs_for_style_str
         self.style_transformation = style_transformation
 
     def __missing__(self, style_str: str) -> Attrs:
         attrs = self.get_attrs_for_style_str(style_str)
         attrs = self.style_transformation.transform_attrs(attrs)
 
         self[style_str] = attrs
         return attrs
 
 
 class CPR_Support(Enum):
-    " Enum: whether or not CPR is supported. "
+    "Enum: whether or not CPR is supported."
     SUPPORTED = "SUPPORTED"
     NOT_SUPPORTED = "NOT_SUPPORTED"
     UNKNOWN = "UNKNOWN"
 
 
 class Renderer:
     """
@@ -295,15 +294,14 @@
         style: BaseStyle,
         output: Output,
         input: Input,
         full_screen: bool = False,
         mouse_support: FilterOrBool = False,
         cpr_not_supported_callback: Optional[Callable[[], None]] = None,
     ) -> None:
-
         self.style = style
         self.output = output
         self.input = input
         self.full_screen = full_screen
         self.mouse_support = to_filter(mouse_support)
         self.cpr_not_supported_callback = cpr_not_supported_callback
 
@@ -322,15 +320,14 @@
         self._last_style_hash: Optional[Hashable] = None
         self._last_transformation_hash: Optional[Hashable] = None
         self._last_color_depth: Optional[ColorDepth] = None
 
         self.reset(_scroll=True)
 
     def reset(self, _scroll: bool = False, leave_alternate_screen: bool = True) -> None:
-
         # Reset position
         self._cursor_pos = Point(x=0, y=0)
 
         # Remember the last screen instance between renderers. This way,
         # we can create a `diff` between two screens and only output the
         # difference. It's also to remember the last height. (To show for
         # instance a toolbar at the bottom position.)
@@ -594,15 +591,20 @@
         self._last_style_hash = self.style.invalidation_hash()
         self._last_transformation_hash = app.style_transformation.invalidation_hash()
         self._last_color_depth = app.color_depth
 
         layout.container.write_to_screen(
             screen,
             mouse_handlers,
-            WritePosition(xpos=0, ypos=0, width=size.columns, height=height,),
+            WritePosition(
+                xpos=0,
+                ypos=0,
+                width=size.columns,
+                height=height,
+            ),
             parent_style="",
             erase_bg=False,
             z_index=None,
         )
         screen.draw_all_floats()
 
         # When grayed. Replace all styles in the new screen.
```

### Comparing `prot-3.8.6/src/prot/prompt/search.py` & `prot-3.9.0/src/prot/prompt/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     def __init__(
         self,
         text: str = "",
         direction: SearchDirection = SearchDirection.FORWARD,
         ignore_case: FilterOrBool = False,
     ) -> None:
-
         self.text = text
         self.direction = direction
         self.ignore_case = to_filter(ignore_case)
 
     def __repr__(self) -> str:
         return "%s(%r, direction=%r, ignore_case=%r)" % (
             self.__class__.__name__,
```

### Comparing `prot-3.8.6/src/prot/prompt/selection.py` & `prot-3.9.0/src/prot/prompt/selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     """
 
     def __init__(
         self,
         original_cursor_position: int = 0,
         type: SelectionType = SelectionType.CHARACTERS,
     ) -> None:
-
         self.original_cursor_position = original_cursor_position
         self.type = type
         self.shift_mode = False
 
     def enter_shift_mode(self) -> None:
         self.shift_mode = True
```

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/__init__.py` & `prot-3.9.0/src/prot/prompt/shortcuts/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/dialogs.py` & `prot-3.9.0/src/prot/prompt/shortcuts/dialogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,18 @@
     textfield = TextArea(
         multiline=False, password=password, completer=completer, accept_handler=accept
     )
 
     dialog = Dialog(
         title=title,
         body=HSplit(
-            [Label(text=text, dont_extend_height=True), textfield,],
+            [
+                Label(text=text, dont_extend_height=True),
+                textfield,
+            ],
             padding=D(preferred=1, max=1),
         ),
         buttons=[ok_button, cancel_button],
         with_background=True,
     )
 
     return _create_app(dialog, style)
@@ -148,15 +151,17 @@
 ) -> Application[None]:
     """
     Display a simple message box and wait until the user presses enter.
     """
     dialog = Dialog(
         title=title,
         body=Label(text=text, dont_extend_height=True),
-        buttons=[Button(text=ok_text, handler=_return_none),],
+        buttons=[
+            Button(text=ok_text, handler=_return_none),
+        ],
         with_background=True,
     )
 
     return _create_app(dialog, style)
 
 
 def radiolist_dialog(
@@ -180,15 +185,19 @@
         get_app().exit(result=radio_list.current_value)
 
     radio_list = RadioList(values)
 
     dialog = Dialog(
         title=title,
         body=HSplit(
-            [Label(text=text, dont_extend_height=True), radio_list,], padding=1
+            [
+                Label(text=text, dont_extend_height=True),
+                radio_list,
+            ],
+            padding=1,
         ),
         buttons=[
             Button(text=ok_text, handler=ok_handler),
             Button(text=cancel_text, handler=_return_none),
         ],
         with_background=True,
     )
@@ -216,15 +225,21 @@
     def ok_handler() -> None:
         get_app().exit(result=cb_list.current_values)
 
     cb_list = CheckboxList(values)
 
     dialog = Dialog(
         title=title,
-        body=HSplit([Label(text=text, dont_extend_height=True), cb_list,], padding=1),
+        body=HSplit(
+            [
+                Label(text=text, dont_extend_height=True),
+                cb_list,
+            ],
+            padding=1,
+        ),
         buttons=[
             Button(text=ok_text, handler=ok_handler),
             Button(text=cancel_text, handler=_return_none),
         ],
         with_background=True,
     )
 
@@ -245,20 +260,24 @@
     """
     loop = get_event_loop()
     progressbar = ProgressBar()
     text_area = TextArea(
         focusable=False,
         # Prefer this text area as big as possible, to avoid having a window
         # that keeps resizing when we add text to it.
-        height=D(preferred=10 ** 10),
+        height=D(preferred=10**10),
     )
 
     dialog = Dialog(
         body=HSplit(
-            [Box(Label(text=text)), Box(text_area, padding=D.exact(1)), progressbar,]
+            [
+                Box(Label(text=text)),
+                Box(text_area, padding=D.exact(1)),
+                progressbar,
+            ]
         ),
         title=title,
         with_background=True,
     )
     app = _create_app(dialog, style)
 
     def set_percentage(value: int) -> None:
@@ -289,17 +308,22 @@
     # Key bindings.
     bindings = KeyBindings()
     bindings.add("tab")(focus_next)
     bindings.add("s-tab")(focus_previous)
 
     return Application(
         layout=Layout(dialog),
-        key_bindings=merge_key_bindings([load_key_bindings(), bindings,]),
+        key_bindings=merge_key_bindings(
+            [
+                load_key_bindings(),
+                bindings,
+            ]
+        ),
         mouse_support=True,
         style=style,
         full_screen=True,
     )
 
 
 def _return_none() -> None:
-    " Button handler that returns None. "
+    "Button handler that returns None."
     get_app().exit()
```

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/base.py` & `prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         style: Optional[BaseStyle] = None,
         key_bindings: Optional[KeyBindings] = None,
         file: Optional[TextIO] = None,
         color_depth: Optional[ColorDepth] = None,
         output: Optional[Output] = None,
         input: Optional[Input] = None,
     ) -> None:
-
         self.title = title
         self.formatters = formatters or create_default_formatters()
         self.bottom_toolbar = bottom_toolbar
         self.counters: List[ProgressBarCounter[object]] = []
         self.style = style
         self.key_bindings = key_bindings
 
@@ -319,15 +318,14 @@
         self,
         progress_bar: ProgressBar,
         data: Optional[Iterable[_CounterItem]] = None,
         label: AnyFormattedText = "",
         remove_when_done: bool = False,
         total: Optional[int] = None,
     ) -> None:
-
         self.start_time = datetime.datetime.now()
         self.stop_time: Optional[datetime.datetime] = None
         self.progress_bar = progress_bar
         self.data = data
         self.items_completed = 0
         self.label = label
         self.remove_when_done = remove_when_done
```

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/progress_bar/formatters.py` & `prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         label = self._add_suffix(progress.label)
         cwidth = fragment_list_width(label)
 
         if cwidth > width:
             # It doesn't fit -> scroll task name.
             label = explode_text_fragments(label)
             max_scroll = cwidth - width
@@ -133,15 +132,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         return HTML(self.template).format(percentage=round(progress.percentage, 1))
 
     def get_width(self, progress_bar: "ProgressBar") -> AnyDimension:
         return D.exact(6)
 
 
 class Bar(Formatter):
@@ -156,15 +154,14 @@
         start: str = "[",
         end: str = "]",
         sym_a: str = "=",
         sym_b: str = ">",
         sym_c: str = " ",
         unknown: str = "#",
     ) -> None:
-
         assert len(sym_a) == 1 and get_cwidth(sym_a) == 1
         assert len(sym_c) == 1 and get_cwidth(sym_c) == 1
 
         self.start = start
         self.end = end
         self.sym_a = sym_a
         self.sym_b = sym_b
@@ -220,15 +217,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         return HTML(self.template).format(
             current=progress.items_completed, total=progress.total or "?"
         )
 
     def get_width(self, progress_bar: "ProgressBar") -> AnyDimension:
         all_lengths = [
             len("{0:>3}".format(c.total or "?")) for c in progress_bar.counters
@@ -254,15 +250,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         text = _format_timedelta(progress.time_elapsed).rjust(width)
         return HTML("<time-elapsed>{time_elapsed}</time-elapsed>").format(
             time_elapsed=text
         )
 
     def get_width(self, progress_bar: "ProgressBar") -> AnyDimension:
         all_values = [
@@ -283,15 +278,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         time_left = progress.time_left
         if time_left is not None:
             formatted_time_left = _format_timedelta(time_left)
         else:
             formatted_time_left = self.unknown
 
         return HTML(self.template).format(time_left=formatted_time_left.rjust(width))
@@ -317,15 +311,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         value = progress.items_completed / progress.time_elapsed.total_seconds()
         return HTML(self.template.format(iterations_per_second=value))
 
     def get_width(self, progress_bar: "ProgressBar") -> AnyDimension:
         all_values = [
             len("{0:.2f}".format(c.items_completed / c.time_elapsed.total_seconds()))
             for c in progress_bar.counters
@@ -344,15 +337,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         index = int(time.time() * 3) % len(self.characters)
         return HTML("<spinning-wheel>{0}</spinning-wheel>").format(
             self.characters[index]
         )
 
     def get_width(self, progress_bar: "ProgressBar") -> AnyDimension:
         return D.exact(1)
@@ -392,15 +384,14 @@
 
     def format(
         self,
         progress_bar: "ProgressBar",
         progress: "ProgressBarCounter[object]",
         width: int,
     ) -> AnyFormattedText:
-
         # Get formatted text from nested formatter, and explode it in
         # text/style tuples.
         result = self.formatter.format(progress_bar, progress, width)
         result = explode_text_fragments(to_formatted_text(result))
 
         # Insert colors.
         result2: StyleAndTextTuples = []
```

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/prompt.py` & `prot-3.9.0/src/prot/prompt/shortcuts/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,14 @@
         erase_when_done: bool = False,
         tempfile_suffix: Optional[Union[str, Callable[[], str]]] = ".txt",
         tempfile: Optional[Union[str, Callable[[], str]]] = None,
         refresh_interval: float = 0,
         input: Optional[Input] = None,
         output: Optional[Output] = None,
     ) -> None:
-
         history = history or InMemoryHistory()
         clipboard = clipboard or InMemoryClipboard()
 
         # Ensure backwards-compatibility, when `vi_mode` is passed.
         if vi_mode:
             editing_mode = EditingMode.VI
 
@@ -478,16 +477,16 @@
         """
         Create and return the default input buffer.
         """
         dyncond = self._dyncond
 
         # Create buffers list.
         def accept(buff: Buffer) -> bool:
-            """ Accept the content of the default buffer. This is called when
-            the validation succeeds. """
+            """Accept the content of the default buffer. This is called when
+            the validation succeeds."""
             cast(Application[str], get_app()).exit(result=buff.document.text)
             return True  # Keep text, we call 'reset' later on.
 
         return Buffer(
             name=DEFAULT_BUFFER,
             # Make sure that complete_while_typing is disabled when
             # enable_history_search is enabled. (First convert to Filter,
@@ -562,24 +561,26 @@
 
         search_toolbar = SearchToolbar(
             search_buffer, ignore_case=dyncond("search_ignore_case")
         )
 
         search_buffer_control = SearchBufferControl(
             buffer=search_buffer,
-            input_processors=[ReverseSearchProcessor(),],
+            input_processors=[
+                ReverseSearchProcessor(),
+            ],
             ignore_case=dyncond("search_ignore_case"),
         )
 
         system_toolbar = SystemToolbar(
             enable_global_bindings=dyncond("enable_system_prompt")
         )
 
         def get_search_buffer_control() -> SearchBufferControl:
-            " Return the UIControl to be focused when searching start. "
+            "Return the UIControl to be focused when searching start."
             if is_true(self.multiline):
                 return search_toolbar.control
             else:
                 return search_buffer_control
 
         default_buffer_control = BufferControl(
             buffer=default_buffer,
@@ -772,44 +773,44 @@
         def do_accept() -> bool:
             return not is_true(self.multiline) and self.app.layout.has_focus(
                 DEFAULT_BUFFER
             )
 
         @handle("enter", filter=do_accept & default_focused)
         def _accept_input(event: E) -> None:
-            " Accept input when enter has been pressed. "
+            "Accept input when enter has been pressed."
             self.default_buffer.validate_and_handle()
 
         @Condition
         def readline_complete_style() -> bool:
             return self.complete_style == CompleteStyle.READLINE_LIKE
 
         @handle("tab", filter=readline_complete_style & default_focused)
         def _complete_like_readline(event: E) -> None:
-            " Display completions (like Readline). "
+            "Display completions (like Readline)."
             display_completions_like_readline(event)
 
         @handle("c-c", filter=default_focused)
         def _keyboard_interrupt(event: E) -> None:
-            " Abort when Control-C has been pressed. "
+            "Abort when Control-C has been pressed."
             event.app.exit(exception=KeyboardInterrupt, style="class:aborting")
 
         @Condition
         def ctrl_d_condition() -> bool:
-            """ Ctrl-D binding is only active when the default buffer is selected
-            and empty. """
+            """Ctrl-D binding is only active when the default buffer is selected
+            and empty."""
             app = get_app()
             return (
                 app.current_buffer.name == DEFAULT_BUFFER
                 and not app.current_buffer.text
             )
 
         @handle("c-d", filter=ctrl_d_condition & default_focused)
         def _eof(event: E) -> None:
-            " Exit when Control-D has been pressed. "
+            "Exit when Control-D has been pressed."
             event.app.exit(exception=EOFError, style="class:exiting")
 
         suspend_supported = Condition(suspend_to_background_supported)
 
         @Condition
         def enable_suspend() -> bool:
             return to_filter(self.enable_suspend)()
@@ -1083,15 +1084,14 @@
         tempfile: Optional[Union[str, Callable[[], str]]] = None,
         # Following arguments are specific to the current `prompt()` call.
         default: Union[str, Document] = "",
         accept_default: bool = False,
         pre_run: Optional[Callable[[], None]] = None,
         set_exception_handler: bool = True,
     ) -> _T:
-
         if message is not None:
             self.message = message
         if editing_mode is not None:
             self.editing_mode = editing_mode
         if refresh_interval is not None:
             self.refresh_interval = refresh_interval
         if vi_mode:
@@ -1266,27 +1266,27 @@
                 return get_prompt_text_2()
 
         # For the next lines, display the appropriate continuation.
         prompt_width = get_cwidth(fragment_list_to_text(get_prompt_text_2()))
         return self._get_continuation(prompt_width, line_number, wrap_count)
 
     def _get_arg_text(self) -> StyleAndTextTuples:
-        " 'arg' toolbar, for in multiline mode. "
+        "'arg' toolbar, for in multiline mode."
         arg = self.app.key_processor.arg
         if arg is None:
             # Should not happen because of the `has_arg` filter in the layout.
             return []
 
         if arg == "-":
             arg = "-1"
 
         return [("class:arg-toolbar", "Repeat: "), ("class:arg-toolbar.text", arg)]
 
     def _inline_arg(self) -> StyleAndTextTuples:
-        " 'arg' prefix, for in single line mode. "
+        "'arg' prefix, for in single line mode."
         app = get_app()
         if app.key_processor.arg is None:
             return []
         else:
             arg = app.key_processor.arg
 
             return [
@@ -1421,15 +1421,15 @@
     @bindings.add("N")
     def no(event: E) -> None:
         session.default_buffer.text = "n"
         event.app.exit(result=False)
 
     @bindings.add(Keys.Any)
     def _(event: E) -> None:
-        " Disallow inserting other text. "
+        "Disallow inserting other text."
         pass
 
     complete_message = merge_formatted_text([message, suffix])
     session: PromptSession[bool] = PromptSession(
         complete_message, key_bindings=bindings
     )
     return session
```

### Comparing `prot-3.8.6/src/prot/prompt/shortcuts/utils.py` & `prot-3.9.0/src/prot/prompt/shortcuts/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/styles/__init__.py` & `prot-3.9.0/src/prot/prompt/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/styles/base.py` & `prot-3.9.0/src/prot/prompt/styles/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/styles/defaults.py` & `prot-3.9.0/src/prot/prompt/styles/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,19 @@
 
 @memoized()
 def default_ui_style() -> BaseStyle:
     """
     Create a default `Style` object.
     """
     return merge_styles(
-        [Style(PROMPT_TOOLKIT_STYLE), Style(COLORS_STYLE), Style(WIDGETS_STYLE),]
+        [
+            Style(PROMPT_TOOLKIT_STYLE),
+            Style(COLORS_STYLE),
+            Style(WIDGETS_STYLE),
+        ]
     )
 
 
 @memoized()
 def default_pygments_style() -> Style:
     """
     Create a `Style` object that contains the default Pygments style.
```

### Comparing `prot-3.8.6/src/prot/prompt/styles/named_colors.py` & `prot-3.9.0/src/prot/prompt/styles/named_colors.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/styles/pygments.py` & `prot-3.9.0/src/prot/prompt/styles/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/styles/style.py` & `prot-3.9.0/src/prot/prompt/styles/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
     """
     Take a list of :class:`.Attrs` instances and merge them into one.
     Every `Attr` in the list can override the styling of the previous one. So,
     the last one has highest priority.
     """
 
     def _or(*values: _T) -> _T:
-        " Take first not-None value, starting at the end. "
+        "Take first not-None value, starting at the end."
         for v in values[::-1]:
             if v is not None:
                 return v
         raise ValueError  # Should not happen, there's always one non-null value.
 
     return Attrs(
         color=_or("", *[a.color for a in list_of_attrs]),
@@ -371,15 +371,15 @@
     #       because it was more precise.)
     def __init__(self, styles: List[BaseStyle]) -> None:
         self.styles = styles
         self._style: SimpleCache[Hashable, Style] = SimpleCache(maxsize=1)
 
     @property
     def _merged_style(self) -> Style:
-        " The `Style` object that has the other styles merged together. "
+        "The `Style` object that has the other styles merged together."
 
         def get() -> Style:
             return Style(self.style_rules)
 
         return self._style.get(self.invalidation_hash(), get)
 
     @property
```

### Comparing `prot-3.8.6/src/prot/prompt/styles/style_transformation.py` & `prot-3.9.0/src/prot/prompt/styles/style_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         foreground.
     :param bg: Like `fg`, but for the background.
     """
 
     def __init__(
         self, fg: Union[str, Callable[[], str]], bg: Union[str, Callable[[], str]]
     ) -> None:
-
         self.fg = fg
         self.bg = bg
 
     def transform_attrs(self, attrs: Attrs) -> Attrs:
         if attrs.bgcolor in ("", "default"):
             attrs = attrs._replace(bgcolor=parse_color(to_str(self.bg)))
 
@@ -151,15 +150,14 @@
     :param max_brightness: Float between 0.0 and 1.0 or a callable that returns
         a float.
     """
 
     def __init__(
         self, min_brightness: AnyFloat = 0.0, max_brightness: AnyFloat = 1.0
     ) -> None:
-
         self.min_brightness = min_brightness
         self.max_brightness = max_brightness
 
     def transform_attrs(self, attrs: Attrs) -> Attrs:
         min_brightness = to_float(self.min_brightness)
         max_brightness = to_float(self.max_brightness)
         assert 0 <= min_brightness <= 1
@@ -248,15 +246,14 @@
     :param get_style_transformation: Callable that returns a
         :class:`.StyleTransformation` instance.
     """
 
     def __init__(
         self, get_style_transformation: Callable[[], Optional[StyleTransformation]]
     ) -> None:
-
         self.get_style_transformation = get_style_transformation
 
     def transform_attrs(self, attrs: Attrs) -> Attrs:
         style_transformation = (
             self.get_style_transformation() or DummyStyleTransformation()
         )
         return style_transformation.transform_attrs(attrs)
@@ -272,15 +269,14 @@
     """
     Apply the style transformation depending on a condition.
     """
 
     def __init__(
         self, style_transformation: StyleTransformation, filter: FilterOrBool
     ) -> None:
-
         self.style_transformation = style_transformation
         self.filter = to_filter(filter)
 
     def transform_attrs(self, attrs: Attrs) -> Attrs:
         if self.filter():
             return self.style_transformation.transform_attrs(attrs)
         return attrs
```

### Comparing `prot-3.8.6/src/prot/prompt/utils.py` & `prot-3.9.0/src/prot/prompt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,20 +64,20 @@
         self.sender = sender
         self._handlers: List[Callable[[_Sender], None]] = []
 
         if handler is not None:
             self += handler
 
     def __call__(self) -> None:
-        " Fire event. "
+        "Fire event."
         for handler in self._handlers:
             handler(self.sender)
 
     def fire(self) -> None:
-        " Alias for just calling the event. "
+        "Alias for just calling the event."
         self()
 
     def add_handler(self, handler: Callable[[_Sender], None]) -> None:
         """
         Add another handler to this callback.
         (Handler should be a callable that takes exactly one parameter: the
         sender object.)
@@ -206,15 +206,15 @@
     """
     True when the current thread is the main thread.
     """
     return threading.current_thread().__class__.__name__ == "_MainThread"
 
 
 def get_term_environment_variable() -> str:
-    " Return the $TERM environment variable. "
+    "Return the $TERM environment variable."
     return os.environ.get("TERM", "")
 
 
 _T = TypeVar("_T")
 
 
 def take_using_weights(
@@ -268,34 +268,34 @@
                     already_taken[item_i] += 1
                     adding = True
 
         i += 1
 
 
 def to_str(value: Union[Callable[[], str], str]) -> str:
-    " Turn callable or string into string. "
+    "Turn callable or string into string."
     if callable(value):
         return to_str(value())
     else:
         return str(value)
 
 
 def to_int(value: Union[Callable[[], int], int]) -> int:
-    " Turn callable or int into int. "
+    "Turn callable or int into int."
     if callable(value):
         return to_int(value())
     else:
         return int(value)
 
 
 AnyFloat = Union[Callable[[], float], float]
 
 
 def to_float(value: AnyFloat) -> float:
-    " Turn callable or float into float. "
+    "Turn callable or float into float."
     if callable(value):
         return to_float(value())
     else:
         return float(value)
 
 
 def is_dumb_terminal(term: Optional[str] = None) -> bool:
```

### Comparing `prot-3.8.6/src/prot/prompt/validation.py` & `prot-3.9.0/src/prot/prompt/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
     """
     Validate input from a simple callable.
     """
 
     def __init__(
         self, func: Callable[[str], bool], error_message: str, move_cursor_to_end: bool
     ) -> None:
-
         self.func = func
         self.error_message = error_message
         self.move_cursor_to_end = move_cursor_to_end
 
     def __repr__(self) -> str:
         return "Validator.from_callable(%r)" % (self.func,)
```

### Comparing `prot-3.8.6/src/prot/prompt/widgets/__init__.py` & `prot-3.9.0/src/prot/prompt/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/prompt/widgets/base.py` & `prot-3.9.0/src/prot/prompt/widgets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     "ProgressBar",
 ]
 
 E = KeyPressEvent
 
 
 class Border:
-    " Box drawing characters. (Thin) "
+    "Box drawing characters. (Thin)"
     HORIZONTAL = "\u2500"
     VERTICAL = "\u2502"
     TOP_LEFT = "\u250c"
     TOP_RIGHT = "\u2510"
     BOTTOM_LEFT = "\u2514"
     BOTTOM_RIGHT = "\u2518"
 
@@ -184,15 +184,14 @@
         scrollbar: bool = False,
         style: str = "",
         search_field: Optional[SearchToolbar] = None,
         preview_search: FilterOrBool = True,
         prompt: AnyFormattedText = "",
         input_processors: Optional[List[Processor]] = None,
     ) -> None:
-
         if search_field is None:
             search_control = None
         elif isinstance(search_field, SearchToolbar):
             search_control = search_field.control
 
         if input_processors is None:
             input_processors = []
@@ -318,15 +317,14 @@
         self,
         text: AnyFormattedText,
         style: str = "",
         width: AnyDimension = None,
         dont_extend_height: bool = True,
         dont_extend_width: bool = False,
     ) -> None:
-
         self.text = text
 
         def get_width() -> AnyDimension:
             if width is None:
                 text_fragments = to_formatted_text(self.text)
                 text = fragment_list_to_text(text_fragments)
                 if text:
@@ -359,15 +357,14 @@
     :param handler: `None` or callable. Called when the button is clicked.
     :param width: Width of the button.
     """
 
     def __init__(
         self, text: str, handler: Optional[Callable[[], None]] = None, width: int = 12
     ) -> None:
-
         self.text = text
         self.handler = handler
         self.width = width
         self.control = FormattedTextControl(
             self._get_text_fragments,
             key_bindings=self._get_key_bindings(),
             focusable=True,
@@ -403,15 +400,15 @@
             ("class:button.arrow", "<", handler),
             ("[SetCursorPosition]", ""),
             ("class:button.text", text, handler),
             ("class:button.arrow", ">", handler),
         ]
 
     def _get_key_bindings(self) -> KeyBindings:
-        " Key bindings for the Button. "
+        "Key bindings for the Button."
         kb = KeyBindings()
 
         @kb.add(" ")
         @kb.add("enter")
         def _(event: E) -> None:
             if self.handler is not None:
                 self.handler()
@@ -440,15 +437,14 @@
         title: AnyFormattedText = "",
         style: str = "",
         width: AnyDimension = None,
         height: AnyDimension = None,
         key_bindings: Optional[KeyBindings] = None,
         modal: bool = False,
     ) -> None:
-
         self.title = title
         self.body = body
 
         fill = partial(Window, style="class:frame.border")
         style = "class:frame " + style
 
         top_row_with_title = VSplit(
@@ -582,15 +578,14 @@
         width: AnyDimension = None,
         height: AnyDimension = None,
         style: str = "",
         char: Union[None, str, Callable[[], str]] = None,
         modal: bool = False,
         key_bindings: Optional[KeyBindings] = None,
     ) -> None:
-
         if padding is None:
             padding = D(preferred=0)
 
         def get(value: AnyDimension) -> D:
             if value is None:
                 value = padding
             return to_dimension(value)
@@ -698,15 +693,17 @@
         self.control = FormattedTextControl(
             self._get_text_fragments, key_bindings=kb, focusable=True
         )
 
         self.window = Window(
             content=self.control,
             style=self.container_style,
-            right_margins=[ScrollbarMargin(display_arrows=True),],
+            right_margins=[
+                ScrollbarMargin(display_arrows=True),
+            ],
             dont_extend_height=True,
         )
 
     def _handle_enter(self) -> None:
         if self.multiple_selection:
             val = self.values[self._selected_index][0]
             if val in self.current_values:
```

### Comparing `prot-3.8.6/src/prot/prompt/widgets/dialogs.py` & `prot-3.9.0/src/prot/prompt/widgets/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         body: AnyContainer,
         title: AnyFormattedText = "",
         buttons: Optional[Sequence[Button]] = None,
         modal: bool = True,
         width: AnyDimension = None,
         with_background: bool = False,
     ) -> None:
-
         self.body = body
         self.title = title
 
         buttons = buttons or []
 
         # When a button is selected, handle left/right key bindings.
         buttons_kb = KeyBindings()
```

### Comparing `prot-3.8.6/src/prot/prompt/widgets/menus.py` & `prot-3.9.0/src/prot/prompt/widgets/menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     def __init__(
         self,
         body: AnyContainer,
         menu_items: List["MenuItem"],
         floats: Optional[List[Float]] = None,
         key_bindings: Optional[KeyBindingsBase] = None,
     ) -> None:
-
         self.body = body
         self.menu_items = menu_items
         self.selected_menu = [0]
 
         # Key bindings.
         kb = KeyBindings()
 
@@ -74,30 +73,30 @@
         @kb.add("down", filter=in_main_menu)
         def _down(event: E) -> None:
             self.selected_menu.append(0)
 
         @kb.add("c-c", filter=in_main_menu)
         @kb.add("c-g", filter=in_main_menu)
         def _cancel(event: E) -> None:
-            " Leave menu. "
+            "Leave menu."
             event.app.layout.focus_last()
 
         # Sub menu navigation.
 
         @kb.add("left", filter=in_sub_menu)
         @kb.add("c-g", filter=in_sub_menu)
         @kb.add("c-c", filter=in_sub_menu)
         def _back(event: E) -> None:
-            " Go back to parent menu. "
+            "Go back to parent menu."
             if len(self.selected_menu) > 1:
                 self.selected_menu.pop()
 
         @kb.add("right", filter=in_sub_menu)
         def _submenu(event: E) -> None:
-            " go into sub menu. "
+            "go into sub menu."
             if self._get_menu(len(self.selected_menu) - 1).children:
                 self.selected_menu.append(0)
 
             # If This item does not have a sub menu. Go up in the parent menu.
             elif (
                 len(self.selected_menu) == 2
                 and self.selected_menu[0] < len(self.menu_items) - 1
@@ -106,15 +105,15 @@
                     min(len(self.menu_items) - 1, self.selected_menu[0] + 1)
                 ]
                 if self.menu_items[self.selected_menu[0]].children:
                     self.selected_menu.append(0)
 
         @kb.add("up", filter=in_sub_menu)
         def _up_in_submenu(event: E) -> None:
-            " Select previous (enabled) menu item or return to main menu. "
+            "Select previous (enabled) menu item or return to main menu."
             # Look for previous enabled items in this sub menu.
             menu = self._get_menu(len(self.selected_menu) - 2)
             index = self.selected_menu[-1]
 
             previous_indexes = [
                 i
                 for i, item in enumerate(menu.children)
@@ -125,30 +124,30 @@
                 self.selected_menu[-1] = previous_indexes[-1]
             elif len(self.selected_menu) == 2:
                 # Return to main menu.
                 self.selected_menu.pop()
 
         @kb.add("down", filter=in_sub_menu)
         def _down_in_submenu(event: E) -> None:
-            " Select next (enabled) menu item. "
+            "Select next (enabled) menu item."
             menu = self._get_menu(len(self.selected_menu) - 2)
             index = self.selected_menu[-1]
 
             next_indexes = [
                 i
                 for i, item in enumerate(menu.children)
                 if i > index and not item.disabled
             ]
 
             if next_indexes:
                 self.selected_menu[-1] = next_indexes[0]
 
         @kb.add("enter")
         def _click(event: E) -> None:
-            " Click the selected menu item. "
+            "Click the selected menu item."
             item = self._get_menu(len(self.selected_menu) - 1)
             if item.handler:
                 event.app.layout.focus_last()
                 item.handler()
 
         # Controls.
         self.control = FormattedTextControl(
@@ -340,15 +339,14 @@
         self,
         text: str = "",
         handler: Optional[Callable[[], None]] = None,
         children: Optional[List["MenuItem"]] = None,
         shortcut: Optional[Sequence[Union[Keys, str]]] = None,
         disabled: bool = False,
     ) -> None:
-
         self.text = text
         self.handler = handler
         self.children = children or []
         self.shortcut = shortcut
         self.disabled = disabled
         self.selected_item = 0
```

### Comparing `prot-3.8.6/src/prot/prompt/widgets/toolbars.py` & `prot-3.9.0/src/prot/prompt/widgets/toolbars.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     """
 
     def __init__(
         self,
         prompt: AnyFormattedText = "Shell command: ",
         enable_global_bindings: FilterOrBool = True,
     ) -> None:
-
         self.prompt = prompt
         self.enable_global_bindings = to_filter(enable_global_bindings)
 
         self.system_buffer = Buffer(name=SYSTEM_BUFFER)
 
         self._bindings = self._build_key_bindings()
 
@@ -118,43 +117,43 @@
         emacs_bindings = KeyBindings()
         handle = emacs_bindings.add
 
         @handle("escape", filter=focused)
         @handle("c-g", filter=focused)
         @handle("c-c", filter=focused)
         def _cancel(event: E) -> None:
-            " Hide system prompt. "
+            "Hide system prompt."
             self.system_buffer.reset()
             event.app.layout.focus_last()
 
         @handle("enter", filter=focused)
         def _accept(event: E) -> None:
-            " Run system command. "
+            "Run system command."
             event.app.run_system_command(
                 self.system_buffer.text,
                 display_before_text=self._get_display_before_text(),
             )
             self.system_buffer.reset(append_to_history=True)
             event.app.layout.focus_last()
 
         # Vi.
         vi_bindings = KeyBindings()
         handle = vi_bindings.add
 
         @handle("escape", filter=focused)
         @handle("c-c", filter=focused)
         def _cancel_vi(event: E) -> None:
-            " Hide system prompt. "
+            "Hide system prompt."
             event.app.vi_state.input_mode = InputMode.NAVIGATION
             self.system_buffer.reset()
             event.app.layout.focus_last()
 
         @handle("enter", filter=focused)
         def _accept_vi(event: E) -> None:
-            " Run system command. "
+            "Run system command."
             event.app.vi_state.input_mode = InputMode.NAVIGATION
             event.app.run_system_command(
                 self.system_buffer.text,
                 display_before_text=self._get_display_before_text(),
             )
             self.system_buffer.reset(append_to_history=True)
             event.app.layout.focus_last()
@@ -162,20 +161,20 @@
         # Global bindings. (Listen to these bindings, even when this widget is
         # not focussed.)
         global_bindings = KeyBindings()
         handle = global_bindings.add
 
         @handle(Keys.Escape, "!", filter=~focused & emacs_mode, is_global=True)
         def _focus_me(event: E) -> None:
-            " M-'!' will focus this user control. "
+            "M-'!' will focus this user control."
             event.app.layout.focus(self.window)
 
         @handle("!", filter=~focused & vi_mode & vi_navigation_mode, is_global=True)
         def _focus_me_vi(event: E) -> None:
-            " Focus. "
+            "Focus."
             event.app.vi_state.input_mode = InputMode.INSERT
             event.app.layout.focus(self.window)
 
         return merge_key_bindings(
             [
                 ConditionalKeyBindings(emacs_bindings, emacs_mode),
                 ConditionalKeyBindings(vi_bindings, vi_mode),
@@ -218,15 +217,14 @@
         search_buffer: Optional[Buffer] = None,
         vi_mode: bool = False,
         text_if_not_searching: AnyFormattedText = "",
         forward_search_prompt: AnyFormattedText = "I-search: ",
         backward_search_prompt: AnyFormattedText = "I-search backward: ",
         ignore_case: FilterOrBool = False,
     ) -> None:
-
         if search_buffer is None:
             search_buffer = Buffer()
 
         @Condition
         def is_searching() -> bool:
             return self.control in get_app().layout.search_links
```

### Comparing `prot-3.8.6/src/prot/prompt/win32_types.py` & `prot-3.9.0/src/prot/prompt/win32_types.py`

 * *Files identical despite different names*

### Comparing `prot-3.8.6/src/prot/wcwidth/tests/test_core.py` & `prot-3.9.0/src/prot/wcwidth/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 """Core tests module for wcwidth."""
 import prot.wcwidth
 
 
 def test_hello_jp():
-    u"""
+    """
     Width of Japanese phrase: コンニチハ, セカイ!
 
     Given a phrase of 5 and 3 Katakana ideographs, joined with
     3 English-ASCII punctuation characters, totaling 11, this
     phrase consumes 19 cells of a terminal emulator.
     """
     # given,
-    phrase = u'コンニチハ, セカイ!'
+    phrase = "コンニチハ, セカイ!"
     expect_length_each = (2, 2, 2, 2, 2, 1, 1, 2, 2, 2, 1)
     expect_length_phrase = sum(expect_length_each)
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase)
 
@@ -29,30 +29,38 @@
     """
     Test wcswidth() optional 2nd parameter, ``n``.
 
     ``n`` determines at which position of the string
     to stop counting length.
     """
     # given,
-    phrase = u'コンニチハ, セカイ!'
+    phrase = "コンニチハ, セカイ!"
     end = 7
-    expect_length_each = (2, 2, 2, 2, 2, 1, 1,)
+    expect_length_each = (
+        2,
+        2,
+        2,
+        2,
+        2,
+        1,
+        1,
+    )
     expect_length_phrase = sum(expect_length_each)
 
     # exercise,
     length_phrase = wcwidth.wcswidth(phrase, end)
 
     # verify,
     assert length_phrase == expect_length_phrase
 
 
 def test_null_width_0():
     """NULL (0) reports width 0."""
     # given,
-    phrase = u'abc\x00def'
+    phrase = "abc\x00def"
     expect_length_each = (1, 1, 1, 0, 1, 1, 1)
     expect_length_phrase = sum(expect_length_each)
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
 
@@ -60,15 +68,15 @@
     assert length_each == expect_length_each
     assert length_phrase == expect_length_phrase
 
 
 def test_control_c0_width_negative_1():
     """CSI (Control sequence initiate) reports width -1."""
     # given,
-    phrase = u'\x1b[0m'
+    phrase = "\x1b[0m"
     expect_length_each = (-1, 1, 1, 1)
     expect_length_phrase = -1
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
 
@@ -76,60 +84,60 @@
     assert length_each == expect_length_each
     assert length_phrase == expect_length_phrase
 
 
 def test_combining_width_negative_1():
     """Simple test combining reports total width of 4."""
     # given,
-    phrase = u'--\u05bf--'
+    phrase = "--\u05bf--"
     expect_length_each = (1, 1, 0, 1, 1)
     expect_length_phrase = 4
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
 
     # verify,
     assert length_each == expect_length_each
     assert length_phrase == expect_length_phrase
 
 
 def test_combining_cafe():
-    u"""Phrase cafe + COMBINING ACUTE ACCENT is café of length 4."""
-    phrase = u"cafe\u0301"
+    """Phrase cafe + COMBINING ACUTE ACCENT is café of length 4."""
+    phrase = "cafe\u0301"
     expect_length_each = (1, 1, 1, 1, 0)
     expect_length_phrase = 4
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
 
     # verify,
     assert length_each == expect_length_each
     assert length_phrase == expect_length_phrase
 
 
 def test_combining_enclosing():
-    u"""CYRILLIC CAPITAL LETTER A + COMBINING CYRILLIC HUNDRED THOUSANDS SIGN is А҈ of length 1."""
-    phrase = u"\u0410\u0488"
+    """CYRILLIC CAPITAL LETTER A + COMBINING CYRILLIC HUNDRED THOUSANDS SIGN is А҈ of length 1."""
+    phrase = "\u0410\u0488"
     expect_length_each = (1, 0)
     expect_length_phrase = 1
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
 
     # verify,
     assert length_each == expect_length_each
     assert length_phrase == expect_length_phrase
 
 
 def test_combining_spacing():
-    u"""Balinese kapal (ship) is ᬓᬨᬮ᭄ of length 4."""
-    phrase = u"\u1B13\u1B28\u1B2E\u1B44"
+    """Balinese kapal (ship) is ᬓᬨᬮ᭄ of length 4."""
+    phrase = "\u1B13\u1B28\u1B2E\u1B44"
     expect_length_each = (1, 1, 1, 1)
     expect_length_phrase = 4
 
     # exercise,
     length_each = tuple(map(wcwidth.wcwidth, phrase))
     length_phrase = wcwidth.wcswidth(phrase, len(phrase))
```

### Comparing `prot-3.8.6/src/prot/wcwidth/wcwidth.py` & `prot-3.9.0/src/prot/wcwidth/wcwidth.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,34 +74,36 @@
 from .table_zero import ZERO_WIDTH
 
 
 # NOTE: created by hand, there isn't anything identifiable other than
 # general Cf category code to identify these, and some characters in Cf
 # category code are of non-zero width.
 # Also includes some Cc, Mn, Zl, and Zp characters
-ZERO_WIDTH_CF = set([
-    0,       # Null (Cc)
-    0x034F,  # Combining grapheme joiner (Mn)
-    0x200B,  # Zero width space
-    0x200C,  # Zero width non-joiner
-    0x200D,  # Zero width joiner
-    0x200E,  # Left-to-right mark
-    0x200F,  # Right-to-left mark
-    0x2028,  # Line separator (Zl)
-    0x2029,  # Paragraph separator (Zp)
-    0x202A,  # Left-to-right embedding
-    0x202B,  # Right-to-left embedding
-    0x202C,  # Pop directional formatting
-    0x202D,  # Left-to-right override
-    0x202E,  # Right-to-left override
-    0x2060,  # Word joiner
-    0x2061,  # Function application
-    0x2062,  # Invisible times
-    0x2063,  # Invisible separator
-])
+ZERO_WIDTH_CF = set(
+    [
+        0,  # Null (Cc)
+        0x034F,  # Combining grapheme joiner (Mn)
+        0x200B,  # Zero width space
+        0x200C,  # Zero width non-joiner
+        0x200D,  # Zero width joiner
+        0x200E,  # Left-to-right mark
+        0x200F,  # Right-to-left mark
+        0x2028,  # Line separator (Zl)
+        0x2029,  # Paragraph separator (Zp)
+        0x202A,  # Left-to-right embedding
+        0x202B,  # Right-to-left embedding
+        0x202C,  # Pop directional formatting
+        0x202D,  # Left-to-right override
+        0x202E,  # Right-to-left override
+        0x2060,  # Word joiner
+        0x2061,  # Function application
+        0x2062,  # Invisible times
+        0x2063,  # Invisible separator
+    ]
+)
 
 UBOUND_ZERO_WIDTH = len(ZERO_WIDTH) - 1
 UBOUND_WIDE_EASTASIAN = len(WIDE_EASTASIAN) - 1
 
 
 def _bisearch(ucs, table, ubound):
     """
```

### Comparing `prot-3.8.6/src/prot.egg-info/PKG-INFO` & `prot-3.9.0/src/prot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prot
-Version: 3.8.6
+Version: 3.9.0
 Summary: A Simple Tool That Contains Advance Functions.
 Home-page: https://github.com/SAPTeamDEV/prot
 Author: Alireza Poodineh
 Author-email: itsaeliux@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

