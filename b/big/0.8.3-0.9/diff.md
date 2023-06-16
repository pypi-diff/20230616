# Comparing `tmp/big-0.8.3.tar.gz` & `tmp/big-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "big-0.8.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "big-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `big-0.8.3.tar` & `big-0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.8.3/.gitignore
--rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.8.3/LICENSE
--rw-r--r--   0        0        0   145903 2023-06-12 05:03:09.037243 big-0.8.3/README.md
--rw-r--r--   0        0        0     1242 2023-05-28 20:40:58.061747 big-0.8.3/big/__init__.py
--rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.8.3/big/all.py
--rw-r--r--   0        0        0     5705 2023-04-12 21:51:57.504191 big-0.8.3/big/boundinnerclass.py
--rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.8.3/big/builtin.py
--rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.8.3/big/file.py
--rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.8.3/big/graph.py
--rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.8.3/big/heap.py
--rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.8.3/big/itertools.py
--rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.8.3/big/scheduler.py
--rw-r--r--   0        0        0   108729 2023-06-12 04:56:42.197905 big-0.8.3/big/text.py
--rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.8.3/big/time.py
--rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.8.3/requirements.txt
--rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.8.3/resources/experiments/alice.in.wonderland.txt
--rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.8.3/resources/experiments/time_multisplit.py
--rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.8.3/resources/images/big.header.png
--rw-r--r--   0        0        0     3470 2023-06-12 04:48:37.949749 big-0.8.3/test/bigtestlib.py
--rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.8.3/test/grepfile
--rw-r--r--   0        0        0     1455 2023-06-12 04:42:29.754589 big-0.8.3/test/test_all.py
--rw-r--r--   0        0        0     5879 2023-06-12 04:41:16.237959 big-0.8.3/test/test_boundinnerclass.py
--rw-r--r--   0        0        0     6518 2023-06-12 04:41:10.137906 big-0.8.3/test/test_builtin.py
--rw-r--r--   0        0        0     8363 2023-06-12 04:41:42.094180 big-0.8.3/test/test_file.py
--rw-r--r--   0        0        0    12333 2023-06-12 04:42:21.830521 big-0.8.3/test/test_graph.py
--rw-r--r--   0        0        0     5007 2023-05-28 20:37:20.059918 big-0.8.3/test/test_heap.py
--rw-r--r--   0        0        0     3403 2023-06-12 04:40:55.577781 big-0.8.3/test/test_itertools.py
--rw-r--r--   0        0        0    11473 2023-05-28 20:36:59.947749 big-0.8.3/test/test_scheduler.py
--rw-r--r--   0        0        0   140256 2023-06-12 04:59:30.039346 big-0.8.3/test/test_text.py
--rw-r--r--   0        0        0     6101 2023-06-12 04:41:31.070086 big-0.8.3/test/test_time.py
--rw-r--r--   0        0        0   146508 1970-01-01 00:00:00.000000 big-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-12-06 08:53:33.203521 big-0.9/.gitignore
+-rw-r--r--   0        0        0     1084 2023-04-12 21:51:57.496190 big-0.9/LICENSE
+-rw-r--r--   0        0        0   147240 2023-06-16 06:38:12.573340 big-0.9/README.md
+-rw-r--r--   0        0        0     1240 2023-06-16 06:35:24.967805 big-0.9/big/__init__.py
+-rw-r--r--   0        0        0     1941 2023-04-12 21:51:57.504191 big-0.9/big/all.py
+-rw-r--r--   0        0        0     7825 2023-06-16 05:58:09.499819 big-0.9/big/boundinnerclass.py
+-rw-r--r--   0        0        0     3274 2023-04-12 21:51:57.504191 big-0.9/big/builtin.py
+-rw-r--r--   0        0        0    11015 2023-04-12 21:51:57.504191 big-0.9/big/file.py
+-rw-r--r--   0        0        0    25350 2023-04-12 21:51:57.504191 big-0.9/big/graph.py
+-rw-r--r--   0        0        0     5347 2023-04-12 21:51:57.504191 big-0.9/big/heap.py
+-rw-r--r--   0        0        0     2499 2023-04-12 21:51:57.504191 big-0.9/big/itertools.py
+-rw-r--r--   0        0        0    12574 2023-04-12 21:51:57.504191 big-0.9/big/scheduler.py
+-rw-r--r--   0        0        0   108729 2023-06-12 04:56:42.197905 big-0.9/big/text.py
+-rw-r--r--   0        0        0     7163 2023-04-12 21:51:57.504191 big-0.9/big/time.py
+-rw-r--r--   0        0        0      613 2023-04-12 21:51:57.504191 big-0.9/pyproject.toml
+-rw-r--r--   0        0        0       16 2022-12-06 08:53:33.203521 big-0.9/requirements.txt
+-rw-r--r--   0        0        0   174313 2022-05-27 04:32:07.000000 big-0.9/resources/experiments/alice.in.wonderland.txt
+-rw-r--r--   0        0        0     6060 2023-04-12 21:51:57.504191 big-0.9/resources/experiments/time_multisplit.py
+-rw-r--r--   0        0        0  1391641 2022-06-02 13:08:28.000000 big-0.9/resources/images/big.header.png
+-rw-r--r--   0        0        0     3576 2023-06-16 06:08:11.681574 big-0.9/tests/bigtestlib.py
+-rw-r--r--   0        0        0       50 2022-05-28 09:56:21.000000 big-0.9/tests/grepfile
+-rw-r--r--   0        0        0     1455 2023-06-12 04:42:29.754589 big-0.9/tests/test_all.py
+-rw-r--r--   0        0        0     8721 2023-06-16 06:17:18.590218 big-0.9/tests/test_boundinnerclass.py
+-rw-r--r--   0        0        0     6518 2023-06-12 04:41:10.137906 big-0.9/tests/test_builtin.py
+-rw-r--r--   0        0        0     8363 2023-06-12 04:41:42.094180 big-0.9/tests/test_file.py
+-rw-r--r--   0        0        0    12333 2023-06-12 04:42:21.830521 big-0.9/tests/test_graph.py
+-rw-r--r--   0        0        0     5007 2023-05-28 20:37:20.059918 big-0.9/tests/test_heap.py
+-rw-r--r--   0        0        0     3403 2023-06-12 04:40:55.577781 big-0.9/tests/test_itertools.py
+-rw-r--r--   0        0        0    11473 2023-05-28 20:36:59.947749 big-0.9/tests/test_scheduler.py
+-rw-r--r--   0        0        0   140256 2023-06-12 04:59:30.039346 big-0.9/tests/test_text.py
+-rw-r--r--   0        0        0     6101 2023-06-12 04:41:31.070086 big-0.9/tests/test_time.py
+-rw-r--r--   0        0        0   147843 1970-01-01 00:00:00.000000 big-0.9/PKG-INFO
```

### Comparing `big-0.8.3/LICENSE` & `big-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `big-0.8.3/README.md` & `big-0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -325,22 +325,32 @@
 > def __init__(self, *args, **kwargs):`
 > ```
 > to
 > ```Python
 > def __init__(self, outer, *args, **kwargs):
 > ```
 > where `outer` is the instance of the outer class.
+>
+> Note that this has an implication for all subclasses.
+> If class ***B*** is decorated with `BoundInnerClass`,
+> and class ***S*** is a subclass of ***B***, such that
+> `issubclass(`***S***`, `***B***`)`,
+> class ***S*** *must* be decorated with either
+> `BoundInnerClass` or `UnboundInnerClass`.
 
 #### `UnboundInnerClass(cls)`
 
 > Class decorator for an inner class that prevents binding
 > the inner class to an instance of the outer class.
 >
-> Subclasses of a class decorated with `BoundInnerClass` must always
-> be decorated with either `BoundInnerClass` or `UnboundInnerClass`.
+> If class ***B*** is decorated with `BoundInnerClass`,
+> and class ***S*** is a subclass of ***B***, such that
+> `issubclass(`***S***`, `***B***`)` returns `True`,
+> class ***S*** *must* be decorated with either
+> `BoundInnerClass` or `UnboundInnerClass`.
 
 
 ## `big.builtin`
 
 Functions for working with builtins.  (Named `builtin` to avoid a
 name collision with the `builtins` module.)
 
@@ -3238,15 +3248,15 @@
     class Inner(object):
         def __init__(self, outer):
             self.outer = outer
 
     @UnboundInnerClass
     class ChildOfInner(Inner.cls):
         def __init__(self):
-            super(Outer.ChildOfInner, self).__init__()
+            super().__init__()
 
 o = Outer()
 i = o.ChildOfInner()
 ```
 
 We followed the rules:
 
