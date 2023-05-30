# Comparing `tmp/su6-0.6.0.tar.gz` & `tmp/su6-0.7.0.tar.gz`

## Comparing `su6-0.6.0.tar` & `su6-0.7.0.tar`

### file list

```diff
@@ -1,1333 +1,1339 @@
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 su6-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 su6-0.6.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    43198 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_tracemalloc.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_tracemalloc.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/atexit.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/atexit.meta.json
--rw-r--r--   0        0        0    50463 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/bdb.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/bdb.meta.json
--rw-r--r--   0        0        0    11205 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/cmd.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/cmd.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    69838 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/fnmatch.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/fnmatch.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/gc.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/gc.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/locale.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/locale.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mypy_test.data.json
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mypy_test.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    92061 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pdb.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pdb.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    31495 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pkgutil.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pkgutil.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src.data.json
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0    48902 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tracemalloc.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tracemalloc.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    41964 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_version.data.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_version.meta.json
--rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   160343 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/capture.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/capture.meta.json
--rw-r--r--   0        0        0    25774 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/compat.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/compat.meta.json
--rw-r--r--   0        0        0    31571 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    51347 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   151482 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    58440 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    62322 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/logging.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/logging.meta.json
--rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/main.data.json
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/main.meta.json
--rw-r--r--   0        0        0    25625 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    57543 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    35138 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   131434 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   116087 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/python.data.json
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/python.meta.json
--rw-r--r--   0        0        0    51104 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/python_api.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    30448 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    51011 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/reports.data.json
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/reports.meta.json
--rw-r--r--   0        0        0    40627 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/runner.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/scope.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/scope.meta.json
--rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/stash.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/stash.meta.json
--rw-r--r--   0        0        0    93209 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/timing.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/timing.meta.json
--rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    26825 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   163843 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    18735 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    61373 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0   100218 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    39840 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   110674 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    44683 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    44423 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_parser.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_parser.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    18021 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/markers.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/markers.meta.json
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/requirements.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/requirements.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0    11134 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pytest/__init__.data.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/pytest/__init__.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/__init__.data.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/__init__.meta.json
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/cli.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/cli.meta.json
--rw-r--r--   0        0        0    43826 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/core.data.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/src/su6/core.meta.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    19368 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    49303 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/__about__.meta.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/__init__.data.json
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/__init__.meta.json
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/cli.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/cli.meta.json
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/core.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/su6_checker/core.meta.json
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tests/examples.data.json
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tests/examples.meta.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tests/examples/good.data.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/tests/examples/good.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.6.0/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.6.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/10595a931c3c881e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1065c8b44fadc39a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1086635a5970b925
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/10ab08017438a66a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/11f25cfda4e2f210
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/13985ae090677282
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/146952ec4263c5d9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1895bed4a0ed65d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1996a22aec44a5c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1cfd31ba4b0b7ef9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/247546336fc4bd59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/248d23bfc4586461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/24e2ebef92fa75b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/26657ed11f8e66de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/269f98f304a03fe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2bc4a20be77b881b
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2bf27b960bc3ded1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2c189a9882594507
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/2e4746b83d2d1cf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/300f9a816018d49f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3271e344462a0ee3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/349f044f89b94587
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/34e1109d49bf09f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/357e837fe90ee680
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/36e48551be186a66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/399d3b28a1a1db47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3a74e1b5704e9b3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3c6b70c96e832bc1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3ca706f99b2d38bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3e0ec316d612ddc6
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3f10d9d7687f3999
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/3f12e7a3fe46c220
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/417040cdeaa7bd81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/429010e306ea9808
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/467fc2e82c277fd8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/49fafbbbbadedf00
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4b5890a0c8dc15df
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4cd4c52ee1dc7ffe
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4eaf3b155fae0dfb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4f2c663677c63589
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/519ab6ce866ef11b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/58240cde188220d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/5da466fd7e3b19f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/5efe825a5e773b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/624348590d33bdc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6278996c2e6b2a87
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/69bb9ea6355c0c25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/69ffc3e7ad0aa6b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6a4adfab73a8d4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6b596d4ac1166741
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6b9f30172d33b6a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6bcca98e41cda3f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6beed9d45ff1a491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6db20c27780d4a5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/6db875fe1541793e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/701212523f7b3b9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/70963c0c68bf76ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/70d6f3b95738758d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/729f212cc9c6cd5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/72de7bec9ecb53aa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/76d56794deeb084d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/76fbe2af0f71bd4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/79a22043e5c16946
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7c37d34a0c059ec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7c806e58272a88ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7cbc35f4e814db65
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7f0f63895e369318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/7f75cbd11ebac70a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/886d14b97dbd4f2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/89e58e5ee0d7d864
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/8df3988e9368cbe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9352425265579062
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/945994955724de24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/94ffcc82bc7ee370
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/968b32ac9319cc53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/98392e87ef3eb254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9db15fb6e71bec4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9e3b1a7c0f34103b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/9edacb4de19eeb8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a113f7e28da04408
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a2fe93c3bba310b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a8da9d8efa986532
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ab360402eb2d795e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ac5b9f591ce9edec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b2d26e3968f3c218
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b4228843afe3d2eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b5c4e8c097cbf198
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b5f69f56d932f0d1
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ba0f74a0540d9a5a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/bbd87fc7f90c1f28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/bdd37795dc331d56
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/bdeb811362915192
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c88465e3c1dc503e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/cc518cf199497e9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/d2cceb9cc8265e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/da4aff17737df0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/dcb2ce27d1f7cc70
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/de1238012a6853f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/dfc2e498a5736fb3
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e067c98663409f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e59ac15827b7f1c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e832a8f80eaf16d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/e98cf82519b9efc2
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ec04e1ad73846b2a
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/ed03e948b89996b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f2942d8cb87b15e9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f4088198fa879c9c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f41987c18d73e01d
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f4d6392808939633
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f4e7c96257c9d24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f586c8a0f5c58b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/f9ab84e0c6669bed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/faa3132a8644ec4d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/fad49b925cd80258
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.6.0/.ruff_cache/content/fbd81c0d9b22b507
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_2602a302b50854cf___about___py.html
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_2602a302b50854cf___init___py.html
--rw-r--r--   0        0        0    80237 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_2602a302b50854cf_cli_py.html
--rw-r--r--   0        0        0   120602 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_2602a302b50854cf_core_py.html
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_a44f0ac069e85531__shared_py.html
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_about_py.html
--rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_core_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-0.6.0/htmlcov/style.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/bad.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/black_good_mypy_bad.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/except_pytest.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/good.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/invalid.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/only_black.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/only_mypy.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/bad.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/bad.meta.json
--rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-0.6.0/src/su6/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 su6-0.6.0/src/su6/__init__.py
--rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 su6-0.6.0/src/su6/cli.py
--rw-r--r--   0        0        0    15269 2020-02-02 00:00:00.000000 su6-0.6.0/src/su6/core.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-0.6.0/tests/_shared.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-0.6.0/tests/test_about.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 su6-0.6.0/tests/test_cli.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 su6-0.6.0/tests/test_core.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-0.6.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 su6-0.6.0/README.md
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 su6-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 su6-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 su6-0.7.0/coverage.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 su6-0.7.0/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    43198 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/atexit.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/atexit.meta.json
+-rw-r--r--   0        0        0    50463 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/bdb.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/bdb.meta.json
+-rw-r--r--   0        0        0    11205 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/cmd.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/cmd.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    69838 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/fnmatch.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/fnmatch.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/gc.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/gc.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/locale.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/locale.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mypy_test.data.json
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mypy_test.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    92061 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pdb.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pdb.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    31495 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pkgutil.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pkgutil.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src.data.json
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0    48902 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tracemalloc.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tracemalloc.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    41964 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   160343 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    25774 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/compat.meta.json
+-rw-r--r--   0        0        0    31571 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    51347 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   151482 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    58440 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    62322 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/main.data.json
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/main.meta.json
+-rw-r--r--   0        0        0    25625 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    57543 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    35138 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   131434 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   116087 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/python.data.json
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/python.meta.json
+-rw-r--r--   0        0        0    51104 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    30448 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    51011 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    40627 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/stash.meta.json
+-rw-r--r--   0        0        0    93209 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    26825 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   163843 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    18735 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    61373 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0   100218 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    39840 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   110674 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45617 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182333 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94672 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    44683 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31404 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    44423 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    18021 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/markers.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/markers.meta.json
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24922 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0    11134 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/pytest/__init__.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175740 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112763 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/__init__.data.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/__init__.meta.json
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/cli.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/cli.meta.json
+-rw-r--r--   0        0        0    43826 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/core.data.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/src/su6/core.meta.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    19550 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    50798 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/__about__.data.json
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/__about__.meta.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/__init__.data.json
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/__init__.meta.json
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/cli.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/cli.meta.json
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/core.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/su6_checker/core.meta.json
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tests/examples.data.json
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tests/examples.meta.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tests/examples/good.data.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/tests/examples/good.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74736 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    57309 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33948 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.7.0/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.7.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1065c8b44fadc39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1086635a5970b925
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/10ab08017438a66a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1322b93a2154c54a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/146952ec4263c5d9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1895bed4a0ed65d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1996a22aec44a5c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/232d0222563916a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/247546336fc4bd59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/248d23bfc4586461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/24e2ebef92fa75b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/26657ed11f8e66de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/269f98f304a03fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2bc4a20be77b881b
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2bf27b960bc3ded1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2c189a9882594507
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/2f9e25dc2ce777cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/300f9a816018d49f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/349f044f89b94587
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/357e837fe90ee680
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/36e48551be186a66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/399d3b28a1a1db47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3a74e1b5704e9b3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3ca706f99b2d38bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3e0ec316d612ddc6
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3f10d9d7687f3999
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/3f12e7a3fe46c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/417040cdeaa7bd81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/429010e306ea9808
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/467fc2e82c277fd8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/49fafbbbbadedf00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4b5890a0c8dc15df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4cd4c52ee1dc7ffe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4eaf3b155fae0dfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4f2c663677c63589
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/519ab6ce866ef11b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/58240cde188220d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/5da466fd7e3b19f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/5efe825a5e773b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/624348590d33bdc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6278996c2e6b2a87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/69bb9ea6355c0c25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/69ffc3e7ad0aa6b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6a4adfab73a8d4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6b596d4ac1166741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6b9f30172d33b6a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6bcca98e41cda3f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6beed9d45ff1a491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/6db875fe1541793e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/701212523f7b3b9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/70963c0c68bf76ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/70bd045859d6cb20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/70d6f3b95738758d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/729f212cc9c6cd5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/72de7bec9ecb53aa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/76fbe2af0f71bd4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/79a22043e5c16946
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7c37d34a0c059ec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7c806e58272a88ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7cbc35f4e814db65
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7f0f63895e369318
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/886d14b97dbd4f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/89e58e5ee0d7d864
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/8df3988e9368cbe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9352425265579062
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/98392e87ef3eb254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9db15fb6e71bec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9e3b1a7c0f34103b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/9edacb4de19eeb8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a113f7e28da04408
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a2fe93c3bba310b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a8da9d8efa986532
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ab360402eb2d795e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ac5b9f591ce9edec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b4228843afe3d2eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b5c4e8c097cbf198
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b5f69f56d932f0d1
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ba0f74a0540d9a5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/bbd87fc7f90c1f28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/bdd37795dc331d56
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c121acc012633d2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c88465e3c1dc503e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/cc518cf199497e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/d2cceb9cc8265e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/dcb2ce27d1f7cc70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e067c98663409f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e59ac15827b7f1c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e832a8f80eaf16d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/e98cf82519b9efc2
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ec04e1ad73846b2a
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/ed03e948b89996b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f2942d8cb87b15e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f4088198fa879c9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f4d6392808939633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f4e7c96257c9d24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f586c8a0f5c58b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/f9ab84e0c6669bed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/faa3132a8644ec4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/fad49b925cd80258
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.7.0/.ruff_cache/content/fbd81c0d9b22b507
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_2602a302b50854cf___about___py.html
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_2602a302b50854cf___init___py.html
+-rw-r--r--   0        0        0    86634 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_2602a302b50854cf_cli_py.html
+-rw-r--r--   0        0        0   123305 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_2602a302b50854cf_core_py.html
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_a44f0ac069e85531__shared_py.html
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_about_py.html
+-rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html
+-rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_core_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-0.7.0/htmlcov/style.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/bad.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/black_good_mypy_bad.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/empty.toml
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/except_pytest.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/good.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/invalid.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/only_black.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/only_mypy.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/bad.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/bad.meta.json
+-rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-0.7.0/src/su6/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 su6-0.7.0/src/su6/__init__.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 su6-0.7.0/src/su6/cli.py
+-rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 su6-0.7.0/src/su6/core.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-0.7.0/tests/_shared.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-0.7.0/tests/test_about.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 su6-0.7.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 su6-0.7.0/tests/test_core.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 su6-0.7.0/README.md
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 su6-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 su6-0.7.0/PKG-INFO
```

