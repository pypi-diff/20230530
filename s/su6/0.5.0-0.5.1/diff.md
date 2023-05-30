# Comparing `tmp/su6-0.5.0.tar.gz` & `tmp/su6-0.5.1.tar.gz`

## Comparing `su6-0.5.0.tar` & `su6-0.5.1.tar`

### file list

```diff
@@ -1,1296 +1,1298 @@
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 su6-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 su6-0.5.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    43198 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_socket.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_socket.meta.json
--rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_tracemalloc.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_tracemalloc.meta.json
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/atexit.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/atexit.meta.json
--rw-r--r--   0        0        0    50463 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/bdb.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/bdb.meta.json
--rw-r--r--   0        0        0    11205 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/cmd.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/cmd.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/colorsys.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/colorsys.meta.json
--rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/configparser.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/configparser.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/contextvars.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/contextvars.meta.json
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/copyreg.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/copyreg.meta.json
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    69838 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/fnmatch.data.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/fnmatch.meta.json
--rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/gc.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/gc.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/hashlib.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/hashlib.meta.json
--rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/hmac.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/hmac.meta.json
--rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/linecache.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/linecache.meta.json
--rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/locale.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/locale.meta.json
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mypy_extensions.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mypy_extensions.meta.json
--rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    92061 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pdb.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pdb.meta.json
--rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    31495 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pkgutil.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pkgutil.meta.json
--rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pty.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pty.meta.json
--rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pydoc.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pydoc.meta.json
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/queue.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/queue.meta.json
--rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/secrets.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/secrets.meta.json
--rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/selectors.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/selectors.meta.json
--rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/socket.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/socket.meta.json
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src.data.json
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ssl.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ssl.meta.json
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0    48902 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tracemalloc.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tracemalloc.meta.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    41964 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/zlib.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/zlib.meta.json
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_version.data.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_version.meta.json
--rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   160343 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/capture.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/capture.meta.json
--rw-r--r--   0        0        0    25774 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/compat.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/compat.meta.json
--rw-r--r--   0        0        0    31571 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    51347 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   151482 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    58440 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    62322 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/logging.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/logging.meta.json
--rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/main.data.json
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/main.meta.json
--rw-r--r--   0        0        0    25625 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    57543 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    35138 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   131434 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   116087 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/python.data.json
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/python.meta.json
--rw-r--r--   0        0        0    51104 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/python_api.data.json
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    30448 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    51011 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/reports.data.json
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/reports.meta.json
--rw-r--r--   0        0        0    40627 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/runner.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/scope.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/scope.meta.json
--rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/stash.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/stash.meta.json
--rw-r--r--   0        0        0    93209 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/timing.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/timing.meta.json
--rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    26825 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   163843 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    18735 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    61373 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0   100218 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    39840 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   110674 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/base_events.meta.json
--rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/events.data.json
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/events.meta.json
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/futures.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/futures.meta.json
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/locks.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/locks.meta.json
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/mixins.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/mixins.meta.json
--rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/queues.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/queues.meta.json
--rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/runners.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/runners.meta.json
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/streams.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/streams.meta.json
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/taskgroups.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json
--rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/threads.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/threads.meta.json
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/timeouts.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/timeouts.meta.json
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/transports.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/transports.meta.json
--rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/__init__.data.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/__init__.meta.json
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/_width_table.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/_width_table.meta.json
--rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/brackets.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/brackets.meta.json
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/cache.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/cache.meta.json
--rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/comments.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/comments.meta.json
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/concurrency.data.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/concurrency.meta.json
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/const.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/const.meta.json
--rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/files.data.json
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/files.meta.json
--rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
--rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/linegen.data.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/linegen.meta.json
--rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/lines.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/lines.meta.json
--rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/mode.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/mode.meta.json
--rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/nodes.data.json
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/nodes.meta.json
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/numerics.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/numerics.meta.json
--rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/output.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/output.meta.json
--rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/parsing.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/parsing.meta.json
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/report.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/report.meta.json
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/rusty.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/rusty.meta.json
--rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/strings.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/strings.meta.json
--rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/trans.data.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/black/trans.meta.json
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ctypes/wintypes.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/ctypes/wintypes.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/html/__init__.data.json
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/html/__init__.meta.json
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/html/entities.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/html/entities.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
--rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
--rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_text.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json
--rw-r--r--   0        0        0    44683 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/__init__.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/__init__.meta.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/_compat.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/_compat.meta.json
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/_punycode.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json
--rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/main.data.json
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/main.meta.json
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_block.data.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_core.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
--rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/renderer.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/renderer.meta.json
--rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/ruler.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/ruler.meta.json
--rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/token.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/token.meta.json
--rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/utils.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/utils.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/entities.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/utils.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/default.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
--rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/__init__.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_decode.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_decode.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_encode.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_encode.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_format.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_format.meta.json
--rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_parse.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_parse.meta.json
--rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_url.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/mdurl/_url.meta.json
--rw-r--r--   0        0        0    31386 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    27253 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    44423 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_parser.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_parser.meta.json
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    18021 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/markers.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/markers.meta.json
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/requirements.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/requirements.meta.json
--rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/__init__.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/__init__.meta.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/_meta.data.json
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/_meta.meta.json
--rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/gitignore.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/gitignore.meta.json
--rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/pathspec.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/pathspec.meta.json
--rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/pattern.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/pattern.meta.json
--rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/util.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/util.meta.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
--rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
--rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/__init__.meta.json
--rw-r--r--   0        0        0    24867 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/android.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/android.meta.json
--rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/api.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/api.meta.json
--rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/unix.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/unix.meta.json
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/version.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/platformdirs/version.meta.json
--rw-r--r--   0        0        0    11134 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pytest/__init__.data.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/pytest/__init__.meta.json
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/__init__.meta.json
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/__main__.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/__main__.meta.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_cell_widths.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_cell_widths.meta.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_emoji_codes.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_emoji_replace.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_export_format.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_export_format.meta.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_extension.data.json
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_extension.meta.json
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_fileno.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_fileno.meta.json
--rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_inspect.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_inspect.meta.json
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_log_render.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_log_render.meta.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_loop.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_loop.meta.json
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_null_file.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_null_file.meta.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_palettes.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_palettes.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_pick.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_pick.meta.json
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_ratio.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_ratio.meta.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_spinners.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_spinners.meta.json
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_stack.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_stack.meta.json
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_timer.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_timer.meta.json
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_win32_console.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_win32_console.meta.json
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_windows.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_windows.meta.json
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_windows_renderer.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_wrap.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/_wrap.meta.json
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/abc.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/abc.meta.json
--rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/align.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/align.meta.json
--rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/ansi.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/ansi.meta.json
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/box.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/box.meta.json
--rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/cells.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/cells.meta.json
--rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/color.data.json
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/color.meta.json
--rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/color_triplet.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/color_triplet.meta.json
--rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/columns.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/columns.meta.json
--rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/console.data.json
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/console.meta.json
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/constrain.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/constrain.meta.json
--rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/containers.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/containers.meta.json
--rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/control.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/control.meta.json
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/default_styles.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/default_styles.meta.json
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/emoji.data.json
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/emoji.meta.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/errors.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/errors.meta.json
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/file_proxy.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/file_proxy.meta.json
--rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/highlighter.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/highlighter.meta.json
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/json.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/json.meta.json
--rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/jupyter.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/jupyter.meta.json
--rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/live.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/live.meta.json
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/live_render.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/live_render.meta.json
--rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/markdown.data.json
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/markdown.meta.json
--rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/markup.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/markup.meta.json
--rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/measure.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/measure.meta.json
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/padding.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/padding.meta.json
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/pager.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/pager.meta.json
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/palette.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/palette.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/panel.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/panel.meta.json
--rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/pretty.data.json
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/pretty.meta.json
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/protocol.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/protocol.meta.json
--rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/region.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/region.meta.json
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/repr.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/repr.meta.json
--rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/rule.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/rule.meta.json
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/scope.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/scope.meta.json
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/screen.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/screen.meta.json
--rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/segment.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/segment.meta.json
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/spinner.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/spinner.meta.json
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/status.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/status.meta.json
--rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/style.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/style.meta.json
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/styled.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/styled.meta.json
--rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/syntax.data.json
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/syntax.meta.json
--rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/table.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/table.meta.json
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/terminal_theme.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/terminal_theme.meta.json
--rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/text.data.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/text.meta.json
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/theme.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/theme.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/themes.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/themes.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/traceback.data.json
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/rich/traceback.meta.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/__init__.data.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/__init__.meta.json
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/cli.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/cli.meta.json
--rw-r--r--   0        0        0    43826 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/core.data.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/src/su6/core.meta.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/__about__.data.json
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/__about__.meta.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/__init__.data.json
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/__init__.meta.json
--rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/cli.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/cli.meta.json
--rw-r--r--   0        0        0    44398 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/core.data.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6/core.meta.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/__about__.data.json
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/__about__.meta.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/__init__.data.json
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/__init__.meta.json
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/cli.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/cli.meta.json
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/core.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/su6_checker/core.meta.json
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tests/examples.data.json
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tests/examples.meta.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tests/examples/good.data.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/tests/examples/good.meta.json
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/__init__.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/__init__.meta.json
--rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_checkers.data.json
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_checkers.meta.json
--rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_config.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_config.meta.json
--rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_decorators.data.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_decorators.meta.json
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_exceptions.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json
--rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_functions.data.json
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_functions.meta.json
--rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_importhook.data.json
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_importhook.meta.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_memo.data.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_memo.meta.json
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_suppression.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_suppression.meta.json
--rw-r--r--   0        0        0    74681 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_transformer.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_transformer.meta.json
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_utils.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typeguard/_utils.meta.json
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/mock.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/mock.meta.json
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.5.0/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/10595a931c3c881e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1065c8b44fadc39a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/11f25cfda4e2f210
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/13985ae090677282
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1895bed4a0ed65d1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1996a22aec44a5c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1cfd31ba4b0b7ef9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1dcbdc62e66ccf0e
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1f88fbdfcbf2d8d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/1fbfdffa4078f509
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/23da3e9165a5513d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/247546336fc4bd59
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/248d23bfc4586461
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/24e2ebef92fa75b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/25d9504d2b6847d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/26657ed11f8e66de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/2a630c7d6d7faa40
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/2b0cdebce71424f0
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/2bf27b960bc3ded1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/2e4746b83d2d1cf8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/300f9a816018d49f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3271e344462a0ee3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/349f044f89b94587
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/34e1109d49bf09f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/35ab5ee4981cdf8c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/36e48551be186a66
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/380a13ecd1a2af25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/399d3b28a1a1db47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3a74e1b5704e9b3f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3c6b70c96e832bc1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3c9bb20c3b57bae
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3ca706f99b2d38bf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3cf13d9d13babf93
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3f10d9d7687f3999
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/3f12e7a3fe46c220
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/417040cdeaa7bd81
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/47ca38fe0242f05d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/49fafbbbbadedf00
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/4d5914600f7e99c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/4eaf3b155fae0dfb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/4f2c663677c63589
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/4f75816f4078d31b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/4f8371badac33c92
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/519ab6ce866ef11b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/54637ff0aaaaf6b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/552fa1eb2057eecc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/55c947c0fa59929
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/58240cde188220d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/5a6dc8ef65620223
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/5b7183ee842066de
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/5da466fd7e3b19f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/624348590d33bdc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6550bbd98b1711bd
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/684d0841c18787fb
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/68c4553df91c1f5e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/69bb9ea6355c0c25
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/69ffc3e7ad0aa6b4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6a4adfab73a8d4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6a74d0efd6350f1e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6b596d4ac1166741
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6b9f30172d33b6a3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6beed9d45ff1a491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6c989c6e4eea10bd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/6db20c27780d4a5f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/70963c0c68bf76ac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/70d6f3b95738758d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/729f212cc9c6cd5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/76d56794deeb084d
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7c37d34a0c059ec7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7c806e58272a88ea
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7cc3783d00621498
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7cf495b196c50222
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7dc27d897f910c11
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7f0f63895e369318
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/7f75cbd11ebac70a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/80844117d21fe12b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/80ded2016f4f413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/835f19fb8c240dbe
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/881c84062ed51136
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/886d14b97dbd4f2e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/89e58e5ee0d7d864
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/8a437c05421c6cb5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/8d2f83aae152de29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/8df3988e9368cbe6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/902eb6f99ee41131
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/9080aaa3f2416b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/922bfc03482db456
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/93fed7ae4120c88e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/945994955724de24
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/94ffcc82bc7ee370
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/968b32ac9319cc53
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/97a72bc70808d2f9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/98392e87ef3eb254
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/9db15fb6e71bec4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/9e3b1a7c0f34103b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/9e915e4e576201bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/9edacb4de19eeb8b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/a0572377dc282cac
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/a24edf91b0bcff12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/a3b201bbf3062966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/a8da9d8efa986532
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/a943564382aec90a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/aa2551751b9adb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/ab360402eb2d795e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/abc8db1325696a17
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/ac5b9f591ce9edec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/acecedeb9f4dd91a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/aff288abf6945582
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b03db5008e4f8099
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b2d26e3968f3c218
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b4228843afe3d2eb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b5f69f56d932f0d1
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b8d965aa2b8fd993
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/b990e7d90d89db2a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/bae3ebdf4629f324
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/bdd37795dc331d56
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/bdeb811362915192
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/be4a1815dbb4c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/beb37e84505d7dd0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c0d14d0162a80714
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c250dc207334d18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c293dd30723003b6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c6dc2ffa42b39365
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c766d7d105d53e92
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/c9d297807d108576
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/cb0e3b769b6a1727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/cbb8b9fccd8c8746
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/ccc4c37cd56e46e5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/d1c81941e3ef2e1d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/d1d63b74d8d929b9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/d2cceb9cc8265e7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/d3a20b1509715554
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/d9cd4c2a9ad4580d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/da4aff17737df0c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/dcb2ce27d1f7cc70
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/de1238012a6853f3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/dfc2e498a5736fb3
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e067c98663409f12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e59ac15827b7f1c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e832a8f80eaf16d4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e8ab3d919ff04fd9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e8cd5143f259cdce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/e98cf82519b9efc2
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/ec04e1ad73846b2a
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/ed03e948b89996b8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/f1af1d1ebb07ad61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/f41987c18d73e01d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/f586c8a0f5c58b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/f58e778cbde5b210
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/f9ab84e0c6669bed
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.0/.ruff_cache/content/fbd81c0d9b22b507
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_2602a302b50854cf___about___py.html
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_2602a302b50854cf___init___py.html
--rw-r--r--   0        0        0    76194 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_2602a302b50854cf_cli_py.html
--rw-r--r--   0        0        0   104474 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_2602a302b50854cf_core_py.html
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_a44f0ac069e85531__shared_py.html
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_about_py.html
--rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_core_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-0.5.0/htmlcov/style.css
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/bad.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/black_good_mypy_bad.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/except_pytest.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/good.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/invalid.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/only_black.toml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/only_mypy.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/bad.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/bad.meta.json
--rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/good.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/good.meta.json
--rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/this.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/this.meta.json
--rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-0.5.0/src/su6/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 su6-0.5.0/src/su6/__init__.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 su6-0.5.0/src/su6/cli.py
--rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 su6-0.5.0/src/su6/core.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-0.5.0/tests/_shared.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-0.5.0/tests/test_about.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 su6-0.5.0/tests/test_cli.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 su6-0.5.0/tests/test_core.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-0.5.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 su6-0.5.0/README.md
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 su6-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 su6-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 su6-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 su6-0.5.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    43198 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171935 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113933 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0   136385 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_socket.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_socket.meta.json
+-rw-r--r--   0        0        0    19707 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23865 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50433 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   150113 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137624 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/atexit.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/atexit.meta.json
+-rw-r--r--   0        0        0    50463 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/bdb.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/bdb.meta.json
+-rw-r--r--   0        0        0    11205 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1130458 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/cmd.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/cmd.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/colorsys.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/colorsys.meta.json
+-rw-r--r--   0        0        0   124134 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/configparser.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/configparser.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    37771 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/contextvars.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/contextvars.meta.json
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    11848 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/copyreg.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/copyreg.meta.json
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142212 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58295 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62910 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    69838 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27280 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/fnmatch.data.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/fnmatch.meta.json
+-rw-r--r--   0        0        0    88781 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132071 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    15964 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/gc.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/gc.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46194 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9508 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    31933 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/hashlib.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/hashlib.meta.json
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/hmac.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/hmac.meta.json
+-rw-r--r--   0        0        0   330892 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266313 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/linecache.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/linecache.meta.json
+-rw-r--r--   0        0        0    32512 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/locale.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/locale.meta.json
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    82542 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    78986 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    92061 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pdb.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pdb.meta.json
+-rw-r--r--   0        0        0    45135 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    31495 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pkgutil.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pkgutil.meta.json
+-rw-r--r--   0        0        0    34956 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pty.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pty.meta.json
+-rw-r--r--   0        0        0   103399 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pydoc.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pydoc.meta.json
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/queue.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/queue.meta.json
+-rw-r--r--   0        0        0    39910 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16739 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/secrets.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/secrets.meta.json
+-rw-r--r--   0        0        0    60874 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/selectors.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/selectors.meta.json
+-rw-r--r--   0        0        0    16500 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71116 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    49828 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/socket.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/socket.meta.json
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src.data.json
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   191473 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ssl.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ssl.meta.json
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27752 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   172772 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148679 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   140329 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19557 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43609 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49274 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57022 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0    48902 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tracemalloc.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tracemalloc.meta.json
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    41964 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0    33590 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23793 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142987 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    17116 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/zlib.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/zlib.meta.json
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    43242 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   160343 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    25774 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/compat.meta.json
+-rw-r--r--   0        0        0    31571 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    51347 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   151482 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    58440 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    62322 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    46849 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/main.data.json
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/main.meta.json
+-rw-r--r--   0        0        0    25625 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    57543 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    35138 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   131434 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   116087 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/python.data.json
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/python.meta.json
+-rw-r--r--   0        0        0    51104 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    30448 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    51011 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    40627 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    13964 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/stash.meta.json
+-rw-r--r--   0        0        0    93209 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    26825 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   163843 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    18735 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0    12813 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    61373 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    23038 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0   100218 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    39840 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   110674 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   104758 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    22606 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   202193 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/events.data.json
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    36802 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/locks.meta.json
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/mixins.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/mixins.meta.json
+-rw-r--r--   0        0        0    17263 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    23099 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/queues.meta.json
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    36129 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/taskgroups.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json
+-rw-r--r--   0        0        0   101522 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/threads.meta.json
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/timeouts.data.json
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/timeouts.meta.json
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    59017 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0    44356 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/__init__.data.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/__init__.meta.json
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/_width_table.data.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/_width_table.meta.json
+-rw-r--r--   0        0        0    29872 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/brackets.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/brackets.meta.json
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/cache.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/cache.meta.json
+-rw-r--r--   0        0        0    18459 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/comments.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/comments.meta.json
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/concurrency.data.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/concurrency.meta.json
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/const.data.json
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/const.meta.json
+-rw-r--r--   0        0        0    19016 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/files.data.json
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/files.meta.json
+-rw-r--r--   0        0        0    30758 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json
+-rw-r--r--   0        0        0    62396 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/linegen.data.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/linegen.meta.json
+-rw-r--r--   0        0        0    67820 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/lines.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/lines.meta.json
+-rw-r--r--   0        0        0    31369 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/mode.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/mode.meta.json
+-rw-r--r--   0        0        0    47653 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/nodes.data.json
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/nodes.meta.json
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/numerics.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/numerics.meta.json
+-rw-r--r--   0        0        0    10439 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/output.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/output.meta.json
+-rw-r--r--   0        0        0    14830 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/parsing.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/parsing.meta.json
+-rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/report.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/report.meta.json
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/rusty.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/rusty.meta.json
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/strings.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/strings.meta.json
+-rw-r--r--   0        0        0    79445 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/trans.data.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/black/trans.meta.json
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47482 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    45562 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   182278 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    56492 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27933 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17765 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    29241 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    34320 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    24111 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81791 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32799 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    72709 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    60949 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    54524 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79291 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/html/__init__.data.json
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/html/__init__.meta.json
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/html/entities.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/html/entities.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64630 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    21576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    94562 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    23200 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    23052 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0    44683 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0    15383 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14508 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   146666 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0    21110 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    24609 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0    23665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    29740 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    35846 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    12652 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    26345 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    31386 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    30645 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0    95597 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   148345 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    51413 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    19728 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    28886 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    67381 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    25551 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    23611 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    27253 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18588 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    44423 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    18021 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/markers.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/markers.meta.json
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    56569 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65871 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/__init__.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/__init__.meta.json
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/_meta.data.json
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/_meta.meta.json
+-rw-r--r--   0        0        0    17220 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/gitignore.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/gitignore.meta.json
+-rw-r--r--   0        0        0    21671 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/pathspec.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/pathspec.meta.json
+-rw-r--r--   0        0        0    16357 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/pattern.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/pattern.meta.json
+-rw-r--r--   0        0        0    41114 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/util.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/util.meta.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json
+-rw-r--r--   0        0        0    16189 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json
+-rw-r--r--   0        0        0    27042 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/__init__.meta.json
+-rw-r--r--   0        0        0    24867 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/android.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/android.meta.json
+-rw-r--r--   0        0        0    42264 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/api.data.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/api.meta.json
+-rw-r--r--   0        0        0    26330 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/unix.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/unix.meta.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/version.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/platformdirs/version.meta.json
+-rw-r--r--   0        0        0    11134 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/pytest/__init__.meta.json
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/__main__.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_extension.data.json
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15113 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_inspect.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_loop.data.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_loop.meta.json
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_pick.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_stack.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_stack.meta.json
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_timer.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_timer.meta.json
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_windows.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/abc.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/abc.meta.json
+-rw-r--r--   0        0        0    23487 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/align.data.json
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/align.meta.json
+-rw-r--r--   0        0        0    24861 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/ansi.data.json
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/ansi.meta.json
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/box.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/box.meta.json
+-rw-r--r--   0        0        0     8545 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/cells.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/cells.meta.json
+-rw-r--r--   0        0        0    54542 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/color.data.json
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/color.meta.json
+-rw-r--r--   0        0        0    20268 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11098 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/columns.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/columns.meta.json
+-rw-r--r--   0        0        0   175685 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/console.data.json
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/console.meta.json
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/constrain.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/constrain.meta.json
+-rw-r--r--   0        0        0    20235 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/containers.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/containers.meta.json
+-rw-r--r--   0        0        0    22423 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/control.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/control.meta.json
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/default_styles.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/emoji.data.json
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/errors.data.json
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/errors.meta.json
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/json.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/json.meta.json
+-rw-r--r--   0        0        0    10113 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29014 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/live.data.json
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/live.meta.json
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/live_render.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/live_render.meta.json
+-rw-r--r--   0        0        0    66647 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/markdown.data.json
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/markdown.meta.json
+-rw-r--r--   0        0        0    25650 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/markup.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/markup.meta.json
+-rw-r--r--   0        0        0    23459 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/measure.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/measure.meta.json
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/padding.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/padding.meta.json
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/pager.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/pager.meta.json
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/palette.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/palette.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/panel.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/panel.meta.json
+-rw-r--r--   0        0        0   112532 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/pretty.data.json
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/protocol.data.json
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/protocol.meta.json
+-rw-r--r--   0        0        0    15313 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/region.data.json
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/region.meta.json
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/repr.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/repr.meta.json
+-rw-r--r--   0        0        0     8791 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/rule.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/rule.meta.json
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/scope.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/scope.meta.json
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/screen.data.json
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/screen.meta.json
+-rw-r--r--   0        0        0    97190 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/segment.data.json
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/segment.meta.json
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/spinner.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/spinner.meta.json
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/status.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/status.meta.json
+-rw-r--r--   0        0        0    56326 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/style.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/style.meta.json
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/styled.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/styled.meta.json
+-rw-r--r--   0        0        0    76686 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/syntax.data.json
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/syntax.meta.json
+-rw-r--r--   0        0        0    77579 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/table.data.json
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/table.meta.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    86746 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/text.data.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/text.meta.json
+-rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/theme.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/theme.meta.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/themes.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/themes.meta.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/traceback.data.json
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/rich/traceback.meta.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/__init__.data.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/__init__.meta.json
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/cli.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/cli.meta.json
+-rw-r--r--   0        0        0    43826 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/core.data.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/src/su6/core.meta.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/__about__.data.json
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/__about__.meta.json
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/__init__.data.json
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/__init__.meta.json
+-rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/cli.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/cli.meta.json
+-rw-r--r--   0        0        0    44398 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/core.data.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6/core.meta.json
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/__about__.data.json
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/__about__.meta.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/__init__.data.json
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/__init__.meta.json
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/cli.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/cli.meta.json
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/core.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/su6_checker/core.meta.json
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tests/examples.data.json
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tests/examples.meta.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tests/examples/good.data.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/tests/examples/good.meta.json
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/__init__.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/__init__.meta.json
+-rw-r--r--   0        0        0    39482 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_checkers.data.json
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_checkers.meta.json
+-rw-r--r--   0        0        0    12462 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_config.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_config.meta.json
+-rw-r--r--   0        0        0    25402 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_decorators.data.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_decorators.meta.json
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_exceptions.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json
+-rw-r--r--   0        0        0    19231 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_functions.data.json
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_functions.meta.json
+-rw-r--r--   0        0        0    22567 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_importhook.data.json
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_importhook.meta.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_memo.data.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_memo.meta.json
+-rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_suppression.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_suppression.meta.json
+-rw-r--r--   0        0        0    74681 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_transformer.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_transformer.meta.json
+-rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_utils.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typeguard/_utils.meta.json
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11890 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    35710 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    48690 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    59399 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    69096 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    57432 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    33728 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   214118 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0   149188 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/mock.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/mock.meta.json
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175316 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 su6-0.5.1/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/10595a931c3c881e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1065c8b44fadc39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/11f25cfda4e2f210
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/13985ae090677282
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1895bed4a0ed65d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1996a22aec44a5c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1cfd31ba4b0b7ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1dcbdc62e66ccf0e
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1f88fbdfcbf2d8d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/1fbfdffa4078f509
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/23da3e9165a5513d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/247546336fc4bd59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/248d23bfc4586461
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/24e2ebef92fa75b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/25d9504d2b6847d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/26657ed11f8e66de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/2a630c7d6d7faa40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/2b0cdebce71424f0
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/2bf27b960bc3ded1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/2e4746b83d2d1cf8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/300f9a816018d49f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3271e344462a0ee3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/349f044f89b94587
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/34e1109d49bf09f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/35ab5ee4981cdf8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/36e48551be186a66
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/380a13ecd1a2af25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/399d3b28a1a1db47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3a74e1b5704e9b3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3c6b70c96e832bc1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3c9bb20c3b57bae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3ca706f99b2d38bf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3cf13d9d13babf93
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3f10d9d7687f3999
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/3f12e7a3fe46c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/417040cdeaa7bd81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/429010e306ea9808
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/47ca38fe0242f05d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/49fafbbbbadedf00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/4d5914600f7e99c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/4eaf3b155fae0dfb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/4f2c663677c63589
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/4f75816f4078d31b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/4f8371badac33c92
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/519ab6ce866ef11b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/54637ff0aaaaf6b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/552fa1eb2057eecc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/55c947c0fa59929
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/58240cde188220d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/5a6dc8ef65620223
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/5b7183ee842066de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/5da466fd7e3b19f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/624348590d33bdc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6550bbd98b1711bd
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/684d0841c18787fb
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/68c4553df91c1f5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/69bb9ea6355c0c25
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/69ffc3e7ad0aa6b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6a4adfab73a8d4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6a74d0efd6350f1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6b596d4ac1166741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6b9f30172d33b6a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6beed9d45ff1a491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6c989c6e4eea10bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/6db20c27780d4a5f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/70963c0c68bf76ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/70d6f3b95738758d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/729f212cc9c6cd5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/76d56794deeb084d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7c37d34a0c059ec7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7c806e58272a88ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7cc3783d00621498
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7cf495b196c50222
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7dc27d897f910c11
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7f0f63895e369318
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/7f75cbd11ebac70a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/80844117d21fe12b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/80ded2016f4f413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/835f19fb8c240dbe
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/881c84062ed51136
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/886d14b97dbd4f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/89e58e5ee0d7d864
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/8a437c05421c6cb5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/8d2f83aae152de29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/8df3988e9368cbe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/902eb6f99ee41131
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/9080aaa3f2416b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/922bfc03482db456
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/93fed7ae4120c88e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/945994955724de24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/94ffcc82bc7ee370
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/968b32ac9319cc53
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/97a72bc70808d2f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/98392e87ef3eb254
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/9db15fb6e71bec4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/9e3b1a7c0f34103b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/9e915e4e576201bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/9edacb4de19eeb8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/a0572377dc282cac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/a24edf91b0bcff12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/a3b201bbf3062966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/a8da9d8efa986532
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/a943564382aec90a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/aa2551751b9adb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/ab360402eb2d795e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/abc8db1325696a17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/ac5b9f591ce9edec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/acecedeb9f4dd91a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/aff288abf6945582
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b03db5008e4f8099
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b2d26e3968f3c218
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b4228843afe3d2eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b5f69f56d932f0d1
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b8d965aa2b8fd993
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/b990e7d90d89db2a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/bae3ebdf4629f324
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/bdd37795dc331d56
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/bdeb811362915192
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/be4a1815dbb4c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/beb37e84505d7dd0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c0d14d0162a80714
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c250dc207334d18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c293dd30723003b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c6dc2ffa42b39365
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c766d7d105d53e92
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/c9d297807d108576
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/cb0e3b769b6a1727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/cbb8b9fccd8c8746
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/ccc4c37cd56e46e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/d1c81941e3ef2e1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/d1d63b74d8d929b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/d2cceb9cc8265e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/d3a20b1509715554
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/d9cd4c2a9ad4580d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/da4aff17737df0c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/dcb2ce27d1f7cc70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/de1238012a6853f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/dfc2e498a5736fb3
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e067c98663409f12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e59ac15827b7f1c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e832a8f80eaf16d4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e8ab3d919ff04fd9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e8cd5143f259cdce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/e98cf82519b9efc2
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/ec04e1ad73846b2a
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/ed03e948b89996b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f1af1d1ebb07ad61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f41987c18d73e01d
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f4d6392808939633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f586c8a0f5c58b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f58e778cbde5b210
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/f9ab84e0c6669bed
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 su6-0.5.1/.ruff_cache/content/fbd81c0d9b22b507
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_2602a302b50854cf___about___py.html
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_2602a302b50854cf___init___py.html
+-rw-r--r--   0        0        0    76194 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_2602a302b50854cf_cli_py.html
+-rw-r--r--   0        0        0   104474 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_2602a302b50854cf_core_py.html
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_a44f0ac069e85531__shared_py.html
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_about_py.html
+-rw-r--r--   0        0        0    50861 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html
+-rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_core_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 su6-0.5.1/htmlcov/style.css
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/bad.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/black_good_mypy_bad.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/empty.toml
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/except_pytest.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/good.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/invalid.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/only_black.toml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/only_mypy.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180372 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52404 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18231 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23340 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60680 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/bad.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/bad.meta.json
+-rw-r--r--   0        0        0  1130416 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123321 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109208 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57749 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0    90127 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22392 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/good.data.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/good.meta.json
+-rw-r--r--   0        0        0    85341 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28771 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87492 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44397 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75201 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167549 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28484 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49745 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   162168 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148658 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/this.data.json
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/this.meta.json
+-rw-r--r--   0        0        0   239636 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432238 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57849 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407992 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128987 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12204 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79274 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30861 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70583 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91123 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350747 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 su6-0.5.1/src/su6/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 su6-0.5.1/src/su6/__init__.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 su6-0.5.1/src/su6/cli.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 su6-0.5.1/src/su6/core.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 su6-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 su6-0.5.1/tests/_shared.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 su6-0.5.1/tests/test_about.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 su6-0.5.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 su6-0.5.1/tests/test_core.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 su6-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 su6-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 su6-0.5.1/README.md
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 su6-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 su6-0.5.1/PKG-INFO
```