@@ -3284,15 +3294,15 @@
     class Inner(object):
         def __init__(self, outer):
             self.outer = outer
 
     @BoundInnerClass
     class ChildOfInner(Inner.cls):
         def __init__(self, outer):
-            super(Outer.ChildOfInner, self).__init__()
+            super().__init__()
             assert self.outer == outer
 
 o = Outer()
 i = o.ChildOfInner()
 ```
 
 Again, `ChildOfInner.__init__` doesn't need to explicitly
@@ -3360,41 +3370,57 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
-**0.8.3**
+**0.9** *2023/06/15*
+
+* Bugfix!  If an outer class `Outer` had an inner class `Inner`
+  decorated with `@BoundInnerClass`, and `o` is an instance of
+  `Outer`, and `o` evaluated to false in a boolean context,
+  `o.Inner` would be the *unbound* version of `Inner`.  Now
+  it's the bound version, as is proper.
+* Modified `tests/test_boundinnerclasses.py`:
+
+    - Added regression test for the above bugfix (of course!).
+    - It now takes advantage of that newfangled "zero-argument `super`".
+    - Added testing of an unbound subclass of an unbound subclass.
+
+**0.8.3** *2023/06/11*
+
 
 * Added
   [`int_to_words`](#int_to_words-flowerytrue).
 * All tests now insert the local **big** directory
   onto `sys.path`, so you can run the tests on your
   local copy without having to install.  Especially
   convenient for testing with old versions of Python!
 
-**0.8.2**
+> *Note:* tomorrow, **big** will be one year old!
+
+**0.8.2** *2023/05/19*
 
 * Convert all iterator functions to use my new approach:
   instead of checking arguments inside the iterator,
   the function you call checks arguments, then has a
   nested iterator function which it runs and returns the
   result.  This means bad inputs raise their exceptions
   at the call site where the iterator is constructed,
   rather than when the first value is yielded by the iterator!
 
-**0.8.1**
+**0.8.1** *2023/05/19*
 
 * Added
   [`parse_delimiters`](#parse_delimiterss-delimitersNone)
   and
   [`Delimiter`.](#delimiteropen-close--backslashfalse-nestedtrue)
 
-**0.8**
+**0.8** *2023/05/18*
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
     for how it works.
   * Functions in `big.text` are now more consistent about raising
@@ -3456,15 +3482,15 @@
   and
   [`re_rpartition`](#re_rpartitiontext-pattern-count1--flags0)
   slightly, should now be very-slightly faster.  (Well, `re_rpartition`
   will be slower if your pattern finds overlapping matches.  But at
   least now it's correct!)
 * Lots and lots of doc improvements, as usual.
 
-**0.7.1**
+**0.7.1** *2023/03/13*
 
 * Tweaked the implementation of
   [`multisplit`.](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   Internally, it does the
   string splitting using `re.split`, which returns a `list`.  It used
   to iterate over the list and yield each element.  But that meant keeping
   the entire list around in memory until `multisplit` exited.  Now,
@@ -3472,15 +3498,15 @@
   reverses the list, pops off the final element, and yields
   that.  This means
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   drops all references to the split strings
   as it iterates over the string, which may help in low-memory situations.
 * Minor doc fixes.
 
-**0.7**
+**0.7** *2023/03/11*
 
 * Breaking changes to the
   [`Scheduler`](#schedulerregulatordefault_regulator):
   * It's no longer thread-safe by default, which means it's much faster
     for non-threaded workloads.
   * The lock has been moved out of the
     [`Scheduler`](#schedulerregulatordefault_regulator)
@@ -3504,47 +3530,47 @@
     shouldn't be manually constructing
     [`Event`](#eventscheduler-event-time-priority-sequence)
     objects anyway.)
   * The `Scheduler` now guarantees that it will only call `now` and `wake`
     on a `Regulator` object while holding that `Regulator`'s lock.
 * Minor doc fixes.
 
-**0.6.18**
+**0.6.18** *2023/03/09*
 
 * Retooled
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   and
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
   argument verification code.  Both functions now consistently check all
   their inputs, and use consistent error messages when raising an exception.
 
-**0.6.17**
+**0.6.17** *2023/03/09*
 
 * Fixed a minor crashing bug in
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse):
   if you passed in a *list* of separators (or `separators`
   was of any non-hashable type), and `reverse` was true,
   `multisplit` would crash.  It used `separators` as a key
   into a dict, which meant `separators` had to be hashable.
 * [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   now verifies that the `s` passed in is either `str` or `bytes`.
 * Updated all copyright date notices to 2023.
 * Lots of doc fixes.
 
-**0.6.16**
+**0.6.16** *2023/02/26*
 
 * Fixed Python 3.6 support! Some equals-signs-in-f-strings and some
   other anachronisms had crept in.  0.6.16 has been tested on all
   versions from 3.6 to 3.11 (as well as having 100% *coverage*).
 * Made the `dateutils` package an optional dependency.  Only one function
   needs it, [`parse_timestamp_3339Z()`](#parse_timestamp_3339zs--timezonenone).
 * Minor cleanup in [`PushbackIterator()`](#pushbackiteratoriterablenone).
   It also uses slots now, which should make it a bit faster.
 
-**0.6.15**
+**0.6.15** *2023/01/07*
 
 * Added the new functions
   [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone) and
   [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone).
   These allow you to ensure or explicitly set a timezone on a `datetime.datetime`
   object.
 * Added the `timezone` argument to 
@@ -3552,59 +3578,60 @@
 * [`gently_title()`](#gently_titles-apostrophesnone-double_quotesnone)
   now capitalizes the first letter after a left parenthesis.
 * Changed the secret `multirpartition` function slightly.  Its `reverse`
   parameter now means to un-reverse its reversing behavior.  Stated
   another way, `multipartition(reverse=X)` and `multirpartition(reverse=not X)`
   now do the same thing.
 
-**0.6.14**
+**0.6.14** *2022/12/11*
 
 * Improved the text of the `RuntimeError` raised by `TopologicalSorter.View`
   when the view is incoherent.  Now it tells you exactly what nodes are
   conflicting.
 * Expanded the deep dive on `multisplit`.
 
-**0.6.13**
+**0.6.13** *2022/12/11*
 
 * Changed [`translate_filename_to_exfat(s)`](#translate_filename_to_exfats)
   behavior: when modifying a string with a colon (`':'`) *not* followed by
   a space, it used to convert it to a dash (`'-'`).  Now it converts the
   colon to a period (`'.'`), which looks a little more natural.  A colon
   followed by a space is still converted to a dash followed by a space.
 
-*p.s.* I forgot to release packages for 0.6.11 and 0.6.12.  But they're
-tagged, in case you want to examine them for some reason.
-
-**0.6.12**
+**0.6.12** *2022/12/04*
 
 * Bugfix: When calling
   [`TopologicalSorter.print()`](#topologicalsorterprintprintprint),
   it sorts the list of nodes, for consistency's sakes.
   But if the node objects don't support `<` or `>` comparison,
   that throws an exception.  `TopologicalSorter.print()` now catches
   that exception and simply 
 * Added a secret (otherwise undocumented!) function: `multirpartition`,
   which is like
   [`multipartition`](#multipartitions-separators-count1--reverseFalse-separateTrue)
   but with `reverse=True`.
 * Added the list of conflicted nodes to the "node is incoherent"
   exception text.
 
-**0.6.11**
+> *Note:* although version **0.6.12** was tagged, it was never packaged for release.
+
+**0.6.11**  *2022/11/13*
 
 * Changed the import strategy.  The top-level **big** module used
   to import all its child modules, and `import *` all the symbols
   from all those modules.  But a friend (hi Mark Shannon!) talked
   me out of this.  It's convenient, but if a user doesn't care about
   a particular module, why make them import it.  So now the top-level
   **big** module contains nothing but a version number, and you
   can either import just the submodules you need, or you can import
   **big.all** to get all the symbols (like **big** itself used to do).
 
-**0.6.10**
+> *Note:* although version **0.6.11** was tagged, it was never packaged for release.
+
+**0.6.10** *2022/10/26*
 
 * All code changes had to do with
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse):
     * Fixed a subtle bug.  When splitting with a separator that can overlap
       itself, like `' x '`, `multisplit` will prefer the *leftmost* instance.
       But when `reverse=True`, it must prefer the *rightmost* instance.
       Thanks to Eric V. Smith for suggesting the clever "reverse everything,
@@ -3627,35 +3654,35 @@
     * Removed `NOT_SEPARATE` (and the not-yet-implemented `STR_STRIP`)
       modes for `strip`.  They're easy to implement yourself, and this
       removes some surface area from the already-too-big
       `multisplit` API.
 * Modernized `pyproject.toml` metadata to make `flit` happier.  This was
   necessary to ensure that `pip install big` also installs its dependencies.
 
-**0.6.8**
+**0.6.8** *2022/10/16*
 
 * Renamed two of the three freshly-added lines modifier functions:
   `lines_filter_contains` is now 
   [`lines_containing`](#lines_containingli-s--invertfalse),
   and `lines_filter_grep` is now
   [`lines_grep`](#lines_grepli-pattern--invertfalse-flags0).
 
-**0.6.7**
+**0.6.7** *2022/10/16*
 
 * Added three new lines modifier functions
   to the [`text`](#bigtext) module:
   `lines_filter_contains`,
   `lines_filter_grep`,
   and
   [`lines_sort`](#lines_sortli--reversefalse).
 * [`gently_title`](#gently_titles-apostrophesnone-double_quotesnone)
   now accepts `str` or `bytes`.  Also added the `apostrophes` and
   `double_quotes` arguments.
 
-**0.6.6**
+**0.6.6** *2022/10/14*
 
 * Fixed a bug in
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse).
   I thought when using `keep=AS_PAIRS` that it shouldn't ever emit a 2-tuple
   containing just empty strings--but on further reflection I've realized that
   that's correct.  This behavior is now tested and documented, along with
   the reasoning behind it.
@@ -3665,36 +3692,36 @@
   end-of-line sequence in them!  Oops!
     * Added a unit test to check that.  The unit test also ensures that
       `whitespace`, `newlines`, and all the variants (`utf8_`, `ascii_`,
       and `_with_dos`) exactly match the set of characters Python considers
       whitespace and newline characters.
 * Lots more documentation and formatting fixes.
 
-**0.6.5**
+**0.6.5** *2022/10/13*
 
 * Added the new [`itertools`](#bigitertools) module, which so far only contains
   [`PushbackIterator`](#pushbackiteratoriterablenone).
 * Added
   [`lines_strip_comments`](#lines_strip_commentsli-comment_separators--quotes--backslash-rstriptrue-triple_quotestrue)
   and
   [`split_quoted_strings`](#split_quoted_stringss-quotes---triple_quotestrue-backslash)
   to the
   [`text`](#bigtext)
   module.
 
-**0.6.1**
+**0.6.1** *2022/10/13*
 
 * I realized that [`whitespace`](#whitespace) should contain the DOS end-of-line
   sequence (`'\r\n'`), as it should be considered a single separator
   when splitting etc.  I added that, along with [`whitespace_no_dos`](#whitespace),
   and naturally [`utf8_whitespace_no_dos`](#whitespace) and
   [`ascii_whitespace_no_dos`](#whitespace) too.
 * Minor doc fixes.
 
-**0.6**
+**0.6** *2022/10/13*
 
 A **big** upgrade!
 
 * Completely retooled and upgraded
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse),
   and added
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
@@ -3748,20 +3775,20 @@
   Added the `separators` and `replacement` parameters,
   and added support for `bytes` objects.
 * Added the `count` parameter to
   [`re_partition`](#re_partitiontext-pattern-count1--flags0)
   and
   [`re_rpartition`](#re_rpartitiontext-pattern-count1--flags0).
 
-**0.5.2**
+**0.5.2** *2022/09/12*
 
 * Added `stripped_lines` and `rstripped_lines` to the [`text`](#bigtext) module.
 * Added support for `len` to the [`TopologicalSorter`](#topologicalsortergraphnone) object.
 
-**0.5.1**
+**0.5.1** *2022/09/04*
 
 * Added
   [`gently_title`](#gently_titles-apostrophesnone-double_quotesnone)
   and
   [`normalize_whitespace`](#normalize_whitespaces-separatorsNone-replacementNone)
   to the [`text`](#bigtext) module.
 * Changed [`translate_filename_to_exfat`](#translate_filename_to_exfats)
@@ -3769,10 +3796,10 @@
   If the colon is followed by a space, then the colon is turned into `' -'`.
   This yields a more natural translation when colons are used in text, e.g.
   `'xXx: The Return Of Xander Cage'` is translated to `'xXx - The Return Of Xander Cage'`.
   If the colon is not followed by a space, turns the colon into `'-'`.
   This is good for tiresome modern gobbledygook like `'Re:code'`, which
   will now be translated to `'Re-code'`.
 
-**0.5**
+**0.5** *2022/06/12*
 
 * Initial release.
```

