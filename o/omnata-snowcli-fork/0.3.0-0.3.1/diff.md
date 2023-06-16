# Comparing `tmp/omnata_snowcli_fork-0.3.0.tar.gz` & `tmp/omnata_snowcli_fork-0.3.1.tar.gz`

## Comparing `omnata_snowcli_fork-0.3.0.tar` & `omnata_snowcli_fork-0.3.1.tar`

### file list

```diff
@@ -1,479 +1,479 @@
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/LEGAL.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/snowcli.spec
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tox.ini
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/@plugins_snapshot.json
--rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/__future__.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/__future__.meta.json
--rw-r--r--   0        0        0   113413 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ast.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ast.meta.json
--rw-r--r--   0        0        0    53328 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_codecs.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_codecs.meta.json
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_collections_abc.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_collections_abc.meta.json
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ctypes.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ctypes.meta.json
--rw-r--r--   0        0        0   140868 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_socket.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_socket.meta.json
--rw-r--r--   0        0        0    24080 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_thread.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_thread.meta.json
--rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_warnings.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_warnings.meta.json
--rw-r--r--   0        0        0    20721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/abc.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/abc.meta.json
--rw-r--r--   0        0        0    64450 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/array.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/array.meta.json
--rw-r--r--   0        0        0  1027196 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/builtins.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/builtins.meta.json
--rw-r--r--   0        0        0   125859 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/codecs.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/codecs.meta.json
--rw-r--r--   0        0        0   127373 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/configparser.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/configparser.meta.json
--rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/contextlib.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/contextlib.meta.json
--rw-r--r--   0        0        0    51616 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/dataclasses.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/dataclasses.meta.json
--rw-r--r--   0        0        0   127581 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/datetime.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/datetime.meta.json
--rw-r--r--   0        0        0    63819 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/enum.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/enum.meta.json
--rw-r--r--   0        0        0   130413 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/functools.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/functools.meta.json
--rw-r--r--   0        0        0    24307 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/genericpath.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/genericpath.meta.json
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/glob.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/glob.meta.json
--rw-r--r--   0        0        0    88170 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/io.data.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/io.meta.json
--rw-r--r--   0        0        0    29442 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/mmap.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/mmap.meta.json
--rw-r--r--   0        0        0    87490 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pathlib.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pathlib.meta.json
--rw-r--r--   0        0        0    48666 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pickle.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pickle.meta.json
--rw-r--r--   0        0        0    32077 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkgutil.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkgutil.meta.json
--rw-r--r--   0        0        0    80760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/posixpath.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/posixpath.meta.json
--rw-r--r--   0        0        0    29877 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/queue.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/queue.meta.json
--rw-r--r--   0        0        0   148949 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/re.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/re.meta.json
--rw-r--r--   0        0        0    73616 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/shutil.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/shutil.meta.json
--rw-r--r--   0        0        0   118796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/socket.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/socket.meta.json
--rw-r--r--   0        0        0    15116 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_compile.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_compile.meta.json
--rw-r--r--   0        0        0    29743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_constants.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_constants.meta.json
--rw-r--r--   0        0        0    52485 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_parse.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_parse.meta.json
--rw-r--r--   0        0        0   188845 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ssl.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ssl.meta.json
--rw-r--r--   0        0        0    28383 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/string.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/string.meta.json
--rw-r--r--   0        0        0   146347 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/subprocess.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/subprocess.meta.json
--rw-r--r--   0        0        0   146865 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sys.data.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sys.meta.json
--rw-r--r--   0        0        0   116339 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/tempfile.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/tempfile.meta.json
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_main.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_main.meta.json
--rw-r--r--   0        0        0    21445 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_printing.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_printing.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_render.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_render.meta.json
--rw-r--r--   0        0        0    32770 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_snow_connector.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_snow_connector.meta.json
--rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_sql.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_sql.meta.json
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_stage.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_stage.meta.json
--rw-r--r--   0        0        0    20630 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/textwrap.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/textwrap.meta.json
--rw-r--r--   0        0        0    66595 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/threading.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/threading.meta.json
--rw-r--r--   0        0        0    43946 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/time.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/time.meta.json
--rw-r--r--   0        0        0   216120 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/types.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/types.meta.json
--rw-r--r--   0        0        0   409062 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing.meta.json
--rw-r--r--   0        0        0    70194 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing_extensions.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing_extensions.meta.json
--rw-r--r--   0        0        0    35325 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/uuid.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/uuid.meta.json
--rw-r--r--   0        0        0    23589 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/warnings.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/warnings.meta.json
--rw-r--r--   0        0        0    71256 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipfile.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipfile.meta.json
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipimport.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipimport.meta.json
--rw-r--r--   0        0        0    91654 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/__init__.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/__init__.meta.json
--rw-r--r--   0        0        0    11123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/_termui_impl.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/_termui_impl.meta.json
--rw-r--r--   0        0        0   115909 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/core.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/core.meta.json
--rw-r--r--   0        0        0    51491 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/decorators.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/decorators.meta.json
--rw-r--r--   0        0        0    23719 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/exceptions.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/exceptions.meta.json
--rw-r--r--   0        0        0    16560 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/formatting.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/formatting.meta.json
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/globals.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/globals.meta.json
--rw-r--r--   0        0        0    24339 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/parser.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/parser.meta.json
--rw-r--r--   0        0        0    26150 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/termui.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/termui.meta.json
--rw-r--r--   0        0        0    24211 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/testing.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/testing.meta.json
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/types.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/types.meta.json
--rw-r--r--   0        0        0    24600 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/utils.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/utils.meta.json
--rw-r--r--   0        0        0   357260 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/__init__.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/__init__.meta.json
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/abc.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/abc.meta.json
--rw-r--r--   0        0        0   132721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/__init__.meta.json
--rw-r--r--   0        0        0    26220 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/version.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/version.meta.json
--rw-r--r--   0        0        0     8090 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/__init__.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/__init__.meta.json
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/charset.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/charset.meta.json
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/contentmanager.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24187 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/errors.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/errors.meta.json
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/header.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/header.meta.json
--rw-r--r--   0        0        0    59332 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/message.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/message.meta.json
--rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/policy.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/policy.meta.json
--rw-r--r--   0        0        0    20060 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/__init__.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/__init__.meta.json
--rw-r--r--   0        0        0    68954 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/client.data.json
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/client.meta.json
--rw-r--r--   0        0        0    60928 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/cookiejar.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/cookiejar.meta.json
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/__init__.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/__init__.meta.json
--rw-r--r--   0        0        0    43073 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/abc.data.json
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/abc.meta.json
--rw-r--r--   0        0        0    69711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/machinery.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/machinery.meta.json
--rw-r--r--   0        0        0    68105 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/__init__.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/__init__.meta.json
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/snowflake_connector.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/snowflake_connector.meta.json
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/test_warehouse.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/test_warehouse.meta.json
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/__init__.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/__init__.meta.json
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/bccache.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/bccache.meta.json
--rw-r--r--   0        0        0    76500 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/environment.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/environment.meta.json
--rw-r--r--   0        0        0    16511 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/exceptions.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/exceptions.meta.json
--rw-r--r--   0        0        0    44831 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/filters.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/filters.meta.json
--rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/loaders.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/loaders.meta.json
--rw-r--r--   0        0        0    47215 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/runtime.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/runtime.meta.json
--rw-r--r--   0        0        0    46950 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/utils.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/utils.meta.json
--rw-r--r--   0        0        0    16587 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/__init__.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/__init__.meta.json
--rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/decoder.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/decoder.meta.json
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/encoder.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/encoder.meta.json
--rw-r--r--   0        0        0   148004 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/logging/__init__.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/logging/__init__.meta.json
--rw-r--r--   0        0        0    33702 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/__init__.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/__init__.meta.json
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_compat.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_compat.meta.json
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_native.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_native.meta.json
--rw-r--r--   0        0        0   346973 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/__init__.data.json
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/__init__.meta.json
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/path.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/path.meta.json
--rw-r--r--   0        0        0   149576 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkg_resources/__init__.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkg_resources/__init__.meta.json
--rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__init__.data.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__init__.meta.json
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__version__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__version__.meta.json
--rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/adapters.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/adapters.meta.json
--rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/api.data.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/api.meta.json
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/auth.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/auth.meta.json
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/compat.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/compat.meta.json
--rw-r--r--   0        0        0    21572 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/cookies.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/cookies.meta.json
--rw-r--r--   0        0        0    24561 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/exceptions.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/exceptions.meta.json
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/hooks.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/hooks.meta.json
--rw-r--r--   0        0        0    69403 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/models.data.json
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/models.meta.json
--rw-r--r--   0        0        0    78465 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/sessions.data.json
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/sessions.meta.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/status_codes.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/status_codes.meta.json
--rw-r--r--   0        0        0    25470 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/structures.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/structures.meta.json
--rw-r--r--   0        0        0    30514 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/utils.data.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/utils.meta.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__about__.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__about__.meta.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__init__.meta.json
--rw-r--r--   0        0        0    46423 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snow_connector.data.json
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snow_connector.meta.json
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snowsql_config.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snowsql_config.meta.json
--rw-r--r--   0        0        0     8510 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/render.data.json
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/render.meta.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/__init__.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/__init__.meta.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/flags.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/flags.meta.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/__init__.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/__init__.meta.json
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/formats.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/formats.meta.json
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/printing.data.json
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/printing.meta.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/__init__.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/__init__.meta.json
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function.meta.json
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function/app.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function/app.meta.json
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/app.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/app.meta.json
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/local_connection.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/local_connection.meta.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/__init__.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/__init__.meta.json
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/result_assertions.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/result_assertions.meta.json
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/__init__.meta.json
--rw-r--r--   0        0        0    49526 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/decoder.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/decoder.meta.json
--rw-r--r--   0        0        0    41892 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/encoder.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/encoder.meta.json
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/__init__.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/__init__.meta.json
--rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/async_case.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/async_case.meta.json
--rw-r--r--   0        0        0   240763 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/case.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/case.meta.json
--rw-r--r--   0        0        0    15492 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/loader.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/loader.meta.json
--rw-r--r--   0        0        0    12416 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/main.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/main.meta.json
--rw-r--r--   0        0        0   146758 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/mock.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/mock.meta.json
--rw-r--r--   0        0        0    21805 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/result.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/result.meta.json
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/runner.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/runner.meta.json
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/signals.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/signals.meta.json
--rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/suite.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/suite.meta.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/__init__.meta.json
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/error.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/error.meta.json
--rw-r--r--   0        0        0   143751 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/parse.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/parse.meta.json
--rw-r--r--   0        0        0   157530 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/request.data.json
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/request.meta.json
--rw-r--r--   0        0        0    27842 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/response.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/response.meta.json
--rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/__init__.data.json
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/__init__.meta.json
--rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/_collections.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/_collections.meta.json
--rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connection.data.json
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connection.meta.json
--rw-r--r--   0        0        0    34033 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connectionpool.data.json
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connectionpool.meta.json
--rw-r--r--   0        0        0    45347 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/exceptions.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/exceptions.meta.json
--rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/fields.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/fields.meta.json
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/filepost.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/filepost.meta.json
--rw-r--r--   0        0        0    10957 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/poolmanager.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/poolmanager.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/request.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/request.meta.json
--rw-r--r--   0        0        0    40848 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/response.data.json
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/response.meta.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/__init__.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/__init__.meta.json
--rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/socks.data.json
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/socks.meta.json
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/__init__.data.json
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/__init__.meta.json
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/connection.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/connection.meta.json
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/queue.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/queue.meta.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/request.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/request.meta.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/response.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/response.meta.json
--rw-r--r--   0        0        0    45795 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/retry.data.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/retry.meta.json
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_.meta.json
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.meta.json
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/timeout.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/timeout.meta.json
--rw-r--r--   0        0        0    44004 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/url.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/url.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/docs/images/coverage_5.png
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/config.py
--rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/snowsql_config.py
--rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/utils.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/common/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/common/flags.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/__init__.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/function.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/package.py
--rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure_coverage/report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/output/formats.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/output/printing.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_function/app.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_function/app.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_procedure/app.toml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test.toml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_main.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_render.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_snow_connector.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_sql.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_stage.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/integration/snowflake_connector.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/integration/test_warehouse.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/output/test_printing.py
--rw-r--r--   0        0        0  1508323 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/LICENSE
--rw-r--r--   0        0        0    11944 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/README.md
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    13181 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/LEGAL.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/snowcli.spec
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tox.ini
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/__future__.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/__future__.meta.json
+-rw-r--r--   0        0        0   113413 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ast.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ast.meta.json
+-rw-r--r--   0        0        0    53328 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_codecs.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_codecs.meta.json
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_collections_abc.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ctypes.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ctypes.meta.json
+-rw-r--r--   0        0        0   140868 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_socket.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_socket.meta.json
+-rw-r--r--   0        0        0    24080 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_thread.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_thread.meta.json
+-rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_warnings.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_warnings.meta.json
+-rw-r--r--   0        0        0    20721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/abc.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/abc.meta.json
+-rw-r--r--   0        0        0    64450 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/array.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/array.meta.json
+-rw-r--r--   0        0        0  1027196 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/builtins.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/builtins.meta.json
+-rw-r--r--   0        0        0   125859 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/codecs.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/codecs.meta.json
+-rw-r--r--   0        0        0   127373 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/configparser.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/configparser.meta.json
+-rw-r--r--   0        0        0    97404 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/contextlib.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/contextlib.meta.json
+-rw-r--r--   0        0        0    51616 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/dataclasses.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/dataclasses.meta.json
+-rw-r--r--   0        0        0   127581 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/datetime.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/datetime.meta.json
+-rw-r--r--   0        0        0    63819 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/enum.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/enum.meta.json
+-rw-r--r--   0        0        0   130413 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/functools.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/functools.meta.json
+-rw-r--r--   0        0        0    24307 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/genericpath.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/genericpath.meta.json
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/glob.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/glob.meta.json
+-rw-r--r--   0        0        0    88170 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/io.data.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/io.meta.json
+-rw-r--r--   0        0        0    29442 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/mmap.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/mmap.meta.json
+-rw-r--r--   0        0        0    87490 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pathlib.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pathlib.meta.json
+-rw-r--r--   0        0        0    48666 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pickle.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pickle.meta.json
+-rw-r--r--   0        0        0    32077 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkgutil.data.json
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkgutil.meta.json
+-rw-r--r--   0        0        0    80760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/posixpath.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/posixpath.meta.json
+-rw-r--r--   0        0        0    29877 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/queue.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/queue.meta.json
+-rw-r--r--   0        0        0   148949 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/re.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/re.meta.json
+-rw-r--r--   0        0        0    73616 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/shutil.data.json
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/shutil.meta.json
+-rw-r--r--   0        0        0   118796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/socket.data.json
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/socket.meta.json
+-rw-r--r--   0        0        0    15116 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_compile.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_compile.meta.json
+-rw-r--r--   0        0        0    29743 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_constants.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_constants.meta.json
+-rw-r--r--   0        0        0    52485 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_parse.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_parse.meta.json
+-rw-r--r--   0        0        0   188845 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ssl.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ssl.meta.json
+-rw-r--r--   0        0        0    28383 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/string.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/string.meta.json
+-rw-r--r--   0        0        0   146347 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/subprocess.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/subprocess.meta.json
+-rw-r--r--   0        0        0   146865 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sys.data.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sys.meta.json
+-rw-r--r--   0        0        0   116339 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/tempfile.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/tempfile.meta.json
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_main.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_main.meta.json
+-rw-r--r--   0        0        0    21445 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_printing.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_printing.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_render.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_render.meta.json
+-rw-r--r--   0        0        0    32770 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_snow_connector.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_snow_connector.meta.json
+-rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_sql.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_sql.meta.json
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_stage.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_stage.meta.json
+-rw-r--r--   0        0        0    20630 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/textwrap.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/textwrap.meta.json
+-rw-r--r--   0        0        0    66595 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/threading.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/threading.meta.json
+-rw-r--r--   0        0        0    43946 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/time.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/time.meta.json
+-rw-r--r--   0        0        0   216120 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/types.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/types.meta.json
+-rw-r--r--   0        0        0   409062 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing.meta.json
+-rw-r--r--   0        0        0    70194 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing_extensions.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing_extensions.meta.json
+-rw-r--r--   0        0        0    35325 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/uuid.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/uuid.meta.json
+-rw-r--r--   0        0        0    23589 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/warnings.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/warnings.meta.json
+-rw-r--r--   0        0        0    71256 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipfile.data.json
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipfile.meta.json
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipimport.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipimport.meta.json
+-rw-r--r--   0        0        0    91654 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/__init__.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/__init__.meta.json
+-rw-r--r--   0        0        0    11123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0   115909 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/core.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/core.meta.json
+-rw-r--r--   0        0        0    51491 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/decorators.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/decorators.meta.json
+-rw-r--r--   0        0        0    23719 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/exceptions.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/exceptions.meta.json
+-rw-r--r--   0        0        0    16560 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/formatting.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/formatting.meta.json
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/globals.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/globals.meta.json
+-rw-r--r--   0        0        0    24339 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/parser.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/parser.meta.json
+-rw-r--r--   0        0        0    26150 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/termui.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/termui.meta.json
+-rw-r--r--   0        0        0    24211 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/testing.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/testing.meta.json
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/types.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/types.meta.json
+-rw-r--r--   0        0        0    24600 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/utils.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/utils.meta.json
+-rw-r--r--   0        0        0   357260 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/__init__.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/abc.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/abc.meta.json
+-rw-r--r--   0        0        0   132721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/__init__.meta.json
+-rw-r--r--   0        0        0    26220 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/version.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/version.meta.json
+-rw-r--r--   0        0        0     8090 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/__init__.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/__init__.meta.json
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/charset.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/charset.meta.json
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    24187 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/errors.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/errors.meta.json
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/header.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/header.meta.json
+-rw-r--r--   0        0        0    59332 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/message.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/message.meta.json
+-rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/policy.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/policy.meta.json
+-rw-r--r--   0        0        0    20060 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/__init__.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/__init__.meta.json
+-rw-r--r--   0        0        0    68954 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/client.data.json
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/client.meta.json
+-rw-r--r--   0        0        0    60928 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/cookiejar.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/cookiejar.meta.json
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    43073 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/abc.data.json
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69711 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    68105 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/__init__.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/__init__.meta.json
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/snowflake_connector.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/snowflake_connector.meta.json
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/test_warehouse.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/test_warehouse.meta.json
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/__init__.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/__init__.meta.json
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/bccache.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/bccache.meta.json
+-rw-r--r--   0        0        0    76500 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/environment.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/environment.meta.json
+-rw-r--r--   0        0        0    16511 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/exceptions.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/exceptions.meta.json
+-rw-r--r--   0        0        0    44831 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/filters.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/filters.meta.json
+-rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/loaders.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/loaders.meta.json
+-rw-r--r--   0        0        0    47215 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/runtime.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/runtime.meta.json
+-rw-r--r--   0        0        0    46950 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/utils.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/utils.meta.json
+-rw-r--r--   0        0        0    16587 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/__init__.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/__init__.meta.json
+-rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/decoder.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/decoder.meta.json
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/encoder.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/encoder.meta.json
+-rw-r--r--   0        0        0   148004 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/logging/__init__.data.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/logging/__init__.meta.json
+-rw-r--r--   0        0        0    33702 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/__init__.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/__init__.meta.json
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_compat.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_compat.meta.json
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_native.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_native.meta.json
+-rw-r--r--   0        0        0   346973 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/__init__.data.json
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/__init__.meta.json
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/path.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/path.meta.json
+-rw-r--r--   0        0        0   149576 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkg_resources/__init__.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkg_resources/__init__.meta.json
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__init__.data.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__init__.meta.json
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__version__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__version__.meta.json
+-rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/adapters.data.json
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/adapters.meta.json
+-rw-r--r--   0        0        0    26873 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/api.data.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/api.meta.json
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/auth.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/auth.meta.json
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/compat.data.json
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/compat.meta.json
+-rw-r--r--   0        0        0    21572 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/cookies.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/cookies.meta.json
+-rw-r--r--   0        0        0    24561 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/exceptions.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/exceptions.meta.json
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/hooks.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/hooks.meta.json
+-rw-r--r--   0        0        0    69403 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/models.data.json
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/models.meta.json
+-rw-r--r--   0        0        0    78465 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/sessions.data.json
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/sessions.meta.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/status_codes.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/status_codes.meta.json
+-rw-r--r--   0        0        0    25470 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/structures.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/structures.meta.json
+-rw-r--r--   0        0        0    30514 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/utils.data.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/utils.meta.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__about__.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__about__.meta.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__init__.meta.json
+-rw-r--r--   0        0        0    46423 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snow_connector.data.json
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snow_connector.meta.json
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snowsql_config.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snowsql_config.meta.json
+-rw-r--r--   0        0        0     8510 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/render.data.json
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/render.meta.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/__init__.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/__init__.meta.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/flags.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/flags.meta.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/__init__.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/__init__.meta.json
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/formats.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/formats.meta.json
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/printing.data.json
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/printing.meta.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/__init__.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/__init__.meta.json
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function.meta.json
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function/app.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function/app.meta.json
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/app.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/app.meta.json
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/local_connection.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/local_connection.meta.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/__init__.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/__init__.meta.json
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/result_assertions.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/result_assertions.meta.json
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/__init__.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/__init__.meta.json
+-rw-r--r--   0        0        0    49526 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/decoder.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/decoder.meta.json
+-rw-r--r--   0        0        0    41892 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/encoder.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/encoder.meta.json
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/__init__.meta.json
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   240763 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/case.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/case.meta.json
+-rw-r--r--   0        0        0    15492 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/loader.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12416 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/main.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/main.meta.json
+-rw-r--r--   0        0        0   146758 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/mock.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/mock.meta.json
+-rw-r--r--   0        0        0    21805 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/result.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/result.meta.json
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/runner.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/signals.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11762 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/suite.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/__init__.meta.json
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/error.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/error.meta.json
+-rw-r--r--   0        0        0   143751 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/parse.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/parse.meta.json
+-rw-r--r--   0        0        0   157530 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/request.data.json
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/request.meta.json
+-rw-r--r--   0        0        0    27842 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/response.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/response.meta.json
+-rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/__init__.data.json
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/__init__.meta.json
+-rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/_collections.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/_collections.meta.json
+-rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connection.data.json
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connection.meta.json
+-rw-r--r--   0        0        0    34033 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connectionpool.data.json
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connectionpool.meta.json
+-rw-r--r--   0        0        0    45347 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/exceptions.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/exceptions.meta.json
+-rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/fields.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/fields.meta.json
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/filepost.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/filepost.meta.json
+-rw-r--r--   0        0        0    10957 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/poolmanager.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/poolmanager.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/request.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/request.meta.json
+-rw-r--r--   0        0        0    40848 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/response.data.json
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/response.meta.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/__init__.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/__init__.meta.json
+-rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/socks.data.json
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/socks.meta.json
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/__init__.data.json
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/__init__.meta.json
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/connection.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/connection.meta.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/queue.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/queue.meta.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/request.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/request.meta.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/response.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/response.meta.json
+-rw-r--r--   0        0        0    45795 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/retry.data.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/retry.meta.json
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_.meta.json
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.meta.json
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/timeout.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/timeout.meta.json
+-rw-r--r--   0        0        0    44004 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/url.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/url.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/docs/images/coverage_5.png
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/__init__.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/config.py
+-rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/snowsql_config.py
+-rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/utils.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0    10631 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/common/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/common/flags.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/__init__.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/function.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/package.py
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5789 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure_coverage/report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/output/formats.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/output/printing.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/drop_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/list_stage.sql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/list_stages.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/snowcli/sql/show_warehouses.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_function/app.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_procedure/app.toml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test.toml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_main.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_render.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_snow_connector.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_sql.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_stage.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/integration/snowflake_connector.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/integration/test_warehouse.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/LICENSE
+-rw-r--r--   0        0        0    11944 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/README.md
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13181 2020-02-02 00:00:00.000000 omnata_snowcli_fork-0.3.1/PKG-INFO
```

