# Comparing `tmp/python-cowsay-1.1.0.tar.gz` & `tmp/python-cowsay-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cowsay-1.1.0.tar", last modified: Sat Apr 22 02:58:39 2023, max compression
+gzip compressed data, was "python-cowsay-1.1.1.tar", last modified: Fri Jun 16 07:11:44 2023, max compression
```

## Comparing `python-cowsay-1.1.0.tar` & `python-cowsay-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.717794 python-cowsay-1.1.0/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-04-22 02:58:39.717662 python-cowsay-1.1.0/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4265 2023-04-22 02:40:00.000000 python-cowsay-1.1.0/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      762 2023-04-22 02:58:34.000000 python-cowsay-1.1.0/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-04-22 02:58:39.717831 python-cowsay-1.1.0/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.706985 python-cowsay-1.1.0/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.707488 python-cowsay-1.1.0/src/cowsay/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     8356 2023-04-22 02:27:59.000000 python-cowsay-1.1.0/src/cowsay/__init__.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.716932 python-cowsay-1.1.0/src/cowsay/cows/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      793 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/TuxStab.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      356 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/armadillo.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      205 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/banana.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      174 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bill-the-cat.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      639 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/blowfish.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      310 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bud-frogs.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      123 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bunny.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      625 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cat.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      480 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cheese.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      250 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/clippy.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      230 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cower.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      569 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/daemon.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      175 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/default.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1284 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/dragon-and-cow.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1000 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/dragon.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      295 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant-in-snake.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      284 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      275 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant2.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      585 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/eyes.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      267 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/fat-banana.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      487 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/flaming-sheep.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      283 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/frogs.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      460 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/ghost.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      411 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/happy-whale.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      257 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/head-in.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      126 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/hellokitty.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      637 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kiss.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      217 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kitten.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      296 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kitty.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      162 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/koala.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      181 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/llama.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      628 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/lobster.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      151 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/lollerskates.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      473 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/meow.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      439 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/milk.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      242 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/moofasa.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      203 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/moose.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      201 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/mutilated.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      884 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/octopus.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      141 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/owl.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      186 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/satanic.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      291 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/seahorse.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      232 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/sheep.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      433 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/skeleton.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      194 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/small.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      854 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/stegosaurus.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      364 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/stimpy.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      280 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/supermilker.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      892 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/surgery.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      428 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/taxi.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      293 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/three-eyes.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1302 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/turkey.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1105 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/turtle.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      215 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/tux.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      392 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/udder.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      317 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/whale.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      248 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/www.cow
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.717471 python-cowsay-1.1.0/src/python_cowsay.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1817 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        7 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:11:44.848067 python-cowsay-1.1.1/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-06-16 07:11:44.847923 python-cowsay-1.1.1/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4265 2023-04-22 02:40:00.000000 python-cowsay-1.1.1/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      762 2023-06-16 06:48:55.000000 python-cowsay-1.1.1/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-06-16 07:11:44.848106 python-cowsay-1.1.1/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:11:44.837363 python-cowsay-1.1.1/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:11:44.837862 python-cowsay-1.1.1/src/cowsay/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     8417 2023-06-16 06:37:53.000000 python-cowsay-1.1.1/src/cowsay/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:11:44.847161 python-cowsay-1.1.1/src/cowsay/cows/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      793 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/TuxStab.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      356 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/armadillo.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      205 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/banana.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      174 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/bill-the-cat.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      639 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/blowfish.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      310 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/bud-frogs.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      123 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/bunny.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      625 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/cat.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      480 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/cheese.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      250 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/clippy.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      230 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/cower.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      569 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/daemon.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      175 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/default.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1284 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/dragon-and-cow.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1000 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/dragon.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      295 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/elephant-in-snake.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      284 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/elephant.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      275 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/elephant2.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      585 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/eyes.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      267 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/fat-banana.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      487 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/flaming-sheep.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      283 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/frogs.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      460 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/ghost.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      411 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/happy-whale.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      257 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/head-in.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      126 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/hellokitty.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      637 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/kiss.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      217 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/kitten.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      296 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/kitty.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      162 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/koala.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      181 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/llama.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      628 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/lobster.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      151 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/lollerskates.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      473 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/meow.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      439 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/milk.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      242 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/moofasa.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      203 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/moose.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      201 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/mutilated.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      884 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/octopus.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      141 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/owl.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      186 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/satanic.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      291 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/seahorse.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      232 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/sheep.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      433 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/skeleton.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      194 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/small.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      854 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/stegosaurus.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      364 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/stimpy.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      280 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/supermilker.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      892 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/surgery.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      428 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/taxi.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      293 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/three-eyes.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1302 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/turkey.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1105 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/turtle.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      215 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/tux.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      392 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/udder.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      317 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/whale.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      248 2022-12-09 22:56:36.000000 python-cowsay-1.1.1/src/cowsay/cows/www.cow
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-16 07:11:44.847697 python-cowsay-1.1.1/src/python_cowsay.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-06-16 07:11:44.000000 python-cowsay-1.1.1/src/python_cowsay.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1817 2023-06-16 07:11:44.000000 python-cowsay-1.1.1/src/python_cowsay.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-06-16 07:11:44.000000 python-cowsay-1.1.1/src/python_cowsay.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        7 2023-06-16 07:11:44.000000 python-cowsay-1.1.1/src/python_cowsay.egg-info/top_level.txt
```

### Comparing `python-cowsay-1.1.0/LICENSE` & `python-cowsay-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/PKG-INFO` & `python-cowsay-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cowsay
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Cowsay clone in Python
 Author: James Finnie-Ansley
 License: MIT License
         
         Copyright (c) 2022 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,15 @@
 Project-URL: repository, https://github.com/James-Ansley/cowsay
 Keywords: cowsay
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Cowsay
 
 A rewrite of cowsay in python. Allows for parsing of existing `.cow` files.