### Comparing `big-0.8.3/big/__init__.py` & `big-0.9/big/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-__version__ = "0.8.3"
+__version__ = "0.9"
```

### Comparing `big-0.8.3/big/all.py` & `big-0.9/big/all.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/boundinnerclass.py` & `big-0.9/big/boundinnerclass.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,95 +20,160 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
 THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
+#
+# If you have a class with an inner class inside,
+# decorate the inner class with BoundInnerClass below
+# and now it'll automatically get a second parameter
+# of the parent instance!
+# _______________________________________
+#
+# class Outer:
+#   @BoundInnerClass
+#   class Inner:
+#       def __init__(self, outer):
+#           global o
+#           print(outer = o)
+# o = Outer()
+# i = o.Inner()
+# _______________________________________
+#
+# This program prints True.  The "outer" parameter
+# to Inner.__init__ was filled in automatically by
+# the BoundInnerClass decorator.
+#
+# Thanks, BoundInnerClass, you've saved the day!
+#
+# -----
+#
+# Infinite extra-special thanks to Alex Martelli for
+# showing me how this could be done in the first place--
+# all the way back in 2010!
+#
+# https://stackoverflow.com/questions/2278426/inner-classes-how-can-i-get-the-outer-class-object-at-construction-time
+#
+# Thanks, Alex, you've saved the day!
+
+
 __all__ = ["BoundInnerClass", "UnboundInnerClass"]
 
 import weakref
 
 class _Worker(object):
     def __init__(self, cls):
         self.cls = cls
 
     def __get__(self, outer, outer_class):