### Comparing `omnata_snowcli_fork-0.3.0/.pre-commit-config.yaml` & `omnata_snowcli_fork-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/snowcli.spec` & `omnata_snowcli_fork-0.3.1/snowcli.spec`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/__future__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/__future__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/__future__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ast.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ast.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ast.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_codecs.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_codecs.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_collections_abc.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_collections_abc.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ctypes.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_ctypes.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_socket.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_socket.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_socket.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_thread.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_thread.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_thread.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_warnings.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_warnings.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/abc.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/abc.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/abc.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/abc.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/array.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/array.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/array.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/array.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/builtins.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/builtins.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/builtins.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/codecs.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/codecs.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/codecs.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/configparser.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/configparser.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/configparser.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/contextlib.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/contextlib.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/dataclasses.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/dataclasses.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/datetime.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/datetime.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/datetime.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/enum.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/enum.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/enum.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/enum.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/functools.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/functools.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/functools.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/functools.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/genericpath.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/genericpath.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/glob.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/glob.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/glob.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/glob.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/io.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/io.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/io.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/io.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/mmap.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/mmap.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/mmap.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pathlib.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pathlib.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pickle.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pickle.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pickle.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkgutil.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkgutil.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/posixpath.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/posixpath.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/queue.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/queue.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/queue.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/queue.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/re.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/re.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/re.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/re.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/shutil.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/shutil.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/shutil.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/socket.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/socket.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/socket.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/socket.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_compile.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_compile.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_constants.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_constants.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_parse.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sre_parse.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ssl.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ssl.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ssl.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/string.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/string.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/string.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/string.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/subprocess.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/subprocess.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sys.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sys.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/sys.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/sys.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/tempfile.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/tempfile.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_main.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_main.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_main.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_main.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_printing.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_printing.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_printing.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_printing.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_render.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_render.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_render.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_render.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_snow_connector.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_snow_connector.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_snow_connector.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_snow_connector.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_sql.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_sql.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_sql.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_sql.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_stage.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_stage.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/test_stage.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/test_stage.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/textwrap.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/textwrap.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/threading.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/threading.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/threading.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/threading.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/time.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/time.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/time.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/time.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/types.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/types.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/types.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/types.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing_extensions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/typing_extensions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/uuid.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/uuid.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/uuid.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/warnings.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/warnings.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/warnings.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipfile.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipfile.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipimport.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipimport.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/zipimport.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/zipimport.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_typeshed/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/_typeshed/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/_termui_impl.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/_termui_impl.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/core.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/core.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/core.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/decorators.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/decorators.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/exceptions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/exceptions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/formatting.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/formatting.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/globals.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/globals.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/parser.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/parser.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/termui.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/termui.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/testing.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/testing.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/testing.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/testing.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/types.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/types.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/types.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/utils.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/click/utils.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/abc.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/collections/abc.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ctypes/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/ctypes/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/version.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/version.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/distutils/version.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/distutils/version.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/charset.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/charset.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/contentmanager.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/contentmanager.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/errors.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/errors.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/header.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/header.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/header.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/message.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/message.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/message.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/policy.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/email/policy.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/client.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/client.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/client.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/client.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/cookiejar.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/cookiejar.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/http/cookiejar.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/http/cookiejar.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/abc.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/abc.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/machinery.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/machinery.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/metadata/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/importlib/metadata/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/snowflake_connector.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/snowflake_connector.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/snowflake_connector.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/snowflake_connector.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/test_warehouse.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/test_warehouse.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/integration/test_warehouse.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/integration/test_warehouse.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/bccache.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/bccache.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/bccache.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/bccache.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/environment.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/environment.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/environment.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/environment.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/exceptions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/exceptions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/filters.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/filters.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/filters.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/filters.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/loaders.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/loaders.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/loaders.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/loaders.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/runtime.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/runtime.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/runtime.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/runtime.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/utils.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/utils.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/jinja2/utils.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/jinja2/utils.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/decoder.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/decoder.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/encoder.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/json/encoder.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/logging/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/logging/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_compat.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_compat.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_compat.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_native.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_native.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/markupsafe/_native.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/markupsafe/_native.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/path.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/path.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/os/path.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkg_resources/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkg_resources/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/pkg_resources/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/pkg_resources/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__version__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__version__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/__version__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/__version__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/adapters.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/adapters.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/adapters.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/adapters.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/api.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/api.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/api.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/api.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/auth.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/auth.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/auth.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/auth.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/compat.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/compat.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/compat.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/compat.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/cookies.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/cookies.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/cookies.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/cookies.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/exceptions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/exceptions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/hooks.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/hooks.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/hooks.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/hooks.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/models.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/models.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/models.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/models.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/sessions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/sessions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/sessions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/sessions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/status_codes.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/status_codes.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/status_codes.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/status_codes.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/structures.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/structures.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/structures.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/structures.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/utils.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/utils.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/requests/utils.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/requests/utils.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__about__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__about__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__about__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snow_connector.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snow_connector.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snow_connector.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snow_connector.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snowsql_config.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snowsql_config.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/snowsql_config.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/snowsql_config.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/render.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/render.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/render.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/render.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/flags.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/flags.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/cli/common/flags.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/cli/common/flags.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/formats.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/formats.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/formats.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/formats.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/printing.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/printing.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/snowcli/output/printing.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/snowcli/output/printing.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function/app.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function/app.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_function/app.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_function/app.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/app.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/app.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/app.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/app.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/local_connection.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/local_connection.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/templates/default_procedure/local_connection.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/templates/default_procedure/local_connection.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/result_assertions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/result_assertions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/testing_utils/result_assertions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/testing_utils/result_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/decoder.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/decoder.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/decoder.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/encoder.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/encoder.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/toml/encoder.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/toml/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/async_case.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/async_case.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/case.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/case.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/loader.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/loader.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/main.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/main.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/mock.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/mock.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/result.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/result.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/runner.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/runner.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/signals.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/signals.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/suite.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/unittest/suite.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/error.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/error.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/error.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/error.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/parse.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/parse.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/request.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/request.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/request.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/request.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/response.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/response.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib/response.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib/response.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/_collections.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/_collections.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/_collections.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connection.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connection.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connection.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connection.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connectionpool.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connectionpool.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/connectionpool.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/connectionpool.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/exceptions.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/exceptions.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/fields.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/fields.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/fields.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/fields.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/filepost.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/filepost.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/filepost.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/filepost.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/poolmanager.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/poolmanager.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/poolmanager.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/poolmanager.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/request.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/request.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/request.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/request.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/response.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/response.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/response.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/response.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/socks.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/socks.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/contrib/socks.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/contrib/socks.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/__init__.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/__init__.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/connection.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/connection.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/connection.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/connection.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/queue.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/queue.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/queue.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/queue.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/request.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/request.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/request.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/request.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/response.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/response.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/response.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/response.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/retry.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/retry.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/retry.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/retry.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/ssl_match_hostname.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/timeout.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/timeout.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/timeout.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/timeout.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/url.data.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/url.data.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.mypy_cache/3.8/urllib3/util/url.meta.json` & `omnata_snowcli_fork-0.3.1/.mypy_cache/3.8/urllib3/util/url.meta.json`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/.pytest_cache/v/cache/nodeids` & `omnata_snowcli_fork-0.3.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/docs/images/coverage_1.png` & `omnata_snowcli_fork-0.3.1/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/docs/images/coverage_2.png` & `omnata_snowcli_fork-0.3.1/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/docs/images/coverage_3.png` & `omnata_snowcli_fork-0.3.1/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/docs/images/coverage_4.png` & `omnata_snowcli_fork-0.3.1/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/docs/images/coverage_5.png` & `omnata_snowcli_fork-0.3.1/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/config.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/config.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/snow_connector.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/snow_connector.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/snowsql_config.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/snowsql_config.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/utils.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/utils.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/__init__.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/connection.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/connection.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/render.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/render.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark_shared.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/sql.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/sql.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/stage.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/stage.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/streamlit.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/warehouse.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/warehouse.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/function.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/function.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/package.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/package.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure_coverage/clear.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure_coverage/clear.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/cli/snowpark/procedure_coverage/report.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/cli/snowpark/procedure_coverage/report.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/output/printing.py` & `omnata_snowcli_fork-0.3.1/src/snowcli/output/printing.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `omnata_snowcli_fork-0.3.1/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `omnata_snowcli_fork-0.3.1/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/snowcli/sql/create_procedure.sql` & `omnata_snowcli_fork-0.3.1/src/snowcli/sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/templates/default_procedure/app.py` & `omnata_snowcli_fork-0.3.1/src/templates/default_procedure/app.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/src/templates/default_procedure/local_connection.py` & `omnata_snowcli_fork-0.3.1/src/templates/default_procedure/local_connection.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_main.py` & `omnata_snowcli_fork-0.3.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_render.py` & `omnata_snowcli_fork-0.3.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_snow_connector.py` & `omnata_snowcli_fork-0.3.1/tests/test_snow_connector.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_sql.py` & `omnata_snowcli_fork-0.3.1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_stage.py` & `omnata_snowcli_fork-0.3.1/tests/test_stage.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_utils.py` & `omnata_snowcli_fork-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/__snapshots__/test_snow_connector.ambr` & `omnata_snowcli_fork-0.3.1/tests/__snapshots__/test_snow_connector.ambr`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/integration/test_warehouse.py` & `omnata_snowcli_fork-0.3.1/tests/integration/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/output/test_printing.py` & `omnata_snowcli_fork-0.3.1/tests/output/test_printing.py`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `omnata_snowcli_fork-0.3.1/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/LICENSE` & `omnata_snowcli_fork-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/README.md` & `omnata_snowcli_fork-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/pyproject.toml` & `omnata_snowcli_fork-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omnata_snowcli_fork-0.3.0/PKG-INFO` & `omnata_snowcli_fork-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnata-snowcli-fork
-Version: 0.3.0
+Version: 0.3.1
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/Snowflake-Labs/snowcli
 Project-URL: Bug Tracker, https://github.com/Snowflake-Labs/snowcli/issues
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