### Comparing `su6-0.6.0/CHANGELOG.md` & `su6-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.0 (2023-05-30)
+### Feature
+* **cov:** Add support for coverage svg badge to pytest ([`ee6c29c`](https://github.com/robinvandernoord/su6-checker/commit/ee6c29c2d16d379d7d4a09f97a6c6fb29943d513))
+
+### Fix
+* **cov:** 100% coverage again (and check for it) ([`c162e0d`](https://github.com/robinvandernoord/su6-checker/commit/c162e0d8b86782dfdc8c7e540a5f73f939cc1fa2))
+
 ## v0.6.0 (2023-05-30)
 ### Feature
 * **format:** Allow `--format json` ([`3c958e5`](https://github.com/robinvandernoord/su6-checker/commit/3c958e5bb8dbfb79f76d3614385c062286429af4))
 
 ### Fix
 * **json:** Format=json did not actually output json... Also update tests ([`df5fd41`](https://github.com/robinvandernoord/su6-checker/commit/df5fd411b8336e046165c6893777ed9abf539ae0))
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/__future__.data.json` & `su6-0.7.0/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/__future__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_ast.data.json` & `su6-0.7.0/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_ast.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_bisect.data.json` & `su6-0.7.0/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_bisect.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_codecs.data.json` & `su6-0.7.0/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.7.0/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_csv.data.json` & `su6-0.7.0/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_csv.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.7.0/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_decimal.data.json` & `su6-0.7.0/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_decimal.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_operator.data.json` & `su6-0.7.0/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_operator.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_random.data.json` & `su6-0.7.0/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_random.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_socket.data.json` & `su6-0.7.0/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_socket.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_stat.data.json` & `su6-0.7.0/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_stat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_thread.data.json` & `su6-0.7.0/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_thread.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_tracemalloc.data.json` & `su6-0.7.0/.mypy_cache/3.11/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_tracemalloc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_warnings.data.json` & `su6-0.7.0/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_warnings.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_weakref.data.json` & `su6-0.7.0/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_weakref.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_weakrefset.data.json` & `su6-0.7.0/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/abc.data.json` & `su6-0.7.0/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/abc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/argparse.data.json` & `su6-0.7.0/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/argparse.meta.json` & `su6-0.7.0/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/array.data.json` & `su6-0.7.0/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/array.meta.json` & `su6-0.7.0/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ast.data.json` & `su6-0.7.0/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ast.meta.json` & `su6-0.7.0/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/atexit.data.json` & `su6-0.7.0/.mypy_cache/3.11/atexit.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/atexit.meta.json` & `su6-0.7.0/.mypy_cache/3.11/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/bdb.data.json` & `su6-0.7.0/.mypy_cache/3.11/bdb.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/bdb.meta.json` & `su6-0.7.0/.mypy_cache/3.11/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/bisect.data.json` & `su6-0.7.0/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/bisect.meta.json` & `su6-0.7.0/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/builtins.data.json` & `su6-0.7.0/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/builtins.meta.json` & `su6-0.7.0/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/cmd.data.json` & `su6-0.7.0/.mypy_cache/3.11/cmd.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/cmd.meta.json` & `su6-0.7.0/.mypy_cache/3.11/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/codecs.data.json` & `su6-0.7.0/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/codecs.meta.json` & `su6-0.7.0/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/colorsys.data.json` & `su6-0.7.0/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/colorsys.meta.json` & `su6-0.7.0/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/configparser.data.json` & `su6-0.7.0/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/configparser.meta.json` & `su6-0.7.0/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/contextlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/contextvars.data.json` & `su6-0.7.0/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/contextvars.meta.json` & `su6-0.7.0/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/copy.data.json` & `su6-0.7.0/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/copy.meta.json` & `su6-0.7.0/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/copyreg.data.json` & `su6-0.7.0/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/copyreg.meta.json` & `su6-0.7.0/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/csv.data.json` & `su6-0.7.0/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/csv.meta.json` & `su6-0.7.0/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.7.0/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.7.0/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/datetime.data.json` & `su6-0.7.0/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/datetime.meta.json` & `su6-0.7.0/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/decimal.data.json` & `su6-0.7.0/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/decimal.meta.json` & `su6-0.7.0/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/difflib.data.json` & `su6-0.7.0/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/difflib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/dis.data.json` & `su6-0.7.0/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/dis.meta.json` & `su6-0.7.0/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/doctest.data.json` & `su6-0.7.0/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/doctest.meta.json` & `su6-0.7.0/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/enum.data.json` & `su6-0.7.0/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/enum.meta.json` & `su6-0.7.0/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/errno.data.json` & `su6-0.7.0/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/errno.meta.json` & `su6-0.7.0/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/fnmatch.data.json` & `su6-0.7.0/.mypy_cache/3.11/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/fnmatch.meta.json` & `su6-0.7.0/.mypy_cache/3.11/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/fractions.data.json` & `su6-0.7.0/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/fractions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/functools.data.json` & `su6-0.7.0/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/functools.meta.json` & `su6-0.7.0/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/gc.data.json` & `su6-0.7.0/.mypy_cache/3.11/gc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/gc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/gc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/genericpath.data.json` & `su6-0.7.0/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.7.0/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/getpass.data.json` & `su6-0.7.0/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/getpass.meta.json` & `su6-0.7.0/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/gettext.data.json` & `su6-0.7.0/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/gettext.meta.json` & `su6-0.7.0/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/glob.data.json` & `su6-0.7.0/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/glob.meta.json` & `su6-0.7.0/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/good.data.json` & `su6-0.7.0/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/good.meta.json` & `su6-0.7.0/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/hashlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/hashlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/hmac.data.json` & `su6-0.7.0/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/hmac.meta.json` & `su6-0.7.0/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/inspect.data.json` & `su6-0.7.0/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/inspect.meta.json` & `su6-0.7.0/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/io.data.json` & `su6-0.7.0/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/io.meta.json` & `su6-0.7.0/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/itertools.data.json` & `su6-0.7.0/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/itertools.meta.json` & `su6-0.7.0/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/linecache.data.json` & `su6-0.7.0/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/linecache.meta.json` & `su6-0.7.0/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/locale.data.json` & `su6-0.7.0/.mypy_cache/3.11/locale.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/locale.meta.json` & `su6-0.7.0/.mypy_cache/3.11/locale.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/marshal.data.json` & `su6-0.7.0/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/marshal.meta.json` & `su6-0.7.0/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/math.data.json` & `su6-0.7.0/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/math.meta.json` & `su6-0.7.0/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mmap.data.json` & `su6-0.7.0/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mmap.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/msvcrt.data.json` & `su6-0.7.0/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/msvcrt.meta.json` & `su6-0.7.0/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mypy_extensions.data.json` & `su6-0.7.0/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mypy_test.data.json` & `su6-0.7.0/.mypy_cache/3.11/mypy_test.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mypy_test.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mypy_test.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/numbers.data.json` & `su6-0.7.0/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/numbers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/opcode.data.json` & `su6-0.7.0/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/opcode.meta.json` & `su6-0.7.0/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/operator.data.json` & `su6-0.7.0/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/operator.meta.json` & `su6-0.7.0/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pdb.data.json` & `su6-0.7.0/.mypy_cache/3.11/pdb.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pdb.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pickle.data.json` & `su6-0.7.0/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pickle.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pkgutil.data.json` & `su6-0.7.0/.mypy_cache/3.11/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pkgutil.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platform.data.json` & `su6-0.7.0/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platform.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/posixpath.data.json` & `su6-0.7.0/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.7.0/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pprint.data.json` & `su6-0.7.0/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pprint.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pty.data.json` & `su6-0.7.0/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pty.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pydoc.data.json` & `su6-0.7.0/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pydoc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/queue.data.json` & `su6-0.7.0/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/queue.meta.json` & `su6-0.7.0/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/random.data.json` & `su6-0.7.0/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/random.meta.json` & `su6-0.7.0/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/re.data.json` & `su6-0.7.0/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/re.meta.json` & `su6-0.7.0/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/reprlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/reprlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/secrets.data.json` & `su6-0.7.0/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/secrets.meta.json` & `su6-0.7.0/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/selectors.data.json` & `su6-0.7.0/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/selectors.meta.json` & `su6-0.7.0/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/shlex.data.json` & `su6-0.7.0/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/shlex.meta.json` & `su6-0.7.0/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/shutil.data.json` & `su6-0.7.0/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/shutil.meta.json` & `su6-0.7.0/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/signal.data.json` & `su6-0.7.0/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/signal.meta.json` & `su6-0.7.0/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/socket.data.json` & `su6-0.7.0/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/socket.meta.json` & `su6-0.7.0/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src.data.json` & `su6-0.7.0/.mypy_cache/3.11/src.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src.meta.json` & `su6-0.7.0/.mypy_cache/3.11/src.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.7.0/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.7.0/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.7.0/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.7.0/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.7.0/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.7.0/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ssl.data.json` & `su6-0.7.0/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ssl.meta.json` & `su6-0.7.0/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/stat.data.json` & `su6-0.7.0/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/stat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/string.data.json` & `su6-0.7.0/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/string.meta.json` & `su6-0.7.0/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/struct.data.json` & `su6-0.7.0/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/struct.meta.json` & `su6-0.7.0/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/subprocess.data.json` & `su6-0.7.0/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.7.0/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sys.data.json` & `su6-0.7.0/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sys.meta.json` & `su6-0.7.0/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sysconfig.data.json` & `su6-0.7.0/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/sysconfig.meta.json` & `su6-0.7.0/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tempfile.data.json` & `su6-0.7.0/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tempfile.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/termios.data.json` & `su6-0.7.0/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/termios.meta.json` & `su6-0.7.0/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/textwrap.data.json` & `su6-0.7.0/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/textwrap.meta.json` & `su6-0.7.0/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/this.data.json` & `su6-0.7.0/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/this.meta.json` & `su6-0.7.0/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/threading.data.json` & `su6-0.7.0/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/threading.meta.json` & `su6-0.7.0/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/time.data.json` & `su6-0.7.0/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/time.meta.json` & `su6-0.7.0/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/token.data.json` & `su6-0.7.0/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/token.meta.json` & `su6-0.7.0/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tokenize.data.json` & `su6-0.7.0/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tokenize.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tomllib.data.json` & `su6-0.7.0/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tomllib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/traceback.data.json` & `su6-0.7.0/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/traceback.meta.json` & `su6-0.7.0/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tracemalloc.data.json` & `su6-0.7.0/.mypy_cache/3.11/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tracemalloc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tty.data.json` & `su6-0.7.0/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tty.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/types.data.json` & `su6-0.7.0/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/types.meta.json` & `su6-0.7.0/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typing.data.json` & `su6-0.7.0/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typing.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.7.0/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unicodedata.data.json` & `su6-0.7.0/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unicodedata.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/uuid.data.json` & `su6-0.7.0/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/uuid.meta.json` & `su6-0.7.0/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/warnings.data.json` & `su6-0.7.0/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/warnings.meta.json` & `su6-0.7.0/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/weakref.data.json` & `su6-0.7.0/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/weakref.meta.json` & `su6-0.7.0/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/webbrowser.data.json` & `su6-0.7.0/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/webbrowser.meta.json` & `su6-0.7.0/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/zlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/zlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_version.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_version.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/capture.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/capture.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/debugging.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/debugging.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/deprecated.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/deprecated.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/doctest.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/doctest.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/fixtures.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/fixtures.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/freeze_support.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/helpconfig.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/hookspec.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/hookspec.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/legacypath.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/legacypath.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/logging.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/logging.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/main.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/main.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/nodes.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/nodes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/outcomes.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/outcomes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pathlib.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pathlib.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pytester.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pytester.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/python.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/python.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/python_api.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/python_api.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/recwarn.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/recwarn.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/reports.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/reports.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/runner.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/runner.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/scope.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/scope.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/stash.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/stash.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/terminal.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/terminal.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/timing.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/timing.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/tmpdir.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/warning_types.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/warning_types.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/warnings.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/warnings.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/code.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/code.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/source.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_code/source.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/util.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/expression.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/structures.data.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/events.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/events.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/futures.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/locks.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/queues.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/runners.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/streams.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/threads.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/transports.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6-0.7.0/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/_width_table.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/_width_table.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/brackets.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/brackets.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/cache.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/cache.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/comments.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/comments.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/concurrency.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/concurrency.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/const.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/const.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/files.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/files.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/linegen.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/linegen.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/lines.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/lines.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/mode.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/mode.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/nodes.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/nodes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/numerics.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/numerics.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/output.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/output.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/parsing.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/parsing.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/report.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/report.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/rusty.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/rusty.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/strings.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/strings.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/trans.data.json` & `su6-0.7.0/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/black/trans.meta.json` & `su6-0.7.0/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/core.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/decorators.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/decorators.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/exceptions.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/formatting.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/formatting.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/globals.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/globals.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/parser.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/parser.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/termui.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/termui.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/types.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/types.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/click/utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.7.0/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6-0.7.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-0.7.0/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/charset.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/errors.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/header.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/header.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/message.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/message.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/policy.data.json` & `su6-0.7.0/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.7.0/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/html/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/html/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/html/entities.data.json` & `su6-0.7.0/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/html/entities.meta.json` & `su6-0.7.0/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/util.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/util.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-0.7.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/_parse.data.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/_parse.meta.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/exceptions.data.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/decoder.data.json` & `su6-0.7.0/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/decoder.meta.json` & `su6-0.7.0/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/encoder.data.json` & `su6-0.7.0/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/json/encoder.meta.json` & `su6-0.7.0/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/logging/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-0.7.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-0.7.0/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6-0.7.0/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/os/path.data.json` & `su6-0.7.0/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/os/path.meta.json` & `su6-0.7.0/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_parser.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_parser.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_structures.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_tokenizer.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/markers.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/markers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/requirements.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/requirements.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/tags.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/tags.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/version.data.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/packaging/version.meta.json` & `su6-0.7.0/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/util.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/util.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/android.data.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/api.data.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/version.data.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6-0.7.0/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pytest/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/pytest/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/__main__.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_extension.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_loop.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_pick.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_stack.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_timer.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_windows.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/abc.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/abc.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/align.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/align.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/ansi.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/box.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/box.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/cells.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/cells.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/color.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/color.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/columns.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/columns.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/console.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/console.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/constrain.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/containers.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/containers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/control.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/control.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/emoji.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/errors.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/errors.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/json.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/json.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/live.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/live.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/live_render.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/markdown.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/markup.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/markup.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/measure.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/measure.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/padding.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/padding.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/pager.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/pager.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/palette.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/palette.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/panel.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/panel.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/pretty.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/protocol.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/region.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/region.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/repr.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/repr.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/rule.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/rule.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/scope.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/scope.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/screen.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/screen.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/segment.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/segment.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/spinner.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/status.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/status.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/style.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/style.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/styled.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/styled.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/syntax.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/table.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/table.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/text.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/text.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/theme.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/theme.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/themes.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/themes.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/traceback.data.json` & `su6-0.7.0/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-0.7.0/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/cli.data.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/cli.meta.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/core.data.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/src/su6/core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/src/su6/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/__about__.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'hash'": "'61dcb8071e7f49a934679436dd12a1d384a6025939a9cf205b10403e0d401ade'",*

 * * "'mtime'": '1685447321'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "fb8c1690022628c6be82a3810aefe2c53847e2a20285ff2038315676a238d812",
+    "hash": "61dcb8071e7f49a934679436dd12a1d384a6025939a9cf205b10403e0d401ade",
     "id": "su6.__about__",
     "ignore_all": false,
     "interface_hash": "f585c505c8d50598658e61be6359ebe7fcc6381e8be269711f79d29222dffbf9",
-    "mtime": 1685447278,
+    "mtime": 1685447321,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1685449110'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1685445422,
+    "data_mtime": 1685449110,
     "dep_lines": [
         9,
         1,
         1,
         1
     ],
     "dep_prios": [
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/cli.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6/cli.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999990915697674%*

 * *Differences: {"'names'": "{'check_all': {'node': {'func': {'arg_kinds': {insert: [(0, 1)]}, 'arg_names': "*

 * *            "{insert: [(3, 'badge')]}, 'type': {'arg_kinds': {insert: [(0, 1)]}, 'arg_names': "*

 * *            "{insert: [(3, 'badge')]}, 'arg_types': {insert: [(3, OrderedDict([('.class', "*

 * *            "'UnionType'), ('items', ['builtins.bool', OrderedDict([('.class', "*

 * *            "'NoneType')])])]))]}}}}}, 'pytest': {'node': {'func': {'arg_kinds': {insert: [(0, "*

 * *            "1)]}, 'arg_names': {insert: [(4, 'badge […]*

```diff
@@ -489,38 +489,42 @@
                 ".class": "Decorator",
                 "func": {
                     ".class": "FuncDef",
                     "abstract_status": 0,
                     "arg_kinds": [
                         1,
                         1,
+                        1,
                         1
                     ],
                     "arg_names": [
                         "directory",
                         "ignore_uninstalled",
-                        "coverage"
+                        "coverage",
+                        "badge"
                     ],
                     "dataclass_transform_spec": null,
                     "flags": [
                         "is_decorated"
                     ],
                     "fullname": "su6.cli.check_all",
                     "name": "check_all",
                     "type": {
                         ".class": "CallableType",
                         "arg_kinds": [
                             1,
                             1,
+                            1,
                             1
                         ],
                         "arg_names": [
                             "directory",
                             "ignore_uninstalled",
-                            "coverage"
+                            "coverage",
+                            "badge"
                         ],
                         "arg_types": [
                             {
                                 ".class": "UnionType",
                                 "items": [
                                     "builtins.str",
                                     {
@@ -533,14 +537,23 @@
                                 ".class": "UnionType",
                                 "items": [
                                     "builtins.float",
                                     {
                                         ".class": "NoneType"
                                     }
                                 ]
+                            },
+                            {
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.bool",
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
                             }
                         ],
                         "bound_args": [],
                         "def_extras": {
                             "first_arg": null
                         },
                         "fallback": "builtins.function",
@@ -1211,41 +1224,45 @@
                 "func": {
                     ".class": "FuncDef",
                     "abstract_status": 0,
                     "arg_kinds": [
                         1,
                         1,
                         1,
+                        1,
                         1
                     ],
                     "arg_names": [
                         "directory",
                         "html",
                         "json",
-                        "coverage"
+                        "coverage",
+                        "badge"
                     ],
                     "dataclass_transform_spec": null,
                     "flags": [
                         "is_decorated"
                     ],
                     "fullname": "su6.cli.pytest",
                     "name": "pytest",
                     "type": {
                         ".class": "CallableType",
                         "arg_kinds": [
                             1,
                             1,
                             1,
+                            1,
                             1
                         ],
                         "arg_names": [
                             "directory",
                             "html",
                             "json",
-                            "coverage"
+                            "coverage",
+                            "badge"
                         ],
                         "arg_types": [
                             {
                                 ".class": "UnionType",
                                 "items": [
                                     "builtins.str",
                                     {
@@ -1259,14 +1276,23 @@
                                 ".class": "UnionType",
                                 "items": [
                                     "builtins.int",
                                     {
                                         ".class": "NoneType"
                                     }
                                 ]
+                            },
+                            {
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.bool",
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
                             }
                         ],
                         "bound_args": [],
                         "def_extras": {
                             "first_arg": null
                         },
                         "fallback": "builtins.function",
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/cli.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6386243386243386%*

 * *Differences: {"'data_mtime'": '1685442320',*

 * * "'dep_lines'": '{insert: [(0, 12), (1, 1), (3, 4), (5, 7), (7, 9)], delete: [22, 21, 12, 11, 10, '*

 * *                '9, 8, 7, 6, 5, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 25), (6, 5), (7, 5), (8, 5)], delete: [22, 21, 13, 12, 11, 10, 9, '*

 * *                '8, 7, 6, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'typeguard._memo'), (1, '__future__'), (2, 'inspect'), (3, "*

 * *                   "'sys'), (4, 'importlib'), (5, 'types'), (7, 'weakref')], delete: [19, 18, 16, "*

 * *               […]*

```diff
@@ -1,87 +1,68 @@
 {
-    "data_mtime": 1685445422,
+    "data_mtime": 1685442320,
     "dep_lines": [
-        10,
-        2,
+        12,
+        1,
         3,
+        4,
         5,
+        7,
         8,
+        9,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        7,
-        6
+        1
     ],
     "dep_prios": [
+        25,
         5,
-        10,
         5,
         10,
         5,
         5,
+        5,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "su6.core",
+        "typeguard._memo",
+        "__future__",
+        "inspect",
+        "sys",
+        "importlib",
+        "types",
         "typing",
-        "json",
-        "typer",
-        "rich",
+        "weakref",
         "builtins",
         "_typeshed",
         "abc",
         "array",
-        "click",
-        "click.core",
         "ctypes",
-        "enum",
-        "io",
-        "json.decoder",
         "mmap",
-        "os",
         "pickle",
-        "typer.core",
-        "typer.main",
         "typing_extensions"
     ],
-    "hash": "702e6a40652b35f5307eedf9250bef99dbb3e12aaf016cc9805ecc84b34404c9",
-    "id": "su6.cli",
-    "ignore_all": false,
-    "interface_hash": "fe0d9920001eb52053a03f62c5c98c2c69d0f3a398683dd6ff413be8473b7630",
-    "mtime": 1685447056,
+    "hash": "c071fcd0a3f20eb32965a0e67916e3f8bdfd34979f6007b78a8226d492d83a37",
+    "id": "typeguard._utils",
+    "ignore_all": true,
+    "interface_hash": "12c1f4adc4b334d6746b506ec1ff5f8c5083ed8945561d9eb1ecee6271f6b6dd",
+    "mtime": 1685293613,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -115,16 +96,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/cli.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_utils.py",
     "plugin_data": null,
-    "size": 8464,
-    "suppressed": [
-        "plumbum.commands.processes",
-        "plumbum"
-    ],
+    "size": 5042,
+    "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/core.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6/core.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987552105837713%*

 * *Differences: {"'names'": "{'ApplicationState': {'node': {'metadata': {'dataclass': {'attributes': {0: {'line': "*

 * *            "428}, 1: {'line': 429}, 2: {'line': 430}, 3: {'line': 431}}}}}}, 'Config': {'node': "*

 * *            "{'metadata': {'dataclass': {'attributes': {0: {'line': 227}, 1: {'line': 228}, 2: "*

 * *            "{'line': 229}, 3: {'line': 230}, 4: {'line': 231}, insert: [(5, "*

 * *            "OrderedDict([('alias', None), ('column', 4), ('has_default', True), ('is_in_init', "*

 * *            "True), ('is_init_var', Fal […]*

```diff
@@ -37,39 +37,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 417,
+                                "line": 428,
                                 "name": "verbosity",
                                 "type": "su6.core.Verbosity"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 418,
+                                "line": 429,
                                 "name": "format",
                                 "type": "su6.core.Format"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 419,
+                                "line": 430,
                                 "name": "config_file",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.str",
                                         {
                                             ".class": "NoneType"
@@ -81,15 +81,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 420,
+                                "line": 431,
                                 "name": "config",
                                 "type": {
                                     ".class": "TypeAliasType",
                                     "args": [],
                                     "type_ref": "su6.core.MaybeConfig"
                                 }
                             }
@@ -536,39 +536,39 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 225,
+                                "line": 227,
                                 "name": "directory",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 226,
+                                "line": 228,
                                 "name": "pyproject",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 227,
+                                "line": 229,
                                 "name": "include",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         {
                                             ".class": "Instance",
                                             "args": [
@@ -586,15 +586,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 228,
+                                "line": 230,
                                 "name": "exclude",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         {
                                             ".class": "Instance",
                                             "args": [
@@ -612,25 +612,43 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": true,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 229,
+                                "line": 231,
                                 "name": "coverage",
                                 "type": {
                                     ".class": "UnionType",
                                     "items": [
                                         "builtins.float",
                                         {
                                             ".class": "NoneType"
                                         }
                                     ]
                                 }
+                            },
+                            {
+                                "alias": null,
+                                "column": 4,
+                                "has_default": true,
+                                "is_in_init": true,
+                                "is_init_var": false,
+                                "is_neither_frozen_nor_nonfrozen": false,
+                                "kw_only": false,
+                                "line": 232,
+                                "name": "badge",
+                                "type": {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        "builtins.bool",
+                                        "builtins.str"
+                                    ]
+                                }
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
                 },
                 "module_name": "su6.core",
@@ -681,45 +699,49 @@
                             "abstract_status": 0,
                             "arg_kinds": [
                                 0,
                                 1,
                                 1,
                                 1,
                                 1,
+                                1,
                                 1
                             ],
                             "arg_names": [
                                 "self",
                                 "directory",
                                 "pyproject",
                                 "include",
                                 "exclude",
-                                "coverage"
+                                "coverage",
+                                "badge"
                             ],
                             "dataclass_transform_spec": null,
                             "flags": [],
                             "fullname": "su6.core.Config.__init__",
                             "name": "__init__",
                             "type": {
                                 ".class": "CallableType",
                                 "arg_kinds": [
                                     0,
                                     1,
                                     1,
                                     1,
                                     1,
+                                    1,
                                     1
                                 ],
                                 "arg_names": [
                                     "self",
                                     "directory",
                                     "pyproject",
                                     "include",
                                     "exclude",
-                                    "coverage"
+                                    "coverage",
+                                    "badge"
                                 ],
                                 "arg_types": [
                                     "su6.core.Config",
                                     "builtins.str",
                                     "builtins.str",
                                     {
                                         ".class": "UnionType",
@@ -755,14 +777,21 @@
                                         ".class": "UnionType",
                                         "items": [
                                             "builtins.float",
                                             {
                                                 ".class": "NoneType"
                                             }
                                         ]
+                                    },
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.bool",
+                                            "builtins.str"
+                                        ]
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {},
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
@@ -813,14 +842,19 @@
                                         "fallback": "builtins.str",
                                         "value": "exclude"
                                     },
                                     {
                                         ".class": "LiteralType",
                                         "fallback": "builtins.str",
                                         "value": "coverage"
+                                    },
+                                    {
+                                        ".class": "LiteralType",
+                                        "fallback": "builtins.str",
+                                        "value": "badge"
                                     }
                                 ],
                                 "partial_fallback": {
                                     ".class": "Instance",
                                     "args": [
                                         {
                                             ".class": "AnyType",
@@ -831,14 +865,80 @@
                                     ],
                                     "type_ref": "builtins.tuple"
                                 }
                             }
                         },
                         "plugin_generated": true
                     },
+                    "__post_init__": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0
+                            ],
+                            "arg_names": [
+                                "self"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [],
+                            "fullname": "su6.core.Config.__post_init__",
+                            "name": "__post_init__",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "arg_types": [
+                                    "su6.core.Config"
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": "self"
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "__post_init__ of Config",
+                                "ret_type": {
+                                    ".class": "NoneType"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        }
+                    },
+                    "badge": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_initialized_in_class",
+                                "is_ready",
+                                "has_explicit_value"
+                            ],
+                            "fullname": "su6.core.Config.badge",
+                            "name": "badge",
+                            "type": {
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.bool",
+                                    "builtins.str"
+                                ]
+                            }
+                        }
+                    },
                     "coverage": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
@@ -1197,27 +1297,27 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 268,
+                                "line": 279,
                                 "name": "key",
                                 "type": "builtins.str"
                             },
                             {
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 269,
+                                "line": 280,
                                 "name": "value",
                                 "type": {
                                     ".class": "AnyType",
                                     "missing_import_name": null,
                                     "source_any": null,
                                     "type_of_any": 2
                                 }
@@ -1226,15 +1326,15 @@
                                 "alias": null,
                                 "column": 4,
                                 "has_default": false,
                                 "is_in_init": true,
                                 "is_init_var": false,
                                 "is_neither_frozen_nor_nonfrozen": false,
                                 "kw_only": false,
-                                "line": 270,
+                                "line": 281,
                                 "name": "expected_type",
                                 "type": "builtins.type"
                             }
                         ],
                         "frozen": false
                     },
                     "dataclass_tag": {}
@@ -1556,14 +1656,29 @@
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
             }
         },
+        "DEFAULT_BADGE": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready",
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "su6.core.DEFAULT_BADGE",
+                "name": "DEFAULT_BADGE",
+                "type": "builtins.str"
+            }
+        },
         "DEFAULT_FORMAT": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_inferred",
@@ -1860,15 +1975,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.MaybeConfig",
-                "line": 243,
+                "line": 254,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "su6.core.Config",
                         {
@@ -2057,15 +2172,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "su6.core.T_typelike",
-                "line": 245,
+                "line": 256,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.type",
                         "types.UnionType",
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6/core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/core.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7050671550671551%*

 * *Differences: {"'data_mtime'": '1685143739',*

 * * "'dep_lines'": '{insert: [(0, 1), (1, 2), (2, 3), (15, 6)], delete: [34, 23, 22, 21, 20, 19, 18, '*

 * *                '17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 3, 2, 0]}',*

 * * "'dep_prios'": '{delete: [24, 23, 22, 21, 20, 19, 18, 17, 14, 12, 11, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(13, 'types')], delete: [32, 31, 30, 29, 26, 25, 23, 22, 17, 15, 13, "*

 * *                   '12, 11, 9, 8, 7, 6, 4, 2, 0]}',*

 * * "'hash'": "'8b0663919c3c0dd90562c38fd1a1b39423b977de5 […]*

```diff
@@ -1,124 +1,67 @@
 {
-    "data_mtime": 1685446800,
+    "data_mtime": 1685143739,
     "dep_lines": [
-        16,
+        1,
+        2,
+        3,
         4,
-        5,
-        6,
         7,
-        8,
-        9,
-        10,
-        11,
-        12,
-        13,
-        14,
-        16,
-        17,
-        19,
-        20,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
-        1,
-        18
+        6
     ],
     "dep_prios": [
         10,
         10,
         10,
         10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        10,
-        5,
-        20,
-        10,
         5,
         5,
-        5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         5
     ],
     "dependencies": [
-        "black.files",
         "enum",
-        "functools",
         "inspect",
-        "json",
         "operator",
-        "os",
-        "sys",
-        "tomllib",
-        "types",
         "typing",
-        "dataclasses",
-        "black",
-        "typer",
         "rich",
-        "typeguard",
         "builtins",
-        "_collections_abc",
         "_operator",
         "_typeshed",
         "abc",
         "array",
-        "click",
-        "click.exceptions",
         "ctypes",
-        "io",
-        "json.encoder",
         "mmap",
         "pickle",
-        "typeguard._config",
-        "typeguard._exceptions",
-        "typeguard._functions",
-        "typeguard._memo",
+        "types",
         "typing_extensions"
     ],
-    "hash": "481309ccc1dae6529421b42d111f8620fbe21de14a7e95af0bcf8de5714f2a63",
-    "id": "su6.core",
+    "hash": "8b0663919c3c0dd90562c38fd1a1b39423b977de58b0bb1c6a616024d4d115d5",
+    "id": "su6_checker.core",
     "ignore_all": false,
-    "interface_hash": "aa2a020ff4c5a2eb73b8cb7b93765b206e3689db50ce1624db4fb9578736a8e2",
-    "mtime": 1685447056,
+    "interface_hash": "b0b2dfd0a37866e3640371d6d066f122b1a7cc5ee332534e093bf5707d163a85",
+    "mtime": 1685144281,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -146,21 +89,21 @@
         "implicit_reexport": false,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
         "strict_concatenate": true,
         "strict_equality": true,
-        "strict_optional": true,
+        "strict_optional": false,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/su6/core.py",
+    "path": "./src/su6_checker/core.py",
     "plugin_data": null,
-    "size": 15269,
+    "size": 2823,
     "suppressed": [
         "plumbum.machines"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/__about__.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/__about__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/cli.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/cli.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/core.data.json` & `su6-0.7.0/.mypy_cache/3.11/su6_checker/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/su6_checker/core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.681059829059829%*

 * *Differences: {"'data_mtime'": '1685449110',*

 * * "'dep_lines'": '{insert: [(0, 10), (3, 5), (4, 8), (5, 1), (6, 1), (7, 1), (8, 1), (9, 1), (10, '*

 * *                '1), (21, 7)], delete: [4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 5), (6, 30), (7, 30), (8, 30), (9, 30), (10, 30), (11, 30), '*

 * *                '(21, 5)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'su6.core'), (2, 'json'), (3, 'typer'), (9, 'click'), (10, "*

 * *                   "'click.core'), (12, 'enum'), (13, 'io'), (14, 'json.decoder'), (16, ' […]*

```diff
@@ -1,67 +1,87 @@
 {
-    "data_mtime": 1685143739,
+    "data_mtime": 1685449110,
     "dep_lines": [
-        1,
+        10,
         2,
         3,
-        4,
-        7,
+        5,
+        8,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
+        1,
+        1,
+        1,
+        7,
         6
     ],
     "dep_prios": [
+        5,
         10,
-        10,
-        10,
+        5,
         10,
         5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        30,
+        5,
         5
     ],
     "dependencies": [
-        "enum",
-        "inspect",
-        "operator",
+        "su6.core",
         "typing",
+        "json",
+        "typer",
         "rich",
         "builtins",
-        "_operator",
         "_typeshed",
         "abc",
         "array",
+        "click",
+        "click.core",
         "ctypes",
+        "enum",
+        "io",
+        "json.decoder",
         "mmap",
+        "os",
         "pickle",
-        "types",
+        "typer.core",
+        "typer.main",
         "typing_extensions"
     ],
-    "hash": "8b0663919c3c0dd90562c38fd1a1b39423b977de58b0bb1c6a616024d4d115d5",
-    "id": "su6_checker.core",
+    "hash": "2799be1bd89096cb7d42c66973a3f4b5565f689ea14cbca319c500506f36bf46",
+    "id": "su6.cli",
     "ignore_all": false,
-    "interface_hash": "b0b2dfd0a37866e3640371d6d066f122b1a7cc5ee332534e093bf5707d163a85",
-    "mtime": 1685144281,
+    "interface_hash": "25902cf8957e60f5abd6ae433a6d809cd70c1565187ebdc6948a58791dac9031",
+    "mtime": 1685449107,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -89,21 +109,22 @@
         "implicit_reexport": false,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
         "strict_concatenate": true,
         "strict_equality": true,
-        "strict_optional": false,
+        "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "./src/su6_checker/core.py",
+    "path": "src/su6/cli.py",
     "plugin_data": null,
-    "size": 2823,
+    "size": 9006,
     "suppressed": [
-        "plumbum.machines"
+        "plumbum.commands.processes",
+        "plumbum"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/tests/examples.data.json` & `su6-0.7.0/.mypy_cache/3.11/tests/examples.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tests/examples.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tests/examples.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tests/examples/good.data.json` & `su6-0.7.0/.mypy_cache/3.11/tests/examples/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/tests/examples/good.meta.json` & `su6-0.7.0/.mypy_cache/3.11/tests/examples/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_config.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7166271929824561%*

 * *Differences: {"'data_mtime'": '1685442323',*

 * * "'dep_lines'": '{insert: [(3, 2), (4, 3), (5, 5)], delete: [7, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [9, 4, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._typing'), (1, 'typer.models'), (3, 'copy'), (5, "*

 * *                   "'typing_extensions'), (8, 'click'), (9, 'click.core'), (10, "*

 * *                   "'click.shell_completion'), (11, 'click.types'), (12, 'types')], delete: [15, "*

 * *                   '14, 13, 12, 11, 9, 7, 5, 4, 3, 1, 0]}',*

 * * "'hash'": "'2eac497a8186c3 […]*

```diff
@@ -1,68 +1,59 @@
 {
-    "data_mtime": 1685442320,
+    "data_mtime": 1685442323,
     "dep_lines": [
-        12,
-        1,
-        3,
-        4,
-        5,
         7,
         8,
-        9,
         1,
+        2,
+        3,
+        5,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        25,
         5,
         5,
         10,
         5,
         5,
         5,
         5,
-        5,
-        30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "typeguard._memo",
-        "__future__",
+        "typer._typing",
+        "typer.models",
         "inspect",
-        "sys",
-        "importlib",
-        "types",
+        "copy",
         "typing",
-        "weakref",
+        "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
-        "typing_extensions"
+        "click",
+        "click.core",
+        "click.shell_completion",
+        "click.types",
+        "types"
     ],
-    "hash": "c071fcd0a3f20eb32965a0e67916e3f8bdfd34979f6007b78a8226d492d83a37",
-    "id": "typeguard._utils",
+    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
+    "id": "typer.utils",
     "ignore_all": true,
-    "interface_hash": "12c1f4adc4b334d6746b506ec1ff5f8c5083ed8945561d9eb1ecee6271f6b6dd",
-    "mtime": 1685293613,
+    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
+    "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -96,13 +87,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typeguard/_utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
     "plugin_data": null,
-    "size": 5042,
+    "size": 7293,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_typing.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/colors.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/colors.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/completion.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/completion.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/core.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/core.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/main.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/main.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/models.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/models.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/params.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/params.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/utils.data.json` & `su6-0.7.0/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/typer/utils.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.726135265700483%*

 * *Differences: {"'data_mtime'": '1685442320',*

 * * "'dep_lines'": '{insert: [(2, 31), (4, 2), (5, 3), (6, 4), (7, 6), (8, 7), (9, 8), (10, 9), (11, '*

 * *                '10), (12, 11)], delete: [9, 8, 7, 6, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (3, 10), (5, 20), (10, 5), (11, 5), (12, 5), (13, 5)], delete: '*

 * *                '[11, 10, 9, 8, 7]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.result'), (1, 'collections.abc'), (2, "*

 * *                   "'unittest._log'), (3, 'logging'), (4, 'sys'), (5, 'unittest'), (6, "*

 * * […]*

```diff
@@ -1,58 +1,64 @@
 {
-    "data_mtime": 1685442323,
+    "data_mtime": 1685442320,
     "dep_lines": [
-        7,
-        8,
-        1,
-        2,
         3,
         5,
+        31,
         1,
-        1,
-        1,
-        1,
-        1,
+        2,
+        3,
+        4,
+        6,
+        7,
+        8,
+        9,
+        10,
+        11,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
         5,
         10,
+        10,
+        20,
+        5,
+        5,
+        5,
+        5,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "typer._typing",
-        "typer.models",
-        "inspect",
-        "copy",
+        "unittest.result",
+        "collections.abc",
+        "unittest._log",
+        "logging",
+        "sys",
+        "unittest",
+        "_typeshed",
+        "contextlib",
+        "re",
+        "types",
         "typing",
         "typing_extensions",
+        "warnings",
         "builtins",
-        "abc",
-        "click",
-        "click.core",
-        "click.shell_completion",
-        "click.types",
-        "types"
+        "abc"
     ],
-    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
-    "id": "typer.utils",
+    "hash": "2e896b10930c0bd8849a3e6b4c584e7eba9265f85efeffa0ba24a2e732a8967b",
+    "id": "unittest.case",
     "ignore_all": true,
-    "interface_hash": "a2a85c807b26672ed4a26c19c9b4e841141ca67ec475f5c25733d86efba2979d",
+    "interface_hash": "6211186fbeefd54fdb8566dd5541d7ca569758703d677367662f6b6bc3b59b68",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +93,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/typer/utils.py",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/case.pyi",
     "plugin_data": null,
-    "size": 7293,
+    "size": 13905,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/_log.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/_log.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/async_case.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/case.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/case.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7686274509803922%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 1), (5, 1)], delete: [12, 11, 10, 9, 8, 7, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 20), (6, 30)], delete: [10, 9, 8, 7, 6, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'unittest.case'), (7, 'typing')], delete: [12, 10, 9, 8, 7, 6, "*

 * *                   '4, 3, 2]}',*

 * * "'hash'": "'82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e'",*

 * * "'id'": "'unittest.suite'",*

 * * "'interface_hash'": "'986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4'",*

 * * "'path' […]*

```diff
@@ -1,64 +1,43 @@
 {
     "data_mtime": 1685442320,
     "dep_lines": [
-        3,
-        5,
-        31,
         1,
         2,
         3,
+        1,
         4,
-        6,
-        7,
-        8,
-        9,
-        10,
-        11,
+        1,
         1,
         1
     ],
     "dep_prios": [
         10,
-        5,
-        5,
-        10,
         10,
-        20,
-        5,
-        5,
-        5,
-        5,
-        5,
         5,
+        20,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
+        "unittest.case",
         "unittest.result",
         "collections.abc",
-        "unittest._log",
-        "logging",
-        "sys",
         "unittest",
-        "_typeshed",
-        "contextlib",
-        "re",
-        "types",
-        "typing",
         "typing_extensions",
-        "warnings",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "2e896b10930c0bd8849a3e6b4c584e7eba9265f85efeffa0ba24a2e732a8967b",
-    "id": "unittest.case",
+    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
+    "id": "unittest.suite",
     "ignore_all": true,
-    "interface_hash": "6211186fbeefd54fdb8566dd5541d7ca569758703d677367662f6b6bc3b59b68",
+    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -93,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/case.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
     "plugin_data": null,
-    "size": 13905,
+    "size": 983,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/loader.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/loader.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/main.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/main.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/mock.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/mock.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/result.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/result.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/runner.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/runner.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/signals.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/signals.meta.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/suite.data.json` & `su6-0.7.0/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/unittest/suite.meta.json` & `su6-0.7.0/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7511111111111111%*

 * *Differences: {"'data_mtime'": '1685442319',*

 * * "'dep_lines'": '{insert: [(2, 3), (4, 7)], delete: [2, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (3, 5)], delete: [3, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'sys'), (2, 'typing'), (4, 'types'), (6, '_typeshed')], delete: "*

 * *                   '[7, 3, 1, 0]}',*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706'",*

 * * "'path'": "'/home/rob […]*

```diff
@@ -1,43 +1,43 @@
 {
-    "data_mtime": 1685442320,
+    "data_mtime": 1685442319,
     "dep_lines": [
-        1,
         2,
-        3,
         1,
+        3,
         4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
-        10,
         5,
-        20,
+        5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "unittest.case",
-        "unittest.result",
         "collections.abc",
-        "unittest",
+        "sys",
+        "typing",
         "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "82ef3fccdbec8d741246f3120bba6b1b44590b298724c431d3de8120f37dd54e",
-    "id": "unittest.suite",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "986949f52fd6afd046d366c86e8a87ac2d0a1185874e4b7711635b5ca43cb4a4",
+    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -72,13 +72,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 983,
+    "size": 6532,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-0.7.0/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-0.7.0/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/urllib/parse.data.json` & `su6-0.7.0/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7363442113442115%*

 * *Differences: {"'data_mtime'": '1685433917',*

 * * "'dep_lines'": '{insert: [(0, 7), (2, 2), (5, 5), (6, 6), (7, 36)], delete: [6, 5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (8, 5)], delete: [7, 6]}',*

 * * "'dependencies'": "{insert: [(1, 'abc'), (2, 'collections'), (5, '_collections_abc'), (6, "*

 * *                   "'_typeshed')], delete: [7, 6, 3]}",*

 * * "'hash'": "'44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65a04119'",*

 * * "'id'": "'typing_extensions'",*

 * * "'interface_hash'": "'97a64b9296f7cd7e33606259f5b17e6 […]*

```diff
@@ -1,84 +1,87 @@
 {
-    "data_mtime": 1685442319,
+    "data_mtime": 1685433917,
     "dep_lines": [
-        2,
+        7,
         1,
+        2,
         3,
         4,
-        7,
-        1,
-        1,
+        5,
+        6,
+        36,
         1
     ],
     "dep_prios": [
         5,
         10,
+        10,
+        10,
         5,
         5,
         5,
         5,
-        30,
-        30
+        5
     ],
     "dependencies": [
         "collections.abc",
+        "abc",
+        "collections",
         "sys",
         "typing",
-        "typing_extensions",
-        "types",
-        "builtins",
+        "_collections_abc",
         "_typeshed",
-        "abc"
+        "types",
+        "builtins"
     ],
-    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
-    "id": "urllib.parse",
+    "hash": "44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65a04119",
+    "id": "typing_extensions",
     "ignore_all": true,
-    "interface_hash": "02fb690cfa1baa81d991e1e0cbefb99675f9ad2e7f882a3fee24c774bfcd0706",
+    "interface_hash": "97a64b9296f7cd7e33606259f5b17e600995b040b31b5c94570b5369924712e9",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
-        "check_untyped_defs": true,
+        "check_untyped_defs": false,
         "disable_bytearray_promotion": false,
         "disable_error_code": [],
         "disable_memoryview_promotion": false,
         "disabled_error_codes": [],
         "disallow_any_decorated": false,
         "disallow_any_explicit": false,
         "disallow_any_expr": false,
-        "disallow_any_generics": true,
+        "disallow_any_generics": false,
         "disallow_any_unimported": false,
-        "disallow_incomplete_defs": true,
-        "disallow_subclassing_any": true,
-        "disallow_untyped_calls": true,
-        "disallow_untyped_decorators": true,
-        "disallow_untyped_defs": true,
+        "disallow_incomplete_defs": false,
+        "disallow_subclassing_any": false,
+        "disallow_untyped_calls": false,
+        "disallow_untyped_decorators": false,
+        "disallow_untyped_defs": false,
         "enable_error_code": [],
         "enabled_error_codes": [],
         "follow_imports": "normal",
         "follow_imports_for_stubs": false,
         "ignore_errors": false,
-        "ignore_missing_imports": true,
-        "implicit_optional": true,
-        "implicit_reexport": false,
+        "ignore_missing_imports": false,
+        "implicit_optional": false,
+        "implicit_reexport": true,
         "local_partial_types": false,
         "mypyc": false,
         "platform": "linux",
         "plugins": [],
-        "strict_concatenate": true,
-        "strict_equality": true,
+        "strict_concatenate": false,
+        "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
-        "warn_return_any": true,
+        "warn_return_any": false,
         "warn_unreachable": false,
-        "warn_unused_ignores": true
+        "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi",
     "plugin_data": null,
-    "size": 6532,
+    "size": 9843,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/.pytest_cache/v/cache/nodeids` & `su6-0.7.0/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-0.7.0/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/2bf27b960bc3ded1` & `su6-0.7.0/.ruff_cache/content/2bf27b960bc3ded1`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/3f10d9d7687f3999` & `su6-0.7.0/.ruff_cache/content/3f10d9d7687f3999`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/684d0841c18787fb` & `su6-0.7.0/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/68c4553df91c1f5e` & `su6-0.7.0/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/881c84062ed51136` & `su6-0.7.0/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/b8d965aa2b8fd993` & `su6-0.7.0/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/b990e7d90d89db2a` & `su6-0.7.0/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/be4a1815dbb4c4` & `su6-0.7.0/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/e067c98663409f12` & `su6-0.7.0/.ruff_cache/content/e067c98663409f12`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/.ruff_cache/content/ed03e948b89996b8` & `su6-0.7.0/.ruff_cache/content/ed03e948b89996b8`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/coverage_html.js` & `su6-0.7.0/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_2602a302b50854cf___about___py.html` & `su6-0.7.0/htmlcov/d_2602a302b50854cf___about___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_2602a302b50854cf___init___py.html` & `su6-0.7.0/htmlcov/d_2602a302b50854cf___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_2602a302b50854cf_cli_py.html` & `su6-0.7.0/htmlcov/d_2602a302b50854cf_cli_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">97 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">97<span class="text"> run</span></button>
+            <span class="text">100 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">100<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">32<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">41<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2602a302b50854cf___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2602a302b50854cf_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:45 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -77,326 +77,350 @@
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""This file contains all Typer Commands."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">json</span> <span class="key">import</span> <span class="nam">load</span> <span class="key">as</span> <span class="nam">json_load</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">plumbum</span> <span class="key">import</span> <span class="nam">local</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">plumbum</span><span class="op">.</span><span class="nam">commands</span><span class="op">.</span><span class="nam">processes</span> <span class="key">import</span> <span class="nam">CommandNotFound</span><span class="op">,</span> <span class="nam">ProcessExecutionError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span> <span class="key">import</span> <span class="nam">print</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="nam">DEFAULT_FORMAT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">EXIT_CODE_ERROR</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">EXIT_CODE_SUCCESS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">GREEN_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">RED_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">YELLOW_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">Format</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">Verbosity</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">dump_tools_with_results</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">info</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">log_cmd_output</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">log_command</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">state</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">warn</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">with_exit_code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="nam">app</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">contextlib</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">math</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">json</span> <span class="key">import</span> <span class="nam">load</span> <span class="key">as</span> <span class="nam">json_load</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">typer</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">plumbum</span> <span class="key">import</span> <span class="nam">local</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">plumbum</span><span class="op">.</span><span class="nam">commands</span><span class="op">.</span><span class="nam">processes</span> <span class="key">import</span> <span class="nam">CommandNotFound</span><span class="op">,</span> <span class="nam">ProcessExecutionError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">rich</span> <span class="key">import</span> <span class="nam">print</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">core</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="nam">DEFAULT_FORMAT</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">EXIT_CODE_ERROR</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">EXIT_CODE_SUCCESS</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">GREEN_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">RED_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">YELLOW_CIRCLE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">Format</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">Verbosity</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">dump_tools_with_results</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">info</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">log_cmd_output</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">log_command</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">state</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">warn</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="nam">with_exit_code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="nam">tool</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    Abstraction to run one of the cli checking tools and process its output.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">        tool: the (bash) name of the tool to run.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        args: cli args to pass to the cli bash tool</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">local</span><span class="op">[</span><span class="nam">tool</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">>=</span> <span class="num">3</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">log_command</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="nam">app</span> <span class="op">=</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Typer</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t"><span class="key">def</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="nam">tool</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="str">    Abstraction to run one of the cli checking tools and process its output.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        tool: the (bash) name of the tool to run.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        args: cli args to pass to the cli bash tool</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="nam">cmd</span> <span class="op">=</span> <span class="nam">local</span><span class="op">[</span><span class="nam">tool</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">cmd</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">GREEN_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">>=</span> <span class="num">3</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">log_command</span><span class="op">(</span><span class="nam">cmd</span><span class="op">,</span> <span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">cmd</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">GREEN_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_SUCCESS</span>  <span class="com"># success</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="key">except</span> <span class="nam">CommandNotFound</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">warn</span><span class="op">(</span><span class="str">f"Tool {tool} not installed!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">YELLOW_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_SUCCESS</span>  <span class="com"># success</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">except</span> <span class="nam">CommandNotFound</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="nam">warn</span><span class="op">(</span><span class="str">f"Tool {tool} not installed!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span>  <span class="com"># command not found</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">except</span> <span class="nam">ProcessExecutionError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">RED_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">e</span><span class="op">.</span><span class="nam">stdout</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_ERROR</span>  <span class="com"># general error</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="com"># 'directory' is an optional cli argument to many commands, so we define the type here for reuse:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="nam">T_directory</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Annotated</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>  <span class="com"># = "."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">YELLOW_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span>  <span class="com"># command not found</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">except</span> <span class="nam">ProcessExecutionError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">RED_CIRCLE</span><span class="op">,</span> <span class="nam">tool</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">            <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">e</span><span class="op">.</span><span class="nam">stdout</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">return</span> <span class="nam">EXIT_CODE_ERROR</span>  <span class="com"># general error</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="key">def</span> <span class="nam">ruff</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">    Runs the Ruff Linter.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="str">        directory: where to run ruff on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="com"># 'directory' is an optional cli argument to many commands, so we define the type here for reuse:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="nam">T_directory</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Annotated</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typer</span><span class="op">.</span><span class="nam">Argument</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>  <span class="com"># = "."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="key">def</span> <span class="nam">ruff</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="str">    Runs the Ruff Linter.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"ruff"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="key">def</span> <span class="nam">black</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">fix</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">    Runs the Black code formatter.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">        directory: where to run black on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">        fix: if --fix is passed, black will be used to reformat the file(s).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">        directory: where to run ruff on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"ruff"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="key">def</span> <span class="nam">black</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">fix</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">    Runs the Black code formatter.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="str">        directory: where to run black on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">        fix: if --fix is passed, black will be used to reformat the file(s).</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">,</span> <span class="str">r"--exclude=venv.+|.+\.bak"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">fix</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="key">elif</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="nam">info</span><span class="op">(</span><span class="str">"note: running WITHOUT --check -> changing files"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"black"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">,</span> <span class="str">r"--exclude=venv.+|.+\.bak"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">fix</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--check"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="key">elif</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="nam">info</span><span class="op">(</span><span class="str">"note: running WITHOUT --check -> changing files"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="key">def</span> <span class="nam">isort</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">fix</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="str">    Runs the import sort (isort) utility.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">        directory: where to run isort on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="str">        fix: if --fix is passed, isort will be used to rearrange imports.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">fix</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--check-only"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">    <span class="key">elif</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">info</span><span class="op">(</span><span class="str">"note: running WITHOUT --check -> changing files"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"isort"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"black"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="key">def</span> <span class="nam">isort</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">fix</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">    Runs the import sort (isort) utility.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t"><span class="str">        directory: where to run isort on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t"><span class="str">        fix: if --fix is passed, isort will be used to rearrange imports.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">fix</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="str">"--check-only"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">    <span class="key">elif</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="nam">info</span><span class="op">(</span><span class="str">"note: running WITHOUT --check -> changing files"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t"><span class="key">def</span> <span class="nam">mypy</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="str">    Runs the mypy static type checker.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">        directory: where to run mypy on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"isort"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="key">def</span> <span class="nam">mypy</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">    Runs the mypy static type checker.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"mypy"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t"><span class="key">def</span> <span class="nam">bandit</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">    Runs the bandit security checker.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">        directory: where to run bandit on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="str">        directory: where to run mypy on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"mypy"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="key">def</span> <span class="nam">bandit</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t"><span class="str">    Runs the bandit security checker.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"bandit"</span><span class="op">,</span> <span class="str">"-r"</span><span class="op">,</span> <span class="str">"-c"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">pyproject</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t"><span class="key">def</span> <span class="nam">pydocstyle</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="str">    Runs the pydocstyle docstring checker.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t"><span class="str">        directory: where to run pydocstyle on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t"><span class="str">        directory: where to run bandit on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"bandit"</span><span class="op">,</span> <span class="str">"-r"</span><span class="op">,</span> <span class="str">"-c"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">pyproject</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t"><span class="key">def</span> <span class="nam">pydocstyle</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t"><span class="str">    Runs the pydocstyle docstring checker.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"pydocstyle"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="key">def</span> <span class="nam">pytest</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">html</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="nam">json</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="nam">coverage</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t"><span class="str">    Runs all pytests.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">        directory: where to run pytests on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="str">        html: generate HTML coverage output?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="str">        json: generate JSON coverage output?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t"><span class="str">        coverage: threshold for coverage (in %)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">        > su6 pytest --coverage 50</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">        if any checks fail: exit 1 and red circle</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">        if all checks pass but coverage is less than 50%: exit 1, green circle for pytest and red for coverage</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">        if all check pass and coverage is at least 50%: exit 0, green circle for pytest and green for coverage</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="str">        if --coverage is not passed, there will be no circle for coverage.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">,</span> <span class="nam">coverage</span><span class="op">=</span><span class="nam">coverage</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="str">"--cov"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="com"># json output required!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="nam">json</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="key">if</span> <span class="nam">html</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--cov-report"</span><span class="op">,</span> <span class="str">"html"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="key">if</span> <span class="nam">json</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--cov-report"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="str">        directory: where to run pydocstyle on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="key">return</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"pydocstyle"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="key">def</span> <span class="nam">pytest</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">    <span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">    <span class="nam">html</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="nam">json</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">    <span class="nam">coverage</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">    <span class="nam">badge</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="str">    Runs all pytests.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t"><span class="str">        directory: where to run pytests on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">        html: generate HTML coverage output?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">        json: generate JSON coverage output?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t"><span class="str">        coverage: threshold for coverage (in %)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="str">        badge: generate coverage badge (svg)? If you want to change the name, do this in pyproject.toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="str">        > su6 pytest --coverage 50</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">        if any checks fail: exit 1 and red circle</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t"><span class="str">        if all checks pass but coverage is less than 50%: exit 1, green circle for pytest and red for coverage</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t"><span class="str">        if all check pass and coverage is at least 50%: exit 0, green circle for pytest and green for coverage</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t"><span class="str">        if --coverage is not passed, there will be no circle for coverage.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">,</span> <span class="nam">coverage</span><span class="op">=</span><span class="nam">coverage</span><span class="op">,</span> <span class="nam">badge</span><span class="op">=</span><span class="nam">badge</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">badge</span> <span class="key">and</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">        <span class="com"># not None but still check cov</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">        <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"pytest"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="str">"--cov"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="str">"coverage.json"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">json_load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">            <span class="nam">percent_covered</span> <span class="op">=</span> <span class="nam">round</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="str">"totals"</span><span class="op">]</span><span class="op">[</span><span class="str">"percent_covered"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="com"># if actual coverage is less than the the threshold, exit code should be success (0)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">percent_covered</span> <span class="op">&lt;</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">circle</span> <span class="op">=</span> <span class="nam">RED_CIRCLE</span> <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">else</span> <span class="nam">GREEN_CIRCLE</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">circle</span><span class="op">,</span> <span class="str">"coverage"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="key">return</span> <span class="nam">exit_code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"all"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="key">def</span> <span class="nam">check_all</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="nam">coverage</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    Run all available checks.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">        directory: where to run the tools on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command not found)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">        coverage: pass to pytest()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">    <span class="nam">ignored_exit_codes</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">if</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="nam">ignored_exit_codes</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="com"># json output required!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">        <span class="nam">json</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="key">if</span> <span class="nam">html</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--cov-report"</span><span class="op">,</span> <span class="str">"html"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="key">if</span> <span class="nam">json</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">args</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="op">[</span><span class="str">"--cov-report"</span><span class="op">,</span> <span class="str">"json"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">_check_tool</span><span class="op">(</span><span class="str">"pytest"</span><span class="op">,</span> <span class="op">*</span><span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="str">"coverage.json"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">            <span class="nam">data</span> <span class="op">=</span> <span class="nam">json_load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="nam">percent_covered</span> <span class="op">=</span> <span class="nam">math</span><span class="op">.</span><span class="nam">floor</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="str">"totals"</span><span class="op">]</span><span class="op">[</span><span class="str">"percent_covered"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="com"># if actual coverage is less than the the threshold, exit code should be success (0)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="nam">exit_code</span> <span class="op">=</span> <span class="nam">percent_covered</span> <span class="op">&lt;</span> <span class="nam">config</span><span class="op">.</span><span class="nam">coverage</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">        <span class="nam">circle</span> <span class="op">=</span> <span class="nam">RED_CIRCLE</span> <span class="key">if</span> <span class="nam">exit_code</span> <span class="key">else</span> <span class="nam">GREEN_CIRCLE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"text"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">circle</span><span class="op">,</span> <span class="str">"coverage"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="key">if</span> <span class="nam">config</span><span class="op">.</span><span class="nam">badge</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">            <span class="key">with</span> <span class="nam">contextlib</span><span class="op">.</span><span class="nam">suppress</span><span class="op">(</span><span class="nam">FileNotFoundError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">                <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">config</span><span class="op">.</span><span class="nam">badge</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">            <span class="nam">result</span> <span class="op">=</span> <span class="nam">local</span><span class="op">[</span><span class="str">"coverage-badge"</span><span class="op">]</span><span class="op">(</span><span class="str">"-o"</span><span class="op">,</span> <span class="nam">config</span><span class="op">.</span><span class="nam">badge</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="nam">tools</span> <span class="op">=</span> <span class="nam">config</span><span class="op">.</span><span class="nam">determine_which_to_run</span><span class="op">(</span><span class="op">[</span><span class="nam">ruff</span><span class="op">,</span> <span class="nam">black</span><span class="op">,</span> <span class="nam">mypy</span><span class="op">,</span> <span class="nam">bandit</span><span class="op">,</span> <span class="nam">isort</span><span class="op">,</span> <span class="nam">pydocstyle</span><span class="op">,</span> <span class="nam">pytest</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">    <span class="key">return</span> <span class="nam">exit_code</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="nam">exit_codes</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">    <span class="key">for</span> <span class="nam">tool</span> <span class="key">in</span> <span class="nam">tools</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">        <span class="nam">a</span> <span class="op">=</span> <span class="op">[</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">_suppress</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_ignore</span><span class="op">=</span><span class="nam">ignored_exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="key">if</span> <span class="nam">tool</span> <span class="key">is</span> <span class="nam">pytest</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">            <span class="nam">kw</span><span class="op">[</span><span class="str">"coverage"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">coverage</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="nam">exit_codes</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">tool</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"json"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="nam">dump_tools_with_results</span><span class="op">(</span><span class="nam">tools</span><span class="op">,</span> <span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span><span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"all"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="key">def</span> <span class="nam">check_all</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">    <span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span> <span class="nam">coverage</span><span class="op">:</span> <span class="nam">float</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">badge</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">    Run all available checks.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">        directory: where to run the tools on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command not found)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">        coverage: pass to pytest()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">        badge: pass to pytest()</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"fix"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="key">def</span> <span class="nam">do_fix</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="str">    Do everything that's safe to fix (so not ruff because that may break semantics).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">        directory: where to run the tools on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command not found)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="nam">ignored_exit_codes</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="key">if</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">        <span class="nam">ignored_exit_codes</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">tools</span> <span class="op">=</span> <span class="nam">config</span><span class="op">.</span><span class="nam">determine_which_to_run</span><span class="op">(</span><span class="op">[</span><span class="nam">black</span><span class="op">,</span> <span class="nam">isort</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="nam">exit_codes</span> <span class="op">=</span> <span class="op">[</span><span class="nam">tool</span><span class="op">(</span><span class="nam">directory</span><span class="op">,</span> <span class="nam">fix</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_suppress</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_ignore</span><span class="op">=</span><span class="nam">ignored_exit_codes</span><span class="op">)</span> <span class="key">for</span> <span class="nam">tool</span> <span class="key">in</span> <span class="nam">tools</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="nam">ignored_exit_codes</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">    <span class="key">if</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">        <span class="nam">ignored_exit_codes</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">tools</span> <span class="op">=</span> <span class="nam">config</span><span class="op">.</span><span class="nam">determine_which_to_run</span><span class="op">(</span><span class="op">[</span><span class="nam">ruff</span><span class="op">,</span> <span class="nam">black</span><span class="op">,</span> <span class="nam">mypy</span><span class="op">,</span> <span class="nam">bandit</span><span class="op">,</span> <span class="nam">isort</span><span class="op">,</span> <span class="nam">pydocstyle</span><span class="op">,</span> <span class="nam">pytest</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="nam">exit_codes</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="key">for</span> <span class="nam">tool</span> <span class="key">in</span> <span class="nam">tools</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="nam">a</span> <span class="op">=</span> <span class="op">[</span><span class="nam">directory</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span><span class="nam">_suppress</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_ignore</span><span class="op">=</span><span class="nam">ignored_exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">        <span class="key">if</span> <span class="nam">tool</span> <span class="key">is</span> <span class="nam">pytest</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">            <span class="nam">kw</span><span class="op">[</span><span class="str">"coverage"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">coverage</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">            <span class="nam">kw</span><span class="op">[</span><span class="str">"badge"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">badge</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="nam">exit_codes</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">tool</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"json"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">        <span class="nam">dump_tools_with_results</span><span class="op">(</span><span class="nam">tools</span><span class="op">,</span> <span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"json"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">dump_tools_with_results</span><span class="op">(</span><span class="nam">tools</span><span class="op">,</span> <span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span><span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span><span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">callback</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="nam">config</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span> <span class="nam">format</span><span class="op">:</span> <span class="nam">Format</span> <span class="op">=</span> <span class="nam">DEFAULT_FORMAT</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    This callback will run before every command, setting the right global flags.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t"><span class="str">        config: path to a different config toml file</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="str">        verbosity: level of detail to print out (1 - 3)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t"><span class="str">        format: output format</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">command</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="str">"fix"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="op">@</span><span class="nam">with_exit_code</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t"><span class="key">def</span> <span class="nam">do_fix</span><span class="op">(</span><span class="nam">directory</span><span class="op">:</span> <span class="nam">T_directory</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">False</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="str">    Do everything that's safe to fix (so not ruff because that may break semantics).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t"><span class="str">        directory: where to run the tools on (default is current dir)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">        ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command not found)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="nam">config</span> <span class="op">=</span> <span class="nam">state</span><span class="op">.</span><span class="nam">update_config</span><span class="op">(</span><span class="nam">directory</span><span class="op">=</span><span class="nam">directory</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="nam">state</span><span class="op">.</span><span class="nam">load_config</span><span class="op">(</span><span class="nam">config_file</span><span class="op">=</span><span class="nam">config</span><span class="op">,</span> <span class="nam">verbosity</span><span class="op">=</span><span class="nam">verbosity</span><span class="op">,</span> <span class="nam">format</span><span class="op">=</span><span class="nam">format</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="nam">ignored_exit_codes</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="key">if</span> <span class="nam">ignore_uninstalled</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">        <span class="nam">ignored_exit_codes</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">EXIT_CODE_COMMAND_NOT_FOUND</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="nam">app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">    <span class="nam">tools</span> <span class="op">=</span> <span class="nam">config</span><span class="op">.</span><span class="nam">determine_which_to_run</span><span class="op">(</span><span class="op">[</span><span class="nam">black</span><span class="op">,</span> <span class="nam">isort</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">    <span class="nam">exit_codes</span> <span class="op">=</span> <span class="op">[</span><span class="nam">tool</span><span class="op">(</span><span class="nam">directory</span><span class="op">,</span> <span class="nam">fix</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_suppress</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">_ignore</span><span class="op">=</span><span class="nam">ignored_exit_codes</span><span class="op">)</span> <span class="key">for</span> <span class="nam">tool</span> <span class="key">in</span> <span class="nam">tools</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="key">if</span> <span class="nam">state</span><span class="op">.</span><span class="nam">format</span> <span class="op">==</span> <span class="str">"json"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">        <span class="nam">dump_tools_with_results</span><span class="op">(</span><span class="nam">tools</span><span class="op">,</span> <span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="key">return</span> <span class="nam">any</span><span class="op">(</span><span class="nam">exit_codes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t"><span class="op">@</span><span class="nam">app</span><span class="op">.</span><span class="nam">callback</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="nam">config</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span> <span class="nam">format</span><span class="op">:</span> <span class="nam">Format</span> <span class="op">=</span> <span class="nam">DEFAULT_FORMAT</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t"><span class="str">    This callback will run before every command, setting the right global flags.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">        config: path to a different config toml file</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">        verbosity: level of detail to print out (1 - 3)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">        format: output format</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="nam">state</span><span class="op">.</span><span class="nam">load_config</span><span class="op">(</span><span class="nam">config_file</span><span class="op">=</span><span class="nam">config</span><span class="op">,</span> <span class="nam">verbosity</span><span class="op">=</span><span class="nam">verbosity</span><span class="op">,</span> <span class="nam">format</span><span class="op">=</span><span class="nam">format</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">    <span class="nam">app</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2602a302b50854cf___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2602a302b50854cf_core_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:45 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,336 +5,362 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 97 statements   97 run 0 missing 32 excluded *****
+***** 100 statements   100 run 0 missing 41 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.6, created
-at 2023-05-30 13:45 +0200
+at 2023-05-30 14:21 +0200
 
 
 1"""This file contains all Typer Commands.""" 
-2import typing 
-3from json import load as json_load 
-4 
-5import typer 
-6from plumbum import local 
-7from plumbum.commands.processes import CommandNotFound, ProcessExecutionError 
-8from rich import print 
-9 
-10from .core import ( 
-11 DEFAULT_FORMAT, 
-12 DEFAULT_VERBOSITY, 
-13 EXIT_CODE_COMMAND_NOT_FOUND, 
-14 EXIT_CODE_ERROR, 
-15 EXIT_CODE_SUCCESS, 
-16 GREEN_CIRCLE, 
-17 RED_CIRCLE, 
-18 YELLOW_CIRCLE, 
-19 Format, 
-20 Verbosity, 
-21 dump_tools_with_results, 
-22 info, 
-23 log_cmd_output, 
-24 log_command, 
-25 state, 
-26 warn, 
-27 with_exit_code, 
-28) 
-29 
-30app = typer.Typer() 
-31 
+2import contextlib 
+3import math 
+4import os 
+5import typing 
+6from json import load as json_load 
+7 
+8import typer 
+9from plumbum import local 
+10from plumbum.commands.processes import CommandNotFound,
+ProcessExecutionError 
+11from rich import print 
+12 
+13from .core import ( 
+14 DEFAULT_FORMAT, 
+15 DEFAULT_VERBOSITY, 
+16 EXIT_CODE_COMMAND_NOT_FOUND, 
+17 EXIT_CODE_ERROR, 
+18 EXIT_CODE_SUCCESS, 
+19 GREEN_CIRCLE, 
+20 RED_CIRCLE, 
+21 YELLOW_CIRCLE, 
+22 Format, 
+23 Verbosity, 
+24 dump_tools_with_results, 
+25 info, 
+26 log_cmd_output, 
+27 log_command, 
+28 state, 
+29 warn, 
+30 with_exit_code, 
+31) 
 32 
-33def _check_tool(tool: str, *args: str) -> int: 
-34 """ 
-35 Abstraction to run one of the cli checking tools and process its output. 
-36 
-37 Args: 
-38 tool: the (bash) name of the tool to run. 
-39 args: cli args to pass to the cli bash tool 
-40 """ 
-41 try: 
-42 cmd = local[tool] 
-43 
-44 if state.verbosity >= 3: 
-45 log_command(cmd, args) 
+33app = typer.Typer() 
+34 
+35 
+36def _check_tool(tool: str, *args: str) -> int: 
+37 """ 
+38 Abstraction to run one of the cli checking tools and process its output. 
+39 
+40 Args: 
+41 tool: the (bash) name of the tool to run. 
+42 args: cli args to pass to the cli bash tool 
+43 """ 
+44 try: 
+45 cmd = local[tool] 
 46 
-47 result = cmd(*args) 
-48 
-49 if state.format == "text": 
-50 print(GREEN_CIRCLE, tool) 
+47 if state.verbosity >= 3: 
+48 log_command(cmd, args) 
+49 
+50 result = cmd(*args) 
 51 
-52 if state.verbosity > 2: # pragma: no cover 
-53 log_cmd_output(result) 
+52 if state.format == "text": 
+53 print(GREEN_CIRCLE, tool) 
 54 
-55 return EXIT_CODE_SUCCESS # success 
-56 except CommandNotFound: # pragma: no cover 
-57 if state.verbosity > 2: 
-58 warn(f"Tool {tool} not installed!") 
-59 
-60 if state.format == "text": 
-61 print(YELLOW_CIRCLE, tool) 
+55 if state.verbosity > 2: # pragma: no cover 
+56 log_cmd_output(result) 
+57 
+58 return EXIT_CODE_SUCCESS # success 
+59 except CommandNotFound: # pragma: no cover 
+60 if state.verbosity > 2: 
+61 warn(f"Tool {tool} not installed!") 
 62 
-63 return EXIT_CODE_COMMAND_NOT_FOUND # command not found 
-64 except ProcessExecutionError as e: 
-65 if state.format == "text": 
-66 print(RED_CIRCLE, tool) 
-67 
-68 if state.verbosity > 1: 
-69 log_cmd_output(e.stdout, e.stderr) 
-70 return EXIT_CODE_ERROR # general error 
-71 
-72 
-73# 'directory' is an optional cli argument to many commands, so we define the
+63 if state.format == "text": 
+64 print(YELLOW_CIRCLE, tool) 
+65 
+66 return EXIT_CODE_COMMAND_NOT_FOUND # command not found 
+67 except ProcessExecutionError as e: 
+68 if state.format == "text": 
+69 print(RED_CIRCLE, tool) 
+70 
+71 if state.verbosity > 1: 
+72 log_cmd_output(e.stdout, e.stderr) 
+73 return EXIT_CODE_ERROR # general error 
+74 
+75 
+76# 'directory' is an optional cli argument to many commands, so we define the
 type here for reuse: 
-74T_directory: typing.TypeAlias = typing.Annotated[str, typer.Argument()] # =
+77T_directory: typing.TypeAlias = typing.Annotated[str, typer.Argument()] # =
 "." 
-75 
-76 
-77@app.command() 
-78@with_exit_code() 
-79def ruff(directory: T_directory = None) -> int: 
-80 """ 
-81 Runs the Ruff Linter. 
-82 
-83 Args: 
-84 directory: where to run ruff on (default is current dir) 
+78 
+79 
+80@app.command() 
+81@with_exit_code() 
+82def ruff(directory: T_directory = None) -> int: 
+83 """ 
+84 Runs the Ruff Linter. 
 85 
-86 """ 
-87 config = state.update_config(directory=directory) 
-88 return _check_tool("ruff", config.directory) 
-89 
-90 
-91@app.command() 
-92@with_exit_code() 
-93def black(directory: T_directory = None, fix: bool = False) -> int: 
-94 """ 
-95 Runs the Black code formatter. 
-96 
-97 Args: 
-98 directory: where to run black on (default is current dir) 
-99 fix: if --fix is passed, black will be used to reformat the file(s). 
-100 
-101 """ 
-102 config = state.update_config(directory=directory) 
+86 Args: 
+87 directory: where to run ruff on (default is current dir) 
+88 
+89 """ 
+90 config = state.update_config(directory=directory) 
+91 return _check_tool("ruff", config.directory) 
+92 
+93 
+94@app.command() 
+95@with_exit_code() 
+96def black(directory: T_directory = None, fix: bool = False) -> int: 
+97 """ 
+98 Runs the Black code formatter. 
+99 
+100 Args: 
+101 directory: where to run black on (default is current dir) 
+102 fix: if --fix is passed, black will be used to reformat the file(s). 
 103 
-104 args = [config.directory, r"--exclude=venv.+|.+\.bak"] 
-105 if not fix: 
-106 args.append("--check") 
-107 elif state.verbosity > 2: 
-108 info("note: running WITHOUT --check -> changing files") 
-109 
-110 return _check_tool("black", *args) 
-111 
+104 """ 
+105 config = state.update_config(directory=directory) 
+106 
+107 args = [config.directory, r"--exclude=venv.+|.+\.bak"] 
+108 if not fix: 
+109 args.append("--check") 
+110 elif state.verbosity > 2: 
+111 info("note: running WITHOUT --check -> changing files") 
 112 
-113@app.command() 
-114@with_exit_code() 
-115def isort(directory: T_directory = None, fix: bool = False) -> int: 
-116 """ 
-117 Runs the import sort (isort) utility. 
-118 
-119 Args: 
-120 directory: where to run isort on (default is current dir) 
-121 fix: if --fix is passed, isort will be used to rearrange imports. 
-122 
-123 """ 
-124 config = state.update_config(directory=directory) 
-125 args = [config.directory] 
-126 if not fix: 
-127 args.append("--check-only") 
-128 elif state.verbosity > 2: 
-129 info("note: running WITHOUT --check -> changing files") 
-130 
-131 return _check_tool("isort", *args) 
-132 
+113 return _check_tool("black", *args) 
+114 
+115 
+116@app.command() 
+117@with_exit_code() 
+118def isort(directory: T_directory = None, fix: bool = False) -> int: 
+119 """ 
+120 Runs the import sort (isort) utility. 
+121 
+122 Args: 
+123 directory: where to run isort on (default is current dir) 
+124 fix: if --fix is passed, isort will be used to rearrange imports. 
+125 
+126 """ 
+127 config = state.update_config(directory=directory) 
+128 args = [config.directory] 
+129 if not fix: 
+130 args.append("--check-only") 
+131 elif state.verbosity > 2: 
+132 info("note: running WITHOUT --check -> changing files") 
 133 
-134@app.command() 
-135@with_exit_code() 
-136def mypy(directory: T_directory = None) -> int: 
-137 """ 
-138 Runs the mypy static type checker. 
-139 
-140 Args: 
-141 directory: where to run mypy on (default is current dir) 
+134 return _check_tool("isort", *args) 
+135 
+136 
+137@app.command() 
+138@with_exit_code() 
+139def mypy(directory: T_directory = None) -> int: 
+140 """ 
+141 Runs the mypy static type checker. 
 142 
-143 """ 
-144 config = state.update_config(directory=directory) 
-145 return _check_tool("mypy", config.directory) 
-146 
-147 
-148@app.command() 
-149@with_exit_code() 
-150def bandit(directory: T_directory = None) -> int: 
-151 """ 
-152 Runs the bandit security checker. 
-153 
-154 Args: 
-155 directory: where to run bandit on (default is current dir) 
+143 Args: 
+144 directory: where to run mypy on (default is current dir) 
+145 
+146 """ 
+147 config = state.update_config(directory=directory) 
+148 return _check_tool("mypy", config.directory) 
+149 
+150 
+151@app.command() 
+152@with_exit_code() 
+153def bandit(directory: T_directory = None) -> int: 
+154 """ 
+155 Runs the bandit security checker. 
 156 
-157 """ 
-158 config = state.update_config(directory=directory) 
-159 return _check_tool("bandit", "-r", "-c", config.pyproject,
+157 Args: 
+158 directory: where to run bandit on (default is current dir) 
+159 
+160 """ 
+161 config = state.update_config(directory=directory) 
+162 return _check_tool("bandit", "-r", "-c", config.pyproject,
 config.directory) 
-160 
-161 
-162@app.command() 
-163@with_exit_code() 
-164def pydocstyle(directory: T_directory = None) -> int: 
-165 """ 
-166 Runs the pydocstyle docstring checker. 
-167 
-168 Args: 
-169 directory: where to run pydocstyle on (default is current dir) 
+163 
+164 
+165@app.command() 
+166@with_exit_code() 
+167def pydocstyle(directory: T_directory = None) -> int: 
+168 """ 
+169 Runs the pydocstyle docstring checker. 
 170 
-171 """ 
-172 config = state.update_config(directory=directory) 
-173 return _check_tool("pydocstyle", config.directory) 
-174 
-175 
-176@app.command() 
-177@with_exit_code() 
-178def pytest( 
-179 directory: T_directory = None, html: bool = False, json: bool = False,
-coverage: int = None 
-180) -> int: # pragma: no cover 
-181 """ 
-182 Runs all pytests. 
-183 
-184 Args: 
-185 directory: where to run pytests on (default is current dir) 
-186 html: generate HTML coverage output? 
-187 json: generate JSON coverage output? 
-188 coverage: threshold for coverage (in %) 
-189 
-190 Example: 
-191 > su6 pytest --coverage 50 
-192 if any checks fail: exit 1 and red circle 
-193 if all checks pass but coverage is less than 50%: exit 1, green circle for
+171 Args: 
+172 directory: where to run pydocstyle on (default is current dir) 
+173 
+174 """ 
+175 config = state.update_config(directory=directory) 
+176 return _check_tool("pydocstyle", config.directory) 
+177 
+178 
+179@app.command() 
+180@with_exit_code() 
+181def pytest( 
+182 directory: T_directory = None, 
+183 html: bool = False, 
+184 json: bool = False, 
+185 coverage: int = None, 
+186 badge: bool = None, 
+187) -> int: # pragma: no cover 
+188 """ 
+189 Runs all pytests. 
+190 
+191 Args: 
+192 directory: where to run pytests on (default is current dir) 
+193 html: generate HTML coverage output? 
+194 json: generate JSON coverage output? 
+195 coverage: threshold for coverage (in %) 
+196 badge: generate coverage badge (svg)? If you want to change the name, do
+this in pyproject.toml 
+197 
+198 Example: 
+199 > su6 pytest --coverage 50 
+200 if any checks fail: exit 1 and red circle 
+201 if all checks pass but coverage is less than 50%: exit 1, green circle for
 pytest and red for coverage 
-194 if all check pass and coverage is at least 50%: exit 0, green circle for
+202 if all check pass and coverage is at least 50%: exit 0, green circle for
 pytest and green for coverage 
-195 
-196 if --coverage is not passed, there will be no circle for coverage. 
-197 """ 
-198 config = state.update_config(directory=directory, coverage=coverage) 
-199 
-200 args = ["--cov", config.directory] 
-201 
-202 if config.coverage: 
-203 # json output required! 
-204 json = True 
-205 
-206 if html: 
-207 args.extend(["--cov-report", "html"]) 
-208 
-209 if json: 
-210 args.extend(["--cov-report", "json"]) 
+203 
+204 if --coverage is not passed, there will be no circle for coverage. 
+205 """ 
+206 config = state.update_config(directory=directory, coverage=coverage,
+badge=badge) 
+207 
+208 if config.badge and config.coverage is None: 
+209 # not None but still check cov 
+210 config.coverage = 0 
 211 
-212 exit_code = _check_tool("pytest", *args) 
+212 args = ["--cov", config.directory] 
 213 
-214 if config.coverage: 
-215 with open("coverage.json") as f: 
-216 data = json_load(f) 
-217 percent_covered = round(data["totals"]["percent_covered"]) 
-218 
-219 # if actual coverage is less than the the threshold, exit code should be
+214 if config.coverage is not None: 
+215 # json output required! 
+216 json = True 
+217 
+218 if html: 
+219 args.extend(["--cov-report", "html"]) 
+220 
+221 if json: 
+222 args.extend(["--cov-report", "json"]) 
+223 
+224 exit_code = _check_tool("pytest", *args) 
+225 
+226 if config.coverage is not None: 
+227 with open("coverage.json") as f: 
+228 data = json_load(f) 
+229 percent_covered = math.floor(data["totals"]["percent_covered"]) 
+230 
+231 # if actual coverage is less than the the threshold, exit code should be
 success (0) 
-220 exit_code = percent_covered < config.coverage 
-221 circle = RED_CIRCLE if exit_code else GREEN_CIRCLE 
-222 if state.format == "text": 
-223 print(circle, "coverage") 
-224 
-225 return exit_code 
-226 
-227 
-228@app.command(name="all") 
-229@with_exit_code() 
-230def check_all(directory: T_directory = None, ignore_uninstalled: bool =
-False, coverage: float = None) -> bool: 
-231 """ 
-232 Run all available checks. 
-233 
-234 Args: 
-235 directory: where to run the tools on (default is current dir) 
-236 ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command
-not found) 
-237 coverage: pass to pytest() 
-238 
-239 """ 
-240 config = state.update_config(directory=directory) 
-241 ignored_exit_codes = set() 
-242 if ignore_uninstalled: 
-243 ignored_exit_codes.add(EXIT_CODE_COMMAND_NOT_FOUND) 
+232 exit_code = percent_covered < config.coverage 
+233 circle = RED_CIRCLE if exit_code else GREEN_CIRCLE 
+234 if state.format == "text": 
+235 print(circle, "coverage") 
+236 
+237 if config.badge: 
+238 with contextlib.suppress(FileNotFoundError): 
+239 os.remove(config.badge) 
+240 
+241 result = local["coverage-badge"]("-o", config.badge) 
+242 if state.verbosity > 2: 
+243 print(result) 
 244 
-245 tools = config.determine_which_to_run([ruff, black, mypy, bandit, isort,
-pydocstyle, pytest]) 
+245 return exit_code 
 246 
-247 exit_codes = [] 
-248 for tool in tools: 
-249 a = [directory] 
-250 kw = dict(_suppress=True, _ignore=ignored_exit_codes) 
-251 
-252 if tool is pytest: # pragma: no cover 
-253 kw["coverage"] = coverage 
-254 
-255 exit_codes.append(tool(*a, **kw)) 
-256 
-257 if state.format == "json": 
-258 dump_tools_with_results(tools, exit_codes) 
-259 
-260 return any(exit_codes) 
+247 
+248@app.command(name="all") 
+249@with_exit_code() 
+250def check_all( 
+251 directory: T_directory = None, ignore_uninstalled: bool = False, coverage:
+float = None, badge: bool = None 
+252) -> bool: 
+253 """ 
+254 Run all available checks. 
+255 
+256 Args: 
+257 directory: where to run the tools on (default is current dir) 
+258 ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command
+not found) 
+259 coverage: pass to pytest() 
+260 badge: pass to pytest() 
 261 
-262 
-263@app.command(name="fix") 
-264@with_exit_code() 
-265def do_fix(directory: T_directory = None, ignore_uninstalled: bool = False)
+262 """ 
+263 config = state.update_config(directory=directory) 
+264 ignored_exit_codes = set() 
+265 if ignore_uninstalled: 
+266 ignored_exit_codes.add(EXIT_CODE_COMMAND_NOT_FOUND) 
+267 
+268 tools = config.determine_which_to_run([ruff, black, mypy, bandit, isort,
+pydocstyle, pytest]) 
+269 
+270 exit_codes = [] 
+271 for tool in tools: 
+272 a = [directory] 
+273 kw = dict(_suppress=True, _ignore=ignored_exit_codes) 
+274 
+275 if tool is pytest: # pragma: no cover 
+276 kw["coverage"] = coverage 
+277 kw["badge"] = badge 
+278 
+279 exit_codes.append(tool(*a, **kw)) 
+280 
+281 if state.format == "json": 
+282 dump_tools_with_results(tools, exit_codes) 
+283 
+284 return any(exit_codes) 
+285 
+286 
+287@app.command(name="fix") 
+288@with_exit_code() 
+289def do_fix(directory: T_directory = None, ignore_uninstalled: bool = False)
 -> bool: 
-266 """ 
-267 Do everything that's safe to fix (so not ruff because that may break
+290 """ 
+291 Do everything that's safe to fix (so not ruff because that may break
 semantics). 
-268 
-269 Args: 
-270 directory: where to run the tools on (default is current dir) 
-271 ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command
+292 
+293 Args: 
+294 directory: where to run the tools on (default is current dir) 
+295 ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command
 not found) 
-272 
-273 """ 
-274 config = state.update_config(directory=directory) 
-275 
-276 ignored_exit_codes = set() 
-277 if ignore_uninstalled: 
-278 ignored_exit_codes.add(EXIT_CODE_COMMAND_NOT_FOUND) 
-279 
-280 tools = config.determine_which_to_run([black, isort]) 
-281 
-282 exit_codes = [tool(directory, fix=True, _suppress=True,
+296 
+297 """ 
+298 config = state.update_config(directory=directory) 
+299 
+300 ignored_exit_codes = set() 
+301 if ignore_uninstalled: 
+302 ignored_exit_codes.add(EXIT_CODE_COMMAND_NOT_FOUND) 
+303 
+304 tools = config.determine_which_to_run([black, isort]) 
+305 
+306 exit_codes = [tool(directory, fix=True, _suppress=True,
 _ignore=ignored_exit_codes) for tool in tools] 
-283 
-284 if state.format == "json": 
-285 dump_tools_with_results(tools, exit_codes) 
-286 
-287 return any(exit_codes) 
-288 
-289 
-290@app.callback() 
-291def main(config: str = None, verbosity: Verbosity = DEFAULT_VERBOSITY,
+307 
+308 if state.format == "json": 
+309 dump_tools_with_results(tools, exit_codes) 
+310 
+311 return any(exit_codes) 
+312 
+313 
+314@app.callback() 
+315def main(config: str = None, verbosity: Verbosity = DEFAULT_VERBOSITY,
 format: Format = DEFAULT_FORMAT) -> None: 
-292 """ 
-293 This callback will run before every command, setting the right global
+316 """ 
+317 This callback will run before every command, setting the right global
 flags. 
-294 
-295 Args: 
-296 config: path to a different config toml file 
-297 verbosity: level of detail to print out (1 - 3) 
-298 format: output format 
-299 
-300 """ 
-301 state.load_config(config_file=config, verbosity=verbosity, format=format) 
-302 
-303 
-304if __name__ == "__main__": # pragma: no cover 
-305 app() 
+318 
+319 Args: 
+320 config: path to a different config toml file 
+321 verbosity: level of detail to print out (1 - 3) 
+322 format: output format 
+323 
+324 """ 
+325 state.load_config(config_file=config, verbosity=verbosity, format=format) 
+326 
+327 
+328if __name__ == "__main__": # pragma: no cover 
+329 app() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.6, created
-at 2023-05-30 13:45 +0200
+at 2023-05-30 14:21 +0200
```

### Comparing `su6-0.6.0/htmlcov/d_2602a302b50854cf_core_py.html` & `su6-0.7.0/htmlcov/d_2602a302b50854cf_core_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">185 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">185<span class="text"> run</span></button>
+            <span class="text">188 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">188<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
-            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
+            <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">4<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2602a302b50854cf_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:47 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -291,263 +291,274 @@
     <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">        <span class="key">return</span> <span class="nam">hash</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="nam">DEFAULT_FORMAT</span> <span class="op">=</span> <span class="nam">Format</span><span class="op">.</span><span class="nam">text</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="nam">C</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"C"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">T_Command</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="key">class</span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    Used as typed version of the [tool.su6] part of pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    Also accessible via state.config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="nam">directory</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="nam">pyproject</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="nam">include</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="nam">exclude</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="nam">coverage</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>  <span class="com"># only relevant for pytest</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="key">def</span> <span class="nam">determine_which_to_run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">options</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">        Filter out any includes/excludes from pyproject.toml (first check include, then exclude).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">include</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">options</span> <span class="key">if</span> <span class="nam">_</span><span class="op">.</span><span class="nam">__name__</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">include</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">        <span class="key">elif</span> <span class="nam">self</span><span class="op">.</span><span class="nam">exclude</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">options</span> <span class="key">if</span> <span class="nam">_</span><span class="op">.</span><span class="nam">__name__</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">exclude</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="com"># if no include or excludes passed, just run all!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">        <span class="key">return</span> <span class="nam">options</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="nam">DEFAULT_BADGE</span> <span class="op">=</span> <span class="str">"coverage.svg"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="key">class</span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    Used as typed version of the [tool.su6] part of pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">    Also accessible via state.config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">    <span class="nam">directory</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">    <span class="nam">pyproject</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"pyproject.toml"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="nam">include</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">    <span class="nam">exclude</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="nam">coverage</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>  <span class="com"># only relevant for pytest</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="nam">badge</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">|</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">False</span>  <span class="com"># only relevant for pytest</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">        Update the value of badge to the default path.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">badge</span> <span class="key">is</span> <span class="key">True</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="com"># no cover because pytest can't test pytest :C</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">badge</span> <span class="op">=</span> <span class="nam">DEFAULT_BADGE</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="nam">MaybeConfig</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">Config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="nam">T_typelike</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">type</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">    Raised if pyproject.toml [su6.tool] contains a variable of \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="str">    which the type does not match that of the corresponding key in Config.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="key">def</span> <span class="nam">determine_which_to_run</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">options</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">list</span><span class="op">[</span><span class="nam">C</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">        Filter out any includes/excludes from pyproject.toml (first check include, then exclude).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">include</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">options</span> <span class="key">if</span> <span class="nam">_</span><span class="op">.</span><span class="nam">__name__</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">include</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="key">elif</span> <span class="nam">self</span><span class="op">.</span><span class="nam">exclude</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">_</span> <span class="key">for</span> <span class="nam">_</span> <span class="key">in</span> <span class="nam">options</span> <span class="key">if</span> <span class="nam">_</span><span class="op">.</span><span class="nam">__name__</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">exclude</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="com"># if no include or excludes passed, just run all!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="key">return</span> <span class="nam">options</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="nam">MaybeConfig</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">Config</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="nam">T_typelike</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeAlias</span> <span class="op">=</span> <span class="nam">type</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="key">def</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">T_typelike</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t"><span class="str">    Given a variable, check if it matches 'expected_type' (which can be a Union, parameterized generic etc.).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">    Based on typeguard but this returns a boolean instead of returning the value or throwing a TypeCheckError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">        <span class="nam">_check_type</span><span class="op">(</span><span class="nam">value</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="key">except</span> <span class="nam">TypeCheckError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value ('{self.value}') with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="key">def</span> <span class="nam">_ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="key">class</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">Exception</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">    Raised if pyproject.toml [su6.tool] contains a variable of \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t"><span class="str">    which the type does not match that of the corresponding key in Config.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">value</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="nam">expected_type</span><span class="op">:</span> <span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="key">def</span> <span class="nam">__post_init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="str">        Store the actual type of the config variable.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">actual_type</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="str">        Custom error message based on dataclass values and calculated actual type.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">            <span class="str">f"Config key '{self.key}' had a value ('{self.value}') with a type (`{self.actual_type}`) "</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">            <span class="str">f"that was not expected: `{self.expected_type}` is the required type."</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="key">def</span> <span class="nam">_ensure_types</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">annotations</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="str">    Make sure all values in 'data' are in line with the ones stored in 'annotations'.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_su6_config</span><span class="op">(</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">MaybeConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t"><span class="str">    Parse the users pyproject.toml (found using black's logic) and extract the tool.su6 part.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t"><span class="str">    The types as entered in the toml are checked using _ensure_types,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t"><span class="str">    to make sure there isn't a string implicitly converted to a list of characters or something.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t"><span class="str">    If an annotated key in missing from data, it will be filled with None for convenience.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="nam">final</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">T</span> <span class="op">|</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="key">for</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">_type</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="nam">compare</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="key">if</span> <span class="nam">compare</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">            <span class="com"># skip!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">check_type</span><span class="op">(</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">            <span class="key">raise</span> <span class="nam">ConfigError</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">=</span><span class="nam">compare</span><span class="op">,</span> <span class="nam">expected_type</span><span class="op">=</span><span class="nam">_type</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t"><span class="str">        overwrites: cli arguments can overwrite the config toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">        toml_path: by default, black will search for a relevant pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">                    If a toml_path is provided, that file will be used instead.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="key">if</span> <span class="nam">toml_path</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">        <span class="nam">toml_path</span> <span class="op">=</span> <span class="nam">black</span><span class="op">.</span><span class="nam">files</span><span class="op">.</span><span class="nam">find_pyproject_toml</span><span class="op">(</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">getcwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">        <span class="nam">final</span><span class="op">[</span><span class="nam">key</span><span class="op">]</span> <span class="op">=</span> <span class="nam">compare</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="key">return</span> <span class="nam">final</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="key">def</span> <span class="nam">_get_su6_config</span><span class="op">(</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">MaybeConfig</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">    Parse the users pyproject.toml (found using black's logic) and extract the tool.su6 part.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">toml_path</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">    The types as entered in the toml are checked using _ensure_types,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    to make sure there isn't a string implicitly converted to a list of characters or something.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">toml_path</span><span class="op">,</span> <span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">        <span class="nam">full_config</span> <span class="op">=</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">=</span> <span class="nam">full_config</span><span class="op">[</span><span class="str">"tool"</span><span class="op">]</span><span class="op">[</span><span class="str">"su6"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">|=</span> <span class="nam">overwrites</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="nam">su6_config_dict</span><span class="op">[</span><span class="str">"pyproject"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">toml_path</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">=</span> <span class="nam">_ensure_types</span><span class="op">(</span><span class="nam">su6_config_dict</span><span class="op">,</span> <span class="nam">Config</span><span class="op">.</span><span class="nam">__annotations__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="key">return</span> <span class="nam">Config</span><span class="op">(</span><span class="op">**</span><span class="nam">su6_config_dict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">        overwrites: cli arguments can overwrite the config toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t"><span class="str">        toml_path: by default, black will search for a relevant pyproject.toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t"><span class="str">                    If a toml_path is provided, that file will be used instead.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">    <span class="key">if</span> <span class="nam">toml_path</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">        <span class="nam">toml_path</span> <span class="op">=</span> <span class="nam">black</span><span class="op">.</span><span class="nam">files</span><span class="op">.</span><span class="nam">find_pyproject_toml</span><span class="op">(</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">getcwd</span><span class="op">(</span><span class="op">)</span><span class="op">,</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">toml_path</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="key">def</span> <span class="nam">get_su6_config</span><span class="op">(</span><span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">    Load the relevant pyproject.toml config settings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">        verbosity: if something goes wrong, level 3+ will show a warning and 4+ will raise the exception.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t"><span class="str">        toml_path: --config can be used to use a different file than ./pyproject.toml</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t"><span class="str">        overwrites (dict[str, typing.Any): cli arguments can overwrite the config toml.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="str">                If a value is None, the key is not overwritten.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="com"># strip out any 'overwrites' with None as value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="nam">overwrites</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">        <span class="key">if</span> <span class="nam">config</span> <span class="op">:=</span> <span class="nam">_get_su6_config</span><span class="op">(</span><span class="nam">overwrites</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">=</span><span class="nam">toml_path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">            <span class="key">return</span> <span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Falsey config?"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">        <span class="com"># something went wrong parsing config, use defaults</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">        <span class="key">if</span> <span class="nam">verbosity</span> <span class="op">></span> <span class="num">3</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">            <span class="com"># verbosity = debug</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">            <span class="key">raise</span> <span class="nam">e</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">        <span class="key">elif</span> <span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">            <span class="com"># verbosity = verbose</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">"Error parsing pyproject.toml, falling back to defaults."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">        <span class="key">return</span> <span class="nam">Config</span><span class="op">(</span><span class="op">**</span><span class="nam">overwrites</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t"><span class="key">def</span> <span class="nam">info</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t"><span class="str">    'print' but with blue text.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[blue]{' '.join(args)}[/blue]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t"><span class="key">def</span> <span class="nam">warn</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="str">    'print' but with yellow text.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[yellow]{' '.join(args)}[/yellow]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="key">def</span> <span class="nam">danger</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    'print' but with red text.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[red]{' '.join(args)}[/red]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="key">def</span> <span class="nam">log_command</span><span class="op">(</span><span class="nam">command</span><span class="op">:</span> <span class="nam">LocalCommand</span><span class="op">,</span> <span class="nam">args</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t"><span class="str">    Print a Plumbum command in blue, prefixed with > to indicate it's a shell command.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="nam">info</span><span class="op">(</span><span class="str">f"> {command[*args]}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="key">def</span> <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">stdout</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">""</span><span class="op">,</span> <span class="nam">stderr</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">""</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t"><span class="str">    Print stdout in yellow and stderr in red.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">    <span class="com"># if you are logging stdout, it's probably because it's not a successful run.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="com"># However, it's not stderr so we make it warning-yellow</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">    <span class="nam">warn</span><span class="op">(</span><span class="nam">stdout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="com"># probably more important error stuff, so stderr goes last:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="nam">danger</span><span class="op">(</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">toml_path</span><span class="op">,</span> <span class="str">"rb"</span><span class="op">)</span> <span class="key">as</span> <span class="nam">f</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">        <span class="nam">full_config</span> <span class="op">=</span> <span class="nam">tomllib</span><span class="op">.</span><span class="nam">load</span><span class="op">(</span><span class="nam">f</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">=</span> <span class="nam">full_config</span><span class="op">[</span><span class="str">"tool"</span><span class="op">]</span><span class="op">[</span><span class="str">"su6"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">|=</span> <span class="nam">overwrites</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="nam">su6_config_dict</span><span class="op">[</span><span class="str">"pyproject"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">toml_path</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">su6_config_dict</span> <span class="op">=</span> <span class="nam">_ensure_types</span><span class="op">(</span><span class="nam">su6_config_dict</span><span class="op">,</span> <span class="nam">Config</span><span class="op">.</span><span class="nam">__annotations__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="nam">Config</span><span class="op">(</span><span class="op">**</span><span class="nam">su6_config_dict</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="key">def</span> <span class="nam">get_su6_config</span><span class="op">(</span><span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    Load the relevant pyproject.toml config settings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">        verbosity: if something goes wrong, level 3+ will show a warning and 4+ will raise the exception.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">        toml_path: --config can be used to use a different file than ./pyproject.toml</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">        overwrites (dict[str, typing.Any): cli arguments can overwrite the config toml.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">                If a value is None, the key is not overwritten.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">    <span class="com"># strip out any 'overwrites' with None as value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">overwrites</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">        <span class="key">if</span> <span class="nam">config</span> <span class="op">:=</span> <span class="nam">_get_su6_config</span><span class="op">(</span><span class="nam">overwrites</span><span class="op">,</span> <span class="nam">toml_path</span><span class="op">=</span><span class="nam">toml_path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">            <span class="key">return</span> <span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Falsey config?"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="com"># something went wrong parsing config, use defaults</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">        <span class="key">if</span> <span class="nam">verbosity</span> <span class="op">></span> <span class="num">3</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">            <span class="com"># verbosity = debug</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">            <span class="key">raise</span> <span class="nam">e</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">        <span class="key">elif</span> <span class="nam">verbosity</span> <span class="op">></span> <span class="num">2</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">            <span class="com"># verbosity = verbose</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">"Error parsing pyproject.toml, falling back to defaults."</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="key">return</span> <span class="nam">Config</span><span class="op">(</span><span class="op">**</span><span class="nam">overwrites</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="key">def</span> <span class="nam">info</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">    'print' but with blue text.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[blue]{' '.join(args)}[/blue]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="key">def</span> <span class="nam">warn</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t"><span class="str">    'print' but with yellow text.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[yellow]{' '.join(args)}[/yellow]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="key">def</span> <span class="nam">danger</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    'print' but with red text.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="nam">print</span><span class="op">(</span><span class="str">f"[red]{' '.join(args)}[/red]"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">sys</span><span class="op">.</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t"><span class="key">def</span> <span class="nam">log_command</span><span class="op">(</span><span class="nam">command</span><span class="op">:</span> <span class="nam">LocalCommand</span><span class="op">,</span> <span class="nam">args</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t"><span class="str">    Print a Plumbum command in blue, prefixed with > to indicate it's a shell command.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">    <span class="nam">info</span><span class="op">(</span><span class="str">f"> {command[*args]}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t"><span class="key">class</span> <span class="nam">ApplicationState</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t"><span class="str">    Application State - global user defined variables.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="str">    State contains generic variables passed BEFORE the subcommand (so --verbosity, --config, ...),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t"><span class="str">    whereas Config contains settings from the config toml file, updated with arguments AFTER the subcommand</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="str">    (e.g. su6 subcommand &lt;directory> --flag), directory and flag will be updated in the config and not the state</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t"><span class="key">def</span> <span class="nam">log_cmd_output</span><span class="op">(</span><span class="nam">stdout</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">""</span><span class="op">,</span> <span class="nam">stderr</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">""</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t"><span class="str">    Print stdout in yellow and stderr in red.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">    <span class="com"># if you are logging stdout, it's probably because it's not a successful run.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">    <span class="com"># However, it's not stderr so we make it warning-yellow</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="nam">warn</span><span class="op">(</span><span class="nam">stdout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">    <span class="com"># probably more important error stuff, so stderr goes last:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="nam">danger</span><span class="op">(</span><span class="nam">stderr</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">    <span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">    <span class="nam">format</span><span class="op">:</span> <span class="nam">Format</span> <span class="op">=</span> <span class="nam">DEFAULT_FORMAT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">    <span class="nam">config_file</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>  <span class="com"># will be filled with black's search logic</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">    <span class="nam">config</span><span class="op">:</span> <span class="nam">MaybeConfig</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">    <span class="key">def</span> <span class="nam">load_config</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t"><span class="str">        Load the su6 config from pyproject.toml (or other config_file) with optional overwriting settings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">        <span class="key">if</span> <span class="str">"verbosity"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">[</span><span class="str">"verbosity"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">        <span class="key">if</span> <span class="str">"config_file"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">config_file</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"config_file"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">        <span class="key">if</span> <span class="str">"format"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">format</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"format"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t"><span class="op">@</span><span class="nam">dataclass</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t"><span class="key">class</span> <span class="nam">ApplicationState</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t"><span class="str">    Application State - global user defined variables.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t"><span class="str">    State contains generic variables passed BEFORE the subcommand (so --verbosity, --config, ...),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t"><span class="str">    whereas Config contains settings from the config toml file, updated with arguments AFTER the subcommand</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t"><span class="str">    (e.g. su6 subcommand &lt;directory> --flag), directory and flag will be updated in the config and not the state</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">    <span class="nam">verbosity</span><span class="op">:</span> <span class="nam">Verbosity</span> <span class="op">=</span> <span class="nam">DEFAULT_VERBOSITY</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="nam">format</span><span class="op">:</span> <span class="nam">Format</span> <span class="op">=</span> <span class="nam">DEFAULT_FORMAT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">    <span class="nam">config_file</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span>  <span class="com"># will be filled with black's search logic</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="nam">config</span><span class="op">:</span> <span class="nam">MaybeConfig</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="op">=</span> <span class="nam">get_su6_config</span><span class="op">(</span><span class="nam">toml_path</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">config_file</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_config</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">        Overwrite default/toml settings with cli values.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">            `config = state.update_config(directory='src')`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="str">            This will update the state's config and return the same object with the updated settings.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">            <span class="com"># not loaded yet!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">            <span class="nam">existing_config</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">load_config</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">            <span class="nam">existing_config</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">        <span class="nam">values</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">        <span class="com"># replace is dataclass' update function</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="op">=</span> <span class="nam">replace</span><span class="op">(</span><span class="nam">existing_config</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t"><span class="nam">state</span> <span class="op">=</span> <span class="nam">ApplicationState</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">    <span class="key">def</span> <span class="nam">load_config</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">        Load the su6 config from pyproject.toml (or other config_file) with optional overwriting settings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">        <span class="key">if</span> <span class="str">"verbosity"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">verbosity</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">[</span><span class="str">"verbosity"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">        <span class="key">if</span> <span class="str">"config_file"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">config_file</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"config_file"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">        <span class="key">if</span> <span class="str">"format"</span> <span class="key">in</span> <span class="nam">overwrites</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">format</span> <span class="op">=</span> <span class="nam">overwrites</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"format"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="op">=</span> <span class="nam">get_su6_config</span><span class="op">(</span><span class="nam">toml_path</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">config_file</span><span class="op">,</span> <span class="op">**</span><span class="nam">overwrites</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_config</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Config</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t"><span class="str">        Overwrite default/toml settings with cli values.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="str">            `config = state.update_config(directory='src')`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t"><span class="str">            This will update the state's config and return the same object with the updated settings.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">            <span class="com"># not loaded yet!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">            <span class="nam">existing_config</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">load_config</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">            <span class="nam">existing_config</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">        <span class="nam">values</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">values</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">v</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">        <span class="com"># replace is dataclass' update function</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">config</span> <span class="op">=</span> <span class="nam">replace</span><span class="op">(</span><span class="nam">existing_config</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">config</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t"><span class="nam">state</span> <span class="op">=</span> <span class="nam">ApplicationState</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2602a302b50854cf_cli_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:47 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 185 statements   185 run 0 missing 2 excluded *****
+***** 188 statements   188 run 0 missing 4 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.6, created
-at 2023-05-30 13:47 +0200
+at 2023-05-30 14:21 +0200
 
 
 1""" 
 2This file contains internal helpers used by cli.py. 
 3""" 
 4import enum 
 5import functools 
@@ -247,274 +247,285 @@
 209 return hash(self.value) 
 210 
 211 
 212DEFAULT_FORMAT = Format.text 
 213 
 214C = typing.TypeVar("C", bound=T_Command) 
 215 
-216 
-217@dataclass 
-218class Config: 
-219 """ 
-220 Used as typed version of the [tool.su6] part of pyproject.toml. 
-221 
-222 Also accessible via state.config 
-223 """ 
-224 
-225 directory: str = "." 
-226 pyproject: str = "pyproject.toml" 
-227 include: typing.Optional[list[str]] = None 
-228 exclude: typing.Optional[list[str]] = None 
-229 coverage: typing.Optional[float] = None # only relevant for pytest 
-230 
-231 def determine_which_to_run(self, options: list[C]) -> list[C]: 
-232 """ 
-233 Filter out any includes/excludes from pyproject.toml (first check include,
-then exclude). 
-234 """ 
-235 if self.include: 
-236 return [_ for _ in options if _.__name__ in self.include] 
-237 elif self.exclude: 
-238 return [_ for _ in options if _.__name__ not in self.exclude] 
-239 # if no include or excludes passed, just run all! 
-240 return options 
+216DEFAULT_BADGE = "coverage.svg" 
+217 
+218 
+219@dataclass 
+220class Config: 
+221 """ 
+222 Used as typed version of the [tool.su6] part of pyproject.toml. 
+223 
+224 Also accessible via state.config 
+225 """ 
+226 
+227 directory: str = "." 
+228 pyproject: str = "pyproject.toml" 
+229 include: typing.Optional[list[str]] = None 
+230 exclude: typing.Optional[list[str]] = None 
+231 coverage: typing.Optional[float] = None # only relevant for pytest 
+232 badge: bool | str = False # only relevant for pytest 
+233 
+234 def __post_init__(self) -> None: 
+235 """ 
+236 Update the value of badge to the default path. 
+237 """ 
+238 if self.badge is True: # pragma: no cover 
+239 # no cover because pytest can't test pytest :C 
+240 self.badge = DEFAULT_BADGE 
 241 
-242 
-243MaybeConfig: typing.TypeAlias = typing.Optional[Config] 
-244 
-245T_typelike: typing.TypeAlias = type | types.UnionType | types.UnionType 
-246 
-247 
-248def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
-249 """ 
-250 Given a variable, check if it matches 'expected_type' (which can be a
+242 def determine_which_to_run(self, options: list[C]) -> list[C]: 
+243 """ 
+244 Filter out any includes/excludes from pyproject.toml (first check include,
+then exclude). 
+245 """ 
+246 if self.include: 
+247 return [_ for _ in options if _.__name__ in self.include] 
+248 elif self.exclude: 
+249 return [_ for _ in options if _.__name__ not in self.exclude] 
+250 # if no include or excludes passed, just run all! 
+251 return options 
+252 
+253 
+254MaybeConfig: typing.TypeAlias = typing.Optional[Config] 
+255 
+256T_typelike: typing.TypeAlias = type | types.UnionType | types.UnionType 
+257 
+258 
+259def check_type(value: typing.Any, expected_type: T_typelike) -> bool: 
+260 """ 
+261 Given a variable, check if it matches 'expected_type' (which can be a
 Union, parameterized generic etc.). 
-251 
-252 Based on typeguard but this returns a boolean instead of returning the
+262 
+263 Based on typeguard but this returns a boolean instead of returning the
 value or throwing a TypeCheckError 
-253 """ 
-254 try: 
-255 _check_type(value, expected_type) 
-256 return True 
-257 except TypeCheckError: 
-258 return False 
-259 
-260 
-261@dataclass 
-262class ConfigError(Exception): 
-263 """ 
-264 Raised if pyproject.toml [su6.tool] contains a variable of \ 
-265 which the type does not match that of the corresponding key in Config. 
-266 """ 
-267 
-268 key: str 
-269 value: typing.Any 
-270 expected_type: type 
+264 """ 
+265 try: 
+266 _check_type(value, expected_type) 
+267 return True 
+268 except TypeCheckError: 
+269 return False 
+270 
 271 
-272 def __post_init__(self) -> None: 
-273 """ 
-274 Store the actual type of the config variable. 
-275 """ 
-276 self.actual_type = type(self.value) 
-277 
-278 def __str__(self) -> str: 
-279 """ 
-280 Custom error message based on dataclass values and calculated actual type. 
-281 """ 
-282 return ( 
-283 f"Config key '{self.key}' had a value ('{self.value}') with a type (`
+272@dataclass 
+273class ConfigError(Exception): 
+274 """ 
+275 Raised if pyproject.toml [su6.tool] contains a variable of \ 
+276 which the type does not match that of the corresponding key in Config. 
+277 """ 
+278 
+279 key: str 
+280 value: typing.Any 
+281 expected_type: type 
+282 
+283 def __post_init__(self) -> None: 
+284 """ 
+285 Store the actual type of the config variable. 
+286 """ 
+287 self.actual_type = type(self.value) 
+288 
+289 def __str__(self) -> str: 
+290 """ 
+291 Custom error message based on dataclass values and calculated actual type. 
+292 """ 
+293 return ( 
+294 f"Config key '{self.key}' had a value ('{self.value}') with a type (`
 {self.actual_type}`) " 
-284 f"that was not expected: `{self.expected_type}` is the required type." 
-285 ) 
-286 
-287 
-288T = typing.TypeVar("T") 
-289 
-290 
-291def _ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
+295 f"that was not expected: `{self.expected_type}` is the required type." 
+296 ) 
+297 
+298 
+299T = typing.TypeVar("T") 
+300 
+301 
+302def _ensure_types(data: dict[str, T], annotations: dict[str, type]) -> dict
 [str, T | None]: 
-292 """ 
-293 Make sure all values in 'data' are in line with the ones stored in
+303 """ 
+304 Make sure all values in 'data' are in line with the ones stored in
 'annotations'. 
-294 
-295 If an annotated key in missing from data, it will be filled with None for
-convenience. 
-296 """ 
-297 final: dict[str, T | None] = {} 
-298 for key, _type in annotations.items(): 
-299 compare = data.get(key) 
-300 if compare is None: 
-301 # skip! 
-302 continue 
-303 if not check_type(compare, _type): 
-304 raise ConfigError(key, value=compare, expected_type=_type) 
 305 
-306 final[key] = compare 
-307 return final 
-308 
-309 
-310def _get_su6_config(overwrites: dict[str, typing.Any], toml_path: str =
+306 If an annotated key in missing from data, it will be filled with None for
+convenience. 
+307 """ 
+308 final: dict[str, T | None] = {} 
+309 for key, _type in annotations.items(): 
+310 compare = data.get(key) 
+311 if compare is None: 
+312 # skip! 
+313 continue 
+314 if not check_type(compare, _type): 
+315 raise ConfigError(key, value=compare, expected_type=_type) 
+316 
+317 final[key] = compare 
+318 return final 
+319 
+320 
+321def _get_su6_config(overwrites: dict[str, typing.Any], toml_path: str =
 None) -> MaybeConfig: 
-311 """ 
-312 Parse the users pyproject.toml (found using black's logic) and extract the
+322 """ 
+323 Parse the users pyproject.toml (found using black's logic) and extract the
 tool.su6 part. 
-313 
-314 The types as entered in the toml are checked using _ensure_types, 
-315 to make sure there isn't a string implicitly converted to a list of
-characters or something. 
-316 
-317 Args: 
-318 overwrites: cli arguments can overwrite the config toml. 
-319 toml_path: by default, black will search for a relevant pyproject.toml. 
-320 If a toml_path is provided, that file will be used instead. 
-321 """ 
-322 if toml_path is None: 
-323 toml_path = black.files.find_pyproject_toml((os.getcwd(),)) 
 324 
-325 if not toml_path: 
-326 return None 
+325 The types as entered in the toml are checked using _ensure_types, 
+326 to make sure there isn't a string implicitly converted to a list of
+characters or something. 
 327 
-328 with open(toml_path, "rb") as f: 
-329 full_config = tomllib.load(f) 
-330 
-331 su6_config_dict = full_config["tool"]["su6"] 
-332 su6_config_dict |= overwrites 
-333 
-334 su6_config_dict["pyproject"] = toml_path 
-335 su6_config_dict = _ensure_types(su6_config_dict, Config.__annotations__) 
-336 
-337 return Config(**su6_config_dict) 
+328 Args: 
+329 overwrites: cli arguments can overwrite the config toml. 
+330 toml_path: by default, black will search for a relevant pyproject.toml. 
+331 If a toml_path is provided, that file will be used instead. 
+332 """ 
+333 if toml_path is None: 
+334 toml_path = black.files.find_pyproject_toml((os.getcwd(),)) 
+335 
+336 if not toml_path: 
+337 return None 
 338 
-339 
-340def get_su6_config(verbosity: Verbosity = DEFAULT_VERBOSITY, toml_path: str
+339 with open(toml_path, "rb") as f: 
+340 full_config = tomllib.load(f) 
+341 
+342 su6_config_dict = full_config["tool"]["su6"] 
+343 su6_config_dict |= overwrites 
+344 
+345 su6_config_dict["pyproject"] = toml_path 
+346 su6_config_dict = _ensure_types(su6_config_dict, Config.__annotations__) 
+347 
+348 return Config(**su6_config_dict) 
+349 
+350 
+351def get_su6_config(verbosity: Verbosity = DEFAULT_VERBOSITY, toml_path: str
 = None, **overwrites: typing.Any) -> Config: 
-341 """ 
-342 Load the relevant pyproject.toml config settings. 
-343 
-344 Args: 
-345 verbosity: if something goes wrong, level 3+ will show a warning and 4+
+352 """ 
+353 Load the relevant pyproject.toml config settings. 
+354 
+355 Args: 
+356 verbosity: if something goes wrong, level 3+ will show a warning and 4+
 will raise the exception. 
-346 toml_path: --config can be used to use a different file than ./
+357 toml_path: --config can be used to use a different file than ./
 pyproject.toml 
-347 overwrites (dict[str, typing.Any): cli arguments can overwrite the config
+358 overwrites (dict[str, typing.Any): cli arguments can overwrite the config
 toml. 
-348 If a value is None, the key is not overwritten. 
-349 """ 
-350 # strip out any 'overwrites' with None as value 
-351 overwrites = {k: v for k, v in overwrites.items() if v is not None} 
-352 
-353 try: 
-354 if config := _get_su6_config(overwrites, toml_path=toml_path): 
-355 return config 
-356 raise ValueError("Falsey config?") 
-357 except Exception as e: 
-358 # something went wrong parsing config, use defaults 
-359 if verbosity > 3: 
-360 # verbosity = debug 
-361 raise e 
-362 elif verbosity > 2: 
-363 # verbosity = verbose 
-364 print("Error parsing pyproject.toml, falling back to defaults.",
+359 If a value is None, the key is not overwritten. 
+360 """ 
+361 # strip out any 'overwrites' with None as value 
+362 overwrites = {k: v for k, v in overwrites.items() if v is not None} 
+363 
+364 try: 
+365 if config := _get_su6_config(overwrites, toml_path=toml_path): 
+366 return config 
+367 raise ValueError("Falsey config?") 
+368 except Exception as e: 
+369 # something went wrong parsing config, use defaults 
+370 if verbosity > 3: 
+371 # verbosity = debug 
+372 raise e 
+373 elif verbosity > 2: 
+374 # verbosity = verbose 
+375 print("Error parsing pyproject.toml, falling back to defaults.",
 file=sys.stderr) 
-365 return Config(**overwrites) 
-366 
-367 
-368def info(*args: str) -> None: 
-369 """ 
-370 'print' but with blue text. 
-371 """ 
-372 print(f"[blue]{' '.join(args)}[/blue]", file=sys.stderr) 
-373 
-374 
-375def warn(*args: str) -> None: 
-376 """ 
-377 'print' but with yellow text. 
-378 """ 
-379 print(f"[yellow]{' '.join(args)}[/yellow]", file=sys.stderr) 
-380 
-381 
-382def danger(*args: str) -> None: 
-383 """ 
-384 'print' but with red text. 
-385 """ 
-386 print(f"[red]{' '.join(args)}[/red]", file=sys.stderr) 
-387 
-388 
-389def log_command(command: LocalCommand, args: typing.Iterable[str]) -> None: 
-390 """ 
-391 Print a Plumbum command in blue, prefixed with > to indicate it's a shell
+376 return Config(**overwrites) 
+377 
+378 
+379def info(*args: str) -> None: 
+380 """ 
+381 'print' but with blue text. 
+382 """ 
+383 print(f"[blue]{' '.join(args)}[/blue]", file=sys.stderr) 
+384 
+385 
+386def warn(*args: str) -> None: 
+387 """ 
+388 'print' but with yellow text. 
+389 """ 
+390 print(f"[yellow]{' '.join(args)}[/yellow]", file=sys.stderr) 
+391 
+392 
+393def danger(*args: str) -> None: 
+394 """ 
+395 'print' but with red text. 
+396 """ 
+397 print(f"[red]{' '.join(args)}[/red]", file=sys.stderr) 
+398 
+399 
+400def log_command(command: LocalCommand, args: typing.Iterable[str]) -> None: 
+401 """ 
+402 Print a Plumbum command in blue, prefixed with > to indicate it's a shell
 command. 
-392 """ 
-393 info(f"> {command[*args]}") 
-394 
-395 
-396def log_cmd_output(stdout: str = "", stderr: str = "") -> None: 
-397 """ 
-398 Print stdout in yellow and stderr in red. 
-399 """ 
-400 # if you are logging stdout, it's probably because it's not a successful
-run. 
-401 # However, it's not stderr so we make it warning-yellow 
-402 warn(stdout) 
-403 # probably more important error stuff, so stderr goes last: 
-404 danger(stderr) 
+403 """ 
+404 info(f"> {command[*args]}") 
 405 
 406 
-407@dataclass() 
-408class ApplicationState: 
-409 """ 
-410 Application State - global user defined variables. 
-411 
-412 State contains generic variables passed BEFORE the subcommand (so --
+407def log_cmd_output(stdout: str = "", stderr: str = "") -> None: 
+408 """ 
+409 Print stdout in yellow and stderr in red. 
+410 """ 
+411 # if you are logging stdout, it's probably because it's not a successful
+run. 
+412 # However, it's not stderr so we make it warning-yellow 
+413 warn(stdout) 
+414 # probably more important error stuff, so stderr goes last: 
+415 danger(stderr) 
+416 
+417 
+418@dataclass() 
+419class ApplicationState: 
+420 """ 
+421 Application State - global user defined variables. 
+422 
+423 State contains generic variables passed BEFORE the subcommand (so --
 verbosity, --config, ...), 
-413 whereas Config contains settings from the config toml file, updated with
+424 whereas Config contains settings from the config toml file, updated with
 arguments AFTER the subcommand 
-414 (e.g. su6 subcommand <directory> --flag), directory and flag will be
+425 (e.g. su6 subcommand <directory> --flag), directory and flag will be
 updated in the config and not the state 
-415 """ 
-416 
-417 verbosity: Verbosity = DEFAULT_VERBOSITY 
-418 format: Format = DEFAULT_FORMAT 
-419 config_file: typing.Optional[str] = None # will be filled with black's
+426 """ 
+427 
+428 verbosity: Verbosity = DEFAULT_VERBOSITY 
+429 format: Format = DEFAULT_FORMAT 
+430 config_file: typing.Optional[str] = None # will be filled with black's
 search logic 
-420 config: MaybeConfig = None 
-421 
-422 def load_config(self, **overwrites: typing.Any) -> Config: 
-423 """ 
-424 Load the su6 config from pyproject.toml (or other config_file) with
-optional overwriting settings. 
-425 """ 
-426 if "verbosity" in overwrites: 
-427 self.verbosity = overwrites["verbosity"] 
-428 if "config_file" in overwrites: 
-429 self.config_file = overwrites.pop("config_file") 
-430 if "format" in overwrites: 
-431 self.format = overwrites.pop("format") 
+431 config: MaybeConfig = None 
 432 
-433 self.config = get_su6_config(toml_path=self.config_file, **overwrites) 
-434 return self.config 
-435 
-436 def update_config(self, **values: typing.Any) -> Config: 
-437 """ 
-438 Overwrite default/toml settings with cli values. 
-439 
-440 Example: 
-441 `config = state.update_config(directory='src')` 
-442 This will update the state's config and return the same object with the
+433 def load_config(self, **overwrites: typing.Any) -> Config: 
+434 """ 
+435 Load the su6 config from pyproject.toml (or other config_file) with
+optional overwriting settings. 
+436 """ 
+437 if "verbosity" in overwrites: 
+438 self.verbosity = overwrites["verbosity"] 
+439 if "config_file" in overwrites: 
+440 self.config_file = overwrites.pop("config_file") 
+441 if "format" in overwrites: 
+442 self.format = overwrites.pop("format") 
+443 
+444 self.config = get_su6_config(toml_path=self.config_file, **overwrites) 
+445 return self.config 
+446 
+447 def update_config(self, **values: typing.Any) -> Config: 
+448 """ 
+449 Overwrite default/toml settings with cli values. 
+450 
+451 Example: 
+452 `config = state.update_config(directory='src')` 
+453 This will update the state's config and return the same object with the
 updated settings. 
-443 """ 
-444 if self.config is None: 
-445 # not loaded yet! 
-446 existing_config = self.load_config() 
-447 else: 
-448 existing_config = self.config 
-449 
-450 values = {k: v for k, v in values.items() if v is not None} 
-451 # replace is dataclass' update function 
-452 self.config = replace(existing_config, **values) 
-453 return self.config 
-454 
-455 
-456state = ApplicationState() 
+454 """ 
+455 if self.config is None: 
+456 # not loaded yet! 
+457 existing_config = self.load_config() 
+458 else: 
+459 existing_config = self.config 
+460 
+461 values = {k: v for k, v in values.items() if v is not None} 
+462 # replace is dataclass' update function 
+463 self.config = replace(existing_config, **values) 
+464 return self.config 
+465 
+466 
+467state = ApplicationState() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.6, created
-at 2023-05-30 13:47 +0200
+at 2023-05-30 14:21 +0200
```

### Comparing `su6-0.6.0/htmlcov/d_a44f0ac069e85531___init___py.html` & `su6-0.7.0/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_a44f0ac069e85531__shared_py.html` & `su6-0.7.0/htmlcov/d_a44f0ac069e85531__shared_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_about_py.html` & `su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_about_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html` & `su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/d_a44f0ac069e85531_test_core_py.html` & `su6-0.7.0/htmlcov/d_a44f0ac069e85531_test_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/favicon_32.png` & `su6-0.7.0/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/index.html` & `su6-0.7.0/htmlcov/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:47 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,46 +73,46 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_2602a302b50854cf_cli_py.html">src/su6/cli.py</a></td>
-                <td>97</td>
+                <td>100</td>
                 <td>0</td>
-                <td>32</td>
-                <td class="right" data-ratio="97 97">100%</td>
+                <td>41</td>
+                <td class="right" data-ratio="100 100">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_2602a302b50854cf_core_py.html">src/su6/core.py</a></td>
-                <td>185</td>
+                <td>188</td>
                 <td>0</td>
-                <td>2</td>
-                <td class="right" data-ratio="185 185">100%</td>
+                <td>4</td>
+                <td class="right" data-ratio="188 188">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>284</td>
+                <td>290</td>
                 <td>0</td>
-                <td>34</td>
-                <td class="right" data-ratio="284 284">100%</td>
+                <td>45</td>
+                <td class="right" data-ratio="290 290">100%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.6">coverage.py v7.2.6</a>,
-            created at 2023-05-30 13:47 +0200
+            created at 2023-05-30 14:21 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_2602a302b50854cf_core_py.html"/>
         <a id="nextFileLink" class="nav" href="d_2602a302b50854cf___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.6, created at 2023-05-30 13:47 +0200
+coverage.py_v7.2.6, created at 2023-05-30 14:21 +0200
 
 Module               statements missing excluded coverage
 src/su6/__about__.py 1          0       0        100%
 src/su6/__init__.py  1          0       0        100%
-src/su6/cli.py       97         0       32       100%
-src/su6/core.py      185        0       2        100%
-Total                284        0       34       100%
+src/su6/cli.py       100        0       41       100%
+src/su6/core.py      188        0       4        100%
+Total                290        0       45       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.6, created at 2023-05-30 13:47 +0200
+coverage.py_v7.2.6, created at 2023-05-30 14:21 +0200
  ____
```

### Comparing `su6-0.6.0/htmlcov/keybd_closed.png` & `su6-0.7.0/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/keybd_open.png` & `su6-0.7.0/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/htmlcov/status.json` & `su6-0.7.0/htmlcov/status.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'files'": "{'d_2602a302b50854cf_cli_py': {'hash': '4e27effeba3cbcde0283c7f1d7ebe5aa', 'index': "*

 * *            "{'nums': {insert: [(2, 100), (3, 41)], delete: [3, 2]}}}, "*

 * *            "'d_2602a302b50854cf_core_py': {'hash': '43be6e9d5f512b43a3d51fbec949190e', 'index': "*

 * *            "{'nums': {insert: [(2, 188), (3, 4)], delete: [3, 2]}}}}"}*

```diff
@@ -31,39 +31,39 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/su6/__init__.py"
             }
         },
         "d_2602a302b50854cf_cli_py": {
-            "hash": "6881ced33988e25343e7e2e9ce7aad34",
+            "hash": "4e27effeba3cbcde0283c7f1d7ebe5aa",
             "index": {
                 "html_filename": "d_2602a302b50854cf_cli_py.html",
                 "nums": [
                     0,
                     1,
-                    97,
-                    32,
+                    100,
+                    41,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6/cli.py"
             }
         },
         "d_2602a302b50854cf_core_py": {
-            "hash": "86e07e93261662c9c03070b494d726b3",
+            "hash": "43be6e9d5f512b43a3d51fbec949190e",
             "index": {
                 "html_filename": "d_2602a302b50854cf_core_py.html",
                 "nums": [
                     0,
                     1,
-                    185,
-                    2,
+                    188,
+                    4,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/su6/core.py"
             }
```

### Comparing `su6-0.6.0/htmlcov/style.css` & `su6-0.7.0/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/except_pytest.toml` & `su6-0.7.0/pytest_examples/except_pytest.toml`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ast.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/abc.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/abc.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/array.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/array.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/bad.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/bad.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/bad.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/bad.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/builtins.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/codecs.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/enum.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/enum.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/good.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/good.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/io.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/io.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/mmap.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/pickle.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/re.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/re.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sys.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/sys.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/this.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/this.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/types.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/types.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7878787878787878%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 11), (6, 8), (7, 1)], delete: [7, 6, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (8, 30)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(4, 'typing'), (5, 'typing_extensions'), (8, 'abc')], delete: [4, 2, "*

 * *                   '1]}',*

 * * "'hash'": "'f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724'",*

 * * "'id'": "'collections'",*

 * * "'interface_hash'": "'02da07e0f9a70efabb774f32b47c3554ef92648b90c2082498e85987d25fdeb8'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/ve […]*

```diff
@@ -1,46 +1,46 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        7,
+        11,
         1,
         2,
         3,
         4,
         5,
-        6,
-        36,
+        8,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
-        10,
         5,
         5,
         5,
         5,
-        5
+        5,
+        5,
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "abc",
-        "collections",
         "sys",
-        "typing",
         "_collections_abc",
         "_typeshed",
+        "typing",
+        "typing_extensions",
         "types",
-        "builtins"
+        "builtins",
+        "abc"
     ],
-    "hash": "44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65a04119",
-    "id": "typing_extensions",
+    "hash": "f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724",
+    "id": "collections",
     "ignore_all": true,
-    "interface_hash": "97a64b9296f7cd7e33606259f5b17e600995b040b31b5c94570b5369924712e9",
+    "interface_hash": "02da07e0f9a70efabb774f32b47c3554ef92648b90c2082498e85987d25fdeb8",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi",
     "plugin_data": null,
-    "size": 9843,
+    "size": 20830,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7787878787878788%*

 * *Differences: {"'dep_lines'": '{insert: [(3, 1)], delete: [6, 5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 30)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'importlib.abc'), (5, 'typing')], delete: [5, 4, 3, 2, 1]}",*

 * * "'hash'": "'93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914'",*

 * * "'id'": "'importlib'",*

 * * "'interface_hash'": "'5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3'",*

 * * "'path'": "'/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdl […]*

```diff
@@ -1,46 +1,37 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        11,
         1,
         2,
         3,
-        4,
-        5,
-        8,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
-        "_collections_abc",
-        "_typeshed",
-        "typing",
-        "typing_extensions",
+        "importlib.abc",
         "types",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724",
-    "id": "collections",
+    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
+    "id": "importlib",
     "ignore_all": true,
-    "interface_hash": "02da07e0f9a70efabb774f32b47c3554ef92648b90c2082498e85987d25fdeb8",
+    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -75,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
     "plugin_data": null,
-    "size": 20830,
+    "size": 801,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/header.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/message.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.76%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 31), (1, 5), (2, 6), (3, 7), (7, 4), (8, 8), (9, 10), (10, 11), '*

 * *                '(11, 12)], delete: [4, 3]}',*

 * * "'dep_prios'": '{insert: [(4, 10), (5, 5), (6, 10), (7, 5), (8, 5), (9, 5), (10, 5), (11, 5), '*

 * *                '(12, 5)], delete: [5, 4]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.metadata._meta'), (2, 'email.message'), (5, "*

 * *                   "'pathlib'), (6, 'sys'), (7, '_typeshed'), (8, 'os'), (9, 're'), (11, "*

 * *                   "'typing_extensions'), (12 […]*

```diff
@@ -1,37 +1,58 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
+        31,
+        5,
+        6,
+        7,
         1,
         2,
         3,
-        1,
-        1,
+        4,
+        8,
+        10,
+        11,
+        12,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        30,
-        30
+        10,
+        5,
+        10,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
+        "importlib.metadata._meta",
         "collections.abc",
+        "email.message",
         "importlib.abc",
-        "types",
-        "builtins",
         "abc",
-        "typing"
+        "pathlib",
+        "sys",
+        "_typeshed",
+        "os",
+        "re",
+        "typing",
+        "typing_extensions",
+        "builtins"
     ],
-    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
-    "id": "importlib",
+    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
+    "id": "importlib.metadata",
     "ignore_all": true,
-    "interface_hash": "5f92435a83c8d015c7f5083f731f4b7db32ae1cd81d45c2986fdcbc6fcba52a3",
+    "interface_hash": "21a4b9857190f7893fd1d564e25c567d7f4777614d1a6990ac158bb2835a9eab",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -66,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
     "plugin_data": null,
-    "size": 801,
+    "size": 6736,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7616677912730545%*

 * *Differences: {"'dep_lines'": '{insert: [(0, 23), (1, 30), (4, 21), (5, 22), (6, 24), (7, 25), (8, 26), (9, 27), '*

 * *                '(10, 28), (11, 33), (12, 1), (13, 1), (14, 1)], delete: [11, 10, 9, 8, 7, 6, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (12, 30), (13, 30), (14, 30), (15, 30)], delete: [6, '*

 * *                '4, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'os.path'), (4, 'abc'), (5, 'builtins'), (6, 'contextlib'), (7, "*

 * *                   "'io'), (8, 'subprocess'), (11, 'types […]*

```diff
@@ -1,58 +1,67 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        31,
-        5,
-        6,
-        7,
+        23,
+        30,
         1,
         2,
-        3,
-        4,
-        8,
-        10,
-        11,
-        12,
+        21,
+        22,
+        24,
+        25,
+        26,
+        27,
+        28,
+        33,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
         5,
         5,
         5,
-        10,
         5,
-        10,
         5,
         5,
         5,
         5,
         5,
-        5
+        30,
+        30,
+        30,
+        30
     ],
     "dependencies": [
-        "importlib.metadata._meta",
         "collections.abc",
-        "email.message",
-        "importlib.abc",
-        "abc",
-        "pathlib",
+        "os.path",
         "sys",
         "_typeshed",
-        "os",
-        "re",
+        "abc",
+        "builtins",
+        "contextlib",
+        "io",
+        "subprocess",
         "typing",
         "typing_extensions",
-        "builtins"
+        "types",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
-    "id": "importlib.metadata",
+    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
+    "id": "os",
     "ignore_all": true,
-    "interface_hash": "21a4b9857190f7893fd1d564e25c567d7f4777614d1a6990ac158bb2835a9eab",
+    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -87,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
     "plugin_data": null,
-    "size": 6736,
+    "size": 36995,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7571486928104575%*

 * *Differences: {"'dep_lines'": '{insert: [(1, 7)], delete: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [13, 12, 9, 8, 7, 6, 5, 4, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'posixpath'), (3, 'abc')], delete: [15, 14, 13, 12, 11, 10, 8, "*

 * *                   '7, 6, 4, 3, 1, 0]}',*

 * * "'hash'": "'1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433'",*

 * * "'id'": "'os.path'",*

 * * "'interface_hash'": "'a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e'",*

 * * "'path'": "'/home/robin/we […]*

```diff
@@ -1,67 +1,34 @@
 {
     "data_mtime": 1685433917,
     "dep_lines": [
-        23,
-        30,
-        1,
-        2,
-        21,
-        22,
-        24,
-        25,
-        26,
-        27,
-        28,
-        33,
         1,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os.path",
         "sys",
-        "_typeshed",
-        "abc",
+        "posixpath",
         "builtins",
-        "contextlib",
-        "io",
-        "subprocess",
-        "typing",
-        "typing_extensions",
-        "types",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "abc",
+        "typing"
     ],
-    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
-    "id": "os",
+    "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
+    "id": "os.path",
     "ignore_all": true,
-    "interface_hash": "7857e0241ab1ae7ccf1c6583d54898fa386079260ac7e105c7e8d281784f77c9",
+    "interface_hash": "a6f6d43232b4bf4602fa5da4d1c8d408ace2330d5501f40fb15a486315e70b2e",
     "mtime": 1685293614,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
@@ -96,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
+    "path": "/home/robin/werk/Eigen/su6-checker/venv/lib/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
     "plugin_data": null,
-    "size": 36995,
+    "size": 186,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `su6-0.6.0/pytest_examples/.mypy_cache/3.11/os/path.data.json` & `su6-0.7.0/pytest_examples/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/src/su6/cli.py` & `su6-0.7.0/src/su6/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """This file contains all Typer Commands."""
+import contextlib
+import math
+import os
 import typing
 from json import load as json_load
 
 import typer
 from plumbum import local
 from plumbum.commands.processes import CommandNotFound, ProcessExecutionError
 from rich import print
@@ -172,73 +175,93 @@
     config = state.update_config(directory=directory)
     return _check_tool("pydocstyle", config.directory)
 
 
 @app.command()
 @with_exit_code()
 def pytest(
-    directory: T_directory = None, html: bool = False, json: bool = False, coverage: int = None
+    directory: T_directory = None,
+    html: bool = False,
+    json: bool = False,
+    coverage: int = None,
+    badge: bool = None,
 ) -> int:  # pragma: no cover
     """
     Runs all pytests.
 
     Args:
         directory: where to run pytests on (default is current dir)
         html: generate HTML coverage output?
         json: generate JSON coverage output?
         coverage: threshold for coverage (in %)
+        badge: generate coverage badge (svg)? If you want to change the name, do this in pyproject.toml
 
     Example:
         > su6 pytest --coverage 50
         if any checks fail: exit 1 and red circle
         if all checks pass but coverage is less than 50%: exit 1, green circle for pytest and red for coverage
         if all check pass and coverage is at least 50%: exit 0, green circle for pytest and green for coverage
 
         if --coverage is not passed, there will be no circle for coverage.
     """
-    config = state.update_config(directory=directory, coverage=coverage)
+    config = state.update_config(directory=directory, coverage=coverage, badge=badge)
+
+    if config.badge and config.coverage is None:
+        # not None but still check cov
+        config.coverage = 0
 
     args = ["--cov", config.directory]
 
-    if config.coverage:
+    if config.coverage is not None:
         # json output required!
         json = True
 
     if html:
         args.extend(["--cov-report", "html"])
 
     if json:
         args.extend(["--cov-report", "json"])
 
     exit_code = _check_tool("pytest", *args)
 
-    if config.coverage:
+    if config.coverage is not None:
         with open("coverage.json") as f:
             data = json_load(f)
-            percent_covered = round(data["totals"]["percent_covered"])
+            percent_covered = math.floor(data["totals"]["percent_covered"])
 
         # if actual coverage is less than the the threshold, exit code should be success (0)
         exit_code = percent_covered < config.coverage
         circle = RED_CIRCLE if exit_code else GREEN_CIRCLE
         if state.format == "text":
             print(circle, "coverage")
 
+        if config.badge:
+            with contextlib.suppress(FileNotFoundError):
+                os.remove(config.badge)
+
+            result = local["coverage-badge"]("-o", config.badge)
+            if state.verbosity > 2:
+                print(result)
+
     return exit_code
 
 
 @app.command(name="all")
 @with_exit_code()
-def check_all(directory: T_directory = None, ignore_uninstalled: bool = False, coverage: float = None) -> bool:
+def check_all(
+    directory: T_directory = None, ignore_uninstalled: bool = False, coverage: float = None, badge: bool = None
+) -> bool:
     """
     Run all available checks.
 
     Args:
         directory: where to run the tools on (default is current dir)
         ignore_uninstalled: use --ignore-uninstalled to skip exit code 127 (command not found)
         coverage: pass to pytest()
+        badge: pass to pytest()
 
     """
     config = state.update_config(directory=directory)
     ignored_exit_codes = set()
     if ignore_uninstalled:
         ignored_exit_codes.add(EXIT_CODE_COMMAND_NOT_FOUND)
 
@@ -247,14 +270,15 @@
     exit_codes = []
     for tool in tools:
         a = [directory]
         kw = dict(_suppress=True, _ignore=ignored_exit_codes)
 
         if tool is pytest:  # pragma: no cover
             kw["coverage"] = coverage
+            kw["badge"] = badge
 
         exit_codes.append(tool(*a, **kw))
 
     if state.format == "json":
         dump_tools_with_results(tools, exit_codes)
 
     return any(exit_codes)
```

### Comparing `su6-0.6.0/src/su6/core.py` & `su6-0.7.0/src/su6/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,28 +209,39 @@
         return hash(self.value)
 
 
 DEFAULT_FORMAT = Format.text
 
 C = typing.TypeVar("C", bound=T_Command)
 
+DEFAULT_BADGE = "coverage.svg"
+
 
 @dataclass
 class Config:
     """
     Used as typed version of the [tool.su6] part of pyproject.toml.
 
     Also accessible via state.config
     """
 
     directory: str = "."
     pyproject: str = "pyproject.toml"
     include: typing.Optional[list[str]] = None
     exclude: typing.Optional[list[str]] = None
     coverage: typing.Optional[float] = None  # only relevant for pytest
+    badge: bool | str = False  # only relevant for pytest
+
+    def __post_init__(self) -> None:
+        """
+        Update the value of badge to the default path.
+        """
+        if self.badge is True:  # pragma: no cover
+            # no cover because pytest can't test pytest :C
+            self.badge = DEFAULT_BADGE
 
     def determine_which_to_run(self, options: list[C]) -> list[C]:
         """
         Filter out any includes/excludes from pyproject.toml (first check include, then exclude).
         """
         if self.include:
             return [_ for _ in options if _.__name__ in self.include]
```

### Comparing `su6-0.6.0/tests/test_cli.py` & `su6-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/tests/test_core.py` & `su6-0.7.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/LICENSE.txt` & `su6-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-0.6.0/README.md` & `su6-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # su6-checker
 
 [![PyPI - Version](https://img.shields.io/pypi/v/su6.svg)](https://pypi.org/project/su6)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)  
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
+[![su6 checks](https://github.com/robinvandernoord/su6-checker/actions/workflows/su6.yml/badge.svg)](https://github.com/robinvandernoord/su6-checker/actions)
+![coverage.svg](coverage.svg)
 
 -----
 su6 (6 is pronounced as '/zɛs/' in Dutch, so 'su6' is basically 'success')  
 This package will hopefully help achieve that!
 
 **Table of Contents**
 
@@ -70,15 +74,15 @@
 - use: `su6 pydocstyle [directory]`
 - functionality: docstring checker
 - pypi: [pydocstyle](https://pypi.org/project/pydocstyle/)
 
 ### pytest
 
 - install: `pip install su6[pytest]`
-- use: `su6 pytest [directory] [--coverage <int>] [--json] [--html]`
+- use: `su6 pytest [directory] [--coverage <int>] [--json] [--html] [--badge <path>]`
 - functionality: tester with coverage
 - pypi: [pytest](https://pypi.org/project/pytest/), [pytest-cov](https://pypi.org/project/pytest-cov/)
 
 ## Usage
 
 ```console
 su6 --help
@@ -92,31 +96,34 @@
 `verbosity` indicates how much information you want to see (default is '2').  
 `config` allows you to select a different `.toml` file (default is `pyproject.toml`).  
 `format` allows you to get a JSON output instead of the textual traffic lights (default is `text`).  
 `directory` is the location you want to run the scans (default is current directory);  
 In the case of `black` and `isort`, another optional parameter `--fix` can be passed.
 This will allow the tools to do the suggested changes (if applicable).
 Running `su6 fix` will run both these tools with the `--fix` flag.  
-For `pytest`, `--json`, `--html` and `--coverage <int>` are supported. The latter can also be configured in the
-pyproject.toml (see ['Configuration'](#configuration)).
+For `pytest`, `--json`, `--html`, `--badge <str>` and `--coverage <int>` are supported. 
+The latter two can also be configured in the pyproject.toml (see ['Configuration'](#configuration)).
 The first two arguments can be used to control the output format of `pytest --cov`. Both options can be used at the same
 time. The `--coverage` flag can be used to set a threshold for code coverage %. If the coverage is less than this
-threshold, the check will fail.
+threshold, the check will fail. 
+If `badge` is set using cli or toml config, a SVG badge with the coverage % will be generated. 
+This badge can be used in for example the README.md.
 
 ### Configuration
 
 In your `pyproject.toml`, you can add a `[tools.su6]` section to configure some of the behavior of this tools.
 Currently, the following keys are supported:
 
 ```toml
 [tool.su6]
 directory = "." # string path to the directory on which to run all tools, e.g. 'src'
 include = [] # list of checks to run (when calling `su6 all`), e.g. ['black', 'mypy']
 exclude = [] # list of checks to skip (when calling `su6 all`), e.g. ['bandit']
 coverage = 100 # int threshold for pytest coverage 
+badge = "coverage.svg"  # str path or bool (true | false) whether and where to output the coverage badge
 ```
 
 All keys are optional. Note that if you have both an `include` as well as an `exclude`, all the tools in `include` will
 run and `exclude` will be fully ignored.
 
 ### Github Action
```

### Comparing `su6-0.6.0/pyproject.toml` & `su6-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "mypy",
     "ruff",
     "bandit",
     "isort",
     "pydocstyle",
     "pytest",
     "pytest-cov",
+    "coverage-badge",
 ]
 
 black = [
     "black"
 ]
 
 mypy = [
@@ -66,14 +67,15 @@
 pydocstyle = [
     "pydocstyle"
 ]
 
 pytest = [
     "pytest",
     "pytest-cov",
+    "coverage-badge",
 ]
 
 dev = [
     "hatch",
     "python-semantic-release",
 ]
 
@@ -98,14 +100,15 @@
 
 ### required in every su6 pyproject: ###
 [tool.su6]
 directory = "src"
 include = []
 exclude = []
 coverage = 99
+badge = true
 
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
```

### Comparing `su6-0.6.0/PKG-INFO` & `su6-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python cli tool to use tools for some common code quality checks (opinionated)
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-checker#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-checker/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-checker
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,14 +18,15 @@
 Requires-Dist: black
 Requires-Dist: plumbum
 Requires-Dist: typeguard
 Requires-Dist: typer[all]
 Provides-Extra: all
 Requires-Dist: bandit; extra == 'all'
 Requires-Dist: black; extra == 'all'
+Requires-Dist: coverage-badge; extra == 'all'
 Requires-Dist: isort; extra == 'all'
 Requires-Dist: mypy; extra == 'all'
 Requires-Dist: pydocstyle; extra == 'all'
 Requires-Dist: pytest; extra == 'all'
 Requires-Dist: pytest-cov; extra == 'all'
 Requires-Dist: ruff; extra == 'all'
 Provides-Extra: bandit
@@ -38,24 +39,29 @@
 Provides-Extra: isort
 Requires-Dist: isort; extra == 'isort'
 Provides-Extra: mypy
 Requires-Dist: mypy; extra == 'mypy'
 Provides-Extra: pydocstyle
 Requires-Dist: pydocstyle; extra == 'pydocstyle'
 Provides-Extra: pytest
+Requires-Dist: coverage-badge; extra == 'pytest'
 Requires-Dist: pytest; extra == 'pytest'
 Requires-Dist: pytest-cov; extra == 'pytest'
 Provides-Extra: ruff
 Requires-Dist: ruff; extra == 'ruff'
 Description-Content-Type: text/markdown
 
 # su6-checker
 
 [![PyPI - Version](https://img.shields.io/pypi/v/su6.svg)](https://pypi.org/project/su6)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/su6.svg)](https://pypi.org/project/su6)  
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
+[![su6 checks](https://github.com/robinvandernoord/su6-checker/actions/workflows/su6.yml/badge.svg)](https://github.com/robinvandernoord/su6-checker/actions)
+![coverage.svg](coverage.svg)
 
 -----
 su6 (6 is pronounced as '/zɛs/' in Dutch, so 'su6' is basically 'success')  
 This package will hopefully help achieve that!
 
 **Table of Contents**
 
@@ -120,15 +126,15 @@
 - use: `su6 pydocstyle [directory]`
 - functionality: docstring checker
 - pypi: [pydocstyle](https://pypi.org/project/pydocstyle/)
 
 ### pytest
 
 - install: `pip install su6[pytest]`
-- use: `su6 pytest [directory] [--coverage <int>] [--json] [--html]`
+- use: `su6 pytest [directory] [--coverage <int>] [--json] [--html] [--badge <path>]`
 - functionality: tester with coverage
 - pypi: [pytest](https://pypi.org/project/pytest/), [pytest-cov](https://pypi.org/project/pytest-cov/)
 
 ## Usage
 
 ```console
 su6 --help
@@ -142,31 +148,34 @@
 `verbosity` indicates how much information you want to see (default is '2').  
 `config` allows you to select a different `.toml` file (default is `pyproject.toml`).  
 `format` allows you to get a JSON output instead of the textual traffic lights (default is `text`).  
 `directory` is the location you want to run the scans (default is current directory);  
 In the case of `black` and `isort`, another optional parameter `--fix` can be passed.
 This will allow the tools to do the suggested changes (if applicable).
 Running `su6 fix` will run both these tools with the `--fix` flag.  
-For `pytest`, `--json`, `--html` and `--coverage <int>` are supported. The latter can also be configured in the
-pyproject.toml (see ['Configuration'](#configuration)).
+For `pytest`, `--json`, `--html`, `--badge <str>` and `--coverage <int>` are supported. 
+The latter two can also be configured in the pyproject.toml (see ['Configuration'](#configuration)).
 The first two arguments can be used to control the output format of `pytest --cov`. Both options can be used at the same
 time. The `--coverage` flag can be used to set a threshold for code coverage %. If the coverage is less than this
-threshold, the check will fail.
+threshold, the check will fail. 
+If `badge` is set using cli or toml config, a SVG badge with the coverage % will be generated. 
+This badge can be used in for example the README.md.
 
 ### Configuration
 
 In your `pyproject.toml`, you can add a `[tools.su6]` section to configure some of the behavior of this tools.
 Currently, the following keys are supported:
 
 ```toml
 [tool.su6]
 directory = "." # string path to the directory on which to run all tools, e.g. 'src'
 include = [] # list of checks to run (when calling `su6 all`), e.g. ['black', 'mypy']
 exclude = [] # list of checks to skip (when calling `su6 all`), e.g. ['bandit']
 coverage = 100 # int threshold for pytest coverage 
+badge = "coverage.svg"  # str path or bool (true | false) whether and where to output the coverage badge
 ```
 
 All keys are optional. Note that if you have both an `include` as well as an `exclude`, all the tools in `include` will
 run and `exclude` will be fully ignored.
 
 ### Github Action
```