-        if not outer:
+
+        #
+        # If outer is not None, we've been accessed through
+        # an *instance* of the class, like so:
+        #    o = Outer()
+        #    ref = o.Inner
+        #
+        # See:
+        #    https://docs.python.org/3/howto/descriptor.html#invocation-from-an-instance
+        #
+        #
+        # If outer is None, we've been accessed through the *class itself*,
+        # like so:
+        #    ref = Outer.Inner
+        #
+        # See:
+        #    https://docs.python.org/3/howto/descriptor.html#invocation-from-a-class
+        #
+        # If someone accesses us through the class, not through an instance,
+        # return the unbound version of the class.
+        #
+        if outer is None:
             return self.cls
 
         name = self.cls.__name__
 
         wrapper_bases = [self.cls]
 
-        # iterate over cls's bases and look in outer to see
-        # if any have bound inner classes in outer.
-        # if so, multiply inherit from the bound inner version(s).
-        multiply_inherit = False
+        # Iterate over cls's bases, and look in outer,
+        #   to see if any have bound inner classes in outer.
+        # If so, multiply inherit from the bound inner version(s).
 
+        multiply_inherit = False
         for base in self.cls.__bases__:
-            # if we can't find a bound inner base,
+            # If we can't find a bound inner base,
             # add the original unbound base instead.
             # this is harmless but helps preserve the original MRO.
             inherit_from = base
 