### Comparing `su6-0.5.0/CHANGELOG.md` & `su6-0.5.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.5.1 (2023-05-30)
+### Fix
+* **cov:** Forgot to add pytest-cov as dependency for 'all' ([`fef9b41`](https://github.com/robinvandernoord/su6-checker/commit/fef9b41543ecce11b8f157be8e7a5c5f59d6f248))
+
 ## v0.5.0 (2023-05-30)
 ### Feature
 * **pytest:** Add pytest with coverage options ([`979ff01`](https://github.com/robinvandernoord/su6-checker/commit/979ff01afec6ea80fbfd08d53a7002b7ec68364c))
 * **pytest:** Start adding pytest with tests, but WIP ([`27c5ccd`](https://github.com/robinvandernoord/su6-checker/commit/27c5ccde03173f1bef3deebc807445aed4c8f7e3))
 
 ### Documentation
 * **readme:** Updated readme to include pytest and new flag order (--verbosity and --config BEFORE subcommand) ([`5db347c`](https://github.com/robinvandernoord/su6-checker/commit/5db347c4c562ad2b11a521ee11ed15c689d497b1))
```

### Comparing `su6-0.5.0/.mypy_cache/3.11/__future__.data.json` & `su6-0.5.1/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/__future__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_ast.data.json` & `su6-0.5.1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_ast.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_bisect.data.json` & `su6-0.5.1/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_bisect.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_codecs.data.json` & `su6-0.5.1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.5.1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_csv.data.json` & `su6-0.5.1/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_csv.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.5.1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_decimal.data.json` & `su6-0.5.1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_decimal.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_operator.data.json` & `su6-0.5.1/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_operator.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_random.data.json` & `su6-0.5.1/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_random.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_socket.data.json` & `su6-0.5.1/.mypy_cache/3.11/_socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_socket.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_stat.data.json` & `su6-0.5.1/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_stat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_thread.data.json` & `su6-0.5.1/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_thread.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_tracemalloc.data.json` & `su6-0.5.1/.mypy_cache/3.11/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_tracemalloc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_warnings.data.json` & `su6-0.5.1/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_warnings.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_weakref.data.json` & `su6-0.5.1/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_weakref.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_weakrefset.data.json` & `su6-0.5.1/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_weakrefset.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/abc.data.json` & `su6-0.5.1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/abc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/argparse.data.json` & `su6-0.5.1/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/argparse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/array.data.json` & `su6-0.5.1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/array.meta.json` & `su6-0.5.1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ast.data.json` & `su6-0.5.1/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ast.meta.json` & `su6-0.5.1/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/atexit.data.json` & `su6-0.5.1/.mypy_cache/3.11/atexit.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/atexit.meta.json` & `su6-0.5.1/.mypy_cache/3.11/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/bdb.data.json` & `su6-0.5.1/.mypy_cache/3.11/bdb.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/bdb.meta.json` & `su6-0.5.1/.mypy_cache/3.11/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/bisect.data.json` & `su6-0.5.1/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/bisect.meta.json` & `su6-0.5.1/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/builtins.data.json` & `su6-0.5.1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/builtins.meta.json` & `su6-0.5.1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/cmd.data.json` & `su6-0.5.1/.mypy_cache/3.11/cmd.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/cmd.meta.json` & `su6-0.5.1/.mypy_cache/3.11/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/codecs.data.json` & `su6-0.5.1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/codecs.meta.json` & `su6-0.5.1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/colorsys.data.json` & `su6-0.5.1/.mypy_cache/3.11/colorsys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/colorsys.meta.json` & `su6-0.5.1/.mypy_cache/3.11/colorsys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/configparser.data.json` & `su6-0.5.1/.mypy_cache/3.11/configparser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/configparser.meta.json` & `su6-0.5.1/.mypy_cache/3.11/configparser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/contextlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/contextvars.data.json` & `su6-0.5.1/.mypy_cache/3.11/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/contextvars.meta.json` & `su6-0.5.1/.mypy_cache/3.11/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/copy.data.json` & `su6-0.5.1/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/copy.meta.json` & `su6-0.5.1/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/copyreg.data.json` & `su6-0.5.1/.mypy_cache/3.11/copyreg.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/copyreg.meta.json` & `su6-0.5.1/.mypy_cache/3.11/copyreg.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/csv.data.json` & `su6-0.5.1/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/csv.meta.json` & `su6-0.5.1/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.5.1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.5.1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/datetime.data.json` & `su6-0.5.1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/datetime.meta.json` & `su6-0.5.1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/decimal.data.json` & `su6-0.5.1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/decimal.meta.json` & `su6-0.5.1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/difflib.data.json` & `su6-0.5.1/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/difflib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/dis.data.json` & `su6-0.5.1/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/dis.meta.json` & `su6-0.5.1/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/doctest.data.json` & `su6-0.5.1/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/doctest.meta.json` & `su6-0.5.1/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/enum.data.json` & `su6-0.5.1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/enum.meta.json` & `su6-0.5.1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/errno.data.json` & `su6-0.5.1/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/errno.meta.json` & `su6-0.5.1/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/fnmatch.data.json` & `su6-0.5.1/.mypy_cache/3.11/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/fnmatch.meta.json` & `su6-0.5.1/.mypy_cache/3.11/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/fractions.data.json` & `su6-0.5.1/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/fractions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/functools.data.json` & `su6-0.5.1/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/functools.meta.json` & `su6-0.5.1/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/gc.data.json` & `su6-0.5.1/.mypy_cache/3.11/gc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/gc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/gc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/genericpath.data.json` & `su6-0.5.1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.5.1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/getpass.data.json` & `su6-0.5.1/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/getpass.meta.json` & `su6-0.5.1/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/gettext.data.json` & `su6-0.5.1/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/gettext.meta.json` & `su6-0.5.1/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/glob.data.json` & `su6-0.5.1/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/glob.meta.json` & `su6-0.5.1/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/good.data.json` & `su6-0.5.1/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/good.meta.json` & `su6-0.5.1/.mypy_cache/3.11/good.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'mtime'": '1685441179'}*

```diff
@@ -18,15 +18,15 @@
         "abc",
         "typing"
     ],
     "hash": "b8878b9730d0d4461b7ebcca5fc632335f9e2cf8bf18f3c92ad14904c58cb250",
     "id": "good",
     "ignore_all": false,
     "interface_hash": "c4bab6fc951abfdddc4e8cabee5d91278a319446b2f38fbd3f27805c1fce6039",
-    "mtime": 1685294287,
+    "mtime": 1685441179,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `su6-0.5.0/.mypy_cache/3.11/hashlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/hashlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/hashlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/hashlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/hmac.data.json` & `su6-0.5.1/.mypy_cache/3.11/hmac.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/hmac.meta.json` & `su6-0.5.1/.mypy_cache/3.11/hmac.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/inspect.data.json` & `su6-0.5.1/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/inspect.meta.json` & `su6-0.5.1/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/io.data.json` & `su6-0.5.1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/io.meta.json` & `su6-0.5.1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/itertools.data.json` & `su6-0.5.1/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/itertools.meta.json` & `su6-0.5.1/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/linecache.data.json` & `su6-0.5.1/.mypy_cache/3.11/linecache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/linecache.meta.json` & `su6-0.5.1/.mypy_cache/3.11/linecache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/locale.data.json` & `su6-0.5.1/.mypy_cache/3.11/locale.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/locale.meta.json` & `su6-0.5.1/.mypy_cache/3.11/locale.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/marshal.data.json` & `su6-0.5.1/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/marshal.meta.json` & `su6-0.5.1/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/math.data.json` & `su6-0.5.1/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/math.meta.json` & `su6-0.5.1/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mmap.data.json` & `su6-0.5.1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mmap.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/msvcrt.data.json` & `su6-0.5.1/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/msvcrt.meta.json` & `su6-0.5.1/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mypy_extensions.data.json` & `su6-0.5.1/.mypy_cache/3.11/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mypy_extensions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/numbers.data.json` & `su6-0.5.1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/numbers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/opcode.data.json` & `su6-0.5.1/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/opcode.meta.json` & `su6-0.5.1/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/operator.data.json` & `su6-0.5.1/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/operator.meta.json` & `su6-0.5.1/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pdb.data.json` & `su6-0.5.1/.mypy_cache/3.11/pdb.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pdb.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pickle.data.json` & `su6-0.5.1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pickle.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pkgutil.data.json` & `su6-0.5.1/.mypy_cache/3.11/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pkgutil.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platform.data.json` & `su6-0.5.1/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platform.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/posixpath.data.json` & `su6-0.5.1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.5.1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pprint.data.json` & `su6-0.5.1/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pprint.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pty.data.json` & `su6-0.5.1/.mypy_cache/3.11/pty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pty.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pydoc.data.json` & `su6-0.5.1/.mypy_cache/3.11/pydoc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pydoc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pydoc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/queue.data.json` & `su6-0.5.1/.mypy_cache/3.11/queue.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/queue.meta.json` & `su6-0.5.1/.mypy_cache/3.11/queue.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/random.data.json` & `su6-0.5.1/.mypy_cache/3.11/random.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/random.meta.json` & `su6-0.5.1/.mypy_cache/3.11/random.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/re.data.json` & `su6-0.5.1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/re.meta.json` & `su6-0.5.1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/reprlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/reprlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/secrets.data.json` & `su6-0.5.1/.mypy_cache/3.11/secrets.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/secrets.meta.json` & `su6-0.5.1/.mypy_cache/3.11/secrets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/selectors.data.json` & `su6-0.5.1/.mypy_cache/3.11/selectors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/selectors.meta.json` & `su6-0.5.1/.mypy_cache/3.11/selectors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/shlex.data.json` & `su6-0.5.1/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/shlex.meta.json` & `su6-0.5.1/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/shutil.data.json` & `su6-0.5.1/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/shutil.meta.json` & `su6-0.5.1/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/signal.data.json` & `su6-0.5.1/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/signal.meta.json` & `su6-0.5.1/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/socket.data.json` & `su6-0.5.1/.mypy_cache/3.11/socket.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/socket.meta.json` & `su6-0.5.1/.mypy_cache/3.11/socket.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src.data.json` & `su6-0.5.1/.mypy_cache/3.11/src.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src.meta.json` & `su6-0.5.1/.mypy_cache/3.11/src.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.5.1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.5.1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.5.1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.5.1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.5.1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ssl.data.json` & `su6-0.5.1/.mypy_cache/3.11/ssl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ssl.meta.json` & `su6-0.5.1/.mypy_cache/3.11/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/stat.data.json` & `su6-0.5.1/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/stat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/string.data.json` & `su6-0.5.1/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/string.meta.json` & `su6-0.5.1/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/struct.data.json` & `su6-0.5.1/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/struct.meta.json` & `su6-0.5.1/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/subprocess.data.json` & `su6-0.5.1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.5.1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sys.data.json` & `su6-0.5.1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sys.meta.json` & `su6-0.5.1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sysconfig.data.json` & `su6-0.5.1/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/sysconfig.meta.json` & `su6-0.5.1/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tempfile.data.json` & `su6-0.5.1/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tempfile.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/termios.data.json` & `su6-0.5.1/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/termios.meta.json` & `su6-0.5.1/.mypy_cache/3.11/termios.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/textwrap.data.json` & `su6-0.5.1/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/textwrap.meta.json` & `su6-0.5.1/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/this.data.json` & `su6-0.5.1/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/this.meta.json` & `su6-0.5.1/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/threading.data.json` & `su6-0.5.1/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/threading.meta.json` & `su6-0.5.1/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/time.data.json` & `su6-0.5.1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/time.meta.json` & `su6-0.5.1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/token.data.json` & `su6-0.5.1/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/token.meta.json` & `su6-0.5.1/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tokenize.data.json` & `su6-0.5.1/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tokenize.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tomllib.data.json` & `su6-0.5.1/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tomllib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/traceback.data.json` & `su6-0.5.1/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/traceback.meta.json` & `su6-0.5.1/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tracemalloc.data.json` & `su6-0.5.1/.mypy_cache/3.11/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tracemalloc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tty.data.json` & `su6-0.5.1/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tty.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/types.data.json` & `su6-0.5.1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/types.meta.json` & `su6-0.5.1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typing.data.json` & `su6-0.5.1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typing.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.5.1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unicodedata.data.json` & `su6-0.5.1/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unicodedata.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/uuid.data.json` & `su6-0.5.1/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/uuid.meta.json` & `su6-0.5.1/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/warnings.data.json` & `su6-0.5.1/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/warnings.meta.json` & `su6-0.5.1/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/weakref.data.json` & `su6-0.5.1/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/weakref.meta.json` & `su6-0.5.1/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/webbrowser.data.json` & `su6-0.5.1/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/webbrowser.meta.json` & `su6-0.5.1/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/zlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/zlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/zlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/zlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_argcomplete.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_argcomplete.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_version.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_version.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/cacheprovider.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/cacheprovider.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/capture.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/capture.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/debugging.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/debugging.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/deprecated.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/deprecated.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/doctest.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/doctest.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/fixtures.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/fixtures.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/freeze_support.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/freeze_support.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/helpconfig.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/helpconfig.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/hookspec.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/hookspec.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/legacypath.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/legacypath.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/logging.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/logging.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/main.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/main.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/monkeypatch.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/monkeypatch.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/nodes.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/nodes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/outcomes.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/outcomes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pathlib.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pathlib.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pytester.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pytester.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pytester_assertions.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/python.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/python.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/python_api.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/python_api.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/recwarn.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/recwarn.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/reports.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/reports.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/runner.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/runner.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/scope.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/scope.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/stash.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/stash.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/terminal.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/terminal.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/timing.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/timing.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/tmpdir.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/tmpdir.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/warning_types.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/warning_types.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/warnings.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/warnings.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/code.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/code.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/source.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_code/source.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/saferepr.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/truncate.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/util.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/assertion/util.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/argparsing.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/argparsing.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/exceptions.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/exceptions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/findpaths.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/config/findpaths.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/expression.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/expression.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/structures.data.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_pytest/mark/structures.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/base_events.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/base_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/base_events.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/base_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/coroutines.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/coroutines.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/coroutines.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/coroutines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/events.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/events.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/exceptions.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/exceptions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/futures.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/futures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/futures.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/futures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/locks.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/locks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/locks.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/locks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/mixins.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/mixins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/mixins.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/protocols.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/protocols.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/protocols.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/protocols.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/queues.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/queues.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/runners.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/runners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/runners.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/runners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/selector_events.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/selector_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/selector_events.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/selector_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/streams.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/streams.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/streams.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/streams.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/subprocess.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/subprocess.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/taskgroups.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/taskgroups.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/taskgroups.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/taskgroups.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/tasks.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/tasks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/tasks.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/tasks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/threads.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/threads.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/threads.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/threads.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/timeouts.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/timeouts.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/timeouts.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/timeouts.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/transports.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/transports.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/transports.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/transports.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/unix_events.data.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/unix_events.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/asyncio/unix_events.meta.json` & `su6-0.5.1/.mypy_cache/3.11/asyncio/unix_events.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/_width_table.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/_width_table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/_width_table.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/_width_table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/brackets.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/brackets.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/brackets.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/brackets.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/cache.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/cache.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/cache.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/cache.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/comments.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/comments.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/comments.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/comments.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/concurrency.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/concurrency.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/concurrency.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/concurrency.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/const.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/const.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/const.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/const.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/files.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/files.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/files.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/files.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/handle_ipynb_magics.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/handle_ipynb_magics.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/handle_ipynb_magics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/linegen.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/linegen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/linegen.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/linegen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/lines.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/lines.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/lines.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/lines.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/mode.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/mode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/mode.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/mode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/nodes.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/nodes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/nodes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/numerics.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/numerics.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/numerics.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/numerics.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/output.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/output.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/output.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/output.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/parsing.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/parsing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/parsing.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/parsing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/report.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/report.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/report.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/report.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/rusty.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/rusty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/rusty.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/rusty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/strings.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/strings.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/strings.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/strings.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/trans.data.json` & `su6-0.5.1/.mypy_cache/3.11/black/trans.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/black/trans.meta.json` & `su6-0.5.1/.mypy_cache/3.11/black/trans.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_termui_impl.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_termui_impl.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_textwrap.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/_textwrap.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/core.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/decorators.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/decorators.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/exceptions.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/exceptions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/formatting.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/formatting.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/globals.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/globals.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/globals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/parser.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/parser.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/shell_completion.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/shell_completion.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/termui.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/termui.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/termui.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/types.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/types.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/click/utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/click/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.5.1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/_base.data.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/_base.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/_base.meta.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/_base.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/process.data.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/process.meta.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/thread.data.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/thread.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/concurrent/futures/thread.meta.json` & `su6-0.5.1/.mypy_cache/3.11/concurrent/futures/thread.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ctypes/wintypes.data.json` & `su6-0.5.1/.mypy_cache/3.11/ctypes/wintypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/ctypes/wintypes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/ctypes/wintypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/charset.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/errors.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/header.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/header.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/message.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/message.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/policy.data.json` & `su6-0.5.1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.5.1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/html/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/html/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/html/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/html/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/html/entities.data.json` & `su6-0.5.1/.mypy_cache/3.11/html/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/html/entities.meta.json` & `su6-0.5.1/.mypy_cache/3.11/html/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/util.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/util.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_adapters.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_adapters.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_adapters.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_collections.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_collections.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_collections.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_collections.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_functools.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_functools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_functools.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_functools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_itertools.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_itertools.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_itertools.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_meta.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_meta.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_py39compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_py39compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_text.data.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/importlib_metadata/_text.meta.json` & `su6-0.5.1/.mypy_cache/3.11/importlib_metadata/_text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/_parse.data.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/_parse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/exceptions.data.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/iniconfig/exceptions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/decoder.data.json` & `su6-0.5.1/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/decoder.meta.json` & `su6-0.5.1/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/encoder.data.json` & `su6-0.5.1/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/json/encoder.meta.json` & `su6-0.5.1/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/logging/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/logging/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/_compat.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/_compat.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/_compat.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/_compat.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/_punycode.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/_punycode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/_punycode.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/_punycode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/main.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/main.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_block.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_block.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_core.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_inline.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/parser_inline.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/parser_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/renderer.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/renderer.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/ruler.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/ruler.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/ruler.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/ruler.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/token.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/token.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/token.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/token.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/entities.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/entities.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/entities.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/entities.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_blocks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_blocks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_re.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/html_re.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/html_re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/normalize_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/normalize_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/common/utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/common/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_destination.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_label.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/helpers/parse_link_title.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/commonmark.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/commonmark.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/default.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/default.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/default.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/default.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/zero.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/zero.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/presets/zero.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/presets/zero.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/blockquote.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/code.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/code.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/code.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/fence.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/fence.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/heading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/heading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/hr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/hr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/html_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/lheading.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/list.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/list.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/list.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/paragraph.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/reference.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/reference.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/state_block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/table.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_block/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/block.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/block.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/block.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/linkify.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/normalize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/replacements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/smartquotes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_core/state_core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/autolink.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/backticks.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/balance_pairs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/emphasis.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/entity.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/escape.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/html_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/image.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/image.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/link.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/link.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/newline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/state_inline.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/strikethrough.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/markdown_it/rules_inline/text_collapse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_decode.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_decode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_decode.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_decode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_encode.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_encode.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_encode.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_encode.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_format.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_format.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_parse.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_parse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_url.data.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_url.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/mdurl/_url.meta.json` & `su6-0.5.1/.mypy_cache/3.11/mdurl/_url.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/connection.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/connection.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/connection.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/connection.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/context.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/context.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/context.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/context.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/managers.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/managers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/managers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/managers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/pool.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/pool.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/pool.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/pool.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_fork.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_fork.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_fork.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_forkserver.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_posix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/popen_spawn_win32.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/process.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/process.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/process.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/process.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/queues.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/queues.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/queues.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/queues.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/reduction.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/reduction.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/reduction.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/reduction.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/shared_memory.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/shared_memory.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/shared_memory.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/sharedctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/sharedctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/spawn.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/spawn.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/spawn.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/spawn.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/synchronize.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/synchronize.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/synchronize.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/synchronize.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/util.data.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/multiprocessing/util.meta.json` & `su6-0.5.1/.mypy_cache/3.11/multiprocessing/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/os/path.data.json` & `su6-0.5.1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/os/path.meta.json` & `su6-0.5.1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_elffile.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_elffile.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_manylinux.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_musllinux.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_parser.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_parser.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_structures.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_structures.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_tokenizer.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/_tokenizer.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/markers.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/markers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/requirements.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/requirements.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/specifiers.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/specifiers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/tags.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/tags.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/version.data.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/packaging/version.meta.json` & `su6-0.5.1/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/_meta.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/_meta.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/gitignore.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/gitignore.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/gitignore.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/gitignore.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/pathspec.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/pathspec.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/pathspec.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/pathspec.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/pattern.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/pattern.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/pattern.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/pattern.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/util.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/util.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/util.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/util.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pathspec/patterns/gitwildmatch.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/android.data.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/android.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/android.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/android.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/api.data.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/api.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/api.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/api.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/unix.data.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/unix.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/unix.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/unix.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/version.data.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/version.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/platformdirs/version.meta.json` & `su6-0.5.1/.mypy_cache/3.11/platformdirs/version.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pytest/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/pytest/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/__main__.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/__main__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/__main__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/__main__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_cell_widths.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_cell_widths.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_cell_widths.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_cell_widths.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_emoji_codes.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_emoji_codes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_emoji_codes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_emoji_codes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_emoji_replace.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_emoji_replace.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_emoji_replace.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_emoji_replace.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_export_format.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_export_format.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_export_format.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_export_format.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_extension.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_extension.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_extension.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_extension.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_fileno.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_fileno.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_fileno.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_fileno.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_inspect.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_inspect.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_log_render.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_log_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_log_render.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_log_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_loop.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_loop.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_loop.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_loop.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_null_file.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_null_file.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_null_file.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_null_file.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_palettes.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_palettes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_palettes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_palettes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_pick.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_pick.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_pick.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_pick.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_ratio.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_ratio.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_ratio.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_ratio.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_spinners.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_spinners.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_spinners.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_spinners.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_stack.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_stack.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_stack.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_stack.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_timer.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_timer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_timer.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_timer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_win32_console.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_win32_console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_win32_console.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_win32_console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_windows.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_windows.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_windows.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_windows.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_windows_renderer.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_windows_renderer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_windows_renderer.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_windows_renderer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_wrap.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_wrap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/_wrap.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/_wrap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/abc.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/abc.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/align.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/align.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/align.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/align.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/ansi.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/ansi.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/ansi.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/ansi.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/box.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/box.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/box.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/box.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/cells.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/cells.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/cells.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/cells.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/color.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/color.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/color.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/color.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/color_triplet.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/color_triplet.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/color_triplet.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/color_triplet.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/columns.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/columns.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/columns.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/columns.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/console.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/console.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/console.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/console.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/constrain.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/constrain.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/constrain.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/constrain.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/containers.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/containers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/containers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/containers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/control.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/control.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/control.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/control.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/default_styles.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/default_styles.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/default_styles.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/default_styles.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/emoji.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/emoji.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/emoji.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/emoji.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/errors.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/errors.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/file_proxy.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/file_proxy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/file_proxy.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/file_proxy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/highlighter.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/highlighter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/highlighter.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/highlighter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/json.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/json.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/json.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/json.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/jupyter.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/jupyter.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/jupyter.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/jupyter.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/live.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/live.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/live.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/live.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/live_render.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/live_render.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/live_render.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/live_render.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/markdown.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/markdown.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/markdown.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/markdown.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/markup.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/markup.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/markup.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/markup.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/measure.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/measure.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/measure.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/measure.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/padding.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/padding.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/padding.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/padding.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/pager.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/pager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/pager.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/pager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/palette.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/palette.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/palette.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/palette.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/panel.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/panel.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/panel.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/panel.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/pretty.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/pretty.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/pretty.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/pretty.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/protocol.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/protocol.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/protocol.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/protocol.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/region.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/region.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/region.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/region.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/repr.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/repr.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/repr.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/repr.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/rule.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/rule.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/rule.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/rule.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/scope.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/scope.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/scope.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/scope.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/screen.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/screen.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/screen.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/screen.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/segment.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/segment.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/segment.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/segment.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/spinner.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/spinner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/spinner.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/spinner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/status.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/status.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/status.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/status.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/style.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/style.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/style.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/style.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/styled.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/styled.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/styled.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/styled.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/syntax.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/syntax.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/syntax.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/syntax.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/table.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/table.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/table.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/table.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/terminal_theme.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/terminal_theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/terminal_theme.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/terminal_theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/text.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/text.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/text.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/text.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/theme.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/theme.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/theme.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/theme.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/themes.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/themes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/themes.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/themes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/traceback.data.json` & `su6-0.5.1/.mypy_cache/3.11/rich/traceback.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/rich/traceback.meta.json` & `su6-0.5.1/.mypy_cache/3.11/rich/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/cli.data.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/cli.meta.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/core.data.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/src/su6/core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/src/su6/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/__about__.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/__about__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/cli.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/cli.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/core.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6/core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/__about__.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/__about__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/__about__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/cli.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/cli.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/cli.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/cli.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/core.data.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/su6_checker/core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/su6_checker/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tests/examples.data.json` & `su6-0.5.1/.mypy_cache/3.11/tests/examples.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tests/examples.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tests/examples.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tests/examples/good.data.json` & `su6-0.5.1/.mypy_cache/3.11/tests/examples/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/tests/examples/good.meta.json` & `su6-0.5.1/.mypy_cache/3.11/tests/examples/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_checkers.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_checkers.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_checkers.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_checkers.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_config.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_config.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_config.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_config.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_decorators.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_decorators.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_exceptions.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_exceptions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_exceptions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_functions.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_functions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_functions.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_functions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_importhook.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_importhook.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_importhook.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_importhook.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_memo.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_memo.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_memo.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_memo.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_suppression.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_suppression.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_suppression.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_suppression.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_transformer.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_transformer.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_transformer.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_transformer.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typeguard/_utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typeguard/_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_compat_utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_click7.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_click7.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_click8.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_shared.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_typing.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/_typing.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/colors.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/colors.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/completion.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/completion.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/core.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/core.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/core.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/main.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/main.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/models.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/models.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/models.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/params.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/params.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/params.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/rich_utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/rich_utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/utils.data.json` & `su6-0.5.1/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/typer/utils.meta.json` & `su6-0.5.1/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/_log.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/_log.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/async_case.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/async_case.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/case.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/case.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/loader.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/loader.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/main.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/main.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/mock.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/mock.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/mock.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/mock.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/result.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/result.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/runner.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/runner.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/signals.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/signals.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/suite.data.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/unittest/suite.meta.json` & `su6-0.5.1/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/urllib/__init__.data.json` & `su6-0.5.1/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/urllib/__init__.meta.json` & `su6-0.5.1/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/urllib/parse.data.json` & `su6-0.5.1/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.mypy_cache/3.11/urllib/parse.meta.json` & `su6-0.5.1/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.pytest_cache/v/cache/nodeids` & `su6-0.5.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/1f88fbdfcbf2d8d6` & `su6-0.5.1/.ruff_cache/content/1f88fbdfcbf2d8d6`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/2bf27b960bc3ded1` & `su6-0.5.1/.ruff_cache/content/2bf27b960bc3ded1`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/3f10d9d7687f3999` & `su6-0.5.1/.ruff_cache/content/3f10d9d7687f3999`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/684d0841c18787fb` & `su6-0.5.1/.ruff_cache/content/684d0841c18787fb`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/68c4553df91c1f5e` & `su6-0.5.1/.ruff_cache/content/68c4553df91c1f5e`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/881c84062ed51136` & `su6-0.5.1/.ruff_cache/content/881c84062ed51136`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/b8d965aa2b8fd993` & `su6-0.5.1/.ruff_cache/content/b8d965aa2b8fd993`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/b990e7d90d89db2a` & `su6-0.5.1/.ruff_cache/content/b990e7d90d89db2a`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/be4a1815dbb4c4` & `su6-0.5.1/.ruff_cache/content/be4a1815dbb4c4`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/e067c98663409f12` & `su6-0.5.1/.ruff_cache/content/e067c98663409f12`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/.ruff_cache/content/ed03e948b89996b8` & `su6-0.5.1/.ruff_cache/content/ed03e948b89996b8`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/coverage_html.js` & `su6-0.5.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_2602a302b50854cf___about___py.html` & `su6-0.5.1/htmlcov/d_2602a302b50854cf___about___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_2602a302b50854cf___init___py.html` & `su6-0.5.1/htmlcov/d_2602a302b50854cf___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_2602a302b50854cf_cli_py.html` & `su6-0.5.1/htmlcov/d_2602a302b50854cf_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_2602a302b50854cf_core_py.html` & `su6-0.5.1/htmlcov/d_2602a302b50854cf_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_a44f0ac069e85531___init___py.html` & `su6-0.5.1/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_a44f0ac069e85531__shared_py.html` & `su6-0.5.1/htmlcov/d_a44f0ac069e85531__shared_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_about_py.html` & `su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_about_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_cli_py.html` & `su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_cli_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/d_a44f0ac069e85531_test_core_py.html` & `su6-0.5.1/htmlcov/d_a44f0ac069e85531_test_core_py.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/favicon_32.png` & `su6-0.5.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/index.html` & `su6-0.5.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/keybd_closed.png` & `su6-0.5.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/keybd_open.png` & `su6-0.5.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/status.json` & `su6-0.5.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/htmlcov/style.css` & `su6-0.5.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/except_pytest.toml` & `su6-0.5.1/pytest_examples/except_pytest.toml`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ast.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ast.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_codecs.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_codecs.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ctypes.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/abc.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/abc.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/array.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/array.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/bad.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/bad.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/bad.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/bad.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/builtins.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/builtins.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/codecs.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/codecs.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/contextlib.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/contextlib.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/dataclasses.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/enum.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/enum.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/genericpath.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/genericpath.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/good.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/good.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/good.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/good.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/io.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/io.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/mmap.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/mmap.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/pathlib.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/pathlib.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/pickle.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/pickle.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/posixpath.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/posixpath.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/re.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/re.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_compile.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_constants.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_parse.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/subprocess.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/subprocess.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sys.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/sys.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/this.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/this.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/this.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/this.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/types.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/types.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/abc.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/charset.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/charset.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/errors.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/errors.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/header.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/header.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/message.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/message.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/policy.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/email/policy.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/__init__.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/path.data.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pytest_examples/.mypy_cache/3.11/os/path.meta.json` & `su6-0.5.1/pytest_examples/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/src/su6/cli.py` & `su6-0.5.1/src/su6/cli.py`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/src/su6/core.py` & `su6-0.5.1/src/su6/core.py`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/tests/test_cli.py` & `su6-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/tests/test_core.py` & `su6-0.5.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/LICENSE.txt` & `su6-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/README.md` & `su6-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `su6-0.5.0/pyproject.toml` & `su6-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "black",
     "mypy",
     "ruff",
     "bandit",
     "isort",
     "pydocstyle",
     "pytest",
+    "pytest-cov",
 ]
 
 black = [
     "black"
 ]
 
 mypy = [
```

### Comparing `su6-0.5.0/PKG-INFO` & `su6-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: su6
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python cli tool to use tools for some common code quality checks (opinionated)
 Project-URL: Documentation, https://github.com/robinvandernoord/su6-checker#readme
 Project-URL: Issues, https://github.com/robinvandernoord/su6-checker/issues
 Project-URL: Source, https://github.com/robinvandernoord/su6-checker
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -22,14 +22,15 @@
 Provides-Extra: all
 Requires-Dist: bandit; extra == 'all'
 Requires-Dist: black; extra == 'all'
 Requires-Dist: isort; extra == 'all'
 Requires-Dist: mypy; extra == 'all'
 Requires-Dist: pydocstyle; extra == 'all'
 Requires-Dist: pytest; extra == 'all'
+Requires-Dist: pytest-cov; extra == 'all'
 Requires-Dist: ruff; extra == 'all'
 Provides-Extra: bandit
 Requires-Dist: bandit; extra == 'bandit'
 Provides-Extra: black
 Requires-Dist: black; extra == 'black'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
```

