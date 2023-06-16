# Comparing `tmp/BayesBoom-0.1.8.tar.gz` & `tmp/BayesBoom-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BayesBoom-0.1.8.tar", last modified: Thu Sep 22 16:35:47 2022, max compression
+gzip compressed data, was "BayesBoom-0.1.9.tar", last modified: Mon Sep 26 17:08:39 2022, max compression
```

## Comparing `BayesBoom-0.1.8.tar` & `BayesBoom-0.1.9.tar`

### file list

```diff
@@ -1,1714 +1,1714 @@
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.214100 BayesBoom-0.1.8/BayesBoom/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.214100 BayesBoom-0.1.8/BayesBoom/R/
--rw-r--r--   0 steve     (1000) steve     (1000)    10387 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/R.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1965 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    20219 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/autoclean.py
--rw-r--r--   0 steve     (1000) steve     (1000)    13212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/bayes.py
--rw-r--r--   0 steve     (1000) steve     (1000)     3915 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/boom_py_utils.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2615 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/cbind.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/data_table.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1954 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/density.py
--rw-r--r--   0 steve     (1000) steve     (1000)    27891 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/encoding.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4949 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/graphics_device.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1764 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/mcmc.py
--rw-r--r--   0 steve     (1000) steve     (1000)    26826 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/plots.py
--rw-r--r--   0 steve     (1000) steve     (1000)     8968 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/probability.py
--rw-r--r--   0 steve     (1000) steve     (1000)      479 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/stats.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1597 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_R.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2461 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_cbind.py
--rw-r--r--   0 steve     (1000) steve     (1000)     6231 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_data_table.py
--rw-r--r--   0 steve     (1000) steve     (1000)     6745 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_encoding.py
--rw-r--r--   0 steve     (1000) steve     (1000)     3946 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_plots.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4134 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_probability.py
--rw-r--r--   0 steve     (1000) steve     (1000)      386 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_utilities.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1337 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/test_utils.py
--rw-r--r--   0 steve     (1000) steve     (1000)     3176 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/R/utils.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.218099 BayesBoom-0.1.8/BayesBoom/boom/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.222099 BayesBoom-0.1.8/BayesBoom/boom/Bmath/
--rw-r--r--   0 steve     (1000) steve     (1000)    14088 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/Bmath.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2455 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/Random.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2741 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/bd0.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5467 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/bessel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17474 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/bessel_k.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3469 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/beta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3172 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/chebyshev.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2715 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/choose.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2634 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/d1mach.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3596 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3409 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2187 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dcauchy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1872 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2746 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/df.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3193 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dgamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2261 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dgeom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3066 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dhyper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2267 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dlnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2154 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dlogis.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3687 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2566 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3197 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2348 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2678 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dpois.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5792 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dpq.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2559 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2055 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dunif.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2279 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/dweibull.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4224 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/fprec.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3757 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/fround.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2001 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/fsign.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1851 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/ftrunc.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9866 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/gamma_cody.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3443 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/gammalims.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2413 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/i1mach.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3030 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/lbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4380 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/lgammacor.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)      469 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/mathlib_error.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5606 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/mlutils.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4533 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/nmath.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2277 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2263 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pcauchy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1914 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2367 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2412 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5819 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pgamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2180 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pgeom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6963 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/phyper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2094 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/plnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2325 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/plogis.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4093 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2297 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4340 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2215 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9866 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5487 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13905 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/polygamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2177 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/ppois.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2858 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13714 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/ptukey.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2101 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/punif.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2343 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/pweibull.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6386 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4154 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2210 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qcauchy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2071 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2416 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5875 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qgamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2227 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qgeom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3351 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qhyper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2128 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qlnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2427 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qlogis.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4252 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2998 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8385 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4046 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qpois.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5782 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6663 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qtukey.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2044 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qunif.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2174 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/qweibull.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5480 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rbeta.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7330 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2172 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rcauchy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2148 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2073 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2275 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7446 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rgamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rgeom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10786 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rhyper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2164 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rlnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2943 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rloggamma_small_alpha.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2088 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rlogis.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4629 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rmultinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2585 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnbinom.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3286 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnchisq.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2402 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9111 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rpois.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2296 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2050 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/runif.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2104 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/rweibull.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3204 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/sexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1988 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/sign.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11122 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/snorm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4539 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/stirlerr.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    60559 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/toms708.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1770 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Bmath/unif_rand.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.226099 BayesBoom-0.1.8/BayesBoom/boom/Eigen/
--rw-r--r--   0 steve     (1000) steve     (1000)     1161 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Cholesky
--rw-r--r--   0 steve     (1000) steve     (1000)     1900 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/CholmodSupport
--rw-r--r--   0 steve     (1000) steve     (1000)    12799 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Core
--rw-r--r--   0 steve     (1000) steve     (1000)      122 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Dense
--rw-r--r--   0 steve     (1000) steve     (1000)       35 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Eigen
--rw-r--r--   0 steve     (1000) steve     (1000)     1777 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Eigenvalues
--rw-r--r--   0 steve     (1000) steve     (1000)     1940 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Geometry
--rw-r--r--   0 steve     (1000) steve     (1000)      829 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Householder
--rw-r--r--   0 steve     (1000) steve     (1000)     2083 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/IterativeLinearSolvers
--rw-r--r--   0 steve     (1000) steve     (1000)      894 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Jacobi
--rw-r--r--   0 steve     (1000) steve     (1000)     1389 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/KLUSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     1268 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/LU
--rw-r--r--   0 steve     (1000) steve     (1000)      991 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/MetisSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     2451 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/OrderingMethods
--rw-r--r--   0 steve     (1000) steve     (1000)     1751 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/PaStiXSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     1116 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/PardisoSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     1272 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/QR
--rw-r--r--   0 steve     (1000) steve     (1000)      900 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/QtAlignedMalloc
--rw-r--r--   0 steve     (1000) steve     (1000)     1162 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SPQRSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     1584 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SVD
--rw-r--r--   0 steve     (1000) steve     (1000)      888 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/Sparse
--rw-r--r--   0 steve     (1000) steve     (1000)     1235 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseCholesky
--rw-r--r--   0 steve     (1000) steve     (1000)     2240 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseCore
--rw-r--r--   0 steve     (1000) steve     (1000)     1814 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseLU
--rw-r--r--   0 steve     (1000) steve     (1000)     1195 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseQR
--rw-r--r--   0 steve     (1000) steve     (1000)      797 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdDeque
--rw-r--r--   0 steve     (1000) steve     (1000)      726 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdList
--rw-r--r--   0 steve     (1000) steve     (1000)      803 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdVector
--rw-r--r--   0 steve     (1000) steve     (1000)     2243 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/SuperLUSupport
--rw-r--r--   0 steve     (1000) steve     (1000)     1382 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/UmfPackSupport
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.210100 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.226099 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/
--rw-r--r--   0 steve     (1000) steve     (1000)    24934 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 steve     (1000) steve     (1000)    18760 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3974 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.226099 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/CholmodSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    25441 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/
--rw-r--r--   0 steve     (1000) steve     (1000)    19214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 steve     (1000) steve     (1000)    16782 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Array.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7018 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2738 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Assign.h
--rw-r--r--   0 steve     (1000) steve     (1000)    41673 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)    12488 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14075 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    18648 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Block.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4429 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5981 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6990 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 steve     (1000) steve     (1000)    63841 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4745 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7909 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)    36282 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3937 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5551 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 steve     (1000) steve     (1000)    31529 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)    24484 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)    25360 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9870 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14670 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)      988 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11654 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Dot.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5841 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4909 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5759 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21679 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)    38812 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11543 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8238 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/IO.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9620 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3503 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Inverse.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Map.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11281 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MapBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)    60784 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7156 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 steve     (1000) steve     (1000)    24343 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Matrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    23856 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2520 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3620 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12884 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9207 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 steve     (1000) steve     (1000)    20748 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    49193 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7336 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Product.h
--rw-r--r--   0 steve     (1000) steve     (1000)    53832 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7756 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Random.h
--rw-r--r--   0 steve     (1000) steve     (1000)    19195 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Redux.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17821 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Ref.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5656 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Replicate.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17033 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4284 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7522 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Reverse.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6143 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Select.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14999 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1697 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6837 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Solve.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9368 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6170 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8700 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21641 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Stride.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2765 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Swap.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17606 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Transpose.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13567 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    38277 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3488 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 steve     (1000) steve     (1000)    35168 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11997 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.210100 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 steve     (1000) steve     (1000)    15223 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8102 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    64608 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2564 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 steve     (1000) steve     (1000)    17160 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13344 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    87891 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2134 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 steve     (1000) steve     (1000)    16540 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2323 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)   119355 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9490 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 steve     (1000) steve     (1000)    24820 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)   102394 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 steve     (1000) steve     (1000)    17317 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/
--rw-r--r--   0 steve     (1000) steve     (1000)    26903 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5251 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 steve     (1000) steve     (1000)    67696 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3770 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 steve     (1000) steve     (1000)    35534 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1746 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3746 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 steve     (1000) steve     (1000)     2695 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    57047 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.210100 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 steve     (1000) steve     (1000)      691 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 steve     (1000) steve     (1000)    17541 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)    16159 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    33615 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.230098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 steve     (1000) steve     (1000)    22503 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6815 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3083 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)   189525 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)    51286 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 steve     (1000) steve     (1000)    14251 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6765 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)    64465 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3650 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 steve     (1000) steve     (1000)     1194 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21200 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1351 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 steve     (1000) steve     (1000)     7428 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12539 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 steve     (1000) steve     (1000)    27786 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21856 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 steve     (1000) steve     (1000)    16728 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8024 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)    36894 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/
--rw-r--r--   0 steve     (1000) steve     (1000)     6686 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 steve     (1000) steve     (1000)    20921 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8334 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4998 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 steve     (1000) steve     (1000)      607 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 steve     (1000) steve     (1000)    40146 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.234098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/
--rw-r--r--   0 steve     (1000) steve     (1000)   108448 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 steve     (1000) steve     (1000)    20104 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15948 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6936 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5106 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21724 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6368 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5582 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21354 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11570 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9958 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5209 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6164 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4126 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 steve     (1000) steve     (1000)    20987 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13867 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14722 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)    10571 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14678 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6707 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5882 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/
--rwxr-xr-x   0 steve     (1000) steve     (1000)    23156 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 steve     (1000) steve     (1000)    19876 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21931 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)     4892 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15555 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6696 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 steve     (1000) steve     (1000)    10949 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/IntegralConstant.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)     4268 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 steve     (1000) steve     (1000)    52909 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 steve     (1000) steve     (1000)    46661 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)    29336 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 steve     (1000) steve     (1000)       85 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1024 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1432 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 steve     (1000) steve     (1000)    10676 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12003 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 steve     (1000) steve     (1000)    35762 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/
--rw-r--r--   0 steve     (1000) steve     (1000)    12559 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17274 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4178 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 steve     (1000) steve     (1000)    22970 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17176 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9716 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14349 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5575 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 steve     (1000) steve     (1000)    23640 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21078 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3650 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 steve     (1000) steve     (1000)    35182 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4104 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 steve     (1000) steve     (1000)    22764 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/
--rw-r--r--   0 steve     (1000) steve     (1000)    18939 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8403 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3624 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 steve     (1000) steve     (1000)    20726 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11962 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8955 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9812 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 steve     (1000) steve     (1000)    34367 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6862 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8063 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6724 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 steve     (1000) steve     (1000)    61930 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7664 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6190 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/arch/
--rw-r--r--   0 steve     (1000) steve     (1000)     5945 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/
--rw-r--r--   0 steve     (1000) steve     (1000)     4784 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5365 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/Householder.h
--rw-r--r--   0 steve     (1000) steve     (1000)    23611 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 steve     (1000) steve     (1000)     6771 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6850 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8887 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15036 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14940 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13379 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7349 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Jacobi/
--rw-r--r--   0 steve     (1000) steve     (1000)    16383 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/KLUSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    11555 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/
--rw-r--r--   0 steve     (1000) steve     (1000)     3439 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/Determinant.h
--rw-r--r--   0 steve     (1000) steve     (1000)    32383 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15727 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 steve     (1000) steve     (1000)    22069 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3555 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/arch/
--rw-r--r--   0 steve     (1000) steve     (1000)    13693 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/MetisSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)     4588 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/
--rw-r--r--   0 steve     (1000) steve     (1000)    16105 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 steve     (1000) steve     (1000)    61681 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5248 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PaStiXSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    22249 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.238098 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PardisoSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    20092 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/
--rw-r--r--   0 steve     (1000) steve     (1000)    25498 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4662 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 steve     (1000) steve     (1000)    23429 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 steve     (1000) steve     (1000)    26768 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14641 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2993 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SPQRSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    11826 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/
--rw-r--r--   0 steve     (1000) steve     (1000)    54214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 steve     (1000) steve     (1000)    32988 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5099 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14743 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15957 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCholesky/
--rw-r--r--   0 steve     (1000) steve     (1000)    24216 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5830 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/
--rw-r--r--   0 steve     (1000) steve     (1000)    10670 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8743 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13166 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2191 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    11368 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 steve     (1000) steve     (1000)    24360 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6485 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13606 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)    25524 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4757 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 steve     (1000) steve     (1000)    13256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5808 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3080 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1107 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12589 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 steve     (1000) steve     (1000)    57475 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)    17451 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7329 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7593 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1699 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 steve     (1000) steve     (1000)    15600 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 steve     (1000) steve     (1000)    25889 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4424 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8704 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3175 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6437 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6827 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 steve     (1000) steve     (1000)    14832 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8127 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9657 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/
--rw-r--r--   0 steve     (1000) steve     (1000)    33316 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4303 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7602 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4974 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12837 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2049 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6712 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6584 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3681 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 steve     (1000) steve     (1000)    10217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4181 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5723 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 steve     (1000) steve     (1000)     8485 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 steve     (1000) steve     (1000)     9028 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4979 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4545 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2889 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseQR/
--rw-r--r--   0 steve     (1000) steve     (1000)    29167 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)     4730 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4155 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 steve     (1000) steve     (1000)     5338 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2809 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.242097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SuperLUSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    34324 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.246097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/UmfPackSupport/
--rw-r--r--   0 steve     (1000) steve     (1000)    24456 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.246097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/
--rw-r--r--   0 steve     (1000) steve     (1000)     2913 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/Image.h
--rw-r--r--   0 steve     (1000) steve     (1000)     2742 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/Kernel.h
--rw-r--r--   0 steve     (1000) steve     (1000)     1748 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 steve     (1000) steve     (1000)    30560 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/blas.h
--rw-r--r--   0 steve     (1000) steve     (1000)     7834 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 steve     (1000) steve     (1000)  1058369 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/lapacke.h
--rw-r--r--   0 steve     (1000) steve     (1000)      474 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.246097 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/
--rw-r--r--   0 steve     (1000) steve     (1000)    14060 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)    21431 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)    59020 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 steve     (1000) steve     (1000)     4828 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6089 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)    12283 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6387 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)     3350 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 steve     (1000) steve     (1000)     6915 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ReshapedMethods.h
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.246097 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/
--rw-r--r--   0 steve     (1000) steve     (1000)    32356 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Array.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17692 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Array.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5300 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/ArrayIterator.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4569 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/ArrayIterator.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4726 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Cholesky.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3114 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Cholesky.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3770 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/CorrelationMatrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2343 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/CorrelationMatrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10711 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/DiagonalMatrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7295 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/DiagonalMatrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5110 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Eigen.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4179 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Eigen.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3075 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/EigenMap.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4361 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Givens.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1711 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Givens.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4997 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/LU.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2493 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/LU.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    43968 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Matrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    21468 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Matrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2907 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/MatrixPartition.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2023 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/MatrixPartition.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4280 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/QR.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3369 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/QR.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3252 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SVD.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1967 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SVD.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3616 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SWEEP.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4191 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SWEEP.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    24476 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Selector.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14090 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Selector.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    22351 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SpdMatrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12246 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SpdMatrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    21032 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SubMatrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9655 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SubMatrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    28588 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Vector.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15270 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Vector.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15255 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorView.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13937 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorView.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5890 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorViewIterator.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1182 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/stack_columns.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1042 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/LinAlg/stack_columns.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.254097 BayesBoom-0.1.8/BayesBoom/boom/Models/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.254097 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/
--rw-r--r--   0 steve     (1000) steve     (1000)    49256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/Bart.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    32137 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/Bart.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2282 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianBartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2834 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianBartModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3644 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2545 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3342 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/LogitBartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/LogitBartModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5313 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PoissonBartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3669 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PoissonBartModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.254097 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)    44524 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14564 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7895 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6611 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4270 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2284 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13591 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6863 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10969 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12867 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8694 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4985 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3370 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ProbitBartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2208 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ProbitBartModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2700 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ResidualRegressionData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3707 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ResidualRegressionData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)      821 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BernoulliModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12653 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BetaBinomialModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6105 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BetaBinomialModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7841 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BetaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4208 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BetaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8085 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BinomialModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5008 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/BinomialModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12814 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CategoricalData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11257 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CategoricalData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3252 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ChisqModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2417 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ChisqModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1589 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2097 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2611 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3176 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5222 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ConstrainedVectorParams.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5687 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ConstrainedVectorParams.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1870 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DataPair.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4337 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DataTypes.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7549 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DataTypes.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7754 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DirichletModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4021 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DirichletModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1618 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DiscreteUniformModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1892 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DiscreteUniformModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3121 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/DoubleModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2575 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/EmMixtureComponent.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3061 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialIncrementModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2655 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialIncrementModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5389 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3680 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10543 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/FiniteMixtureModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6345 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/FiniteMixtureModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11231 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6000 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3425 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2319 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7367 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6581 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3823 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelGivenSigma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3421 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelGivenSigma.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.258096 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/
--rw-r--r--   0 steve     (1000) steve     (1000)    12614 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9536 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7332 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialLogitModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4010 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialLogitModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10076 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialProbitModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3905 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialProbitModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2427 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialRegressionData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2126 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialRegressionData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3988 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ChoiceData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4387 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ChoiceData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13227 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GammaRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8175 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GammaRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3054 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/Glm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7762 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/Glm.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11581 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmCoefs.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7142 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmCoefs.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3012 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmMvnPriorBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3527 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2793 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1715 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/IndependentRegressionModels.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2102 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/IndependentRegressionModels.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5252 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LogisticRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3558 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LogisticRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15690 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LoglinearModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14955 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LoglinearModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ModelSelectionConcepts.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13665 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialLogitModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9541 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialLogitModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9731 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialProbitModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4969 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialProbitModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9559 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultivariateRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8264 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultivariateRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12066 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvnGivenX.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14175 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvnGivenX.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4966 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvtRegModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2870 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvtRegModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17582 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10927 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2785 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2605 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4752 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3987 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.266096 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     9585 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6223 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2478 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1855 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8481 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5924 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4926 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6361 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10902 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4166 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9540 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8640 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2526 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2194 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2993 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3766 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8610 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3815 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2539 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3171 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2678 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2658 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2874 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2621 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3819 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1741 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18303 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11159 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4096 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3667 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11888 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4263 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6607 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3323 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8510 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7435 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2669 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/IndependentRegressionModelsPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2903 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2265 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4561 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1727 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3327 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1885 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1566 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1896 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6302 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4862 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3025 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2631 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1605 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2524 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2027 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1848 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1462 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2360 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2082 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11276 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2529 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2353 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13016 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7843 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3445 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2226 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4314 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4189 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    19527 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10834 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1120 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1282 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3785 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2887 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8362 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3814 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4600 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4807 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6175 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5486 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1650 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3862 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3325 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2421 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2015 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4936 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2243 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3342 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6063 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2711 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3184 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2733 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2425 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5876 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2868 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4421 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4408 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18383 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12175 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7604 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2168 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6586 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4992 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2734 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2128 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5148 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2422 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1946 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedGammaRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4611 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5058 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10518 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3544 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1179 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    24944 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_1.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    37882 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_2.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    36405 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_3.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2474 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1615 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5123 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ProbitRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2950 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ProbitRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1372 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/QuantileRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2894 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/QuantileRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    25293 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    19860 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3340 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionSlabPrior.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5286 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionSlabPrior.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8699 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/TRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3703 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/TRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18211 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/VariableSelectionPrior.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11282 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/VariableSelectionPrior.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10314 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/WeightedRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6246 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/WeightedRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4537 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4325 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5542 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4072 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5057 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5284 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.266096 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.266096 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/
--rw-r--r--   0 steve     (1000) steve     (1000)     1261 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Event.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1914 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Event.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    28929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8485 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.266096 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     1859 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2507 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Session.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2001 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Session.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2774 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Stream.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1807 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Stream.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4192 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmm.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3618 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3229 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9550 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HMM2.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5190 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HMM2.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8130 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HealthStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5268 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HealthStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3206 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1933 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8250 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmFilter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3293 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmFilter.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.270096 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     2865 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1984 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4305 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2726 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/hmm_tools.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1188 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/hmm_tools.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.270096 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/
--rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3356 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5273 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3224 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3461 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4355 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4078 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2287 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8747 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8044 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6919 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7646 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.270096 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     5776 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4242 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2629 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1824 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3286 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3860 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2617 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1866 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2795 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2708 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4463 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4836 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4537 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2358 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.270096 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/
--rw-r--r--   0 steve     (1000) steve     (1000)     3992 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcr.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4197 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5131 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrItemSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2595 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwm.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3374 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwmItemSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3646 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwmSubject.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5340 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrSubject.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1545 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IRT.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1972 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IRT.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11273 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IrtModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3923 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IrtModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6612 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Item.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5757 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Item.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3351 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/ItemDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1446 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/ItemSliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12317 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PartialCreditModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6787 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PartialCreditModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2613 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PcrNid.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5174 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Subject.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2875 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Subject.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2225 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectPrior.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3271 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectPrior.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectSliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2029 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectSliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2369 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/multisubscale_logit_cutpoint_model.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/
--rw-r--r--   0 steve     (1000) steve     (1000)    30178 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    27208 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17331 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15322 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    28663 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    20299 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9061 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7233 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3756 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3925 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2794 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/LognormalModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2691 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/LognormalModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1858 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1889 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14356 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MarkovModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10890 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MarkovModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3029 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MatrixNormalModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5179 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MatrixNormalModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/
--rw-r--r--   0 steve     (1000) steve     (1000)     4277 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4889 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8232 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7920 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17257 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    16764 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5920 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6687 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2562 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2659 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     6573 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4466 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1713 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1515 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3190 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3231 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6986 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4600 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14856 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7211 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3394 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2854 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    25219 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18376 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7226 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/identify_permutation.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/identify_permutation.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7622 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ModelTypes.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14802 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ModelTypes.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7194 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MultinomialModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4155 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MultinomialModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8904 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6967 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3699 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenScalarSigma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4363 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenScalarSigma.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4682 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenSigma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3849 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenSigma.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3701 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3547 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvnModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8244 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvtModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3398 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/MvtModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/
--rw-r--r--   0 steve     (1000) steve     (1000)     1955 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2657 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4707 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/Nnet.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8152 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/Nnet.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     8569 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4090 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8430 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7055 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4616 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ParamTypes.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7169 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ParamTypes.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/
--rw-r--r--   0 steve     (1000) steve     (1000)     1969 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1771 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2382 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2466 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6194 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4076 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    44343 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    26563 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10670 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PointProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5650 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PointProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    42734 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18834 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2257 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonProcess.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.274095 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     1509 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1558 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1525 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1531 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1608 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/PoissonClusterPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6096 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2471 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15049 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6242 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7742 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonGammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4080 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonGammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6129 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4312 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.278095 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/
--rw-r--r--   0 steve     (1000) steve     (1000)     2122 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/CompositeParamPolicy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3107 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/CompositeParamPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2000 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/DataInfoPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3037 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/DeferredDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5337 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/IID_DataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1190 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ManyParamPolicy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2331 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ManyParamPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4852 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/MixtureDataPolicy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3960 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/MixtureDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1681 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NonparametricParamPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1448 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1283 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullParamPolicy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1574 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullParamPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1822 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullPriorPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2931 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_1.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3202 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_2.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3605 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_3.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4000 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_4.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1761 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/PriorPolicy.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2268 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/PriorPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5920 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/SufstatDataPolicy.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.286095 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     4788 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2628 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12706 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10121 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4912 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5825 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2374 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1689 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1671 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2269 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2595 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5499 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2422 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18203 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12901 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2582 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1630 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2130 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1667 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2226 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FiniteMixturePosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1534 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1455 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2215 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedSpdSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1688 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedUnivariateSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7046 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2697 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2970 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2062 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2440 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1794 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1792 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2820 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2291 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3541 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3938 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4588 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3065 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1260 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2447 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2484 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/Imputer.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15489 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/Imputer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2814 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3401 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2923 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4233 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2501 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3465 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2608 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4024 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3033 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6964 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5927 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3464 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1866 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3931 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3077 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3605 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4712 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3236 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2111 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2657 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1707 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2296 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4427 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2756 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2324 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13532 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3573 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1808 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1796 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2495 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2055 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1587 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1661 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3164 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1765 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5382 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4227 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2569 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1974 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4913 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3062 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5154 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ProductDirichletModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4019 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ProductDirichletModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5508 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ProductVectorModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5063 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ProductVectorModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2787 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ScaledChisqModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2178 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ScaledChisqModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5555 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3462 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1521 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1274 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1613 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdParams.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1879 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SpdParams.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/
--rw-r--r--   0 steve     (1000) steve     (1000)    23820 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14940 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9961 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10573 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    17857 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicRegression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    22212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicRegression.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/
--rw-r--r--   0 steve     (1000) steve     (1000)     7513 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3682 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9275 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4282 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2901 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8920 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3346 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4631 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    18566 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10779 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8120 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5271 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10145 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10965 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    81076 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    87759 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6919 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3545 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1900 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/MultiplexedData.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2085 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/MultiplexedData.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/
--rw-r--r--   0 steve     (1000) steve     (1000)    16599 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    25817 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    26600 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    30983 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     2541 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1776 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3869 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2359 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1547 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8063 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6368 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/
--rw-r--r--   0 steve     (1000) steve     (1000)     6122 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9841 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15166 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13608 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1870 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedStateModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.290094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/tests/
--rw-r--r--   0 steve     (1000) steve     (1000)    13056 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/tests/mv_framework.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     1687 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1513 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicInterceptRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2067 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11536 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4657 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5504 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5172 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3235 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5917 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3165 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4015 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1169 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceRegressionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5402 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7297 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2332 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/SufstatManager.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6852 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModelVector.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10394 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModelVector.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/
--rw-r--r--   0 steve     (1000) steve     (1000)     6791 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3993 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9520 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10581 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11487 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7024 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7470 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7155 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5552 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10020 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14749 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14059 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4975 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4526 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5575 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3573 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     3663 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2955 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4679 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4386 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10143 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15161 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4999 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5018 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9111 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6074 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8808 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6174 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2644 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10057 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2011 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5094 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11694 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7385 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9989 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10303 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/
--rw-r--r--   0 steve     (1000) steve     (1000)     2481 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/ArStateModelTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7737 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/HolidayTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2332 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLevelModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2642 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLinearTrendModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3437 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SeasonalTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3230 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SemilocalLinearTrendTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4990 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StateTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2288 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StaticInterceptTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2968 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StudentLocalLinearTrendTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3003 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/TrigTestModule.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14943 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12691 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9780 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7096 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    35806 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    40273 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1512 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2481 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    15952 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11504 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13057 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9124 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13021 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8273 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/
--rw-r--r--   0 steve     (1000) steve     (1000)     2411 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/DynamicInterceptTestFramework.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/StateSpaceTestFramework.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2865 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/TestFrameworkBase.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2414 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/state_space_test_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1505 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Sufstat.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5093 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/Sufstat.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1421 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/SufstatAbstractCombineImpl.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.294094 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/
--rw-r--r--   0 steve     (1000) steve     (1000)     9181 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6034 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14219 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11901 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1269 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaPriors.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2026 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaPriors.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2185 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/MarkovLink.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6743 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4340 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.298094 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     5510 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3557 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6560 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4355 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1356 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaGibbsMhSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3216 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2061 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5807 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2452 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5315 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeries.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3766 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeriesDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3495 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeriesSufstatDataPolicy.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2424 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TruncatedGammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/TruncatedGammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1775 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformCorrelationModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1880 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformCorrelationModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5092 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3498 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2680 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformShrinkagePriorModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2353 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/UniformShrinkagePriorModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2770 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/VectorModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2803 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedData.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2766 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedGaussianSuf.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedGaussianSuf.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6885 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedMvnModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3585 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedMvnModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7503 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WishartModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5797 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/WishartModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7410 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedGammaModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5550 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedGammaModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5901 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedLognormalModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3552 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedLognormalModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8109 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedPoissonModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4560 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedPoissonModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2525 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanGaussianModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2060 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanGaussianModel.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2659 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanMvnModel.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2081 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanMvnModel.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.298094 BayesBoom-0.1.8/BayesBoom/boom/Samplers/
--rw-r--r--   0 steve     (1000) steve     (1000)     3209 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ARMS.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ARMS.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1779 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/DirectProposal.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/DirectProposal.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.298094 BayesBoom-0.1.8/BayesBoom/boom/Samplers/Gilks/
--rw-r--r--   0 steve     (1000) steve     (1000)    28708 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/Gilks/arms.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1057 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/Gilks/arms.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3212 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ImportanceResampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2649 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ImportanceResampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3091 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MH_Proposals.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6222 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MH_Proposals.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3952 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MetropolisHastings.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2150 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MetropolisHastings.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5519 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MoveAccounting.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4426 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/MoveAccounting.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2087 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/RejectionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2671 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/RejectionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1569 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/Sampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2370 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/Sampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    19024 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10831 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2673 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarLangevinSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2344 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarLangevinSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9747 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarSliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3172 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarSliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5875 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/SliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2612 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/SliceSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4630 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/TIM.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4288 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/TIM.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1755 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateLangevinSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1859 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateLangevinSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2633 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateSliceSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3071 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateSliceSampler.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.298094 BayesBoom-0.1.8/BayesBoom/boom/Samplers/failed_experiments/
--rw-r--r--   0 steve     (1000) steve     (1000)     4929 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/failed_experiments/AdaptiveGaussianMixtureMhSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1774 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/Samplers/failed_experiments/AdaptiveRandomWalkMetropolisSampler.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.298094 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/
--rw-r--r--   0 steve     (1000) steve     (1000)     7454 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/JacobianChecker.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3988 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/JacobianChecker.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2996 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogPost.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2598 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogPost.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1597 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogTransform.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3600 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogTransform.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1775 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogitTransform.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3743 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogitTransform.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2244 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Loglike.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8470 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/MultinomialLogitTransform.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6055 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/MultinomialLogitTransform.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1408 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/ScalarLogpostTF.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1352 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/ScalarLogpostTF.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3939 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/TargetFun.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7193 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/TargetFun.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5263 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Transformation.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7368 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Transformation.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)       73 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/__init__.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.302093 BayesBoom-0.1.8/BayesBoom/boom/cpputil/
--rw-r--r--   0 steve     (1000) steve     (1000)     3518 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/AsciiGraph.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4446 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/AsciiGraph.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1610 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Constants.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    24173 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Date.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9088 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Date.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6869 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/DateTime.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4942 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/DateTime.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1199 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/DefaultVnames.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1157 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/DefaultVnames.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1839 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/LongString.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1485 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/LongString.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1789 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/OutputTable.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1470 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/OutputTable.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4854 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamFileIoManager.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1837 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamHolder.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2425 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamHolder.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    35880 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Polynomial.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2477 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Polynomial.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2329 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ProgressTracker.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4778 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Ptr.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1172 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Redirector.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1392 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Redirector.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1550 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/RefCounted.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4787 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/Split.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2924 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThreadTools.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8150 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThreadTools.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1335 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThrowException.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1647 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ToString.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2320 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/apply_permutation.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1471 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/apply_permutation.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1538 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/ask_to_continue.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2027 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/compare_vector_bool.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2196 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/compare_vector_bool.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1217 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/concatenate_strings.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1027 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/date_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1546 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/file_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1334 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/get_date.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1647 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/gll.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1114 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/gll.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2834 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/index_table.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1105 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/is_all_white.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1925 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/is_numeric.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1097 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/legalize_file_name.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1754 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/lse.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1579 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/lse.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1932 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/make_unique_preserve_order.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1616 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/math_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1090 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/nyi.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2563 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/parse_range.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1411 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/parse_range.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1435 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/portable_math.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1477 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/print.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2088 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/print_columns.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1167 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/random_element.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1230 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/read_file.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1201 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/rep.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1058 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/rep.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1613 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/replace_all.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1430 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/report_error.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2214 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/report_error.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1006 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/safelog.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1305 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/scan.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2471 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/seq.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1887 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/shift_element.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1722 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/shuffle.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5144 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/split.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1327 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/split_delimited.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1460 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/split_string.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1146 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/stream.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3358 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/string_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1137 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1107 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip_path.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1119 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip_white_space.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1218 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/substring_delimited.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1667 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/timer.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1387 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/trim_white_space.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1586 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/cpputil/unmap.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.306093 BayesBoom-0.1.8/BayesBoom/boom/distributions/
--rw-r--r--   0 steve     (1000) steve     (1000)     5146 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/BinomialDistribution.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1576 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/BinomialDistribution.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7472 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4719 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3958 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2521 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3326 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Markov.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2451 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Markov.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    12589 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Rmath_dist.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10922 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Rmath_dist.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3927 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Tn2Sampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4334 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/Wishart.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7684 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/dirichlet.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/extreme_value.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    21009 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/gig.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2335 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/inverse_gaussian.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1915 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/inverse_gaussian.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3055 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/matrix_normal.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7057 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/mvn.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2521 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/mvt.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2608 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/random_cor.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1137 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/random_int.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1155 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/rlexp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3268 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/rmulti.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1450 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/rng.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2084 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/rng.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5451 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/rtriangle.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2182 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/student_fix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_exp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4879 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_gamma.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2705 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_gamma.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6156 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_logit.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3096 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_logit.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11546 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_norm.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2385 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions/usp.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    19623 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/distributions.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.306093 BayesBoom-0.1.8/BayesBoom/boom/math/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.306093 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/
--rwxr-xr-x   0 steve     (1000) steve     (1000)     1759 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephes_impl.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4250 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephes_rgamma.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     1759 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephus_impl.hpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     2679 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/chbevl.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     5151 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/dawsn.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     8875 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/ei.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     4782 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/expn.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     3845 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/fac.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     5999 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/fresnl.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     5860 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/planck.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     2836 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/polevl.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     8719 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/polylog.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     4006 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/powi.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     7229 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/shichi.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     7129 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/sici.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     3389 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/spence.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     4604 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/zeta.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     6667 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/cephes/zetac.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     2097 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/lmultigamma.cpp
--rwxr-xr-x   0 steve     (1000) steve     (1000)     2593 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/math/special_functions.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/numopt/
--rw-r--r--   0 steve     (1000) steve     (1000)    10194 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Brent.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2434 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Brent.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    89336 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Integral.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2622 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Integral.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1345 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/LinearAssignment.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2512 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/LinearAssignment.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3909 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/MarkovDecisionProcess.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3206 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/MarkovDecisionProcess.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1278 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Negate.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14430 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/NelderMead.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3514 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/NelderMead.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5865 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/NumericalDerivatives.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3997 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/NumericalDerivatives.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    81136 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Powell.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2119 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Powell.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1448 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Qlearning.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2331 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/Qlearning.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4048 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarLaplaceApproximation.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2193 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarLaplaceApproximation.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1629 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarNewtonMax.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1398 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarNewtonMax.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5977 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/bfgs.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5773 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/conj_grad.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1960 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/initialize_derivatives.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1923 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/initialize_derivatives.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/numopt/linear_assignment/
--rw-r--r--   0 steve     (1000) steve     (1000)    10408 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/linear_assignment/lap.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7127 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/max_nd.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7508 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/nelder_mead.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7285 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/newton.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3197 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt/simulated_annealing.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    14809 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/numopt.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/LinAlg/
--rw-r--r--   0 steve     (1000) steve     (1000)    15089 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/LinAlg/LinAlgWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/
--rw-r--r--   0 steve     (1000) steve     (1000)     3226 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/BetaBinomialWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2232 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/BetaModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3015 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/DataWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2182 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/DirichletWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2170 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/GammaModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    10155 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/GaussianModelWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Glm/
--rw-r--r--   0 steve     (1000) steve     (1000)    28906 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Glm/GlmModel_def.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     9712 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Glm/MlogitModel_def.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Impute/
--rw-r--r--   0 steve     (1000) steve     (1000)    35381 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Impute/Imputer_def.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/
--rw-r--r--   0 steve     (1000) steve     (1000)     8043 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/beta_binomial_mixture_wrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4719 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/dpmvn_wrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2465 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/finite_mixture_wrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4186 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/ModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3126 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/MultinomialWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7371 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/MvnWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2758 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/ParameterWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/
--rw-r--r--   0 steve     (1000) steve     (1000)    15004 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/DynamicRegressionModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    21028 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/MultivariateStateSpaceModelWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/
--rw-r--r--   0 steve     (1000) steve     (1000)     4288 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/MultivariateStateModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    38513 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/StateModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    23890 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateSpaceModelWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/TimeSeries/
--rw-r--r--   0 steve     (1000) steve     (1000)     8403 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/TimeSeries/time_series_model_def.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)      662 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/UniformModelWrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1415 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/WishartModelWrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/cpputil/
--rw-r--r--   0 steve     (1000) steve     (1000)     1489 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/cpputil/cpputil_wrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/distributions/
--rw-r--r--   0 steve     (1000) steve     (1000)      978 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/distributions/distribution_wrapper.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3285 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/module.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/numopt/
--rw-r--r--   0 steve     (1000) steve     (1000)     1148 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/numopt/numopt_wrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/stats/
--rw-r--r--   0 steve     (1000) steve     (1000)    14413 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/stats/stats_wrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.310093 BayesBoom-0.1.8/BayesBoom/boom/pybind11/test_utils/
--rw-r--r--   0 steve     (1000) steve     (1000)     4699 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/pybind11/test_utils/test_utils_wrapper.cpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.314092 BayesBoom-0.1.8/BayesBoom/boom/stats/
--rw-r--r--   0 steve     (1000) steve     (1000)     3093 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/AsciiDistributionCompare.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2910 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/AsciiDistributionCompare.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6422 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Bspline.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4082 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Bspline.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5078 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ChiSquareTest.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3729 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ChiSquareTest.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    26671 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/DataTable.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    13496 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/DataTable.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)    46981 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Design.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    38370 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Design.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2748 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ECDF.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ECDF.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3009 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/EmpiricalDensity.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3246 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/EmpiricalDensity.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4165 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Encoders.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5677 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Encoders.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5754 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/FreqDist.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4401 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/FreqDist.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8114 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/IQagent.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2141 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/IQagent.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3708 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Mspline.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     5626 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Mspline.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     8401 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/NaturalSpline.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2990 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/NaturalSpline.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2669 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Resampler.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4459 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Resampler.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2455 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Spline.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3852 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/Spline.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3710 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/compare_binomial_proportions.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1434 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/compare_binomial_proportions.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3101 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/compare_predictions.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1855 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/compare_predictions.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1529 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/diff.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1228 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/diff.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4620 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/hexbin.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3028 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/hexbin.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1844 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ks_critical_value.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2491 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/logit.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3524 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/logit.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     6021 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/moments.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2113 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/moments.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1052 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/ols.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1177 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/regression.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1052 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/regression.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1204 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/simple_random_sample.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     2052 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/simple_random_sample.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4976 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/summary.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     4464 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/stats/summary.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.314092 BayesBoom-0.1.8/BayesBoom/boom/test_utils/
--rw-r--r--   0 steve     (1000) steve     (1000)     4947 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_derivatives.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3179 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_derivatives.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     7108 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_mcmc_matrix.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)     3486 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/test_utils/distributions_match.cpp
--rw-r--r--   0 steve     (1000) steve     (1000)    11321 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/test_utils/test_utils.hpp
--rw-r--r--   0 steve     (1000) steve     (1000)     1367 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/to_data_table.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1085 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/boom/uint.hpp
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.314092 BayesBoom-0.1.8/BayesBoom/bsts/
--rw-r--r--   0 steve     (1000) steve     (1000)     1781 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)      967 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/airpass.py
--rw-r--r--   0 steve     (1000) steve     (1000)     8387 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/ar.py
--rw-r--r--   0 steve     (1000) steve     (1000)    65415 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/bsts.py
--rw-r--r--   0 steve     (1000) steve     (1000)      362 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/bsts_test.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1058 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/data.py
--rw-r--r--   0 steve     (1000) steve     (1000)     7111 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/dynamic_regression_state_model.py
--rw-r--r--   0 steve     (1000) steve     (1000)     9594 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/gaussian.py
--rw-r--r--   0 steve     (1000) steve     (1000)     7246 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/general_seasonal_llt.py
--rw-r--r--   0 steve     (1000) steve     (1000)    10011 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/holiday.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4029 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/holiday_models.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4827 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/local_level.py
--rw-r--r--   0 steve     (1000) steve     (1000)     7464 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/local_linear_trend.py
--rw-r--r--   0 steve     (1000) steve     (1000)     5720 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/logit.py
--rw-r--r--   0 steve     (1000) steve     (1000)     5561 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/poisson.py
--rw-r--r--   0 steve     (1000) steve     (1000)     8236 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/seasonal.py
--rw-r--r--   0 steve     (1000) steve     (1000)    11847 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/semilocal_linear_trend.py
--rw-r--r--   0 steve     (1000) steve     (1000)     5255 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/state_models.py
--rw-r--r--   0 steve     (1000) steve     (1000)     8455 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/student.py
--rw-r--r--   0 steve     (1000) steve     (1000)    10235 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/student_local_linear_trend.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2209 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_ar.py
--rw-r--r--   0 steve     (1000) steve     (1000)    11721 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_bsts.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2144 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_dynamic_regression.py
--rw-r--r--   0 steve     (1000) steve     (1000)     2156 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_holidays.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1940 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_seasonal_llt.py
--rw-r--r--   0 steve     (1000) steve     (1000)     8239 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_state_models.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1942 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_student_llt.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1659 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_trig.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1108 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/test_utilities.py
--rw-r--r--   0 steve     (1000) steve     (1000)     5249 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/bsts/trig.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.314092 BayesBoom-0.1.8/BayesBoom/dynreg/
--rw-r--r--   0 steve     (1000) steve     (1000)       93 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/dynreg/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    20164 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/dynreg/dynreg.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4824 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/dynreg/test_dynreg.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.314092 BayesBoom-0.1.8/BayesBoom/impute/
--rw-r--r--   0 steve     (1000) steve     (1000)       37 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/impute/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    19204 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/impute/impute.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1695 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/impute/test_imputer.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/BayesBoom/mixtures/
--rw-r--r--   0 steve     (1000) steve     (1000)      179 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/mixtures/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)    14726 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/mixtures/beta_binomial_mixture.py
--rw-r--r--   0 steve     (1000) steve     (1000)    13065 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/mixtures/dirichlet_process.py
--rw-r--r--   0 steve     (1000) steve     (1000)     3265 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/mixtures/test_dirichlet_process.py
--rw-r--r--   0 steve     (1000) steve     (1000)      686 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/mixtures/utils.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/BayesBoom/spikeslab/
--rw-r--r--   0 steve     (1000) steve     (1000)      784 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)     6775 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/mlogit_spike.py
--rw-r--r--   0 steve     (1000) steve     (1000)     1211 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/mlogit_test.py
--rw-r--r--   0 steve     (1000) steve     (1000)    16737 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/priors.py
--rw-r--r--   0 steve     (1000) steve     (1000)    23516 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/spikeslab.py
--rw-r--r--   0 steve     (1000) steve     (1000)     5060 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/spikeslab/spikeslab_test.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/BayesBoom/test_utils/
--rw-r--r--   0 steve     (1000) steve     (1000)      153 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/test_utils/__init__.py
--rw-r--r--   0 steve     (1000) steve     (1000)      505 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/test_utils/find_project_root.py
--rw-r--r--   0 steve     (1000) steve     (1000)      413 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/test_utils/simulate_data.py
--rw-r--r--   0 steve     (1000) steve     (1000)     4484 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/BayesBoom/test_utils/test_utils.py
-drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-22 16:35:47.214100 BayesBoom-0.1.8/BayesBoom.egg-info/
--rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-22 16:35:47.000000 BayesBoom-0.1.8/BayesBoom.egg-info/PKG-INFO
--rw-r--r--   0 steve     (1000) steve     (1000)    82465 2022-09-22 16:35:47.000000 BayesBoom-0.1.8/BayesBoom.egg-info/SOURCES.txt
--rw-r--r--   0 steve     (1000) steve     (1000)        1 2022-09-22 16:35:47.000000 BayesBoom-0.1.8/BayesBoom.egg-info/dependency_links.txt
--rw-r--r--   0 steve     (1000) steve     (1000)        1 2022-01-04 15:04:54.000000 BayesBoom-0.1.8/BayesBoom.egg-info/not-zip-safe
--rw-r--r--   0 steve     (1000) steve     (1000)       14 2022-09-22 16:35:47.000000 BayesBoom-0.1.8/BayesBoom.egg-info/requires.txt
--rw-r--r--   0 steve     (1000) steve     (1000)       16 2022-09-22 16:35:47.000000 BayesBoom-0.1.8/BayesBoom.egg-info/top_level.txt
--rw-r--r--   0 steve     (1000) steve     (1000)      909 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/MANIFEST.in
--rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/PKG-INFO
--rw-r--r--   0 steve     (1000) steve     (1000)       38 2022-09-22 16:35:47.318092 BayesBoom-0.1.8/setup.cfg
--rw-r--r--   0 steve     (1000) steve     (1000)    15688 2022-09-22 16:35:46.000000 BayesBoom-0.1.8/setup.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.008032 BayesBoom-0.1.9/BayesBoom/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.008032 BayesBoom-0.1.9/BayesBoom/R/
+-rw-r--r--   0 steve     (1000) steve     (1000)    10387 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/R.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1965 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    20219 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/autoclean.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    13212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/bayes.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     3915 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/boom_py_utils.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2615 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/cbind.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/data_table.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1954 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/density.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    27891 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/encoding.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4949 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/graphics_device.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1764 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/mcmc.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    26826 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/plots.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     8968 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/probability.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      479 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/stats.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1597 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_R.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2461 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_cbind.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     6231 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_data_table.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     6745 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_encoding.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     3946 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_plots.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4134 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_probability.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      386 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_utilities.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1337 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/test_utils.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     3176 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/R/utils.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.008032 BayesBoom-0.1.9/BayesBoom/boom/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.016032 BayesBoom-0.1.9/BayesBoom/boom/Bmath/
+-rw-r--r--   0 steve     (1000) steve     (1000)    14088 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/Bmath.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2455 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/Random.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2741 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/bd0.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5467 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/bessel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17474 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/bessel_k.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3469 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/beta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3172 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/chebyshev.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2715 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/choose.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2634 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/d1mach.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3596 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3409 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2187 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dcauchy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1872 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2746 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/df.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3193 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dgamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2261 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dgeom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3066 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dhyper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2267 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dlnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2154 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dlogis.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3687 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2566 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3197 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2348 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2678 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dpois.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5792 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dpq.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2559 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2055 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dunif.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2279 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/dweibull.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4224 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/fprec.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3757 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/fround.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2001 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/fsign.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1851 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/ftrunc.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9866 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/gamma_cody.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3443 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/gammalims.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2413 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/i1mach.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3030 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/lbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4380 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/lgammacor.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)      469 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/mathlib_error.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5606 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/mlutils.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4533 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/nmath.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2277 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2263 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pcauchy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1914 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2367 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2412 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5819 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pgamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2180 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pgeom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6963 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/phyper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2094 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/plnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2325 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/plogis.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4093 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2297 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4340 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2215 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9866 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5487 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13905 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/polygamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2177 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/ppois.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2858 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13714 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/ptukey.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2101 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/punif.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2343 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/pweibull.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6386 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4154 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2210 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qcauchy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2071 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2416 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5875 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qgamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2227 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qgeom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3351 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qhyper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2128 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qlnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2427 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qlogis.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4252 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2998 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8385 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4046 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qpois.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5782 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6663 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qtukey.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2044 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qunif.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2174 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/qweibull.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5480 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rbeta.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7330 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2172 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rcauchy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2148 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2073 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2275 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7446 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rgamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rgeom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10786 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rhyper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2164 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rlnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2943 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rloggamma_small_alpha.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2088 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rlogis.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4629 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rmultinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2585 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnbinom.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3286 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnchisq.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2402 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9111 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rpois.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2296 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2050 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/runif.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2104 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/rweibull.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3204 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/sexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1988 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/sign.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11122 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/snorm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4539 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/stirlerr.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    60559 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/toms708.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1770 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Bmath/unif_rand.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.016032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1161 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Cholesky
+-rw-r--r--   0 steve     (1000) steve     (1000)     1900 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/CholmodSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)    12799 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Core
+-rw-r--r--   0 steve     (1000) steve     (1000)      122 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Dense
+-rw-r--r--   0 steve     (1000) steve     (1000)       35 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Eigen
+-rw-r--r--   0 steve     (1000) steve     (1000)     1777 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Eigenvalues
+-rw-r--r--   0 steve     (1000) steve     (1000)     1940 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Geometry
+-rw-r--r--   0 steve     (1000) steve     (1000)      829 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Householder
+-rw-r--r--   0 steve     (1000) steve     (1000)     2083 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 steve     (1000) steve     (1000)      894 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Jacobi
+-rw-r--r--   0 steve     (1000) steve     (1000)     1389 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/KLUSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     1268 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/LU
+-rw-r--r--   0 steve     (1000) steve     (1000)      991 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/MetisSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     2451 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/OrderingMethods
+-rw-r--r--   0 steve     (1000) steve     (1000)     1751 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/PaStiXSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     1116 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/PardisoSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     1272 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/QR
+-rw-r--r--   0 steve     (1000) steve     (1000)      900 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/QtAlignedMalloc
+-rw-r--r--   0 steve     (1000) steve     (1000)     1162 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SPQRSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     1584 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SVD
+-rw-r--r--   0 steve     (1000) steve     (1000)      888 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/Sparse
+-rw-r--r--   0 steve     (1000) steve     (1000)     1235 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseCholesky
+-rw-r--r--   0 steve     (1000) steve     (1000)     2240 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseCore
+-rw-r--r--   0 steve     (1000) steve     (1000)     1814 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseLU
+-rw-r--r--   0 steve     (1000) steve     (1000)     1195 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseQR
+-rw-r--r--   0 steve     (1000) steve     (1000)      797 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdDeque
+-rw-r--r--   0 steve     (1000) steve     (1000)      726 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdList
+-rw-r--r--   0 steve     (1000) steve     (1000)      803 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdVector
+-rw-r--r--   0 steve     (1000) steve     (1000)     2243 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/SuperLUSupport
+-rw-r--r--   0 steve     (1000) steve     (1000)     1382 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/UmfPackSupport
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.004032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.016032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/
+-rw-r--r--   0 steve     (1000) steve     (1000)    24934 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    18760 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3974 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.016032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/CholmodSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    25441 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/
+-rw-r--r--   0 steve     (1000) steve     (1000)    19214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    16782 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Array.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7018 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2738 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Assign.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    41673 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)    12488 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14075 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    18648 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Block.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4429 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5981 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6990 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    63841 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4745 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7909 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    36282 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3937 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5551 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    31529 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    24484 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    25360 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9870 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14670 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)      988 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11654 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Dot.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5841 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4909 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5759 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21679 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    38812 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11543 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8238 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/IO.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9620 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3503 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Map.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11281 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    60784 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7156 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    24343 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    23856 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2520 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3620 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12884 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9207 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    20748 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    49193 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7336 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Product.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    53832 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7756 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Random.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    19195 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Redux.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17821 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Ref.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5656 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17033 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4284 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7522 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6143 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Select.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14999 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1697 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6837 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Solve.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9368 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6170 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8700 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21641 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Stride.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2765 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Swap.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17606 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13567 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    38277 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3488 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    35168 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11997 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.004032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 steve     (1000) steve     (1000)    15223 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8102 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    64608 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2564 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 steve     (1000) steve     (1000)    17160 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13344 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    87891 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2134 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 steve     (1000) steve     (1000)    16540 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2323 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)   119355 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9490 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    24820 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)   102394 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 steve     (1000) steve     (1000)    17317 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 steve     (1000) steve     (1000)    26903 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5251 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    67696 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3770 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    35534 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1746 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3746 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2695 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    57047 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.004032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 steve     (1000) steve     (1000)      691 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.024032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 steve     (1000) steve     (1000)    17541 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    16159 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    33615 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 steve     (1000) steve     (1000)    22503 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6815 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3083 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)   189525 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    51286 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 steve     (1000) steve     (1000)    14251 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6765 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)    64465 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3650 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1194 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21200 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1351 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7428 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12539 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    27786 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21856 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 steve     (1000) steve     (1000)    16728 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8024 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)    36894 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/
+-rw-r--r--   0 steve     (1000) steve     (1000)     6686 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    20921 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8334 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4998 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 steve     (1000) steve     (1000)      607 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    40146 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.028032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/
+-rw-r--r--   0 steve     (1000) steve     (1000)   108448 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    20104 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15948 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6936 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5106 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21724 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6368 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5582 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21354 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11570 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9958 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5209 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6164 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4126 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    20987 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13867 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14722 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    10571 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14678 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6707 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5882 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/
+-rwxr-xr-x   0 steve     (1000) steve     (1000)    23156 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    19876 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21931 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     4892 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15555 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6696 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    10949 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     4268 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    52909 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    46661 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)    29336 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 steve     (1000) steve     (1000)       85 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1024 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1432 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    10676 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12003 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    35762 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/
+-rw-r--r--   0 steve     (1000) steve     (1000)    12559 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17274 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4178 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    22970 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17176 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9716 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14349 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5575 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    23640 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21078 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3650 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    35182 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4104 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    22764 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/
+-rw-r--r--   0 steve     (1000) steve     (1000)    18939 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8403 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3624 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    20726 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11962 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8955 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9812 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    34367 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6862 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8063 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6724 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    61930 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7664 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6190 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/arch/
+-rw-r--r--   0 steve     (1000) steve     (1000)     5945 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4784 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5365 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    23611 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     6771 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6850 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8887 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15036 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14940 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13379 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7349 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Jacobi/
+-rw-r--r--   0 steve     (1000) steve     (1000)    16383 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.032032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/KLUSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    11555 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3439 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    32383 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15727 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    22069 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3555 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/arch/
+-rw-r--r--   0 steve     (1000) steve     (1000)    13693 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/MetisSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4588 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/
+-rw-r--r--   0 steve     (1000) steve     (1000)    16105 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    61681 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5248 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    22249 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PardisoSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    20092 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/
+-rw-r--r--   0 steve     (1000) steve     (1000)    25498 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4662 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    23429 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    26768 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14641 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2993 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SPQRSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    11826 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/
+-rw-r--r--   0 steve     (1000) steve     (1000)    54214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    32988 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5099 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14743 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15957 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCholesky/
+-rw-r--r--   0 steve     (1000) steve     (1000)    24216 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5830 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.036032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/
+-rw-r--r--   0 steve     (1000) steve     (1000)    10670 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8743 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13166 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2191 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    11368 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    24360 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6485 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13606 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    25524 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4757 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    13256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5808 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3080 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1107 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12589 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    57475 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    17451 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7329 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7593 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1699 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    15600 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    25889 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4424 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8704 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3175 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6437 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6827 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    14832 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8127 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9657 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/
+-rw-r--r--   0 steve     (1000) steve     (1000)    33316 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4303 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7602 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4974 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12837 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2049 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6712 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6584 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3681 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    10217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4181 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5723 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     8485 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     9028 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4979 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4545 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2889 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseQR/
+-rw-r--r--   0 steve     (1000) steve     (1000)    29167 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4730 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4155 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     5338 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2809 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    34324 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 steve     (1000) steve     (1000)    24456 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2913 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/Image.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     2742 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     1748 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    30560 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/blas.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     7834 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 steve     (1000) steve     (1000)  1058369 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 steve     (1000) steve     (1000)      474 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.040032 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/
+-rw-r--r--   0 steve     (1000) steve     (1000)    14060 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    21431 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    59020 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     4828 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6089 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)    12283 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6387 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     3350 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 steve     (1000) steve     (1000)     6915 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.044032 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/
+-rw-r--r--   0 steve     (1000) steve     (1000)    32356 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Array.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17692 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Array.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5300 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/ArrayIterator.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4569 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/ArrayIterator.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4726 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Cholesky.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3114 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Cholesky.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3770 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/CorrelationMatrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2343 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/CorrelationMatrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10711 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/DiagonalMatrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7295 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/DiagonalMatrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5110 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Eigen.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4179 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Eigen.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3075 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/EigenMap.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4361 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Givens.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1711 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Givens.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4997 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/LU.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2493 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/LU.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    43968 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Matrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    21468 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Matrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2907 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/MatrixPartition.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2023 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/MatrixPartition.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4280 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/QR.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3369 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/QR.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3252 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SVD.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1967 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SVD.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3616 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SWEEP.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4191 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SWEEP.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    24476 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Selector.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14090 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Selector.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    22351 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SpdMatrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12246 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SpdMatrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    21032 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SubMatrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9655 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SubMatrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    28588 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Vector.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15270 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Vector.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15255 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorView.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13937 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorView.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5890 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorViewIterator.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1182 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/stack_columns.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1042 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/LinAlg/stack_columns.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.048032 BayesBoom-0.1.9/BayesBoom/boom/Models/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.052033 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/
+-rw-r--r--   0 steve     (1000) steve     (1000)    49256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/Bart.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    32137 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/Bart.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2282 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianBartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2834 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianBartModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3644 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2545 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3342 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/LogitBartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/LogitBartModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5313 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PoissonBartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3669 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PoissonBartModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.052033 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)    44524 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14564 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7895 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6611 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4270 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2284 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13591 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6863 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10969 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12867 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8694 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4985 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3370 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ProbitBartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2208 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ProbitBartModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2700 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ResidualRegressionData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3707 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ResidualRegressionData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)      821 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BernoulliModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12653 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BetaBinomialModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6105 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BetaBinomialModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7841 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BetaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4208 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BetaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8085 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BinomialModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5008 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/BinomialModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12814 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CategoricalData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11257 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CategoricalData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3252 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ChisqModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2417 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ChisqModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1589 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2097 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2611 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3176 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5222 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ConstrainedVectorParams.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5687 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ConstrainedVectorParams.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1870 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DataPair.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4337 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DataTypes.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7549 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DataTypes.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7754 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DirichletModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4021 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DirichletModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1618 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DiscreteUniformModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1892 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DiscreteUniformModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3121 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/DoubleModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2575 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/EmMixtureComponent.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3061 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialIncrementModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2655 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialIncrementModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5389 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3680 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10543 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/FiniteMixtureModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6345 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/FiniteMixtureModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11231 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6000 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3425 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2319 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7367 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6581 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3823 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelGivenSigma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3421 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelGivenSigma.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.056033 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/
+-rw-r--r--   0 steve     (1000) steve     (1000)    12614 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9536 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7332 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialLogitModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4010 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialLogitModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10076 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialProbitModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3905 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialProbitModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2427 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialRegressionData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2126 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialRegressionData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3988 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ChoiceData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4387 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ChoiceData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13227 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GammaRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8175 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GammaRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3054 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/Glm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7762 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/Glm.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11581 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmCoefs.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7142 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmCoefs.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3012 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmMvnPriorBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3527 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2793 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1715 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/IndependentRegressionModels.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2102 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/IndependentRegressionModels.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5252 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LogisticRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3558 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LogisticRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15690 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LoglinearModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14955 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LoglinearModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ModelSelectionConcepts.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13665 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialLogitModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9541 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialLogitModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9731 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialProbitModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4969 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialProbitModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9559 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultivariateRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8264 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultivariateRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12066 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvnGivenX.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14175 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvnGivenX.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4966 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvtRegModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2870 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvtRegModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17582 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10927 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2785 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2605 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4752 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3987 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.064033 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     9585 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6223 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2478 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1855 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8481 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5924 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4926 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6361 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10902 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4166 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9540 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8640 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2526 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2194 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2993 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3766 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8610 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3815 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2539 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3171 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2678 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2658 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2874 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2621 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3819 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1741 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18303 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11159 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4096 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3667 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11888 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4263 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6607 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3323 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8510 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7435 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2669 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/IndependentRegressionModelsPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2903 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2265 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4561 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1727 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3327 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1885 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1566 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1896 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6302 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4862 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3025 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2631 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1605 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2524 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2027 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1848 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1462 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2360 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2082 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11276 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2529 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2353 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13016 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7843 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3445 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2226 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4314 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4189 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    19527 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10834 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1120 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1282 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3785 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2887 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8362 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3814 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4600 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4807 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6175 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5486 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1650 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3862 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3325 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2421 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2015 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4936 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2243 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3342 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6063 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2711 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3184 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2733 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2425 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5876 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2868 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4421 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4408 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18383 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12175 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7604 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2168 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6586 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4992 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2734 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2128 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5148 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2422 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1946 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedGammaRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4611 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5058 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10518 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3544 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1179 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    24944 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_1.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    37882 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_2.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    36405 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_3.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2474 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1615 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5123 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ProbitRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2950 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ProbitRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1372 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/QuantileRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2894 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/QuantileRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    25293 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    19860 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3340 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionSlabPrior.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5286 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionSlabPrior.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8699 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/TRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3703 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/TRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18211 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/VariableSelectionPrior.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11282 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/VariableSelectionPrior.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10314 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/WeightedRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6246 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/WeightedRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4537 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4325 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5542 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4072 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5057 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5284 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.064033 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.064033 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1261 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Event.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1914 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Event.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    28929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8485 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.064033 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1859 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2507 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Session.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2001 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Session.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2774 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Stream.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1807 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Stream.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4192 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmm.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3618 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3229 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9550 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HMM2.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5190 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HMM2.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8130 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HealthStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5268 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HealthStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3206 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1933 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8250 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmFilter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3293 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmFilter.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.064033 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2865 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1984 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4305 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2726 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/hmm_tools.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1188 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/hmm_tools.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.068033 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3356 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5273 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3224 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3461 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4355 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4078 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2287 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8747 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8044 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6919 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7646 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.068033 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     5776 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4242 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2629 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1824 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3286 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3860 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2617 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1866 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2795 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2708 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4463 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4836 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4537 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2358 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.068033 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3992 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcr.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4197 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5131 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrItemSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2595 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwm.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3374 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwmItemSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3646 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwmSubject.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5340 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrSubject.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1545 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IRT.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1972 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IRT.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11273 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IrtModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3923 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IrtModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6612 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Item.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5757 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Item.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3351 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/ItemDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1446 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/ItemSliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12317 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PartialCreditModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6787 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PartialCreditModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2613 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PcrNid.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5174 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Subject.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2875 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Subject.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2225 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectPrior.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3271 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectPrior.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectSliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2029 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectSliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2369 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/multisubscale_logit_cutpoint_model.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.068033 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/
+-rw-r--r--   0 steve     (1000) steve     (1000)    30178 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    27208 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17331 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15322 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    28663 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    20299 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9061 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7233 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3756 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3925 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2794 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/LognormalModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2691 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/LognormalModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1858 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1889 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14356 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MarkovModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10890 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MarkovModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3029 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MatrixNormalModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5179 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MatrixNormalModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.068033 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4277 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4889 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8232 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7920 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17257 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    16764 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5920 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6687 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2562 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2659 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     6573 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4466 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1713 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1515 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3190 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3231 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6986 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4600 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14856 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7211 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3394 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2854 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    25219 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18376 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7226 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/identify_permutation.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/identify_permutation.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7622 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ModelTypes.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14802 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ModelTypes.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7194 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MultinomialModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4155 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MultinomialModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8904 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6967 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3699 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenScalarSigma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4363 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenScalarSigma.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4682 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenSigma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3849 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenSigma.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3701 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3547 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvnModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8244 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvtModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3398 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/MvtModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1955 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2657 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4707 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/Nnet.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8152 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/Nnet.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     8569 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4090 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8430 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7055 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4616 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ParamTypes.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7169 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ParamTypes.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1969 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1771 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2382 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2466 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6194 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4076 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    44343 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    26563 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10670 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PointProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5650 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PointProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    42734 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18834 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2257 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonProcess.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1509 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1558 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1525 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1531 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1608 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/PoissonClusterPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6096 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2471 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15049 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6242 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7742 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonGammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4080 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonGammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6129 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4312 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.072033 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2122 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/CompositeParamPolicy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3107 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/CompositeParamPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2000 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/DataInfoPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3037 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/DeferredDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5337 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/IID_DataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1190 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ManyParamPolicy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2331 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ManyParamPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4852 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/MixtureDataPolicy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3960 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/MixtureDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1681 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NonparametricParamPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1448 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1283 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullParamPolicy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1574 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullParamPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1822 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullPriorPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2931 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_1.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3202 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_2.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3605 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_3.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4000 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_4.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1761 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/PriorPolicy.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2268 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/PriorPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5920 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/SufstatDataPolicy.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.080033 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4788 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2628 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12706 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10121 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4912 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5825 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2374 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1689 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1671 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2269 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2595 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5499 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2422 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18203 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12901 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2582 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1630 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2130 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1667 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2226 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FiniteMixturePosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1534 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1455 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2215 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedSpdSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1688 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedUnivariateSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7046 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2697 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2970 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2062 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2440 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1794 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2149 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1792 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2820 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2291 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3541 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3938 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4588 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3065 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1260 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2447 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2484 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/Imputer.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15489 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/Imputer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2814 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3401 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2923 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4233 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2501 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3465 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2608 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4024 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3033 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6964 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5927 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3464 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1866 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3931 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3077 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3605 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4712 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3236 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2111 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2657 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1707 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2296 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4427 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2756 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2324 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13532 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3573 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1808 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1796 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2495 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2055 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1587 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1661 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3164 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1765 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5382 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4227 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2569 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1974 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4913 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3062 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5154 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ProductDirichletModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4019 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ProductDirichletModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5508 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ProductVectorModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5063 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ProductVectorModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2787 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ScaledChisqModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2178 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ScaledChisqModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5555 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3462 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1521 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1274 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1613 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdParams.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1879 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SpdParams.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.080033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/
+-rw-r--r--   0 steve     (1000) steve     (1000)    23820 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14940 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9961 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10573 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    17857 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicRegression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    22212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicRegression.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.080033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7513 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3682 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9275 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4282 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2901 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8920 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3346 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4631 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    18855 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10779 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8120 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5271 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10145 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10965 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    81076 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    87759 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6919 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3545 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1900 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/MultiplexedData.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2085 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/MultiplexedData.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.080033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/
+-rw-r--r--   0 steve     (1000) steve     (1000)    16801 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    25817 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    26600 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    30983 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2541 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1776 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3869 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2359 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2251 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1547 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8063 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6368 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/
+-rw-r--r--   0 steve     (1000) steve     (1000)     6182 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9841 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15166 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13608 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1870 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedStateModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/tests/
+-rw-r--r--   0 steve     (1000) steve     (1000)    13056 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/tests/mv_framework.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1687 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1513 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2377 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicInterceptRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2067 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11536 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8256 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4657 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5504 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5172 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3235 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5917 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3165 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4015 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1169 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceRegressionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5402 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7297 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2332 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/SufstatManager.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6852 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModelVector.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10394 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModelVector.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/
+-rw-r--r--   0 steve     (1000) steve     (1000)     6791 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3993 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9520 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10581 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11487 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7024 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7470 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7155 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5552 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10020 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14749 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14059 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4975 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4526 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5575 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3573 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.084033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3663 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2955 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4679 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4386 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10143 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15161 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4999 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5018 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9111 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6074 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8808 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6174 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2644 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10057 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2011 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5094 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11694 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7385 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9989 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10303 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2481 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/ArStateModelTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7737 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/HolidayTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2332 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLevelModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2642 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLinearTrendModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3437 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SeasonalTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3230 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SemilocalLinearTrendTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4990 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StateTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2288 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StaticInterceptTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2968 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StudentLocalLinearTrendTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3003 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/TrigTestModule.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14943 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12691 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9780 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7096 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    35806 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    40273 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1512 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2481 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    15952 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11504 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13057 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9124 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13021 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8273 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/
+-rw-r--r--   0 steve     (1000) steve     (1000)     2411 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/DynamicInterceptTestFramework.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/StateSpaceTestFramework.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2865 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/TestFrameworkBase.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2414 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/state_space_test_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1505 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Sufstat.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5093 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/Sufstat.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1421 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/SufstatAbstractCombineImpl.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/
+-rw-r--r--   0 steve     (1000) steve     (1000)     9181 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6034 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14219 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11901 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1269 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaPriors.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2026 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaPriors.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2185 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/MarkovLink.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6743 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4340 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     5510 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3557 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6560 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4355 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1356 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaGibbsMhSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3216 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2061 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5807 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2452 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5315 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeries.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3766 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeriesDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3495 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeriesSufstatDataPolicy.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2424 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TruncatedGammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/TruncatedGammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1775 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformCorrelationModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1880 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformCorrelationModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5092 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3498 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2680 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformShrinkagePriorModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2353 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/UniformShrinkagePriorModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2770 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/VectorModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2803 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedData.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2766 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedGaussianSuf.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedGaussianSuf.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6885 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedMvnModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3585 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedMvnModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7503 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WishartModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5797 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/WishartModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7410 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedGammaModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5550 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedGammaModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5901 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedLognormalModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3552 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedLognormalModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8109 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedPoissonModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4560 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedPoissonModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2525 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanGaussianModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2060 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanGaussianModel.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2659 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanMvnModel.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2081 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanMvnModel.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Samplers/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3209 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ARMS.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ARMS.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1779 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/DirectProposal.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2326 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/DirectProposal.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Samplers/Gilks/
+-rw-r--r--   0 steve     (1000) steve     (1000)    28708 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/Gilks/arms.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1057 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/Gilks/arms.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3212 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ImportanceResampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2649 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ImportanceResampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3091 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MH_Proposals.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6222 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MH_Proposals.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3952 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MetropolisHastings.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2150 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MetropolisHastings.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5519 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MoveAccounting.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4426 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/MoveAccounting.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2087 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/RejectionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2671 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/RejectionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1569 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/Sampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2370 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/Sampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    19024 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10831 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2673 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarLangevinSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2344 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarLangevinSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9747 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarSliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3172 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarSliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5875 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/SliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2612 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/SliceSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4630 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/TIM.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4288 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/TIM.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1755 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateLangevinSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1859 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateLangevinSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2633 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateSliceSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3071 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateSliceSampler.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.088033 BayesBoom-0.1.9/BayesBoom/boom/Samplers/failed_experiments/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4929 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/failed_experiments/AdaptiveGaussianMixtureMhSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1774 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/Samplers/failed_experiments/AdaptiveRandomWalkMetropolisSampler.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.092033 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7454 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/JacobianChecker.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3988 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/JacobianChecker.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2996 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogPost.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2598 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogPost.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1597 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogTransform.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3600 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogTransform.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1775 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogitTransform.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3743 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogitTransform.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2244 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Loglike.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8470 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/MultinomialLogitTransform.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6055 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/MultinomialLogitTransform.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1408 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/ScalarLogpostTF.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1352 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/ScalarLogpostTF.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3939 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/TargetFun.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7193 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/TargetFun.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5263 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Transformation.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7368 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Transformation.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)       73 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/__init__.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.096033 BayesBoom-0.1.9/BayesBoom/boom/cpputil/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3518 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/AsciiGraph.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4446 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/AsciiGraph.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1610 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Constants.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    24173 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Date.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9088 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Date.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6869 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/DateTime.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4942 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/DateTime.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1199 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/DefaultVnames.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1157 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/DefaultVnames.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1839 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/LongString.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1485 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/LongString.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1789 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/OutputTable.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1470 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/OutputTable.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4854 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamFileIoManager.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1837 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamHolder.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2425 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamHolder.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    35880 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Polynomial.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2477 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Polynomial.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2329 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ProgressTracker.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4778 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Ptr.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1172 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Redirector.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1392 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Redirector.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1550 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/RefCounted.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4787 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/Split.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2924 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThreadTools.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8150 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThreadTools.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1335 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThrowException.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1647 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ToString.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2320 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/apply_permutation.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1471 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/apply_permutation.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1538 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/ask_to_continue.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2027 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/compare_vector_bool.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2196 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/compare_vector_bool.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1217 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/concatenate_strings.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1027 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/date_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1546 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/file_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1334 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/get_date.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1647 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/gll.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1114 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/gll.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2834 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/index_table.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1105 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/is_all_white.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1925 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/is_numeric.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1097 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/legalize_file_name.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1754 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/lse.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1579 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/lse.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1932 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/make_unique_preserve_order.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1616 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/math_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1090 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/nyi.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2563 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/parse_range.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1411 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/parse_range.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1435 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/portable_math.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1477 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/print.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2088 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/print_columns.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1167 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/random_element.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1230 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/read_file.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1201 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/rep.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1058 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/rep.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1613 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/replace_all.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1430 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/report_error.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2214 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/report_error.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1006 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/safelog.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1305 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/scan.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2471 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/seq.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1887 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/shift_element.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1722 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/shuffle.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5144 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/split.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1327 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/split_delimited.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1460 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/split_string.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1146 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/stream.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3358 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/string_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1137 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1107 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip_path.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1119 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip_white_space.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1218 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/substring_delimited.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1667 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/timer.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1387 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/trim_white_space.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1586 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/cpputil/unmap.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.096033 BayesBoom-0.1.9/BayesBoom/boom/distributions/
+-rw-r--r--   0 steve     (1000) steve     (1000)     5146 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/BinomialDistribution.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1576 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/BinomialDistribution.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7472 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4719 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3958 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2521 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3326 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Markov.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2451 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Markov.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    12589 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Rmath_dist.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10922 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Rmath_dist.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3927 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Tn2Sampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4334 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/Wishart.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7684 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/dirichlet.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2121 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/extreme_value.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    21009 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/gig.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2335 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/inverse_gaussian.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1915 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/inverse_gaussian.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3055 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/matrix_normal.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7057 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/mvn.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2521 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/mvt.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2608 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/random_cor.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1137 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/random_int.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1155 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/rlexp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3268 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/rmulti.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1450 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/rng.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2084 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/rng.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5451 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/rtriangle.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2182 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/student_fix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_exp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4879 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_gamma.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2705 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_gamma.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6156 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_logit.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3096 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_logit.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11546 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_norm.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2385 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions/usp.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    19623 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/distributions.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.096033 BayesBoom-0.1.9/BayesBoom/boom/math/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     1759 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephes_impl.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4250 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephes_rgamma.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     1759 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephus_impl.hpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     2679 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/chbevl.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     5151 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/dawsn.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     8875 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/ei.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     4782 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/expn.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     3845 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/fac.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     5999 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/fresnl.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     5860 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/planck.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     2836 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/polevl.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     8719 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/polylog.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     4006 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/powi.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     7229 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/shichi.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     7129 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/sici.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     3389 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/spence.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     4604 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/zeta.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     6667 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/cephes/zetac.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     2097 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/lmultigamma.cpp
+-rwxr-xr-x   0 steve     (1000) steve     (1000)     2593 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/math/special_functions.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/numopt/
+-rw-r--r--   0 steve     (1000) steve     (1000)    10194 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Brent.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2434 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Brent.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    89336 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Integral.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2622 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Integral.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1345 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/LinearAssignment.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2512 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/LinearAssignment.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3909 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/MarkovDecisionProcess.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3206 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/MarkovDecisionProcess.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1278 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Negate.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14430 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/NelderMead.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3514 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/NelderMead.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5865 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/NumericalDerivatives.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3997 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/NumericalDerivatives.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    81136 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Powell.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2119 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Powell.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1448 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Qlearning.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2331 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/Qlearning.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4048 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarLaplaceApproximation.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2193 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarLaplaceApproximation.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1629 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarNewtonMax.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1398 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarNewtonMax.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5977 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/bfgs.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5773 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/conj_grad.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1960 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/initialize_derivatives.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1923 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/initialize_derivatives.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/numopt/linear_assignment/
+-rw-r--r--   0 steve     (1000) steve     (1000)    10408 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/linear_assignment/lap.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7127 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/max_nd.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7508 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/nelder_mead.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7285 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/newton.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3197 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt/simulated_annealing.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    14809 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/numopt.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/pybind11/
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/pybind11/LinAlg/
+-rw-r--r--   0 steve     (1000) steve     (1000)    15089 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/LinAlg/LinAlgWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3226 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/BetaBinomialWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2232 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/BetaModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3015 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/DataWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2182 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/DirichletWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2170 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/GammaModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    10155 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/GaussianModelWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Glm/
+-rw-r--r--   0 steve     (1000) steve     (1000)    28906 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Glm/GlmModel_def.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     9712 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Glm/MlogitModel_def.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.100033 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Impute/
+-rw-r--r--   0 steve     (1000) steve     (1000)    35381 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Impute/Imputer_def.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/
+-rw-r--r--   0 steve     (1000) steve     (1000)     8043 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/beta_binomial_mixture_wrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4719 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/dpmvn_wrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2465 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/finite_mixture_wrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4186 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/ModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3126 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/MultinomialWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7371 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/MvnWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2758 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/ParameterWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/
+-rw-r--r--   0 steve     (1000) steve     (1000)    15004 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/DynamicRegressionModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    21028 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/MultivariateStateSpaceModelWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4288 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/MultivariateStateModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    38513 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/StateModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    23890 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateSpaceModelWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/TimeSeries/
+-rw-r--r--   0 steve     (1000) steve     (1000)     8403 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/TimeSeries/time_series_model_def.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)      662 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/UniformModelWrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1415 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/WishartModelWrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/cpputil/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1489 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/cpputil/cpputil_wrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/distributions/
+-rw-r--r--   0 steve     (1000) steve     (1000)      978 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/distributions/distribution_wrapper.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3285 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/module.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/numopt/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1148 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/numopt/numopt_wrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/stats/
+-rw-r--r--   0 steve     (1000) steve     (1000)    14413 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/stats/stats_wrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.104034 BayesBoom-0.1.9/BayesBoom/boom/pybind11/test_utils/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4699 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/pybind11/test_utils/test_utils_wrapper.cpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.108034 BayesBoom-0.1.9/BayesBoom/boom/stats/
+-rw-r--r--   0 steve     (1000) steve     (1000)     3093 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/AsciiDistributionCompare.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2910 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/AsciiDistributionCompare.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6422 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Bspline.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4082 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Bspline.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5078 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ChiSquareTest.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3729 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ChiSquareTest.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    26671 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/DataTable.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    13496 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/DataTable.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    46981 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Design.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    38370 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Design.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2748 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ECDF.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2736 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ECDF.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3009 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/EmpiricalDensity.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3246 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/EmpiricalDensity.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4165 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Encoders.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5677 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Encoders.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5754 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/FreqDist.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4401 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/FreqDist.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8114 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/IQagent.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2141 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/IQagent.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3708 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Mspline.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     5626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Mspline.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     8401 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/NaturalSpline.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2990 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/NaturalSpline.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2669 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Resampler.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4459 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Resampler.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2455 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Spline.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3852 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/Spline.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3710 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/compare_binomial_proportions.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1434 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/compare_binomial_proportions.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3101 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/compare_predictions.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1855 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/compare_predictions.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1529 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/diff.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1228 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/diff.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4620 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/hexbin.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3028 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/hexbin.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1844 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ks_critical_value.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2491 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/logit.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3524 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/logit.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     6021 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/moments.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2113 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/moments.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1052 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/ols.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1177 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/regression.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1052 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/regression.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1204 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/simple_random_sample.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     2052 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/simple_random_sample.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4976 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/summary.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     4464 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/stats/summary.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.108034 BayesBoom-0.1.9/BayesBoom/boom/test_utils/
+-rw-r--r--   0 steve     (1000) steve     (1000)     4947 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_derivatives.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3179 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_derivatives.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     7108 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_mcmc_matrix.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     3486 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/test_utils/distributions_match.cpp
+-rw-r--r--   0 steve     (1000) steve     (1000)    11321 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/test_utils/test_utils.hpp
+-rw-r--r--   0 steve     (1000) steve     (1000)     1367 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/to_data_table.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1085 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/boom/uint.hpp
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.108034 BayesBoom-0.1.9/BayesBoom/bsts/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1781 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      967 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/airpass.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     8387 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/ar.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    65415 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/bsts.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      362 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/bsts_test.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1058 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/data.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     7111 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/dynamic_regression_state_model.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     9594 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/gaussian.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     7246 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/general_seasonal_llt.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    10011 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/holiday.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4029 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/holiday_models.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4827 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/local_level.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     7464 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/local_linear_trend.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     5720 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/logit.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     5561 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/poisson.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     8236 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/seasonal.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    11847 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/semilocal_linear_trend.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     5255 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/state_models.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     8455 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/student.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    10235 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/student_local_linear_trend.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2209 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_ar.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    11721 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_bsts.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2144 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_dynamic_regression.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     2156 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_holidays.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1940 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_seasonal_llt.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     8239 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_state_models.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1942 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_student_llt.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1659 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_trig.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1108 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/test_utilities.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     5249 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/bsts/trig.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/BayesBoom/dynreg/
+-rw-r--r--   0 steve     (1000) steve     (1000)       93 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/dynreg/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    20164 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/dynreg/dynreg.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4824 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/dynreg/test_dynreg.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/BayesBoom/impute/
+-rw-r--r--   0 steve     (1000) steve     (1000)       37 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/impute/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    19204 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/impute/impute.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1695 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/impute/test_imputer.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/BayesBoom/mixtures/
+-rw-r--r--   0 steve     (1000) steve     (1000)      179 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/mixtures/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    14726 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/mixtures/beta_binomial_mixture.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    13065 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/mixtures/dirichlet_process.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     3265 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/mixtures/test_dirichlet_process.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      686 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/mixtures/utils.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/BayesBoom/spikeslab/
+-rw-r--r--   0 steve     (1000) steve     (1000)      784 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     6775 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/mlogit_spike.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     1211 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/mlogit_test.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    16737 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/priors.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    23516 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/spikeslab.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     5060 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/spikeslab/spikeslab_test.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/BayesBoom/test_utils/
+-rw-r--r--   0 steve     (1000) steve     (1000)      153 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/test_utils/__init__.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      505 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/test_utils/find_project_root.py
+-rw-r--r--   0 steve     (1000) steve     (1000)      413 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/test_utils/simulate_data.py
+-rw-r--r--   0 steve     (1000) steve     (1000)     4484 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom/test_utils/test_utils.py
+drwxr-xr-x   0 steve     (1000) steve     (1000)        0 2022-09-26 17:08:39.008032 BayesBoom-0.1.9/BayesBoom.egg-info/
+-rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom.egg-info/PKG-INFO
+-rw-r--r--   0 steve     (1000) steve     (1000)    82465 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom.egg-info/SOURCES.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)        1 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom.egg-info/dependency_links.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)        1 2022-01-04 15:04:54.000000 BayesBoom-0.1.9/BayesBoom.egg-info/not-zip-safe
+-rw-r--r--   0 steve     (1000) steve     (1000)       14 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom.egg-info/requires.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)       16 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/BayesBoom.egg-info/top_level.txt
+-rw-r--r--   0 steve     (1000) steve     (1000)      909 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/MANIFEST.in
+-rw-r--r--   0 steve     (1000) steve     (1000)     1626 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/PKG-INFO
+-rw-r--r--   0 steve     (1000) steve     (1000)       38 2022-09-26 17:08:39.112034 BayesBoom-0.1.9/setup.cfg
+-rw-r--r--   0 steve     (1000) steve     (1000)    15688 2022-09-26 17:08:38.000000 BayesBoom-0.1.9/setup.py
```

### Comparing `BayesBoom-0.1.8/BayesBoom/R/R.py` & `BayesBoom-0.1.9/BayesBoom/R/R.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/__init__.py` & `BayesBoom-0.1.9/BayesBoom/R/__init__.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/autoclean.py` & `BayesBoom-0.1.9/BayesBoom/R/autoclean.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/bayes.py` & `BayesBoom-0.1.9/BayesBoom/R/bayes.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/boom_py_utils.py` & `BayesBoom-0.1.9/BayesBoom/R/boom_py_utils.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/cbind.py` & `BayesBoom-0.1.9/BayesBoom/R/cbind.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/data_table.py` & `BayesBoom-0.1.9/BayesBoom/R/data_table.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/density.py` & `BayesBoom-0.1.9/BayesBoom/R/density.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/encoding.py` & `BayesBoom-0.1.9/BayesBoom/R/encoding.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/graphics_device.py` & `BayesBoom-0.1.9/BayesBoom/R/graphics_device.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/mcmc.py` & `BayesBoom-0.1.9/BayesBoom/R/mcmc.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/plots.py` & `BayesBoom-0.1.9/BayesBoom/R/plots.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/probability.py` & `BayesBoom-0.1.9/BayesBoom/R/probability.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_R.py` & `BayesBoom-0.1.9/BayesBoom/R/test_R.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_cbind.py` & `BayesBoom-0.1.9/BayesBoom/R/test_cbind.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_data_table.py` & `BayesBoom-0.1.9/BayesBoom/R/test_data_table.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_encoding.py` & `BayesBoom-0.1.9/BayesBoom/R/test_encoding.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_plots.py` & `BayesBoom-0.1.9/BayesBoom/R/test_plots.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_probability.py` & `BayesBoom-0.1.9/BayesBoom/R/test_probability.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/test_utils.py` & `BayesBoom-0.1.9/BayesBoom/R/test_utils.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/R/utils.py` & `BayesBoom-0.1.9/BayesBoom/R/utils.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/Bmath.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/Bmath.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/Random.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/Random.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/bd0.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/bd0.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/bessel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/bessel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/bessel_k.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/bessel_k.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/beta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/beta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/chebyshev.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/chebyshev.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/choose.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/choose.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/d1mach.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/d1mach.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dcauchy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dcauchy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/df.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/df.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dgamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dgamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dgeom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dgeom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dhyper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dhyper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dlnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dlnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dlogis.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dlogis.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dpois.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dpois.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dpq.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dpq.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dunif.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dunif.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/dweibull.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/dweibull.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/fprec.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/fprec.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/fround.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/fround.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/fsign.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/fsign.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/ftrunc.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/ftrunc.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/gamma_cody.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/gamma_cody.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/gammalims.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/gammalims.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/i1mach.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/i1mach.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/lbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/lbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/lgammacor.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/lgammacor.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/mlutils.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/mlutils.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/nmath.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/nmath.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pcauchy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pcauchy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pgamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pgamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pgeom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pgeom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/phyper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/phyper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/plnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/plnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/plogis.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/plogis.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pnt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pnt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/polygamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/polygamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/ppois.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/ppois.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/ptukey.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/ptukey.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/punif.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/punif.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/pweibull.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/pweibull.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qcauchy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qcauchy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qgamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qgamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qgeom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qgeom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qhyper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qhyper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qlnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qlnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qlogis.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qlogis.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qpois.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qpois.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qtukey.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qtukey.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qunif.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qunif.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/qweibull.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/qweibull.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rbeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rbeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rcauchy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rcauchy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rgamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rgamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rgeom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rgeom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rhyper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rhyper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rlnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rlnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rloggamma_small_alpha.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rloggamma_small_alpha.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rlogis.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rlogis.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rmultinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rmultinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnbinom.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnbinom.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnchisq.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnchisq.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rnorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rnorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rpois.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rpois.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/runif.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/runif.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/rweibull.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/rweibull.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/sexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/sexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/sign.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/sign.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/snorm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/snorm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/stirlerr.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/stirlerr.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/toms708.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/toms708.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Bmath/unif_rand.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Bmath/unif_rand.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Cholesky` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/CholmodSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Core` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Core`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Eigenvalues` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Geometry` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Householder` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/IterativeLinearSolvers` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Jacobi` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/KLUSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/LU` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/LU`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/MetisSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/OrderingMethods` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/PaStiXSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/PardisoSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/QR` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/QR`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/QtAlignedMalloc` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SPQRSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SVD` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/Sparse` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseCholesky` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseCore` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseLU` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SparseQR` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdDeque` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdList` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/StdVector` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/SuperLUSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/UmfPackSupport` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LDLT.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LLT.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Cholesky/LLT_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/CholmodSupport/CholmodSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArithmeticSequence.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Array.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArrayBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ArrayWrapper.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Assign.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/AssignEvaluator.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Assign_MKL.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/BandMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Block.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/BooleanRedux.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CommaInitializer.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ConditionEstimator.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CoreEvaluators.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CoreIterators.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseBinaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseNullaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseTernaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseUnaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/CwiseUnaryView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseCoeffsBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DenseStorage.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Diagonal.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DiagonalMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/DiagonalProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Dot.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/EigenBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ForceAlignedAccess.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Fuzzy.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GeneralProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GenericPacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/GlobalFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/IO.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/IndexedView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Inverse.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Map.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MapBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MathFunctionsImpl.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Matrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/MatrixBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NestByValue.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NoAlias.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/NumTraits.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PartialReduxEvaluator.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PermutationMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/PlainObjectBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Product.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ProductEvaluators.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Random.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Redux.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Ref.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Replicate.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Reshaped.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/ReturnByValue.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Reverse.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Select.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SelfAdjointView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SelfCwiseBinaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Solve.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SolveTriangular.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/SolverBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/StableNorm.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/StlIterators.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Stride.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Swap.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Transpose.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Transpositions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/TriangularMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/VectorBlock.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/VectorwiseOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/Visitor.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/CUDA/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/BFloat16.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/ConjHelper.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/Half.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/Settings.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/Default/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/GPU/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/MSA/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/NEON/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SSE/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SVE/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/Complex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/arch/ZVector/PacketMath.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/AssignmentFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/BinaryFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/NullaryFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/StlFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/TernaryFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/functors/UnaryFunctors.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/Parallelizer.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/SelfadjointRank2Update.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/BlasUtil.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ConfigureVectorization.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Constants.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/DisableStupidWarnings.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ForwardDeclarations.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/IndexedViewHelper.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/IntegralConstant.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/MKL_support.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Macros.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Memory.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/Meta.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ReenableStupidWarnings.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/ReshapedHelper.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/StaticAssert.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/SymbolicIndex.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Core/util/XprHelper.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/EigenSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealQZ.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Eigenvalues/Tridiagonalization.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/AlignedBox.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/AngleAxis.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/EulerAngles.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Homogeneous.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Hyperplane.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/OrthoMethods.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/ParametrizedLine.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Quaternion.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Rotation2D.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/RotationBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Scaling.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Transform.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Translation.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/Umeyama.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/BlockHouseholder.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/Householder.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Householder/HouseholderSequence.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/Jacobi/Jacobi.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/KLUSupport/KLUSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/Determinant.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/FullPivLU.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/InverseImpl.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/PartialPivLU.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/LU/arch/InverseSize4.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/MetisSupport/MetisSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Amd.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/OrderingMethods/Ordering.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/PardisoSupport/PardisoSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/FullPivHouseholderQR.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/HouseholderQR.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/BDCSVD.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/JacobiSVD.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/SVDBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SVD/UpperBidiagonalization.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/AmbiVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/CompressedStorage.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/MappedSparseMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseAssign.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseBlock.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseColEtree.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCompressedBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDenseProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseDot.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseFuzzy.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMap.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrixBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparsePermutation.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseProduct.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseRedux.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseRef.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSolverBase.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseTranspose.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseTriangularView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseUtil.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/SparseView.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseCore/TriangularSolver.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLUImpl.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Memory.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Structs.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Utils.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pivotL.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pruneL.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SparseQR/SparseQR.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdDeque.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdList.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/StdVector.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/StlSupport/details.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/Image.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/Kernel.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/RealSvd2x2.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/blas.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/lapack.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/misc/lapacke.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/BlockMethods.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/IndexedViewMethods.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Eigen/src/plugins/ReshapedMethods.h` & `BayesBoom-0.1.9/BayesBoom/boom/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Array.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Array.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Array.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Array.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/ArrayIterator.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/ArrayIterator.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/ArrayIterator.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/ArrayIterator.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Cholesky.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Cholesky.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Cholesky.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Cholesky.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/CorrelationMatrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/CorrelationMatrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/CorrelationMatrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/CorrelationMatrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/DiagonalMatrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/DiagonalMatrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/DiagonalMatrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/DiagonalMatrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Eigen.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Eigen.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Eigen.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Eigen.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/EigenMap.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/EigenMap.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Givens.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Givens.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Givens.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Givens.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/LU.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/LU.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/LU.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/LU.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Matrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Matrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Matrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/MatrixPartition.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/MatrixPartition.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/MatrixPartition.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/MatrixPartition.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/QR.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/QR.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/QR.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/QR.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SVD.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SVD.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SVD.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SVD.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SWEEP.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SWEEP.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SWEEP.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SWEEP.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Selector.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Selector.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Selector.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Selector.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SpdMatrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SpdMatrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SpdMatrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SpdMatrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SubMatrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SubMatrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/SubMatrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/SubMatrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Vector.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Vector.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/Vector.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/Vector.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorView.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorView.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorView.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorView.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/VectorViewIterator.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/VectorViewIterator.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/stack_columns.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/stack_columns.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/LinAlg/stack_columns.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/LinAlg/stack_columns.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/Bart.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/Bart.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/Bart.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/Bart.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianBartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianBartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianBartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianBartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/GaussianLinearBartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/LogitBartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/LogitBartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/LogitBartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/LogitBartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PoissonBartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PoissonBartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PoissonBartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PoissonBartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/BartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianBartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/GaussianLinearBartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/LogitBartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/PoissonBartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/PosteriorSamplers/ProbitBartPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ProbitBartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ProbitBartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ProbitBartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ProbitBartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ResidualRegressionData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ResidualRegressionData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Bart/ResidualRegressionData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Bart/ResidualRegressionData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BernoulliModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BernoulliModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BetaBinomialModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BetaBinomialModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BetaBinomialModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BetaBinomialModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BetaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BetaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BetaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BetaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BinomialModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BinomialModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/BinomialModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/BinomialModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CategoricalData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CategoricalData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CategoricalData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CategoricalData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ChisqModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ChisqModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ChisqModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ChisqModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/CompositeModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/CompositeModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ConstrainedVectorParams.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ConstrainedVectorParams.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ConstrainedVectorParams.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ConstrainedVectorParams.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DataPair.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DataPair.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DataTypes.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DataTypes.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DataTypes.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DataTypes.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DirichletModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DirichletModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DirichletModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DirichletModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DiscreteUniformModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DiscreteUniformModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DiscreteUniformModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DiscreteUniformModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/DoubleModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/DoubleModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/EmMixtureComponent.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/EmMixtureComponent.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialIncrementModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialIncrementModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialIncrementModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialIncrementModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ExponentialModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ExponentialModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/FiniteMixtureModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/FiniteMixtureModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/FiniteMixtureModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/FiniteMixtureModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelBase.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelGivenSigma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelGivenSigma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/GaussianModelGivenSigma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/GaussianModelGivenSigma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/AggregatedRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialLogitModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialLogitModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialLogitModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialLogitModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialProbitModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialProbitModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialProbitModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialProbitModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialRegressionData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialRegressionData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/BinomialRegressionData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/BinomialRegressionData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ChoiceData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ChoiceData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ChoiceData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ChoiceData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GammaRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GammaRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GammaRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GammaRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/Glm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/Glm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/Glm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/Glm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmCoefs.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmCoefs.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmCoefs.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmCoefs.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/GlmMvnPriorBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/GlmMvnPriorBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/HierarchicalPoissonRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/IndependentRegressionModels.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/IndependentRegressionModels.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/IndependentRegressionModels.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/IndependentRegressionModels.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LogisticRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LogisticRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LogisticRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LogisticRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LoglinearModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LoglinearModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/LoglinearModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/LoglinearModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ModelSelectionConcepts.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ModelSelectionConcepts.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialLogitModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialLogitModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialLogitModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialLogitModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialProbitModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialProbitModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultinomialProbitModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultinomialProbitModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultivariateRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultivariateRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MultivariateRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MultivariateRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvnGivenX.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvnGivenX.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvnGivenX.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvnGivenX.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvtRegModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvtRegModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/MvtRegModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/MvtRegModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/OrdinalCutpointModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PoissonRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PoissonRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AdaptiveSpikeSlabRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/AggregatedRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BigAssSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitAuxmixSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitCompositeSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerRwm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSamplerTim.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialLogitSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitCompositeSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BinomialProbitTimSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/BregVsSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/CorrelationMap.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/DAFE_MLM.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/GammaRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/HierarchicalPoissonRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/IndependentRegressionModelsPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/IndependentRegressionModelsPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LogitSamplerBma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/LoglinearModelBipfSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLAuxMixSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MLVS_data_imputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MlogitRwm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaGivenSigmaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MnpBetaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompleteDataSuf.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultinomialLogitCompositeSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MultivariateRegressionSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/MvtRegSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NonconjugateRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/NormalMixtureApproximation.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/OrdinalLogitPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PartRegSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionAuxMixSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionRwmSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/PoissonRegressionSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ProbitSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/QuantileRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionCoefficientSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionSemiconjugateSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/RegressionShrinkageSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabDaRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/SpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/TRegressionSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/VsPriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedGammaRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedGammaRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedLognormalRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/ZeroInflatedPoissonRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/draw_logit_lambda.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_1.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_1.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_2.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_2.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_3.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/fill_poisson_mixture_approximation_table_3.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/PosteriorSamplers/poisson_mixture_approximation_table.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ProbitRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ProbitRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ProbitRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ProbitRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/QuantileRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/QuantileRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/QuantileRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/QuantileRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionSlabPrior.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionSlabPrior.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/RegressionSlabPrior.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/RegressionSlabPrior.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/TRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/TRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/TRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/TRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/VariableSelectionPrior.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/VariableSelectionPrior.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/VariableSelectionPrior.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/VariableSelectionPrior.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/WeightedRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/WeightedRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/WeightedRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/WeightedRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedGammaRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedLognormalRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Glm/ZeroInflatedPoissonRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Event.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Event.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Event.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Event.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/NestedHmm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/PosteriorSamplers/NestedHmmPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Session.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Session.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Session.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Session.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Stream.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Stream.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/Clickstream/Stream.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/Clickstream/Stream.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/GeneralHmmStateSpaceWrapper.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HMM2.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HMM2.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HMM2.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HMM2.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HealthStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HealthStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HealthStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HealthStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmFilter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmFilter.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/HmmFilter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/HmmFilter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/HmmPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/PosteriorSamplers/LiuWestParticleFilter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/hmm_tools.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/hmm_tools.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/HMM/hmm_tools.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/HMM/hmm_tools.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalDirichletModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalGaussianRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalPoissonModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedGammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/HierarchicalZeroInflatedPoissonModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierGaussianRegressionAsisSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalDirichletPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGammaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalGaussianRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalPoissonSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedGammaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Hierarchical/PosteriorSamplers/HierarchicalZeroInflatedPoissonSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcr.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcr.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrItemSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrItemSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwm.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwm.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwmItemSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwmItemSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrRwmSubject.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrRwmSubject.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/DafePcrSubject.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/DafePcrSubject.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IRT.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IRT.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IRT.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IRT.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IrtModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IrtModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/IrtModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/IrtModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Item.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Item.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Item.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Item.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/ItemDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/ItemDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/ItemSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/ItemSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PartialCreditModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PartialCreditModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PartialCreditModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PartialCreditModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/PcrNid.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/PcrNid.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Subject.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Subject.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/Subject.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/Subject.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectPrior.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectPrior.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectPrior.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectPrior.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectSliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectSliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/SubjectSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/SubjectSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IRT/multisubscale_logit_cutpoint_model.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IRT/multisubscale_logit_cutpoint_model.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MixedDataImputerWithErrorCorrection.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Impute/MvRegCopulaDataImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/IndependentMvnModelGivenScalarSigma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/LognormalModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/LognormalModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/LognormalModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/LognormalModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MarginallyUniformCorrelationModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MarkovModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MarkovModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MarkovModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MarkovModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MatrixNormalModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MatrixNormalModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MatrixNormalModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MatrixNormalModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/BetaBinomialMixture.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/ConditionalFiniteMixtureModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMixture.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/DirichletProcessMvnModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/MvnMetaAnalysisDPMPriorModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/BetaBinomialMixturePosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/ConditionalFiniteMixtureSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessCollapsedGibbsSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessMvnCollapsedGibbsSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/DirichletProcessSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/MvnMetaAnalysisDPMPriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/PosteriorSamplers/SplitMerge.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/identify_permutation.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/identify_permutation.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Mixtures/identify_permutation.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Mixtures/identify_permutation.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ModelTypes.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ModelTypes.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ModelTypes.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ModelTypes.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MultinomialModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MultinomialModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MultinomialModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MultinomialModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnBase.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenScalarSigma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenScalarSigma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenScalarSigma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenScalarSigma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenSigma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenSigma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnGivenSigma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnGivenSigma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvnModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvnModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvtModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvtModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/MvtModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/MvtModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/GaussianFeedForwardNeuralNetwork.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/Nnet.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/Nnet.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/Nnet.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/Nnet.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/GaussianFeedForwardPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Nnet/PosteriorSamplers/HiddenLayerImputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ParamTypes.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ParamTypes.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ParamTypes.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ParamTypes.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/BoundedPoissonProcessSimulator.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/CosinePoissonProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/HomogeneousPoissonProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/MarkovModulatedPoissonProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PointProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PointProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PointProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PointProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonClusterProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PoissonProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PoissonProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/HomogPoissonProcessPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/MmppPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/PoissonClusterPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/PoissonClusterPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/PosteriorSamplers/WeeklyCyclePoissonProcessSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PointProcess/WeeklyCyclePoissonProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonGammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonGammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonGammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonGammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PoissonModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PoissonModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/CompositeParamPolicy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/CompositeParamPolicy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/CompositeParamPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/CompositeParamPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/DataInfoPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/DataInfoPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/DeferredDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/DeferredDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/IID_DataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/IID_DataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ManyParamPolicy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ManyParamPolicy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ManyParamPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ManyParamPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/MixtureDataPolicy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/MixtureDataPolicy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/MixtureDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/MixtureDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NonparametricParamPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NonparametricParamPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullParamPolicy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullParamPolicy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullParamPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullParamPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/NullPriorPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/NullPriorPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_1.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_1.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_2.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_2.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_3.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_3.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/ParamPolicy_4.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/ParamPolicy_4.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/PriorPolicy.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/PriorPolicy.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/PriorPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/PriorPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Policies/SufstatDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Policies/SufstatDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/AbsorbingMarkovConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaBinomialSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/BetaPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeModelSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CompositeSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/CorrelationSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/DirichletPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExchangeableDirichletSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ExponentialGammaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FiniteMixturePosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FiniteMixturePosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedProbBinomialSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedSpdSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedSpdSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/FixedUnivariateSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/FixedUnivariateSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GammaPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianGivenSigmaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianMeanSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GaussianVarSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericGaussianVarianceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/GenericStudentSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/HierarchicalPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/Imputer.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/Imputer.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/Imputer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/Imputer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/IndependentMvnVarSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MarkovConjShrinkageSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MultinomialDirichletSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnIndependentVarianceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnMeanSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/MvnVarSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PoissonGammaSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/PosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ProductDirichletPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SepStratSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/SharedSigsqSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedGammaPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedLognormalPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroInflatedPoissonSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanGaussianConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnConjSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/PosteriorSamplers/ZeroMeanMvnIndependenceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ProductDirichletModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ProductDirichletModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ProductDirichletModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ProductDirichletModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ProductVectorModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ProductVectorModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ProductVectorModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ProductVectorModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ScaledChisqModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ScaledChisqModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ScaledChisqModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ScaledChisqModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdParams.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdParams.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SpdParams.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SpdParams.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/AggregatedStateSpaceRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicInterceptRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicRegression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicRegression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/DynamicRegression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/DynamicRegression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionalIidKalmanFilter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ConditionallyIndependentKalmanFilter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanFilterBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/KalmanTools.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -322,25 +322,29 @@
       //  L[t] = T[t] - K[t] Z[t]
       // so
       // r[t-1] = Z' * Finv * v - T'r + Z'K'r
       //
       // u = Finv * v - K'r
       // r = T'r + Z'u
       const Selector &observed(model()->observed_status(t));