-            # if we inherit from a boundinnerclass from another outer class,
-            # we might have the same name as a legitimate base class.
-            # but if we look it up, we'll call __get__ recursively... forever.
-            # if the name is the same as our own name, there's no way it's a
-            # bound inner class we need to inherit from, so just skip it.
+            # If we inherit from a BoundInnerClass from another outer class,
+            # we *might* have the same name as a legitimate base class.
+            # But if we get that attribute, we'll call __get__ recursively...
+            # forever.
+            #
+            # If the name is the same as our own name, there's no way it's
+            # a bound inner class we need to inherit from, so just skip it.
             if base.__name__ != name:
                 bound_inner_base = getattr(outer, base.__name__, None)
                 if bound_inner_base:
                     bases = getattr(bound_inner_base, "__bases__", (None,))
-                    # the unbound class is always the first base of
+                    # The unbound class is always the first base of
                     # the bound inner class.
                     if bases[0] == base:
                         inherit_from = bound_inner_base
                         multiply_inherit = True
             wrapper_bases.append(inherit_from)
 
         Wrapper = self._wrap(outer, wrapper_bases[0])
         Wrapper.__name__ = name
 
         # Assigning to __bases__ is startling, but it's the only way to get
         # this code working simultaneously in both Python 2 and Python 3.
         if multiply_inherit:
             Wrapper.__bases__ = tuple(wrapper_bases)
 
-        # cache the bound instance in outer's dict
-        # (which means in the future it won't call the property)
+        # Cache the bound instance in outer's dict.
+        # This also means that future requests for us won't call our
+        # __get__ again, it'll automatically use the cached copy.
         outer.__dict__[name] = Wrapper
         return Wrapper
 
+
 class BoundInnerClass(_Worker):
     """
     Class decorator for an inner class.  When accessing the inner class
     through an instance of the outer class, "binds" the inner class to
     the instance.  This changes the signature of the inner class's __init__
     from
 
         def __init__(self, *args, **kwargs):
 
     to
 
         def __init__(self, outer, *args, **kwargs):
 
     where "outer" is the instance of the outer class.
+
+    Note that this has an implication for all subclasses.
+    If class B is decorated with BoundInnerClass, and class
+    S is a subclass of B, such that issubclass(S, B) returns True,
+    class S must be decorated with either BoundInnerClass
+    or UnboundInnerClass.
     """
     def _wrap(self, outer, base):
         wrapper_self = self
-        assert outer
+        assert outer is not None
         outer_weakref = weakref.ref(outer)
         class Wrapper(base):
-            def __init__(self, *args, **kwargs):
+            def __init__(self, *bic_args, **bic_kwargs):
                 wrapper_self.cls.__init__(self,
-                                          outer_weakref(), *args, **kwargs)
+                                          outer_weakref(), *bic_args, **bic_kwargs)
 