```

### Comparing `python-cowsay-1.1.0/README.md` & `python-cowsay-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/pyproject.toml` & `python-cowsay-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-cowsay"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Cowsay clone in Python"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["cowsay"]
 authors = [{ name = "James Finnie-Ansley" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
```

### Comparing `python-cowsay-1.1.0/src/cowsay/__init__.py` & `python-cowsay-1.1.1/src/cowsay/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import re
 from dataclasses import dataclass
 from os import PathLike
 from pathlib import Path, PurePath
 from textwrap import wrap
-from typing import TextIO
+from typing import TextIO, Union, Dict, List
 from unicodedata import east_asian_width
 
 HEREDOC_PATTERN = re.compile(
     r'\$.* = <<["\']?(.*)["\']?;?(?P<the_cow>[\w\W]*)\1'
 )
 
 
@@ -44,25 +44,24 @@
     bl: str = '\\'
     br: str = '/'
 
 
 THOUGHT_OPTIONS = {
     'cowsay': Bubble('\\', '<', '>', '/', '\\', '|', '|', '\\', '/'),
     'cowthink': Bubble('o', '(', ')', '(', ')', '(', ')', '(', ')'),
-    'cowsay': Bubble('\\', '<', '>', '/', '\\', '|', '|', '\\', '/'),
 }
 
 ESCAPES = {
     r'\@': '@',
     r'\$': '$',
     r'\\': '\\',
 }
 
 
-def read_dot_cow(f: TextIO, escapes: dict[str, str] = None) -> str:
+def read_dot_cow(f: TextIO, escapes: Dict[str, str] = None) -> str:
     """
     Reads and parses a .cow file to a string. Unescapes characters in doing
     so. This function will search for a heredoc in the .cow file. If found,
     it will extract the cow in the heredoc, otherwise the whole file is used.
 
     :param f: The File to read from
     :param escapes: A dictionary mapping escape codes to their respective
@@ -76,21 +75,21 @@
     if match is not None:
         the_cow = match.group('the_cow')
     for escape, replacement in escapes.items():
         the_cow = the_cow.replace(escape, replacement)
     return the_cow.strip('\r\n')
 
 
-def list_cows(cow_path: str | PathLike[str] = COW_PEN):
+def list_cows(cow_path: Union[str, PathLike] = COW_PEN):
     """Lists all cow file names in the given directory"""
     cows = Path(cow_path).glob('*.cow')
     return [cow.stem for cow in cows]
 
 
-def get_random_cow(path: str | PathLike[str] = COW_PEN) -> str:
+def get_random_cow(path: Union[str, PathLike] = COW_PEN) -> str:
     """
     Searches the given dir for all .cow files and returns the name of a
     random one
     """
     cows = list_cows(path)
     return random.choice(cows)
 
@@ -131,15 +130,15 @@
         wrap_text=wrap_text,
     )
     return '\n'.join((message, the_cow))
 
 
 def fit_text(text: str,
              width: int,
-             wrap_text: bool = True) -> list[str]:
+             wrap_text: bool = True) -> List[str]:
     """
     Wraps each paragraph in the given text to the specified width and pads
     each line such that they are all the same length with at least one space
     of padding. If wrap_text is False, paragraphs are not wrapped but are
     still padded with spaces.
     """
     text = text.replace('\t', ' ' * 4)
@@ -156,15 +155,15 @@
 
 
 def pad_lines(lines):
     max_width = max(len(line) for line in lines)
     return [f' {line:<{max_width}} ' for line in lines]
 
 
-def wrap_bubble(lines: list[str], ops: Bubble) -> str:
+def wrap_bubble(lines: List[str], ops: Bubble) -> str:
     """
     Puts text into a text bubble. This is done by just inserting the given
     bracket characters onto the ends of each line.
     """
     res = [*f' {"_" * len(lines[0])} \n']
     if len(lines) == 1:
         res += f'{ops.l}{lines[0]}{ops.r}\n'
@@ -206,22 +205,22 @@
     If any full-width characters are found, convert all characters to full width
     """
     if any(east_asian_width(c) in ("W", "F", "A") for c in cow):
         return to_full_width(cow)
     return cow
 
 
-def cowsay(message,
-           cow='default',
-           preset=None,
-           eyes=Option.eyes,
-           tongue=Option.tongue,
-           width=40,
-           wrap_text=True,
-           cowfile=None) -> str:
+def cowsay(message: str,
+           cow: str = 'default',
+           preset: str = None,
+           eyes: str = Option.eyes,
+           tongue: str = Option.tongue,
+           width: int = 40,
+           wrap_text: bool = True,
+           cowfile: str = None) -> str:
     """
     Similar to the cowsay command. Parameters are listed with their
     corresponding options in the cowsay command. Returns the resulting cowsay
     string
 
     :param message: The message to be displayed
     :param cow: -f – the available cows can be found by calling list_cows
@@ -236,22 +235,22 @@
     """
     the_cow = get_cow(cow) if cowfile is None else cowfile
     cow_ops = COW_OPTIONS.get(preset, Option(eyes=eyes, tongue=tongue))
     thought_ops = THOUGHT_OPTIONS['cowsay']
     return build_cow(message, the_cow, cow_ops, thought_ops, width, wrap_text)
 
 
-def cowthink(message,
-             cow='default',
-             preset=None,
-             eyes=Option.eyes,
-             tongue=Option.tongue,
-             width=40,
-             wrap_text=True,
-             cowfile=None) -> str:
+def cowthink(message: str,
+             cow: str = 'default',
+             preset: str = None,
+             eyes: str = Option.eyes,
+             tongue: str = Option.tongue,
+             width: int = 40,
+             wrap_text: bool = True,
+             cowfile: str = None) -> str:
     """
     Similar to the cowthink command. Parameters are listed with their
     corresponding options in the cowthink command. Returns the resulting
     cowthink string
 
     :param message: The message to be displayed
     :param cow: -f – the available cows can be found by calling list_cows
```

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/TuxStab.cow` & `python-cowsay-1.1.1/src/cowsay/cows/TuxStab.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/blowfish.cow` & `python-cowsay-1.1.1/src/cowsay/cows/blowfish.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/cat.cow` & `python-cowsay-1.1.1/src/cowsay/cows/cat.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/daemon.cow` & `python-cowsay-1.1.1/src/cowsay/cows/daemon.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/dragon-and-cow.cow` & `python-cowsay-1.1.1/src/cowsay/cows/dragon-and-cow.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/dragon.cow` & `python-cowsay-1.1.1/src/cowsay/cows/dragon.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/eyes.cow` & `python-cowsay-1.1.1/src/cowsay/cows/eyes.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/kiss.cow` & `python-cowsay-1.1.1/src/cowsay/cows/kiss.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/lobster.cow` & `python-cowsay-1.1.1/src/cowsay/cows/lobster.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/octopus.cow` & `python-cowsay-1.1.1/src/cowsay/cows/octopus.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/stegosaurus.cow` & `python-cowsay-1.1.1/src/cowsay/cows/stegosaurus.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/surgery.cow` & `python-cowsay-1.1.1/src/cowsay/cows/surgery.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/turkey.cow` & `python-cowsay-1.1.1/src/cowsay/cows/turkey.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/cowsay/cows/turtle.cow` & `python-cowsay-1.1.1/src/cowsay/cows/turtle.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.1.0/src/python_cowsay.egg-info/PKG-INFO` & `python-cowsay-1.1.1/src/python_cowsay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cowsay
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Cowsay clone in Python
 Author: James Finnie-Ansley
 License: MIT License
         
         Copyright (c) 2022 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,15 @@
 Project-URL: repository, https://github.com/James-Ansley/cowsay
 Keywords: cowsay
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Cowsay
 
 A rewrite of cowsay in python. Allows for parsing of existing `.cow` files.
```

### Comparing `python-cowsay-1.1.0/src/python_cowsay.egg-info/SOURCES.txt` & `python-cowsay-1.1.1/src/python_cowsay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