-      Ptr<SparseKalmanMatrix> observation_coefficients(
-          model()->observation_coefficients(t, observed));
       Ptr<SparseKalmanMatrix> transition(
           model()->state_transition_matrix(t));
-      Ptr<SparseKalmanMatrix> forecast_precision_ptr(
-          marg.sparse_forecast_precision());
-      const SparseKalmanMatrix &forecast_precision(
-          *forecast_precision_ptr);
-      Vector u = forecast_precision * marg.prediction_error()
-          - marg.sparse_kalman_gain(observed, forecast_precision_ptr)->Tmult(r);
-      r = transition->Tmult(r) + observation_coefficients->Tmult(u);
+      if (observed.nvars() > 0) {
+        Ptr<SparseKalmanMatrix> observation_coefficients(
+            model()->observation_coefficients(t, observed));
+        Ptr<SparseKalmanMatrix> forecast_precision_ptr(
+            marg.sparse_forecast_precision());
+        const SparseKalmanMatrix &forecast_precision(
+            *forecast_precision_ptr);
+        Vector u = forecast_precision * marg.prediction_error()
+            - marg.sparse_kalman_gain(observed, forecast_precision_ptr)->Tmult(r);
+        r = transition->Tmult(r) + observation_coefficients->Tmult(u);
+      } else {
+        r = transition->Tmult(r);
+      }
     }
     set_initial_scaled_state_error(r);
   }
 
   //===========================================================================
   void MultivariateKalmanFilterBase::smooth() {
     // All implicit subsctipts are [t].
@@ -394,45 +398,46 @@
       //  where
       //  L[t] = T[t] - K[t] Z[t]
       // so
       // r[t-1] = Z' * Finv * v - T'r + Z'K'r
       //
       // u = Finv * v - K'r
       // r = T'r + Z'u
-      const Selector &observed(model()->observed_status(t));
-      Ptr<SparseKalmanMatrix> observation_coefficients(
-          model()->observation_coefficients(t, observed));
       Ptr<SparseKalmanMatrix> transition(
           model()->state_transition_matrix(t));
-      Ptr<SparseKalmanMatrix> forecast_precision_ptr(
-          marg.sparse_forecast_precision());
-      const SparseKalmanMatrix &forecast_precision(
-          *forecast_precision_ptr);
-      Ptr<SparseKalmanMatrix> kalman_gain(marg.sparse_kalman_gain(
-          observed, forecast_precision_ptr));
-
-
-      NEW(SparseMatrixProduct, KZ)();
-      KZ->add_term(kalman_gain);
-      KZ->add_term(observation_coefficients);
-      NEW(SparseMatrixSum, L)();
-      L->add_term(transition);
-      L->add_term(KZ, -1);
-
-      Vector u = forecast_precision * marg.prediction_error()
-          - kalman_gain->Tmult(r);
-
-      // Turn r[t] into r[t-1]
-      r = transition->Tmult(r) + observation_coefficients->Tmult(u);
-
-      // Turn N[t] into N[t-1]
-      Matrix tmp = observation_coefficients->Tmult(
-          forecast_precision * observation_coefficients->dense())
-          + L->sandwich_transpose(N);
-      N = tmp;
+      const Selector &observed(model()->observed_status(t));
+      if (observed.nvars() > 0) {
+        Ptr<SparseKalmanMatrix> observation_coefficients(
+            model()->observation_coefficients(t, observed));
+        Ptr<SparseKalmanMatrix> forecast_precision_ptr(
+            marg.sparse_forecast_precision());
+        const SparseKalmanMatrix &forecast_precision(
+            *forecast_precision_ptr);
+        Ptr<SparseKalmanMatrix> kalman_gain(marg.sparse_kalman_gain(
+            observed, forecast_precision_ptr));
+        NEW(SparseMatrixProduct, KZ)();
+        KZ->add_term(kalman_gain);
+        KZ->add_term(observation_coefficients);
+        NEW(SparseMatrixSum, L)();
+        L->add_term(transition);
+        L->add_term(KZ, -1);
+        Vector u = forecast_precision * marg.prediction_error()
+            - kalman_gain->Tmult(r);
+
+        // Turn r[t] into r[t-1]
+        r = transition->Tmult(r) + observation_coefficients->Tmult(u);
+        // Turn N[t] into N[t-1]
+        Matrix tmp = observation_coefficients->Tmult(
+            forecast_precision * observation_coefficients->dense())
+            + L->sandwich_transpose(N);
+        N = tmp;
+      } else {
+        r = transition->Tmult(r);
+        N = transition->sandwich_transpose(N);
+      }
 
       Vector filtered_state_mean;
       SpdMatrix filtered_state_variance;
       if (t > 0) {
         Kalman::MultivariateMarginalDistributionBase &prev(node(t-1));
         filtered_state_mean = prev.state_mean();
         filtered_state_variance = prev.state_variance();
```

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/MultivariateKalmanFilterBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/ScalarKalmanFilter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseKalmanTools.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Filters/SparseVector.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/MultiplexedData.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/MultiplexedData.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/MultiplexedData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/MultiplexedData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -359,21 +359,25 @@
       : filter_(this),
         simulation_filter_(this)
   {}
 
   // A precondition is that the state at time t was simulated by the forward
   // portion of the Durbin-Koopman data augmentation algorithm.
   Vector CiidBase::simulate_fake_observation(RNG &rng, int t) {
-     Vector ans = (*observation_coefficients(
-         t, observed_status(t))) * shared_state().col(t);
-     double sigma = sqrt(observation_variance(t));
-     for (int i = 0; i < ans.size(); ++i) {
-       ans[i] += rnorm_mt(rng, 0, sigma);
-     }
-     return ans;
+    const Selector &obs(observed_status(t));
+    if (obs.nvars() == 0) {
+      return Vector(0);
+    } else {
+      Vector ans = (*observation_coefficients(t, obs) * shared_state().col(t));
+      double sigma = sqrt(observation_variance(t));
+      for (int i = 0; i < ans.size(); ++i) {
+        ans[i] += rnorm_mt(rng, 0, sigma);
+      }
+      return ans;
+    }
    }
 
   ConditionalIidKalmanFilter & CiidBase::get_filter() {
     return filter_;
   }
 
   const ConditionalIidKalmanFilter & CiidBase::get_filter() const {
@@ -401,21 +405,25 @@
   //===========================================================================
 
   namespace {
     using CindBase = ConditionallyIndependentMultivariateStateSpaceModelBase;
   }  // namespace
 
   Vector CindBase::simulate_fake_observation(RNG &rng, int t) {
-    Vector ans = (*observation_coefficients(t, observed_status(t)))
-        * shared_state().col(t);
-    for (int i = 0; i < ans.size(); ++i) {
-      double sigma = sqrt(single_observation_variance(t, i));
-      ans[i] += rnorm_mt(rng, 0, sigma);
+    const Selector &obs(observed_status(t));
+    if (obs.nvars() == 0) {
+      return Vector(0);
+    } else {
+      Vector ans = (*observation_coefficients(t, obs)) * shared_state().col(t);
+      for (int i = 0; i < ans.size(); ++i) {
+        double sigma = sqrt(single_observation_variance(t, i));
+        ans[i] += rnorm_mt(rng, 0, sigma);
+      }
+      return ans;
     }
-    return ans;
   }
 
   void CindBase::update_observation_model(
       Vector &r,
       SpdMatrix &N,
       int t,
       bool save_state_distributions,
```

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceModelBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/MultivariateStateSpaceRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MultivariateStateSpaceModelSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/MvStateSpaceRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/ScalarStateModelAdapterPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/PosteriorSamplers/SharedLocalLevelPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -133,26 +133,28 @@
       state_model(s)->observe_state(
           state_component(then, s),
           state_component(now, s),
           time_now);
     }
 
     const Selector &observed(host_->observed_status(time_now));
-    Vector residual_y =
-        host_->adjusted_observation(time_now)
-        - (*host_->observation_coefficients(time_now, observed)
-           * host_->shared_state(time_now))
-        + (*observation_coefficients(time_now, observed)) * now;
+    if (observed.nvars() > 0) {
+      Vector residual_y =
+          host_->adjusted_observation(time_now)
+          - (*host_->observation_coefficients(time_now, observed)
+             * host_->shared_state(time_now))
+          + (*observation_coefficients(time_now, observed)) * now;
 
-    double predictive_state = component_observation_coefficients(
-        time_now).dot(now);
+      double predictive_state = component_observation_coefficients(
+          time_now).dot(now);
 
-    for (int i = 0; i < observed.nvars(); ++i) {
-      int I = observed.sparse_index(i);
-      sufficient_statistics_[I].increment(predictive_state, residual_y[i]);
+      for (int i = 0; i < observed.nvars(); ++i) {
+        int I = observed.sparse_index(i);
+        sufficient_statistics_[I].increment(predictive_state, residual_y[i]);
+      }
     }
   }
 
   // The observation coefficients are Beta * Z[t], where Z[t] is the set of
   // observation coefficients from the component state models and Beta is the
   // set of regression coefficients.  If the dimension of y[t] is m x 1 and the
   // dimension of the managed state is p x 1, then Beta is m x 1, Z[t] is 1 x p,
```

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/ScalarStateModelAdapter.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedLocalLevel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/StateModels/SharedStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/Multivariate/tests/mv_framework.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/Multivariate/tests/mv_framework.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/AggregatedStateSpacePosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicInterceptRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicInterceptRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionArPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionDirectGibbs.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/DynamicRegressionPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceLogitPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePoissonPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpacePosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceRegressionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceRegressionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StateSpaceStudentPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/StudentLocalLinearTrendPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/SufstatManager.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/PosteriorSamplers/SufstatManager.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModelVector.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModelVector.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModelVector.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModelVector.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/ArStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionArStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/DynamicRegressionStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/GeneralSeasonalStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/HierarchicalRegressionHolidayStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/Holiday.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLevelStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/LocalLinearTrend.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/PosteriorSamplers/GeneralSeasonalLLTPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RandomWalkHolidayStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionHolidayStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/RegressionStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SeasonalStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/SemilocalLinearTrend.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StaticInterceptStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/StudentLocalLinearTrend.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/TrigStateModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/ArStateModelTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/ArStateModelTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/HolidayTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/HolidayTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLevelModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLevelModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLinearTrendModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/LocalLinearTrendModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SeasonalTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SeasonalTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SemilocalLinearTrendTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/SemilocalLinearTrendTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StateTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StateTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StaticInterceptTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StaticInterceptTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StudentLocalLinearTrendTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/StudentLocalLinearTrendTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/TrigTestModule.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateModels/test_utils/TrigTestModule.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceLogitModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceModelBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceNormalMixture.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpacePoissonModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/StateSpaceStudentRegressionModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/DynamicInterceptTestFramework.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/DynamicInterceptTestFramework.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/StateSpaceTestFramework.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/StateSpaceTestFramework.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/TestFrameworkBase.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/TestFrameworkBase.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/StateSpace/tests/state_space_test_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/StateSpace/tests/state_space_test_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Sufstat.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Sufstat.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/Sufstat.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/Sufstat.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/SufstatAbstractCombineImpl.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/SufstatAbstractCombineImpl.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaPriors.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaPriors.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/ArmaPriors.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/ArmaPriors.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/MarkovLink.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/MarkovLink.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/NonzeroMeanAr1Model.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArPosteriorSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArSpikeSlabSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaGibbsMhSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaGibbsMhSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/ArmaSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/PosteriorSamplers/NonzeroMeanAr1Sampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeries.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeries.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeriesDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeriesDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TimeSeries/TimeSeriesSufstatDataPolicy.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TimeSeries/TimeSeriesSufstatDataPolicy.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TruncatedGammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TruncatedGammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/TruncatedGammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/TruncatedGammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformCorrelationModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformCorrelationModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformCorrelationModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformCorrelationModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformShrinkagePriorModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformShrinkagePriorModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/UniformShrinkagePriorModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/UniformShrinkagePriorModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/VectorModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/VectorModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedData.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedData.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedGaussianSuf.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedGaussianSuf.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedGaussianSuf.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedGaussianSuf.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedMvnModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedMvnModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WeightedMvnModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WeightedMvnModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WishartModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WishartModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/WishartModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/WishartModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedGammaModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedGammaModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedGammaModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedGammaModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedLognormalModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedLognormalModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedLognormalModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedLognormalModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedPoissonModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedPoissonModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroInflatedPoissonModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroInflatedPoissonModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanGaussianModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanGaussianModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanGaussianModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanGaussianModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanMvnModel.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanMvnModel.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Models/ZeroMeanMvnModel.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Models/ZeroMeanMvnModel.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ARMS.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ARMS.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ARMS.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ARMS.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/DirectProposal.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/DirectProposal.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/DirectProposal.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/DirectProposal.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/Gilks/arms.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/Gilks/arms.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/Gilks/arms.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/Gilks/arms.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ImportanceResampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ImportanceResampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ImportanceResampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ImportanceResampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MH_Proposals.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MH_Proposals.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MH_Proposals.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MH_Proposals.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MetropolisHastings.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MetropolisHastings.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MetropolisHastings.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MetropolisHastings.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MoveAccounting.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MoveAccounting.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/MoveAccounting.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/MoveAccounting.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/RejectionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/RejectionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/RejectionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/RejectionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/Sampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/Sampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/Sampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/Sampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarAdaptiveRejectionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarLangevinSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarLangevinSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarLangevinSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarLangevinSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarSliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarSliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/ScalarSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/ScalarSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/SliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/SliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/SliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/SliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/TIM.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/TIM.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/TIM.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/TIM.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateLangevinSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateLangevinSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateLangevinSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateLangevinSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateSliceSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateSliceSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/UnivariateSliceSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/UnivariateSliceSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/failed_experiments/AdaptiveGaussianMixtureMhSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/failed_experiments/AdaptiveGaussianMixtureMhSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/Samplers/failed_experiments/AdaptiveRandomWalkMetropolisSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/Samplers/failed_experiments/AdaptiveRandomWalkMetropolisSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/JacobianChecker.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/JacobianChecker.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/JacobianChecker.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/JacobianChecker.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogPost.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogPost.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogPost.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogPost.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogTransform.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogTransform.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogTransform.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogTransform.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogitTransform.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogitTransform.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/LogitTransform.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/LogitTransform.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Loglike.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Loglike.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/MultinomialLogitTransform.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/MultinomialLogitTransform.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/MultinomialLogitTransform.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/MultinomialLogitTransform.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/ScalarLogpostTF.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/ScalarLogpostTF.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/ScalarLogpostTF.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/ScalarLogpostTF.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/TargetFun.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/TargetFun.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/TargetFun.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/TargetFun.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Transformation.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Transformation.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/TargetFun/Transformation.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/TargetFun/Transformation.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/AsciiGraph.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/AsciiGraph.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/AsciiGraph.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/AsciiGraph.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Constants.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Constants.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Date.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Date.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Date.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Date.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/DateTime.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/DateTime.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/DateTime.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/DateTime.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/DefaultVnames.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/DefaultVnames.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/DefaultVnames.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/DefaultVnames.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/LongString.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/LongString.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/LongString.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/LongString.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/OutputTable.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/OutputTable.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/OutputTable.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/OutputTable.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamFileIoManager.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamFileIoManager.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamHolder.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamHolder.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ParamHolder.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ParamHolder.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Polynomial.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Polynomial.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Polynomial.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Polynomial.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ProgressTracker.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ProgressTracker.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Ptr.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Ptr.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Redirector.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Redirector.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Redirector.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Redirector.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/RefCounted.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/RefCounted.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/Split.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/Split.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThreadTools.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThreadTools.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThreadTools.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThreadTools.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ThrowException.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ThrowException.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ToString.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ToString.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/apply_permutation.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/apply_permutation.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/apply_permutation.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/apply_permutation.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/ask_to_continue.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/ask_to_continue.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/compare_vector_bool.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/compare_vector_bool.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/compare_vector_bool.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/compare_vector_bool.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/concatenate_strings.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/concatenate_strings.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/date_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/date_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/file_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/file_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/get_date.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/get_date.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/gll.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/gll.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/gll.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/gll.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/index_table.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/index_table.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/is_all_white.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/is_all_white.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/is_numeric.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/is_numeric.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/legalize_file_name.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/legalize_file_name.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/lse.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/lse.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/lse.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/lse.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/make_unique_preserve_order.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/make_unique_preserve_order.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/math_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/math_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/nyi.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/nyi.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/parse_range.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/parse_range.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/parse_range.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/parse_range.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/portable_math.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/portable_math.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/print.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/print.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/print_columns.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/print_columns.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/random_element.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/random_element.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/read_file.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/read_file.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/rep.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/rep.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/rep.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/rep.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/replace_all.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/replace_all.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/report_error.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/report_error.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/report_error.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/report_error.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/safelog.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/safelog.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/scan.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/scan.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/seq.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/seq.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/shift_element.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/shift_element.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/shuffle.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/shuffle.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/split.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/split.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/split_delimited.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/split_delimited.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/split_string.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/split_string.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/stream.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/stream.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/string_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/string_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip_path.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip_path.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/strip_white_space.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/strip_white_space.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/substring_delimited.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/substring_delimited.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/timer.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/timer.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/trim_white_space.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/trim_white_space.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/cpputil/unmap.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/cpputil/unmap.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/BinomialDistribution.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/BinomialDistribution.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/BinomialDistribution.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/BinomialDistribution.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/BoundedAdaptiveRejectionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/DoublyBoundedAdaptiveRejectionSampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Markov.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Markov.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Markov.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Markov.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Rmath_dist.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Rmath_dist.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Rmath_dist.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Rmath_dist.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Tn2Sampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Tn2Sampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/Wishart.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/Wishart.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/dirichlet.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/dirichlet.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/extreme_value.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/extreme_value.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/gig.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/gig.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/inverse_gaussian.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/inverse_gaussian.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/inverse_gaussian.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/inverse_gaussian.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/matrix_normal.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/matrix_normal.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/mvn.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/mvn.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/mvt.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/mvt.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/random_cor.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/random_cor.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/random_int.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/random_int.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/rlexp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/rlexp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/rmulti.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/rmulti.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/rng.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/rng.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/rng.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/rng.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/rtriangle.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/rtriangle.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/student_fix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/student_fix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_exp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_exp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_gamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_gamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_gamma.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_gamma.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_logit.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_logit.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_logit.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_logit.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/trun_norm.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/trun_norm.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions/usp.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions/usp.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/distributions.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/distributions.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephes_impl.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephes_impl.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephes_rgamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephes_rgamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/cephus_impl.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/cephus_impl.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/chbevl.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/chbevl.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/dawsn.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/dawsn.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/ei.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/ei.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/expn.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/expn.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/fac.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/fac.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/fresnl.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/fresnl.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/planck.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/planck.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/polevl.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/polevl.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/polylog.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/polylog.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/powi.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/powi.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/shichi.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/shichi.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/sici.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/sici.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/spence.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/spence.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/zeta.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/zeta.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/cephes/zetac.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/cephes/zetac.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/lmultigamma.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/lmultigamma.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/math/special_functions.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/math/special_functions.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Brent.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Brent.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Brent.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Brent.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Integral.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Integral.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Integral.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Integral.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/LinearAssignment.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/LinearAssignment.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/LinearAssignment.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/LinearAssignment.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/MarkovDecisionProcess.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/MarkovDecisionProcess.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/MarkovDecisionProcess.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/MarkovDecisionProcess.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Negate.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Negate.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/NelderMead.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/NelderMead.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/NelderMead.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/NelderMead.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/NumericalDerivatives.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/NumericalDerivatives.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/NumericalDerivatives.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/NumericalDerivatives.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Powell.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Powell.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Powell.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Powell.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Qlearning.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Qlearning.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/Qlearning.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/Qlearning.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarLaplaceApproximation.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarLaplaceApproximation.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarLaplaceApproximation.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarLaplaceApproximation.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarNewtonMax.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarNewtonMax.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/ScalarNewtonMax.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/ScalarNewtonMax.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/bfgs.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/bfgs.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/conj_grad.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/conj_grad.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/initialize_derivatives.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/initialize_derivatives.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/initialize_derivatives.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/initialize_derivatives.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/linear_assignment/lap.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/linear_assignment/lap.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/max_nd.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/max_nd.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/nelder_mead.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/nelder_mead.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/newton.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/newton.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt/simulated_annealing.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt/simulated_annealing.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/numopt.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/numopt.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/LinAlg/LinAlgWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/LinAlg/LinAlgWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/BetaBinomialWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/BetaBinomialWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/BetaModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/BetaModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/DataWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/DataWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/DirichletWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/DirichletWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/GammaModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/GammaModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/GaussianModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/GaussianModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Glm/GlmModel_def.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Glm/GlmModel_def.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Glm/MlogitModel_def.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Glm/MlogitModel_def.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Impute/Imputer_def.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Impute/Imputer_def.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/beta_binomial_mixture_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/beta_binomial_mixture_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/dpmvn_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/dpmvn_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/Mixtures/finite_mixture_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/Mixtures/finite_mixture_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/ModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/ModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/MultinomialWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/MultinomialWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/MvnWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/MvnWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/ParameterWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/ParameterWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/DynamicRegressionModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/DynamicRegressionModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/MultivariateStateSpaceModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/MultivariateStateSpaceModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/MultivariateStateModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/MultivariateStateModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/StateModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateModels/StateModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/StateSpace/StateSpaceModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/StateSpace/StateSpaceModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/TimeSeries/time_series_model_def.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/TimeSeries/time_series_model_def.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/UniformModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/UniformModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/Models/WishartModelWrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/Models/WishartModelWrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/cpputil/cpputil_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/cpputil/cpputil_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/distributions/distribution_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/distributions/distribution_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/module.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/module.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/numopt/numopt_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/numopt/numopt_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/stats/stats_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/stats/stats_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/pybind11/test_utils/test_utils_wrapper.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/pybind11/test_utils/test_utils_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/AsciiDistributionCompare.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/AsciiDistributionCompare.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/AsciiDistributionCompare.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/AsciiDistributionCompare.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Bspline.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Bspline.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Bspline.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Bspline.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ChiSquareTest.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ChiSquareTest.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ChiSquareTest.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ChiSquareTest.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/DataTable.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/DataTable.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/DataTable.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/DataTable.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Design.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Design.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Design.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Design.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ECDF.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ECDF.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ECDF.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ECDF.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/EmpiricalDensity.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/EmpiricalDensity.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/EmpiricalDensity.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/EmpiricalDensity.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Encoders.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Encoders.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Encoders.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Encoders.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/FreqDist.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/FreqDist.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/FreqDist.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/FreqDist.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/IQagent.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/IQagent.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/IQagent.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/IQagent.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Mspline.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Mspline.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Mspline.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Mspline.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/NaturalSpline.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/NaturalSpline.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/NaturalSpline.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/NaturalSpline.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Resampler.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Resampler.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Resampler.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Resampler.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Spline.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Spline.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/Spline.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/Spline.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/compare_binomial_proportions.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/compare_binomial_proportions.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/compare_binomial_proportions.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/compare_binomial_proportions.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/compare_predictions.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/compare_predictions.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/compare_predictions.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/compare_predictions.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/diff.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/diff.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/diff.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/diff.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/hexbin.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/hexbin.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/hexbin.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/hexbin.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ks_critical_value.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ks_critical_value.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/logit.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/logit.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/logit.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/logit.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/moments.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/moments.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/moments.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/moments.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/ols.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/ols.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/regression.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/regression.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/regression.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/regression.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/simple_random_sample.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/simple_random_sample.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/simple_random_sample.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/simple_random_sample.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/summary.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/summary.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/stats/summary.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/stats/summary.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_derivatives.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_derivatives.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_derivatives.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_derivatives.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/test_utils/check_mcmc_matrix.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/test_utils/check_mcmc_matrix.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/test_utils/distributions_match.cpp` & `BayesBoom-0.1.9/BayesBoom/boom/test_utils/distributions_match.cpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/test_utils/test_utils.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/test_utils/test_utils.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/to_data_table.py` & `BayesBoom-0.1.9/BayesBoom/boom/to_data_table.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/boom/uint.hpp` & `BayesBoom-0.1.9/BayesBoom/boom/uint.hpp`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/__init__.py` & `BayesBoom-0.1.9/BayesBoom/bsts/__init__.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/airpass.py` & `BayesBoom-0.1.9/BayesBoom/bsts/airpass.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/ar.py` & `BayesBoom-0.1.9/BayesBoom/bsts/ar.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/bsts.py` & `BayesBoom-0.1.9/BayesBoom/bsts/bsts.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/data.py` & `BayesBoom-0.1.9/BayesBoom/bsts/data.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/dynamic_regression_state_model.py` & `BayesBoom-0.1.9/BayesBoom/bsts/dynamic_regression_state_model.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/gaussian.py` & `BayesBoom-0.1.9/BayesBoom/bsts/gaussian.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/general_seasonal_llt.py` & `BayesBoom-0.1.9/BayesBoom/bsts/general_seasonal_llt.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/holiday.py` & `BayesBoom-0.1.9/BayesBoom/bsts/holiday.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/holiday_models.py` & `BayesBoom-0.1.9/BayesBoom/bsts/holiday_models.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/local_level.py` & `BayesBoom-0.1.9/BayesBoom/bsts/local_level.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/local_linear_trend.py` & `BayesBoom-0.1.9/BayesBoom/bsts/local_linear_trend.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/logit.py` & `BayesBoom-0.1.9/BayesBoom/bsts/logit.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/poisson.py` & `BayesBoom-0.1.9/BayesBoom/bsts/poisson.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/seasonal.py` & `BayesBoom-0.1.9/BayesBoom/bsts/seasonal.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/semilocal_linear_trend.py` & `BayesBoom-0.1.9/BayesBoom/bsts/semilocal_linear_trend.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/state_models.py` & `BayesBoom-0.1.9/BayesBoom/bsts/state_models.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/student.py` & `BayesBoom-0.1.9/BayesBoom/bsts/student.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/student_local_linear_trend.py` & `BayesBoom-0.1.9/BayesBoom/bsts/student_local_linear_trend.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_ar.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_ar.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_bsts.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_bsts.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_dynamic_regression.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_dynamic_regression.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_holidays.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_holidays.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_seasonal_llt.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_seasonal_llt.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_state_models.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_state_models.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_student_llt.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_student_llt.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_trig.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_trig.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/test_utilities.py` & `BayesBoom-0.1.9/BayesBoom/bsts/test_utilities.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/bsts/trig.py` & `BayesBoom-0.1.9/BayesBoom/bsts/trig.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/dynreg/dynreg.py` & `BayesBoom-0.1.9/BayesBoom/dynreg/dynreg.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/dynreg/test_dynreg.py` & `BayesBoom-0.1.9/BayesBoom/dynreg/test_dynreg.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/impute/impute.py` & `BayesBoom-0.1.9/BayesBoom/impute/impute.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/impute/test_imputer.py` & `BayesBoom-0.1.9/BayesBoom/impute/test_imputer.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/mixtures/beta_binomial_mixture.py` & `BayesBoom-0.1.9/BayesBoom/mixtures/beta_binomial_mixture.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/mixtures/dirichlet_process.py` & `BayesBoom-0.1.9/BayesBoom/mixtures/dirichlet_process.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/mixtures/test_dirichlet_process.py` & `BayesBoom-0.1.9/BayesBoom/mixtures/test_dirichlet_process.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/mixtures/utils.py` & `BayesBoom-0.1.9/BayesBoom/mixtures/utils.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/__init__.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/__init__.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/mlogit_spike.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/mlogit_spike.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/mlogit_test.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/mlogit_test.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/priors.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/priors.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/spikeslab.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/spikeslab.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/spikeslab/spikeslab_test.py` & `BayesBoom-0.1.9/BayesBoom/spikeslab/spikeslab_test.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom/test_utils/test_utils.py` & `BayesBoom-0.1.9/BayesBoom/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/BayesBoom.egg-info/PKG-INFO` & `BayesBoom-0.1.9/BayesBoom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BayesBoom
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for Bayesian modeling.
 Home-page: https://github.com/steve-the-bayesian/BOOM
 Author: Steven L. Scott
 Author-email: steve.the.bayesian@gmail.com
 License: UNKNOWN
 Description: Boom stands for 'Bayesian object oriented modeling'.
             It is also the sound your computer makes when it crashes.
```

### Comparing `BayesBoom-0.1.8/BayesBoom.egg-info/SOURCES.txt` & `BayesBoom-0.1.9/BayesBoom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/MANIFEST.in` & `BayesBoom-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `BayesBoom-0.1.8/PKG-INFO` & `BayesBoom-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BayesBoom
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for Bayesian modeling.
 Home-page: https://github.com/steve-the-bayesian/BOOM
 Author: Steven L. Scott
 Author-email: steve.the.bayesian@gmail.com
 License: UNKNOWN
 Description: Boom stands for 'Bayesian object oriented modeling'.
             It is also the sound your computer makes when it crashes.
```

### Comparing `BayesBoom-0.1.8/setup.py` & `BayesBoom-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Bump the major version when making backwards incompatible changes.
 MAJOR = 0
 
 # Bump the minor version when adding backwards compatible features.
 MINOR = 1
 
 # Bump the patch version when making bug fixes.
-PATCH = 8
+PATCH = 9
 
 __version__ = f'{MAJOR}.{MINOR}.{PATCH}'
 
 # Note the nonstandard file configuration in this setup.py.  In the main BOOM
 # repository stored on github, setup.py and the pybind11 bindings are kept in
 # .../Interfaces/python/BayesBoom/... For setup.py to work the C++ code must be
 # in a subdirectory below setup.py.
```