-            # give the bound inner class a nice repr
+            # give the bound inner class a nicer repr
             # (but only if it doesn't already have a custom repr)
             if wrapper_self.cls.__repr__ is object.__repr__:
                 def __repr__(self):
                     return "".join([
                         "<",
                         wrapper_self.cls.__module__,
                         ".",
@@ -122,21 +187,24 @@
         Wrapper.__module__ = self.cls.__module__
         Wrapper.__qualname__ = self.cls.__qualname__
         Wrapper.__doc__ = self.cls.__doc__
         if hasattr(self.cls, '__annotations__'):
             Wrapper.__annotations__ = self.cls.__annotations__
         return Wrapper
 
+
 class UnboundInnerClass(_Worker):
     """
     Class decorator for an inner class that prevents binding
     the inner class to an instance of the outer class.
 
-    Subclasses of a class decorated with BoundInnerClass must always
-    be decorated with either BoundInnerClass or UnboundInnerClass.
+    If class B is decorated with BoundInnerClass, and class
+    S is a subclass of B, such that issubclass(S, B) returns True,
+    class S must be decorated with either BoundInnerClass
+    or UnboundInnerClass.
     """
     def _wrap(self, outer, base):
         class Wrapper(base):
             pass
         Wrapper.__name__ = self.cls.__name__
         Wrapper.__module__ = self.cls.__module__
         Wrapper.__qualname__ = self.cls.__qualname__
```

### Comparing `big-0.8.3/big/builtin.py` & `big-0.9/big/builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/file.py` & `big-0.9/big/file.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/graph.py` & `big-0.9/big/graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/heap.py` & `big-0.9/big/heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/itertools.py` & `big-0.9/big/itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/scheduler.py` & `big-0.9/big/scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/text.py` & `big-0.9/big/text.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/big/time.py` & `big-0.9/big/time.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/pyproject.toml` & `big-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `big-0.8.3/resources/experiments/alice.in.wonderland.txt` & `big-0.9/resources/experiments/alice.in.wonderland.txt`

 * *Files identical despite different names*

### Comparing `big-0.8.3/resources/experiments/time_multisplit.py` & `big-0.9/resources/experiments/time_multisplit.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/resources/images/big.header.png` & `big-0.9/resources/images/big.header.png`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/bigtestlib.py` & `big-0.9/tests/bigtestlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,16 +87,17 @@
     for line in sio.getvalue().split("\n"):
         if not line.startswith("Ran"):
             print(line)
             continue
 
         if permutations:
             fields = line.split()
-            assert fields[2] == "tests"
-            fields[2] = f"tests, with {permutations()} total permutations,"
+            tests = fields[2]
+            assert tests in ("test", "tests"), f"expected fields[2] to be 'test' or 'tests', but fields={fields}"
+            fields[2] = f"{tests}, with {permutations()} total permutations,"
             line = " ".join(fields)
         print(line)
         print()
         # prevent printing the  \n and OK
         break
 
 def finish():
```

### Comparing `big-0.8.3/test/test_all.py` & `big-0.9/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_builtin.py` & `big-0.9/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_file.py` & `big-0.9/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_graph.py` & `big-0.9/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_heap.py` & `big-0.9/tests/test_heap.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_itertools.py` & `big-0.9/tests/test_itertools.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_scheduler.py` & `big-0.9/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_text.py` & `big-0.9/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/test/test_time.py` & `big-0.9/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `big-0.8.3/PKG-INFO` & `big-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: big
-Version: 0.8.3
+Version: 0.9
 Summary: The big package is a grab-bag of cool code for use in your programs.
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -341,22 +341,32 @@
 > def __init__(self, *args, **kwargs):`
 > ```
 > to
 > ```Python
 > def __init__(self, outer, *args, **kwargs):
 > ```
 > where `outer` is the instance of the outer class.
+>
+> Note that this has an implication for all subclasses.
+> If class ***B*** is decorated with `BoundInnerClass`,
+> and class ***S*** is a subclass of ***B***, such that
+> `issubclass(`***S***`, `***B***`)`,
+> class ***S*** *must* be decorated with either
+> `BoundInnerClass` or `UnboundInnerClass`.
 
 #### `UnboundInnerClass(cls)`
 
 > Class decorator for an inner class that prevents binding
 > the inner class to an instance of the outer class.
 >
-> Subclasses of a class decorated with `BoundInnerClass` must always
-> be decorated with either `BoundInnerClass` or `UnboundInnerClass`.
+> If class ***B*** is decorated with `BoundInnerClass`,
+> and class ***S*** is a subclass of ***B***, such that
+> `issubclass(`***S***`, `***B***`)` returns `True`,
+> class ***S*** *must* be decorated with either
+> `BoundInnerClass` or `UnboundInnerClass`.
 
 
 ## `big.builtin`
 
 Functions for working with builtins.  (Named `builtin` to avoid a
 name collision with the `builtins` module.)
 
@@ -3254,15 +3264,15 @@
     class Inner(object):
         def __init__(self, outer):
             self.outer = outer
 
     @UnboundInnerClass
     class ChildOfInner(Inner.cls):
         def __init__(self):
-            super(Outer.ChildOfInner, self).__init__()
+            super().__init__()
 
 o = Outer()
 i = o.ChildOfInner()
 ```
 
 We followed the rules:
 
@@ -3300,15 +3310,15 @@
     class Inner(object):
         def __init__(self, outer):
             self.outer = outer
 
     @BoundInnerClass
     class ChildOfInner(Inner.cls):
         def __init__(self, outer):
-            super(Outer.ChildOfInner, self).__init__()
+            super().__init__()
             assert self.outer == outer
 
 o = Outer()
 i = o.ChildOfInner()
 ```
 
 Again, `ChildOfInner.__init__` doesn't need to explicitly
@@ -3376,41 +3386,57 @@
   class from the `__init__` of the outer class, which should allow
   the code to cache the bound inner class instance before a second
   thread could ever get a reference to the outer object.
 
 
 ## Release history
 
-**0.8.3**
+**0.9** *2023/06/15*
+
+* Bugfix!  If an outer class `Outer` had an inner class `Inner`
+  decorated with `@BoundInnerClass`, and `o` is an instance of
+  `Outer`, and `o` evaluated to false in a boolean context,
+  `o.Inner` would be the *unbound* version of `Inner`.  Now
+  it's the bound version, as is proper.
+* Modified `tests/test_boundinnerclasses.py`:
+
+    - Added regression test for the above bugfix (of course!).
+    - It now takes advantage of that newfangled "zero-argument `super`".
+    - Added testing of an unbound subclass of an unbound subclass.
+
+**0.8.3** *2023/06/11*
+
 
 * Added
   [`int_to_words`](#int_to_words-flowerytrue).
 * All tests now insert the local **big** directory
   onto `sys.path`, so you can run the tests on your
   local copy without having to install.  Especially
   convenient for testing with old versions of Python!
 
-**0.8.2**
+> *Note:* tomorrow, **big** will be one year old!
+
+**0.8.2** *2023/05/19*
 
 * Convert all iterator functions to use my new approach:
   instead of checking arguments inside the iterator,
   the function you call checks arguments, then has a
   nested iterator function which it runs and returns the
   result.  This means bad inputs raise their exceptions
   at the call site where the iterator is constructed,
   rather than when the first value is yielded by the iterator!
 
-**0.8.1**
+**0.8.1** *2023/05/19*
 
 * Added
   [`parse_delimiters`](#parse_delimiterss-delimitersNone)
   and
   [`Delimiter`.](#delimiteropen-close--backslashfalse-nestedtrue)
 
-**0.8**
+**0.8** *2023/05/18*
 
 * Major retooling of `str` and `bytes` support in `big.text`.
   * Functions in `big.text` now uniformly accept `str` or `bytes`
     or a subclass of either.  See the
     [Support for bytes and str](#Support-for-bytes-and-str) section
     for how it works.
   * Functions in `big.text` are now more consistent about raising
@@ -3472,15 +3498,15 @@
   and
   [`re_rpartition`](#re_rpartitiontext-pattern-count1--flags0)
   slightly, should now be very-slightly faster.  (Well, `re_rpartition`
   will be slower if your pattern finds overlapping matches.  But at
   least now it's correct!)
 * Lots and lots of doc improvements, as usual.
 
-**0.7.1**
+**0.7.1** *2023/03/13*
 
 * Tweaked the implementation of
   [`multisplit`.](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   Internally, it does the
   string splitting using `re.split`, which returns a `list`.  It used
   to iterate over the list and yield each element.  But that meant keeping
   the entire list around in memory until `multisplit` exited.  Now,
@@ -3488,15 +3514,15 @@
   reverses the list, pops off the final element, and yields
   that.  This means
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   drops all references to the split strings
   as it iterates over the string, which may help in low-memory situations.
 * Minor doc fixes.
 
-**0.7**
+**0.7** *2023/03/11*
 
 * Breaking changes to the
   [`Scheduler`](#schedulerregulatordefault_regulator):
   * It's no longer thread-safe by default, which means it's much faster
     for non-threaded workloads.
   * The lock has been moved out of the
     [`Scheduler`](#schedulerregulatordefault_regulator)
@@ -3520,47 +3546,47 @@
     shouldn't be manually constructing
     [`Event`](#eventscheduler-event-time-priority-sequence)
     objects anyway.)
   * The `Scheduler` now guarantees that it will only call `now` and `wake`
     on a `Regulator` object while holding that `Regulator`'s lock.
 * Minor doc fixes.
 
-**0.6.18**
+**0.6.18** *2023/03/09*
 
 * Retooled
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   and
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
   argument verification code.  Both functions now consistently check all
   their inputs, and use consistent error messages when raising an exception.
 
-**0.6.17**
+**0.6.17** *2023/03/09*
 
 * Fixed a minor crashing bug in
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse):
   if you passed in a *list* of separators (or `separators`
   was of any non-hashable type), and `reverse` was true,
   `multisplit` would crash.  It used `separators` as a key
   into a dict, which meant `separators` had to be hashable.
 * [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse)
   now verifies that the `s` passed in is either `str` or `bytes`.
 * Updated all copyright date notices to 2023.
 * Lots of doc fixes.
 
-**0.6.16**
+**0.6.16** *2023/02/26*
 
 * Fixed Python 3.6 support! Some equals-signs-in-f-strings and some
   other anachronisms had crept in.  0.6.16 has been tested on all
   versions from 3.6 to 3.11 (as well as having 100% *coverage*).
 * Made the `dateutils` package an optional dependency.  Only one function
   needs it, [`parse_timestamp_3339Z()`](#parse_timestamp_3339zs--timezonenone).
 * Minor cleanup in [`PushbackIterator()`](#pushbackiteratoriterablenone).
   It also uses slots now, which should make it a bit faster.
 
-**0.6.15**
+**0.6.15** *2023/01/07*
 
 * Added the new functions
   [`datetime_ensure_timezone(d, timezone)`](#datetime_ensure_timezoned-timezone) and
   [`datetime_set_timezone(d, timezone)`](#datetime_set_timezoned-timezone).
   These allow you to ensure or explicitly set a timezone on a `datetime.datetime`
   object.
 * Added the `timezone` argument to 
@@ -3568,59 +3594,60 @@
 * [`gently_title()`](#gently_titles-apostrophesnone-double_quotesnone)
   now capitalizes the first letter after a left parenthesis.
 * Changed the secret `multirpartition` function slightly.  Its `reverse`
   parameter now means to un-reverse its reversing behavior.  Stated
   another way, `multipartition(reverse=X)` and `multirpartition(reverse=not X)`
   now do the same thing.
 
-**0.6.14**
+**0.6.14** *2022/12/11*
 
 * Improved the text of the `RuntimeError` raised by `TopologicalSorter.View`
   when the view is incoherent.  Now it tells you exactly what nodes are
   conflicting.
 * Expanded the deep dive on `multisplit`.
 
-**0.6.13**
+**0.6.13** *2022/12/11*
 
 * Changed [`translate_filename_to_exfat(s)`](#translate_filename_to_exfats)
   behavior: when modifying a string with a colon (`':'`) *not* followed by
   a space, it used to convert it to a dash (`'-'`).  Now it converts the
   colon to a period (`'.'`), which looks a little more natural.  A colon
   followed by a space is still converted to a dash followed by a space.
 
-*p.s.* I forgot to release packages for 0.6.11 and 0.6.12.  But they're
-tagged, in case you want to examine them for some reason.
-
-**0.6.12**
+**0.6.12** *2022/12/04*
 
 * Bugfix: When calling
   [`TopologicalSorter.print()`](#topologicalsorterprintprintprint),
   it sorts the list of nodes, for consistency's sakes.
   But if the node objects don't support `<` or `>` comparison,
   that throws an exception.  `TopologicalSorter.print()` now catches
   that exception and simply 
 * Added a secret (otherwise undocumented!) function: `multirpartition`,
   which is like
   [`multipartition`](#multipartitions-separators-count1--reverseFalse-separateTrue)
   but with `reverse=True`.
 * Added the list of conflicted nodes to the "node is incoherent"
   exception text.
 
-**0.6.11**
+> *Note:* although version **0.6.12** was tagged, it was never packaged for release.
+
+**0.6.11**  *2022/11/13*
 
 * Changed the import strategy.  The top-level **big** module used
   to import all its child modules, and `import *` all the symbols
   from all those modules.  But a friend (hi Mark Shannon!) talked
   me out of this.  It's convenient, but if a user doesn't care about
   a particular module, why make them import it.  So now the top-level
   **big** module contains nothing but a version number, and you
   can either import just the submodules you need, or you can import
   **big.all** to get all the symbols (like **big** itself used to do).
 
-**0.6.10**
+> *Note:* although version **0.6.11** was tagged, it was never packaged for release.
+
+**0.6.10** *2022/10/26*
 
 * All code changes had to do with
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse):
     * Fixed a subtle bug.  When splitting with a separator that can overlap
       itself, like `' x '`, `multisplit` will prefer the *leftmost* instance.
       But when `reverse=True`, it must prefer the *rightmost* instance.
       Thanks to Eric V. Smith for suggesting the clever "reverse everything,
@@ -3643,35 +3670,35 @@
     * Removed `NOT_SEPARATE` (and the not-yet-implemented `STR_STRIP`)
       modes for `strip`.  They're easy to implement yourself, and this
       removes some surface area from the already-too-big
       `multisplit` API.
 * Modernized `pyproject.toml` metadata to make `flit` happier.  This was
   necessary to ensure that `pip install big` also installs its dependencies.
 
-**0.6.8**
+**0.6.8** *2022/10/16*
 
 * Renamed two of the three freshly-added lines modifier functions:
   `lines_filter_contains` is now 
   [`lines_containing`](#lines_containingli-s--invertfalse),
   and `lines_filter_grep` is now
   [`lines_grep`](#lines_grepli-pattern--invertfalse-flags0).
 
-**0.6.7**
+**0.6.7** *2022/10/16*
 
 * Added three new lines modifier functions
   to the [`text`](#bigtext) module:
   `lines_filter_contains`,
   `lines_filter_grep`,
   and
   [`lines_sort`](#lines_sortli--reversefalse).
 * [`gently_title`](#gently_titles-apostrophesnone-double_quotesnone)
   now accepts `str` or `bytes`.  Also added the `apostrophes` and
   `double_quotes` arguments.
 
-**0.6.6**
+**0.6.6** *2022/10/14*
 
 * Fixed a bug in
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse).
   I thought when using `keep=AS_PAIRS` that it shouldn't ever emit a 2-tuple
   containing just empty strings--but on further reflection I've realized that
   that's correct.  This behavior is now tested and documented, along with
   the reasoning behind it.
@@ -3681,36 +3708,36 @@
   end-of-line sequence in them!  Oops!
     * Added a unit test to check that.  The unit test also ensures that
       `whitespace`, `newlines`, and all the variants (`utf8_`, `ascii_`,
       and `_with_dos`) exactly match the set of characters Python considers
       whitespace and newline characters.
 * Lots more documentation and formatting fixes.
 
-**0.6.5**
+**0.6.5** *2022/10/13*
 
 * Added the new [`itertools`](#bigitertools) module, which so far only contains
   [`PushbackIterator`](#pushbackiteratoriterablenone).
 * Added
   [`lines_strip_comments`](#lines_strip_commentsli-comment_separators--quotes--backslash-rstriptrue-triple_quotestrue)
   and
   [`split_quoted_strings`](#split_quoted_stringss-quotes---triple_quotestrue-backslash)
   to the
   [`text`](#bigtext)
   module.
 
-**0.6.1**
+**0.6.1** *2022/10/13*
 
 * I realized that [`whitespace`](#whitespace) should contain the DOS end-of-line
   sequence (`'\r\n'`), as it should be considered a single separator
   when splitting etc.  I added that, along with [`whitespace_no_dos`](#whitespace),
   and naturally [`utf8_whitespace_no_dos`](#whitespace) and
   [`ascii_whitespace_no_dos`](#whitespace) too.
 * Minor doc fixes.
 
-**0.6**
+**0.6** *2022/10/13*
 
 A **big** upgrade!
 
 * Completely retooled and upgraded
   [`multisplit`](#multisplits-separators--keepFalse-maxsplit-1-reverseFalse-separateFalse-stripFalse),
   and added
   [`multistrip`](#multistrips-separators-leftTrue-rightTrue)
@@ -3764,20 +3791,20 @@
   Added the `separators` and `replacement` parameters,
   and added support for `bytes` objects.
 * Added the `count` parameter to
   [`re_partition`](#re_partitiontext-pattern-count1--flags0)
   and
   [`re_rpartition`](#re_rpartitiontext-pattern-count1--flags0).
 
-**0.5.2**
+**0.5.2** *2022/09/12*
 
 * Added `stripped_lines` and `rstripped_lines` to the [`text`](#bigtext) module.
 * Added support for `len` to the [`TopologicalSorter`](#topologicalsortergraphnone) object.
 
-**0.5.1**
+**0.5.1** *2022/09/04*
 
 * Added
   [`gently_title`](#gently_titles-apostrophesnone-double_quotesnone)
   and
   [`normalize_whitespace`](#normalize_whitespaces-separatorsNone-replacementNone)
   to the [`text`](#bigtext) module.
 * Changed [`translate_filename_to_exfat`](#translate_filename_to_exfats)
@@ -3785,11 +3812,11 @@
   If the colon is followed by a space, then the colon is turned into `' -'`.
   This yields a more natural translation when colons are used in text, e.g.
   `'xXx: The Return Of Xander Cage'` is translated to `'xXx - The Return Of Xander Cage'`.
   If the colon is not followed by a space, turns the colon into `'-'`.
   This is good for tiresome modern gobbledygook like `'Re:code'`, which
   will now be translated to `'Re-code'`.
 
-**0.5**
+**0.5** *2022/06/12*
 
 * Initial release.
```

