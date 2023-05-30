# Comparing `tmp/iydon-2023.3.1.tar.gz` & `tmp/iydon-2023.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iydon-2023.3.1.tar", max compression
+gzip compressed data, was "iydon-2023.3.2.tar", max compression
```

## Comparing `iydon-2023.3.1.tar` & `iydon-2023.3.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
--rw-r--r--   0        0        0      266 2023-03-21 14:55:32.483611 iydon-2023.3.1/iydon/__init__.py
--rw-r--r--   0        0        0       66 2023-03-21 14:54:40.262377 iydon-2023.3.1/iydon/base/__init__.py
--rw-r--r--   0        0        0      326 2023-03-23 18:49:05.372064 iydon-2023.3.1/iydon/base/constant.py
--rw-r--r--   0        0        0      905 2023-03-21 14:55:36.902346 iydon-2023.3.1/iydon/base/type.py
--rw-r--r--   0        0        0      150 2023-03-22 18:17:20.934552 iydon-2023.3.1/iydon/rust/__init__.py
--rw-r--r--   0        0        0       66 2023-03-22 10:08:40.715364 iydon-2023.3.1/iydon/rust/std/__init__.py
--rw-r--r--   0        0        0    15824 2023-03-22 17:56:38.822862 iydon-2023.3.1/iydon/rust/std/option.py
--rw-r--r--   0        0        0    16772 2023-03-23 08:09:43.753318 iydon-2023.3.1/iydon/rust/std/result.py
--rw-r--r--   0        0        0        0 2023-03-22 18:00:04.704606 iydon-2023.3.1/iydon/test/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 18:00:01.065676 iydon-2023.3.1/iydon/test/rust/__init__.py
--rw-r--r--   0        0        0      249 2023-03-22 18:01:34.738873 iydon-2023.3.1/iydon/test/rust/test_std.py
--rw-r--r--   0        0        0    35823 2022-05-01 07:51:55.316123 iydon-2023.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1562 2023-03-23 18:51:39.469811 iydon-2023.3.1/pyproject.toml
--rw-r--r--   0        0        0     7997 2023-03-21 03:16:42.021543 iydon-2023.3.1/README.md
--rw-r--r--   0        0        0     8770 2023-03-23 18:51:54.967283 iydon-2023.3.1/setup.py
--rw-r--r--   0        0        0     9042 2023-03-23 18:51:54.967283 iydon-2023.3.1/PKG-INFO
+-rw-r--r--   0        0        0      266 2023-03-28 14:28:37.296806 iydon-2023.3.2/iydon/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-21 14:54:40.262377 iydon-2023.3.2/iydon/base/__init__.py
+-rw-r--r--   0        0        0      326 2023-03-28 14:59:19.407554 iydon-2023.3.2/iydon/base/constant.py
+-rw-r--r--   0        0        0      817 2023-03-28 14:35:27.045363 iydon-2023.3.2/iydon/base/type.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:36:49.171772 iydon-2023.3.2/iydon/namespace/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:40:21.306083 iydon-2023.3.2/iydon/namespace/brief.py
+-rw-r--r--   0        0        0      226 2023-03-28 14:58:59.359564 iydon-2023.3.2/iydon/namespace/full.py
+-rw-r--r--   0        0        0      204 2023-03-28 14:41:46.533808 iydon-2023.3.2/iydon/namespace/private.py
+-rw-r--r--   0        0        0       78 2023-03-28 14:29:48.482416 iydon-2023.3.2/iydon/test/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-28 14:29:29.413206 iydon-2023.3.2/iydon/test/test_glhf.py
+-rw-r--r--   0        0        0      254 2023-03-28 14:28:08.272139 iydon-2023.3.2/iydon/test/test_rust.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:33:53.095849 iydon-2023.3.2/iydon/util/__init__.py
+-rw-r--r--   0        0        0       80 2023-03-27 10:26:00.514888 iydon-2023.3.2/iydon/util/glhf/__init__.py
+-rw-r--r--   0        0        0     1821 2023-03-28 14:24:40.190531 iydon-2023.3.2/iydon/util/glhf/end.py
+-rw-r--r--   0        0        0      262 2023-03-28 14:25:08.077434 iydon-2023.3.2/iydon/util/glhf/silver_bullet.py
+-rw-r--r--   0        0        0      150 2023-03-28 14:26:12.106703 iydon-2023.3.2/iydon/util/rust/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-28 14:25:49.036826 iydon-2023.3.2/iydon/util/rust/std/__init__.py
+-rw-r--r--   0        0        0    19368 2023-03-28 14:25:51.255666 iydon-2023.3.2/iydon/util/rust/std/option.py
+-rw-r--r--   0        0        0    21087 2023-03-28 14:27:54.803371 iydon-2023.3.2/iydon/util/rust/std/result.py
+-rw-r--r--   0        0        0    35823 2022-05-01 07:51:55.316123 iydon-2023.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     1668 2023-03-28 14:59:19.388320 iydon-2023.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8396 2023-03-23 19:03:38.960567 iydon-2023.3.2/README.md
+-rw-r--r--   0        0        0     9214 2023-03-28 14:59:27.260791 iydon-2023.3.2/setup.py
+-rw-r--r--   0        0        0     9438 2023-03-28 14:59:27.260791 iydon-2023.3.2/PKG-INFO
```

### Comparing `iydon-2023.3.1/iydon/rust/std/option.py` & `iydon-2023.3.2/iydon/util/rust/std/option.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __all__ = ['NONE', 'Option', 'Some']
 
 
 import copy
 import typing as t
 
-from ...base.type import Ta, Tb, Tc, Func0, Func1, Func2
+from ....base.type import Ta, Tb, Tc, Func0, Func1, Func2
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     from .result import Result
 
 
 class Option(t.Generic[Ta]):  # type: ignore [misc]
     '''Optional values.
 
-    Reference:
+    References:
         - https://doc.rust-lang.org/std/option/
         - https://doc.rust-lang.org/src/core/option.rs.html
         - https://github.com/iydon/iydon/blob/main/static/rust/option.rs
     '''
 
     __slots__ = ('_is_none', '_value')
     _none: t.Optional['te.Self[Ta]'] = None  # type: ignore [misc]
@@ -53,192 +53,299 @@
     @classmethod
     def none(cls) -> 'te.Self[Ta]':  # type: ignore [misc]
         if cls._none is None:
             cls._none = cls(None, True)
         return cls._none  # type: ignore [return-value]
 
     def is_some(self) -> bool:
-        '''Returns `true` if the option is a [`Some`] value.
+        '''Returns `true` if the option is a `Some` value.
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(2)
             >>> assert x.is_some()
 
             >>> x = Option.none()
             >>> assert not x.is_some()
         '''
         return not self.is_none()
 
     def is_some_and(self, f: Func1[Ta, bool]) -> bool:  # type: ignore [type-arg, valid-type]
-        '''Returns `true` if the option is a [`Some`] and the value inside of it matches a predicate.
+        '''Returns `true` if the option is a `Some` and the value inside of it matches a predicate.
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(2)
             >>> assert x.is_some_and(lambda x: x>1)
 
             >>> x = Option.some(0)
             >>> assert not x.is_some_and(lambda x: x>1)
 
             >>> x = Option.none()
             >>> assert not x.is_some_and(lambda x: x>1)
         '''
         return self.is_some() and f(self._value)
 
     def is_none(self) -> bool:
-        '''Returns `true` if the option is a [`None`] value.
+        '''Returns `true` if the option is a `None` value.
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> x = Option.some(2)
             >>> assert not x.is_none()
 
             >>> x = Option.none()
             >>> assert x.is_none()
         '''
         return self._is_none
 
     def expect(self, msg: str) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Some`] value, consuming the `self` value.
+        '''Returns the contained `Some` value, consuming the `self` value.
+
+        Args:
+            msg: ...
+
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the value is a `None` with a custom panic message provided by `msg`.
 
-        Example:
+        Examples:
             >>> x = Option.some('value')
             >>> assert x.expect('fruits are healthy') == 'value'
 
             >>> x = Option.none()
             >>> x.expect('fruits are healthy')
             Traceback (most recent call last):
                 ...
             AssertionError: fruits are healthy
         '''
         assert self.is_some(), msg
 
         return self._value
 
     def unwrap(self) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Some`] value, consuming the `self` value.
+        '''Returns the contained `Some` value, consuming the `self` value.
 
-        Example:
+        Because this function may panic, its use is generally discouraged.
+        Instead, prefer to use pattern matching and handle the `None`
+        case explicitly, or call `unwrap_or`, `unwrap_or_else`.
+
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the self value equals `None`.
+
+        Examples:
             >>> x = Option.some('air')
             >>> assert x.unwrap() == 'air'
 
             >>> x = Option.none()
             >>> x.unwrap()
             Traceback (most recent call last):
                 ...
             AssertionError: called `Option::unwrap()` on a `None` value
         '''
         return self.expect('called `Option::unwrap()` on a `None` value')
 
     def unwrap_or(self, default: Ta) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Some`] value or a provided default.
+        '''Returns the contained `Some` value or a provided default.
+
+        Arguments passed to `unwrap_or` are eagerly evaluated; if you are passing
+        the result of a function call, it is recommended to use `unwrap_or_else`,
+        which is lazily evaluated.
 
-        Example:
+        Args:
+            default: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> assert Option.some('car').unwrap_or('bike') == 'car'
             >>> assert Option.none().unwrap_or('bike') == 'bike'
         '''
         return self._match(lambda v: v, lambda: default)
 
     def unwrap_or_else(self, f: Func0[Ta]) -> Ta:  # type: ignore [type-arg, valid-type]
-        '''Returns the contained [`Some`] value or computes it from a closure.
+        '''Returns the contained `Some` value or computes it from a closure.
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> k = 10
             >>> assert Option.some(4).unwrap_or_else(lambda: 2*k) == 4
             >>> assert Option.none().unwrap_or_else(lambda: 2*k) == 20
         '''
         return self._match(lambda v: v, f)
 
     def map(self, f: Func1[Ta, Tb]) -> 'te.Self[Tb]':  # type: ignore [misc, type-arg, valid-type]
         '''Maps an `Option<T>` to `Option<U>` by applying a function to a contained value (if `Some`) or returns `None` (if `None`).
 
-        Example:
+        Args:
+            f: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> maybe_some_string = Option.some('Hello, World!')
             >>> maybe_some_len = maybe_some_string.map(len)
             >>> assert maybe_some_len == Option.some(13)
 
             >>> x = Option.none()
             >>> assert x.map(len) == Option.none()
         '''
         # TODO: self.some or self.new?
         return self._match(lambda v: self.some(f(v)), lambda: self)
 
     def inspect(self, f: Func1[Ta, None]) -> 'te.Self[Ta]':  # type: ignore [misc, type-arg, valid-type]
-        '''Calls the provided closure with a reference to the contained value (if [`Some`]).
+        '''Calls the provided closure with a reference to the contained value (if `Some`).
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(4).inspect(lambda x: print(f'got: {x}'))
             got: 4
 
             >>> x = Option.none().inspect(lambda x: print(f'got: {x}'))
         '''
         if self.is_some():
             f(self._value)
         return self
 
     def map_or(self, default: Tb, f: Func1[Ta, Tb]) -> Tb:  # type: ignore [type-arg, valid-type]
-        '''Returns the provided default result (if none), or applies a function to the contained value (if any).
+        '''Returns the provided default result (if none),
+            or applies a function to the contained value (if any).
+
+        Arguments passed to `map_or` are eagerly evaluated; if you are passing
+        the result of a function call, it is recommended to use `map_or_else`,
+        which is lazily evaluated.
+
+        Args:
+            default: ...
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some('foo')
             >>> assert x.map_or(42, len) == 3
 
             >>> x = Option.none()
             >>> assert x.map_or(42, len) == 42
         '''
         return self._match(lambda v: f(v), lambda: default)
 
     def map_or_else(self, default: Func0[Tb], f: Func1[Ta, Tb]) -> Tb:  # type: ignore [type-arg, valid-type]
-        '''Computes a default function result (if none), or applies a different function to the contained value (if any).
+        '''Computes a default function result (if none),
+            or applies a different function to the contained value (if any).
+
+        Args:
+            default: ...
+            f: ...
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> k = 21
 
             >>> x = Option.some('foo')
             >>> assert x.map_or_else(lambda: 2*k, len) == 3
 
             >>> x = Option.none()
             >>> assert x.map_or_else(lambda: 2*k, len) == 42
         '''
         return self._match(lambda v: f(v), default)
 
     def ok_or(self, err: Tb) -> 'Result[Ta, Tb]':  # type: ignore [type-arg, valid-type]
-        '''Transforms the `Option<T>` into a [`Result<T, E>`], mapping [`Some(v)`] to [`Ok(v)`] and [`None`] to [`Err(err)`].
+        '''Transforms the `Option<T>` into a `Result<T, E>`, mapping `Some(v)` to
+            `Ok(v)` and `None` to `Err(err)`.
+
+        Arguments passed to `ok_or` are eagerly evaluated; if you are passing the
+        result of a function call, it is recommended to use `ok_or_else`, which is
+        lazily evaluated.
+
+        Args:
+            err: ...
+
+        Returns:
+            ans: ...
 
-        Example:
-            >>> from iydon.rust.std.result import Result
+        Examples:
+            >>> from iydon.util.rust.std.result import Result
 
             >>> x = Option.some('foo')
             >>> assert x.ok_or(0) == Result.ok('foo')
 
             >>> x = Option.none()
             >>> assert x.ok_or(0) == Result.err(0)
         '''
         from .result import Result
 
         return self._match(lambda v: Result.ok(v), lambda: Result.err(err))
 
     def ok_or_else(self, err: Func0[Tb]) -> 'Result[Ta, Tb]':  # type: ignore [type-arg, valid-type]
-        '''Transforms the `Option<T>` into a [`Result<T, E>`], mapping [`Some(v)`] to [`Ok(v)`] and [`None`] to [`Err(err())`].
+        '''Transforms the `Option<T>` into a `Result<T, E>`, mapping `Some(v)` to
+            `Ok(v)` and `None` to `Err(err())`.
 
-        Example:
-            >>> from iydon.rust.std.result import Result
+        Args:
+            err: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
+            >>> from iydon.util.rust.std.result import Result
 
             >>> x = Option.some('foo')
             >>> assert x.ok_or_else(lambda: 0) == Result.ok('foo')
 
             >>> x = Option.none()
             >>> assert x.ok_or_else(lambda: 0) == Result.err(0)
         '''
         from .result import Result
 
         return self._match(lambda v: Result.ok(v), lambda: Result.err(err()))
 
     def and_(self, optb: 'te.Self[Tb]') -> 'te.Self[Tb]':  # type: ignore [misc]
-        '''Returns [`None`] if the option is [`None`], otherwise returns `optb`.
+        '''Returns `None` if the option is `None`, otherwise returns `optb`.
+
+        Arguments passed to `and` are eagerly evaluated; if you are passing the
+        result of a function call, it is recommended to use `and_then`, which is
+        lazily evaluated.
+
+        Args:
+            optb: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(2)
             >>> y = Option.none()
             >>> assert x.and_(y) == Option.none()
 
             >>> x = Option.none()
             >>> y = Option.some('foo')
             >>> assert x.and_(y) == Option.none()
@@ -250,17 +357,26 @@
             >>> x = Option.none()
             >>> y = Option.none()
             >>> assert x.and_(y) == Option.none()
         '''
         return self._match(lambda v: optb, lambda: self)
 
     def and_then(self, f: Func1[Ta, 'te.Self[Tb]']) -> 'te.Self[Tb]':  # type: ignore [misc, type-arg, valid-type]
-        '''Returns [`None`] if the option is [`None`], otherwise calls `f` with the wrapped value and returns the result.
+        '''Returns `None` if the option is `None`, otherwise calls `f` with the
+            wrapped value and returns the result.
+
+        Some languages call this operation flatmap.
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> u32 = int
             >>> def sq_then_to_string(x: u32) -> Option[str]:
             ...     # u32::checked_mul
             ...     if 0 <= x < 65536:
             ...         ans = Option.some(x*x)
             ...     else:
             ...         ans = Option.none()
@@ -269,19 +385,27 @@
             >>> assert Option.some(2).and_then(sq_then_to_string) == Option.some('4')
             >>> assert Option.some(1_000_000).and_then(sq_then_to_string) == Option.none()  # overflowed!
             >>> assert Option.none().and_then(sq_then_to_string) == Option.none()
         '''
         return self._match(lambda v: f(v), lambda: self)
 
     def filter(self, predicate: Func1[Ta, bool]) -> 'te.Self[Ta]':  # type: ignore [misc, type-arg, valid-type]
-        '''Returns [`None`] if the option is [`None`], otherwise calls `predicate` with the wrapped value and returns:
-        - [`Some(t)`] if `predicate` returns `true` (where `t` is the wrapped value), and
-        - [`None`] if `predicate` returns `false`.
+        '''Returns `None` if the option is `None`, otherwise calls `predicate`
+            with the wrapped value and returns:
+
+        - `Some(t)` if `predicate` returns `true` (where `t` is the wrapped value), and
+        - `None` if `predicate` returns `false`.
+
+        Args:
+            predicate: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> def is_even(n: int) -> bool:
             ...     return n % 2 == 0
 
             >>> assert Option.none().filter(is_even) == Option.none()
             >>> assert Option.some(3).filter(is_even) == Option.none()
             >>> assert Option.some(4).filter(is_even) == Option.some(4)
         '''
@@ -289,15 +413,25 @@
             if predicate(self._value):
                 return self
         return self.none()
 
     def or_(self, optb: 'te.Self[Ta]') -> 'te.Self[Ta]':  # type: ignore [misc]
         '''Returns the option if it contains a value, otherwise returns `optb`.
 
-        Example:
+        Arguments passed to `or` are eagerly evaluated; if you are passing the
+        result of a function call, it is recommended to use `or_else`, which is
+        lazily evaluated.
+
+        Args:
+            optb: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(2)
             >>> y = Option.none()
             >>> assert x.or_(y) == Option.some(2)
 
             >>> x = Option.none()
             >>> y = Option.some(100)
             >>> assert x.or_(y) == Option.some(100)
@@ -309,30 +443,43 @@
             >>> x = Option.none()
             >>> y = Option.none()
             >>> assert x.or_(y) == Option.none()
         '''
         return self._match(lambda v: self, lambda: optb)
 
     def or_else(self, f: Func0['te.Self[Ta]']) -> 'te.Self[Ta]':  # type: ignore [misc, type-arg]
-        '''Returns the option if it contains a value, otherwise calls `f` and returns the result.
+        '''Returns the option if it contains a value, otherwise calls `f` and
+            returns the result.
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> def nobody() -> Option[str]: return Option.none()
             >>> def vikings() -> Option[str]: return Option.some('vikings')
 
             >>> assert Option.some('barbarians').or_else(vikings) == Option.some('barbarians')
             >>> assert Option.none().or_else(vikings) == Option.some('vikings')
             >>> assert Option.none().or_else(nobody) == Option.none()
         '''
         return self._match(lambda v: self, f)
 
-    def xor(self, opt: 'te.Self[Ta]') -> 'te.Self[Ta]':  # type: ignore [misc]
-        '''Returns [`Some`] if exactly one of `self`, `optb` is [`Some`], otherwise returns [`None`].
+    def xor(self, optb: 'te.Self[Ta]') -> 'te.Self[Ta]':  # type: ignore [misc]
+        '''Returns `Some` if exactly one of `self`, `optb` is `Some`, otherwise returns `None`.
+
+        Args:
+            optb: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(2)
             >>> y = Option.none()
             >>> assert x.xor(y) == Option.some(2)
 
             >>> x = Option.none()
             >>> y = Option.some(2)
             >>> assert x.xor(y) == Option.some(2)
@@ -342,37 +489,52 @@
             >>> assert x.xor(y) == Option.none()
 
             >>> x = Option.none()
             >>> y = Option.none()
             >>> assert x.xor(y) == Option.none()
         '''
         return self._match(
-            lambda v1: opt._match(lambda v2: self.none(), lambda: self),
-            lambda: opt._match(lambda v2: opt, self.none),
+            lambda v1: optb._match(lambda v2: self.none(), lambda: self),
+            lambda: optb._match(lambda v2: optb, self.none),
         )
 
     def contains(self, x: Ta) -> bool:  # type: ignore [valid-type]
-        '''Returns `true` if the option is a [`Some`] value containing the given value.
+        '''Returns `true` if the option is a `Some` value containing the given value.
+
+        Args:
+            x: ...
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> x = Option.some(2)
             >>> assert x.contains(2)
 
             >>> x = Option.some(3)
             >>> assert not x.contains(2)
 
             >>> x = Option.none()
             >>> assert not x.contains(2)
         '''
         return self._match(lambda v: x==v, lambda: False)  # type: ignore [operator]
 
     def zip(self, other: 'te.Self[Tb]') -> 'te.Self[t.Tuple[Ta, Tb]]':  # type: ignore [misc]
         '''Zips `self` with another `Option`.
 
-        Example:
+        If `self` is `Some(s)` and `other` is `Some(o)`, this method returns `Some((s, o))`.
+        Otherwise, `None` is returned.
+
+        Args:
+            other: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Option.some(1)
             >>> y = Option.some('hi')
             >>> z = Option.none()
 
             >>> assert x.zip(y) == Option.some((1, 'hi'))
             >>> assert x.zip(z) == Option.none()
         '''
@@ -380,15 +542,25 @@
             return self.some((self._value, other._value))
         else:
             return self.none()
 
     def zip_with(self, other: 'te.Self[Tb]', f: Func2[Ta, Tb, Tc]) -> 'te.Self[Tc]':  # type: ignore [misc, type-arg, valid-type]
         '''Zips `self` and another `Option` with function `f`.
 
-        Example:
+        If `self` is `Some(s)` and `other` is `Some(o)`, this method returns `Some(f(s, o))`.
+        Otherwise, `None` is returned.
+
+        Args:
+            other: ...
+            f: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> class Point:
             ...     def __init__(self, x: float, y: float) -> None:
             ...         self.x, self.y = x, y
             ...
             ...     def __eq__(self, other: 'Point') -> bool:
             ...         return self.x == other.x and self.y == other.y
 
@@ -401,15 +573,15 @@
         if self.is_some() and other.is_some():
             return self.some(f(self._value, other._value))
         else:
             return self.none()
 
     def _match(self, f4some: Func1[Ta, Tb], f4none: Func0[Tb]) -> Tb:  # type: ignore [type-arg, valid-type]
         '''
-        Principle:
+        Prototype:
             ```Rust
             return match self {
                 Some(v) => f4some(v),
                 None => f4none(),
             };
             ```
         '''
```

### Comparing `iydon-2023.3.1/iydon/rust/std/result.py` & `iydon-2023.3.2/iydon/util/rust/std/result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 __all__ = ['Err', 'Ok', 'Result']
 
 
 import typing as t
 
-from ...base.type import Ta, Tb, Tc, Func1
+from ....base.type import Ta, Tb, Tc, Func1
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     from .option import Option
 
 
 class Result(t.Generic[Ta, Tb]):  # type: ignore [misc]
     '''Error handling with the `Result` type.
 
-    Reference:
+    References:
         - https://doc.rust-lang.org/std/result/
         - https://doc.rust-lang.org/src/core/result.rs.html
         - https://github.com/iydon/iydon/blob/main/static/rust/result.rs
     '''
 
     __slots__ = ('_ok', '_err')
 
@@ -48,72 +48,96 @@
         return cls(ok, None)
 
     @classmethod
     def err(cls, err: Tb) -> 'te.Self[Ta, Tb]':  # type: ignore [misc, valid-type]
         return cls(None, err)
 
     def is_ok(self) -> bool:
-        '''Returns `true` if the result is [`Ok`].
+        '''Returns `true` if the result is `Ok`.
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(-3)
             >>> assert x.is_ok()
 
             >>> x = Result.err('Some error message')
             >>> assert not x.is_ok()
         '''
         return self._ok is not None
 
     def is_ok_and(self, f: Func1[Ta, bool]) -> bool:  # type: ignore [type-arg, valid-type]
-        '''Returns `true` if the result is [`Ok`] and the value inside of it matches a predicate.
+        '''Returns `true` if the result is `Ok` and the value inside of it matches a predicate.
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(2)
             >>> assert x.is_ok_and(lambda x: x>1)
 
             >>> x = Result.ok(0)
             >>> assert not x.is_ok_and(lambda x: x>1)
 
             >>> x = Result.err('hey')
             >>> assert not x.is_ok_and(lambda x: x>1)
         '''
         return self.is_ok() and f(self._ok)
 
     def is_err(self) -> bool:
-        '''Returns `true` if the result is [`Err`].
+        '''Returns `true` if the result is `Err`.
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> x = Result.ok(-3)
             >>> assert not x.is_err()
 
             >>> x = Result.err('Some error message')
             >>> assert x.is_err()
         '''
         return not self.is_ok()
 
     def is_err_and(self, f: Func1[Tb, bool]) -> bool:  # type: ignore [type-arg, valid-type]
-        '''Returns `true` if the result is [`Err`] and the value inside of it matches a predicate.
+        '''Returns `true` if the result is `Err` and the value inside of it matches a predicate.
 
-        Example:
+        Args:
+            f: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.err(FileNotFoundError('!'))
             >>> assert x.is_err_and(lambda x: type(x) is FileNotFoundError)
 
             >>> x = Result.err(PermissionError('!'))
             >>> assert not x.is_err_and(lambda x: type(x) is FileNotFoundError)
 
             >>> x = Result.ok(123)
             >>> assert not x.is_err_and(lambda x: type(x) is FileNotFoundError)
         '''
         return self.is_err() and f(self._err)
 
     def get_ok(self) -> 'Option[Ta]':  # type: ignore [type-arg, valid-type]
-        '''Converts from `Result<T, E>` to [`Option<T>`].
+        '''Converts from `Result<T, E>` to `Option<T>`.
+
+        Converts `self` into an `Option<T>`, consuming `self`,
+        and discarding the error, if any.
+
+        Returns:
+            ans: ...
 
-        Example:
-            >>> from iydon.rust.std.option import Option
+        Examples:
+            >>> from iydon.util.rust.std.option import Option
 
             >>> x = Result.ok(2)
             >>> assert x.get_ok() == Option.some(2)
 
             >>> x = Result.err('Nothing here')
             >>> assert x.get_ok() == Option.none()
 
@@ -121,18 +145,24 @@
             - `pub const fn ok(self) -> Option<T>`
         '''
         from .option import Option
 
         return Option.new(self._ok)
 
     def get_err(self) -> 'Option[Tb]':  # type: ignore [type-arg, valid-type]
-        '''Converts from `Result<T, E>` to [`Option<E>`].
+        '''Converts from `Result<T, E>` to `Option<E>`.
 
-        Example:
-            >>> from iydon.rust.std.option import Option
+        Converts `self` into an `Option<E>`, consuming `self`,
+        and discarding the success value, if any.
+
+        Returns:
+            ans: ...
+
+        Examples:
+            >>> from iydon.util.rust.std.option import Option
 
             >>> x = Result.ok(2)
             >>> assert x.get_err() == Option.none()
 
             >>> x = Result.err('Nothing here')
             >>> assert x.get_err() == Option.some('Nothing here')
 
@@ -140,17 +170,26 @@
             - `pub const fn err(self) -> Option<E>`
         '''
         from .option import Option
 
         return Option.new(self._err)
 
     def map(self, op: Func1[Ta, Tc]) -> 'te.Self[Tc, Tb]':  # type: ignore [misc, type-arg, valid-type]
-        '''Maps a `Result<T, E>` to `Result<U, E>` by applying a function to a contained [`Ok`] value, leaving an [`Err`] value untouched.
+        '''Maps a `Result<T, E>` to `Result<U, E>` by applying a function to a
+            contained `Ok` value, leaving an `Err` value untouched.
+
+        This function can be used to compose the results of two functions.
+
+        Args:
+            op: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> lines = '1\\n2\\n3\\n4\\n'
 
             >>> for line in lines.splitlines():
             ...     try:
             ...         ans = Result.ok(int(line))
             ...     except Exception as e:
             ...         ans = Result.err(e)
@@ -164,147 +203,244 @@
             Ok: 4
             Ok: 6
             Ok: 8
         '''
         return self._match(lambda o: self.ok(op(o)), lambda e: self)
 
     def map_or(self, default: Tc, f: Func1[Ta, Tc]) -> Tc:  # type: ignore [type-arg, valid-type]
-        '''Returns the provided default (if [`Err`]), or applies a function to the contained value (if [`Ok`]).
+        '''Returns the provided default (if `Err`), or
+            applies a function to the contained value (if `Ok`).
+
+        Arguments passed to `map_or` are eagerly evaluated; if you are passing
+        the result of a function call, it is recommended to use `map_or_else`,
+        which is lazily evaluated.
+
+        Args:
+            default: ...
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok('foo')
             >>> assert x.map_or(42, len) == 3
 
             >>> x = Result.err('bar')
             >>> assert x.map_or(42, len) == 42
 
         TODO:
             - Typo @ https://github.com/iydon/iydon/blob/main/static/rust/result.rs#L768
         '''
         return self._match(lambda o: f(o), lambda e: default)
 
     def map_or_else(self, default: Func1[Tb, Tc], f: Func1[Ta, Tc]) -> Tc:  # type: ignore [type-arg, valid-type]
-        '''Maps a `Result<T, E>` to `U` by applying fallback function `default` to a contained [`Err`] value, or function `f` to a contained [`Ok`] value.
+        '''Maps a `Result<T, E>` to `U` by applying fallback function `default` to
+            a contained `Err` value, or function `f` to a contained `Ok` value.
+
+        This function can be used to unpack a successful result
+        while handling an error.
+
+        Args:
+            default: ...
+            f: ...
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> k = 21
 
             >>> x = Result.ok('foo')
             >>> assert x.map_or_else(lambda e: k*2, len) == 3
 
             >>> x = Result.err('bar')
             >>> assert x.map_or_else(lambda e: k*2, len) == 42
         '''
         return self._match(lambda o: f(o), lambda e: default(e))
 
     def map_err(self, op: Func1[Tb, Tc]) -> 'te.Self[Ta, Tc]':  # type: ignore [misc, type-arg, valid-type]
-        '''Maps a `Result<T, E>` to `Result<T, F>` by applying a function to a contained [`Err`] value, leaving an [`Ok`] value untouched.
+        '''Maps a `Result<T, E>` to `Result<T, F>` by applying a function to a
+            contained `Err` value, leaving an `Ok` value untouched.
 
-        Example:
+        This function can be used to pass through a successful result while handling
+        an error.
+
+        Args:
+            op: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> def stringify(x: int) -> str: return f'error code: {x}'
 
             >>> x = Result.ok(2)
             >>> assert x.map_err(stringify) == Result.ok(2)
 
             >>> x = Result.err(13)
             >>> assert x.map_err(stringify) == Result.err('error code: 13')
         '''
         return self._match(lambda o: self, lambda e: self.err(op(e)))
 
     def inspect(self, f: Func1[Ta, None]) -> 'te.Self[Ta, Tb]':  # type: ignore [misc, type-arg, valid-type]
-        '''Calls the provided closure with a reference to the contained value (if [`Ok`]).
+        '''Calls the provided closure with a reference to the contained value (if `Ok`).
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(4)
             >>> y = x \\
             ...     .inspect(lambda x: print(f'original: {x}')) \\
             ...     .map(lambda x: x**3) \\
             ...     .expect('failed to parse number')
             original: 4
             >>> assert y == 64
         '''
         if self.is_ok():
             f(self._ok)
         return self
 
     def inspect_err(self, f: Func1[Tb, None]) -> 'te.Self[Ta, Tb]':  # type: ignore [misc, type-arg, valid-type]
-        '''Calls the provided closure with a reference to the contained error (if [`Err`]).
+        '''Calls the provided closure with a reference to the contained error (if `Err`).
+
+        Args:
+            f: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.err('address.txt') \\
             ...     .inspect_err(lambda e: print(f'failed to read file: {e}'))
             failed to read file: address.txt
             >>> assert x.is_err()
         '''
         if self.is_err():
             f(self._err)
         return self
 
     def expect(self, msg: str) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Ok`] value, consuming the `self` value.
+        '''Returns the contained `Ok` value, consuming the `self` value.
+
+        Because this function may panic, its use is generally discouraged.
+        Instead, prefer to use pattern matching and handle the `Err`
+        case explicitly, or call `unwrap_or`, `unwrap_or_else`.
+
+        Args:
+            msg: ...
+
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the value is an `Err`, with a panic message including the
+                passed message, and the content of the `Err`.
 
-        Example:
+        Examples:
             >>> x = Result.err('emergency failure')
             >>> x.expect('Testing expect')
             Traceback (most recent call last):
                 ...
             AssertionError: Testing expect
         '''
         assert self.is_ok(), msg
 
         return self._ok
 
     def unwrap(self) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Ok`] value, consuming the `self` value.
+        '''Returns the contained `Ok` value, consuming the `self` value.
 
-        Example:
+        Because this function may panic, its use is generally discouraged.
+        Instead, prefer to use pattern matching and handle the `Err`
+        case explicitly, or call `unwrap_or`, `unwrap_or_else`.
+
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the value is an `Err`, with a panic message provided by the
+                `Err`'s value.
+
+        Examples:
             >>> x = Result.ok(2)
             >>> assert x.unwrap() == 2
 
             >>> x = Result.err('emergency failure')
             >>> x.unwrap()
             Traceback (most recent call last):
                 ...
             AssertionError: called `Result::unwrap()` on an `Err` value
         '''
         return self.expect('called `Result::unwrap()` on an `Err` value')
 
     def expect_err(self, msg: str) -> Tb:  # type: ignore [valid-type]
-        '''Returns the contained [`Err`] value, consuming the `self` value.
+        '''Returns the contained `Err` value, consuming the `self` value.
+
+        Args:
+            msg: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the value is an `Ok`, with a panic message including the
+                passed message, and the content of the `Ok`.
+
+        Examples:
             >>> x = Result.ok(10)
             >>> x.expect_err('Testing expect_err')
             Traceback (most recent call last):
                 ...
             AssertionError: Testing expect_err
         '''
         assert self.is_err(), msg
 
         return self._err
 
     def unwrap_err(self) -> Tb:  # type: ignore [valid-type]
-        '''Returns the contained [`Err`] value, consuming the `self` value.
+        '''Returns the contained `Err` value, consuming the `self` value.
+
+        Returns:
+            ans: ...
+
+        Raises:
+            AssertionError: Panics if the value is an `Ok`, with a custom panic message provided
+                by the `Ok`'s value.
 
-        Example:
+        Examples:
             >>> x = Result.ok(2)
             >>> x.unwrap_err()
             Traceback (most recent call last):
                 ...
             AssertionError: called `Result::unwrap_err()` on an `Ok` value
 
             >>> x = Result.err('emergency failure')
             >>> assert x.unwrap_err() == 'emergency failure'
         '''
         return self.expect_err('called `Result::unwrap_err()` on an `Ok` value')
 
     def and_(self, res: 'te.Self[Tc, Tb]') -> 'te.Self[Tc, Tb]':  # type: ignore [misc]
-        '''Returns `res` if the result is [`Ok`], otherwise returns the [`Err`] value of `self`.
+        '''Returns `res` if the result is `Ok`, otherwise returns the `Err` value of `self`.
 
-        Example:
+        Arguments passed to `and` are eagerly evaluated; if you are passing the
+        result of a function call, it is recommended to use `and_then`, which is
+        lazily evaluated.
+
+        Args:
+            res: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(2)
             >>> y = Result.err('late error')
             >>> assert x.and_(y) == Result.err('late error')
 
             >>> x = Result.err('early error')
             >>> y = Result.ok('foo')
             >>> assert x.and_(y) == Result.err('early error')
@@ -316,18 +452,26 @@
             >>> x = Result.ok(2)
             >>> y = Result.ok('different result type')
             >>> assert x.and_(y) == Result.ok('different result type')
         '''
         return self._match(lambda o: res, lambda e: self)
 
     def and_then(self, op: Func1[Ta, 'te.Self[Tc, Tb]']) -> 'te.Self[Tc, Tb]':  # type: ignore [misc, type-arg, valid-type]
-        '''Calls `op` if the result is [`Ok`], otherwise returns the [`Err`] value of `self`.
+        '''Calls `op` if the result is `Ok`, otherwise returns the `Err` value of `self`.
+
+        This function can be used for control flow based on `Result` values.
 
-        Example:
-            >>> from iydon.rust.std.option import Option
+        Args:
+            op: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
+            >>> from iydon.util.rust.std.option import Option
             >>> u32 = int
             >>> def sq_then_to_string(x: u32) -> Result[str, str]:
             ...     # u32::checked_mul
             ...     if 0 <= x < 65536:
             ...         ans = Option.some(x*x)
             ...     else:
             ...         ans = Option.none()
@@ -336,17 +480,27 @@
             >>> assert Result.ok(2).and_then(sq_then_to_string) == Result.ok('4')
             >>> assert Result.ok(1_000_000).and_then(sq_then_to_string) == Result.err('overflowed')
             >>> assert Result.err('not a number').and_then(sq_then_to_string) == Result.err('not a number')
         '''
         return self._match(lambda o: op(o), lambda e: self)
 
     def or_(self, res: 'te.Self[Ta, Tc]') -> 'te.Self[Ta, Tc]':  # type: ignore [misc]
-        '''Returns `res` if the result is [`Err`], otherwise returns the [`Ok`] value of `self`.
+        '''Returns `res` if the result is `Err`, otherwise returns the `Ok` value of `self`.
+
+        Arguments passed to `or` are eagerly evaluated; if you are passing the
+        result of a function call, it is recommended to use `or_else`, which is
+        lazily evaluated.
 
-        Example:
+        Args:
+            res: ...
+
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(2)
             >>> y = Result.err('late error')
             >>> assert x.or_(y) == Result.ok(2)
 
             >>> x = Result.err('early error')
             >>> y = Result.ok(2)
             >>> assert x.or_(y) == Result.ok(2)
@@ -358,85 +512,121 @@
             >>> x = Result.ok(2)
             >>> y = Result.ok('different result type')
             >>> assert x.or_(y) == Result.ok(2)
         '''
         return self._match(lambda o: self, lambda e: res)
 
     def or_else(self, op: Func1[Tb, 'te.Self[Ta, Tc]']) -> 'te.Self[Ta, Tc]':  # type: ignore [misc, type-arg, valid-type]
-        '''Calls `op` if the result is [`Err`], otherwise returns the [`Ok`] value of `self`.
+        '''Calls `op` if the result is `Err`, otherwise returns the `Ok` value of `self`.
+
+        This function can be used for control flow based on result values.
+
+        Args:
+            op: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> def sq(x: int) -> Result[int, int]: return Result.ok(x*x)
             >>> def err(x: int) -> Result[int, int]: return Result.err(x)
 
             >>> assert Result.ok(2).or_else(sq).or_else(sq) == Result.ok(2)
             >>> assert Result.ok(2).or_else(err).or_else(sq) == Result.ok(2)
             >>> assert Result.err(3).or_else(sq).or_else(err) == Result.ok(9)
             >>> assert Result.err(3).or_else(err).or_else(err) == Result.err(3)
         '''
         return self._match(lambda o: self, lambda e: op(e))
 
     def unwrap_or(self, default: Ta) -> Ta:  # type: ignore [valid-type]
-        '''Returns the contained [`Ok`] value or a provided default.
+        '''Returns the contained `Ok` value or a provided default.
+
+        Arguments passed to `unwrap_or` are eagerly evaluated; if you are passing
+        the result of a function call, it is recommended to use `unwrap_or_else`,
+        which is lazily evaluated.
+
+        Args:
+            default: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> default = 2
 
             >>> x = Result.ok(9)
             >>> assert x.unwrap_or(default) == 9
 
             >>> x = Result.err('error')
             >>> assert x.unwrap_or(default) == default
         '''
         return self._match(lambda o: o, lambda e: default)
 
     def unwrap_or_else(self, op: Func1[Tb, Ta]) -> Ta:  # type: ignore [type-arg, valid-type]
-        '''Returns the contained [`Ok`] value or computes it from a closure.
+        '''Returns the contained `Ok` value or computes it from a closure.
+
+        Args:
+            op: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> def count(x: str) -> int: return len(x)
 
             >>> assert Result.ok(2).unwrap_or_else(count) == 2
             >>> assert Result.err('foo').unwrap_or_else(count) == 3
         '''
         return self._match(lambda o: o, lambda e: op(e))
 
     def contains(self, x: Ta) -> bool:  # type: ignore [valid-type]
-        '''Returns `true` if the result is an [`Ok`] value containing the given value.
+        '''Returns `true` if the result is an `Ok` value containing the given value.
+
+        Args:
+            x: ...
 
-        Example:
+        Returns:
+            ans: ...
+
+        Examples:
             >>> x = Result.ok(2)
             >>> assert x.contains(2)
 
             >>> x = Result.ok(3)
             >>> assert not x.contains(2)
 
             >>> x = Result.err('Some error message')
             >>> assert not x.contains(2)
         '''
         return self._match(lambda o: o==x, lambda e: False)  # type: ignore [operator]
 
     def contains_err(self, f: Tb) -> bool:  # type: ignore [valid-type]
-        '''Returns `true` if the result is an [`Err`] value containing the given value.
+        '''Returns `true` if the result is an `Err` value containing the given value.
+
+        Args:
+            f: ...
+
+        Returns:
+            ans: ...
 
-        Example:
+        Examples:
             >>> x = Result.ok(2)
             >>> assert not x.contains_err('Some error message')
 
             >>> x = Result.err('Some error message')
             >>> assert   x.contains_err('Some error message')
 
             >>> x = Result.err('Some other error message')
             >>> assert not x.contains_err('Some error message')
         '''
         return self._match(lambda o: False, lambda e: e==f)  # type: ignore [operator]
 
     def _match(self, f4ok: Func1[Ta, Tc], f4err: Func1[Tb, Tc]) -> Tc:  # type: ignore [type-arg, valid-type]
         '''
-        Principle:
+        Prototype:
             ```Rust
             return match self {
                 Ok(o) => f4ok(o),
                 Err(e) => f4err(e),
             };
             ```
         '''
```

### Comparing `iydon-2023.3.1/LICENSE.txt` & `iydon-2023.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.1/pyproject.toml` & `iydon-2023.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iydon"
-version = "2023.3.1"  # year.month.iota
+version = "2023.3.2"  # year.month.iota
 description = "Iydon's common tools"
 authors = ["Iydon Liang <liangiydon@gmail.com>"]
 keywords = ["utilities"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/iydon/iydon"
 repository = "https://github.com/iydon/iydon"
@@ -40,11 +40,14 @@
 
 [tool.poetry.dev-dependencies]
 PyGithub = "^1.58.1"
 tqdm = "^4.65.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 nox-poetry = "^1.0.2"
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.4"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iydon-2023.3.1/README.md` & `iydon-2023.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,45 +57,44 @@
  Cython                  1           16            7            5            4
  Dockerfile              3          215           95          100           20
  Forge Config            2           38           38            0            0
  FORTRAN Modern          2          201          164            0           37
  Go                      2          140          118            0           22
  INI                     1            6            6            0            0
  JavaScript              2            4            4            0            0
- JSON                   79       21,919       21,917            0            2
+ JSON                   79       21,932       21,930            0            2
  Julia                   2          120          105            0           15
  M4                      2        1,069          927            0          142
  MATLAB                155        6,266        4,650        1,017          599
- Makefile               70        1,301          910           79          312
- Python                831       87,567       75,254        2,112       10,201
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
  R                       5          256          215            6           35
  ReStructuredText       21        1,046          705            0          341
- Rust                  144        9,551        8,301          259          991
  Shell                   9          158           91           38           29
  SQL                    22        8,027        7,823          118           86
  SVG                     6          968          883            1           84
  TeX Class              26       14,091       10,548        2,413        1,130
  TeX Definition          3          207          195           12            0
  TeX                   676      328,270      178,952        3,421      145,897
- Plain Text             66      181,661            0      179,586        2,075
- TOML                   15          435          376            7           52
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
  XML                     1            7            7            0            0
  YAML                   93       37,661       35,816        1,147          698
 ───────────────────────────────────────────────────────────────────────────────
  HTML                   32        2,626        2,231          322           73
  |- CSS                  6          123          122            0            1
  |- JavaScript          10          530          457           11           62
  (Total)                          3,279        2,810          333          136
 ───────────────────────────────────────────────────────────────────────────────
  Jupyter Notebooks      11          658          324          270           64
  |- Markdown             7          288            0          259           29
  |- Python              10          370          324           11           35
  (Total)                          1,316          648          540          128
 ───────────────────────────────────────────────────────────────────────────────
- Markdown              375       27,397            0       20,914        6,483
+ Markdown              377       27,448            0       20,957        6,491
  |- C                    1            7            6            0            1
  |- C++                  2           78           63            2           13
  |- HTML                 2           66           66            0            0
  |- JSON                 2        1,096        1,096            0            0
  |- MATLAB               1           62           28           29            5
  |- Markdown             1           51            0           50            1
  |- Python              36        2,017        1,621           82          314
@@ -103,13 +102,17 @@
  |- Rust                 2          269          237            6           26
  |- Shell               23        1,027          979            0           48
  |- SQL                  1            2            2            0            0
  |- TeX                  2           42           35            0            7
  |- TOML                 1           13           11            0            2
  |- XML                  1            8            8            0            0
  |- YAML                 7          263          234           17           12
- (Total)                         32,612        4,564       21,136        6,912
+ (Total)                         32,663        4,564       21,179        6,920
+───────────────────────────────────────────────────────────────────────────────
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Total               2,805      747,631      362,258      213,955      171,418
+ Total               2,822      754,196      364,792      216,825      172,579
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
   </code></pre>
 </details>
```

#### html2text {}

```diff
@@ -29,45 +29,44 @@
  Cython                  1           16            7            5            4
  Dockerfile              3          215           95          100           20
  Forge Config            2           38           38            0            0
  FORTRAN Modern          2          201          164            0           37
  Go                      2          140          118            0           22
  INI                     1            6            6            0            0
  JavaScript              2            4            4            0            0
- JSON                   79       21,919       21,917            0            2
+ JSON                   79       21,932       21,930            0            2
  Julia                   2          120          105            0           15
  M4                      2        1,069          927            0          142
  MATLAB                155        6,266        4,650        1,017          599
- Makefile               70        1,301          910           79          312
- Python                831       87,567       75,254        2,112       10,201
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
  R                       5          256          215            6           35
  ReStructuredText       21        1,046          705            0          341
- Rust                  144        9,551        8,301          259          991
  Shell                   9          158           91           38           29
  SQL                    22        8,027        7,823          118           86
  SVG                     6          968          883            1           84
  TeX Class              26       14,091       10,548        2,413        1,130
  TeX Definition          3          207          195           12            0
  TeX                   676      328,270      178,952        3,421      145,897
- Plain Text             66      181,661            0      179,586        2,075
- TOML                   15          435          376            7           52
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
  XML                     1            7            7            0            0
  YAML                   93       37,661       35,816        1,147          698
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
  HTML                   32        2,626        2,231          322           73
  |- CSS                  6          123          122            0            1
  |- JavaScript          10          530          457           11           62
  (Total)                          3,279        2,810          333          136
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
  Jupyter Notebooks      11          658          324          270           64
  |- Markdown             7          288            0          259           29
  |- Python              10          370          324           11           35
  (Total)                          1,316          648          540          128
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
- Markdown              375       27,397            0       20,914        6,483
+ Markdown              377       27,448            0       20,957        6,491
  |- C                    1            7            6            0            1
  |- C++                  2           78           63            2           13
  |- HTML                 2           66           66            0            0
  |- JSON                 2        1,096        1,096            0            0
  |- MATLAB               1           62           28           29            5
  |- Markdown             1           51            0           50            1
  |- Python              36        2,017        1,621           82          314
@@ -75,13 +74,17 @@
  |- Rust                 2          269          237            6           26
  |- Shell               23        1,027          979            0           48
  |- SQL                  1            2            2            0            0
  |- TeX                  2           42           35            0            7
  |- TOML                 1           13           11            0            2
  |- XML                  1            8            8            0            0
  |- YAML                 7          263          234           17           12
- (Total)                         32,612        4,564       21,136        6,912
+ (Total)                         32,663        4,564       21,179        6,920
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
- Total               2,805      747,631      362,258      213,955      171,418
+ Total               2,822      754,196      364,792      216,825      172,579
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
```

### Comparing `iydon-2023.3.1/setup.py` & `iydon-2023.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,149 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: iydon
+Version: 2023.3.2
+Summary: Iydon's common tools
+Home-page: https://github.com/iydon/iydon
+License: GPL-3.0-only
+Keywords: utilities
+Author: Iydon Liang
+Author-email: liangiydon@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Provides-Extra: full
+Provides-Extra: type
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0); extra == "type" or extra == "full"
+Project-URL: Bug Tracker, https://github.com/iydon/iydon/issues
+Project-URL: Repository, https://github.com/iydon/iydon
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://github.com/iydon/iydon">
+    🔵⬜🟦⬜🟦<br />
+    ⬜⬜🟦⬜🟦<br />
+    🟦⬜🟦🟦🟦<br />
+    🟦⬜⬜⬜🟦<br />
+    🟦⬜🟦🟦🟦<br />
+  </a>
+
+  <h3 align="center">Iydon (梁钰栋 in Chinese)</h3>
+
+  <p align="center">
+    <a href="https://www.iydon.top">
+      <img src="https://img.shields.io/static/v1?label=Blog&message=iydon.top&color=brightgreen" />
+    </a>
+    ·
+    <a href="https://github.com/iydon">
+      <img src="https://img.shields.io/static/v1?label=GitHub&message=iydon&color=green" />
+    </a>
+    ·
+    <a href="mailto:liangiydon@gmail.com">
+      <img src="https://img.shields.io/static/v1?label=Gmail&message=liangiydon&color=yellowgreen" />
+    </a>
+    ·
+    <a href="https://steamcommunity.com/id/iydon">
+      <img src="https://img.shields.io/static/v1?label=Steam&message=iydon&color=yellow" />
+    </a>
+    ·
+    <img src="https://visitor-badge.glitch.me/badge?page_id=iydon&right_color=orange&left_text=Visitors" />
+    ·
+    <img src="https://img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red" />
+  </p>
+</div>
+
+
+
+<details>
+  <summary><strong>GitHub Statistics</strong></summary>
+  <img src="https://github-readme-stats.vercel.app/api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite" />
+</details>
+
+
+
+<details>
+  <summary><strong>Code Statistics</strong></summary>
+  <pre><code>
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Language            Files        Lines         Code     Comments       Blanks
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Autoconf                9           45           36            0            9
+ BASH                   32           98           34           32           32
+ Batch                   7          343          289            3           51
+ C                      35        4,264        2,477        1,053          734
+ C Header               46        3,370        2,351          485          534
+ C++                    13          611          462           40          109
+ CSS                     6          493          480           12            1
+ Cython                  1           16            7            5            4
+ Dockerfile              3          215           95          100           20
+ Forge Config            2           38           38            0            0
+ FORTRAN Modern          2          201          164            0           37
+ Go                      2          140          118            0           22
+ INI                     1            6            6            0            0
+ JavaScript              2            4            4            0            0
+ JSON                   79       21,932       21,930            0            2
+ Julia                   2          120          105            0           15
+ M4                      2        1,069          927            0          142
+ MATLAB                155        6,266        4,650        1,017          599
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
+ R                       5          256          215            6           35
+ ReStructuredText       21        1,046          705            0          341
+ Shell                   9          158           91           38           29
+ SQL                    22        8,027        7,823          118           86
+ SVG                     6          968          883            1           84
+ TeX Class              26       14,091       10,548        2,413        1,130
+ TeX Definition          3          207          195           12            0
+ TeX                   676      328,270      178,952        3,421      145,897
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
+ XML                     1            7            7            0            0
+ YAML                   93       37,661       35,816        1,147          698
+───────────────────────────────────────────────────────────────────────────────
+ HTML                   32        2,626        2,231          322           73
+ |- CSS                  6          123          122            0            1
+ |- JavaScript          10          530          457           11           62
+ (Total)                          3,279        2,810          333          136
+───────────────────────────────────────────────────────────────────────────────
+ Jupyter Notebooks      11          658          324          270           64
+ |- Markdown             7          288            0          259           29
+ |- Python              10          370          324           11           35
+ (Total)                          1,316          648          540          128
+───────────────────────────────────────────────────────────────────────────────
+ Markdown              377       27,448            0       20,957        6,491
+ |- C                    1            7            6            0            1
+ |- C++                  2           78           63            2           13
+ |- HTML                 2           66           66            0            0
+ |- JSON                 2        1,096        1,096            0            0
+ |- MATLAB               1           62           28           29            5
+ |- Markdown             1           51            0           50            1
+ |- Python              36        2,017        1,621           82          314
+ |- R                    2          214          178           36            0
+ |- Rust                 2          269          237            6           26
+ |- Shell               23        1,027          979            0           48
+ |- SQL                  1            2            2            0            0
+ |- TeX                  2           42           35            0            7
+ |- TOML                 1           13           11            0            2
+ |- XML                  1            8            8            0            0
+ |- YAML                 7          263          234           17           12
+ (Total)                         32,663        4,564       21,179        6,920
+───────────────────────────────────────────────────────────────────────────────
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Total               2,822      754,196      364,792      216,825      172,579
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+  </code></pre>
+</details>
 
-packages = \
-['iydon',
- 'iydon.base',
- 'iydon.rust',
- 'iydon.rust.std',
- 'iydon.test',
- 'iydon.test.rust']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'full': ['typing-extensions>=4.5.0,<5.0.0'],
- 'type': ['typing-extensions>=4.5.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'iydon',
-    'version': '2023.3.1',
-    'description': "Iydon's common tools",
-    'long_description': '<div align="center">\n  <a href="https://github.com/iydon/iydon">\n    🔵⬜🟦⬜🟦<br />\n    ⬜⬜🟦⬜🟦<br />\n    🟦⬜🟦🟦🟦<br />\n    🟦⬜⬜⬜🟦<br />\n    🟦⬜🟦🟦🟦<br />\n  </a>\n\n  <h3 align="center">Iydon (梁钰栋 in Chinese)</h3>\n\n  <p align="center">\n    <a href="https://www.iydon.top">\n      <img src="https://img.shields.io/static/v1?label=Blog&message=iydon.top&color=brightgreen" />\n    </a>\n    ·\n    <a href="https://github.com/iydon">\n      <img src="https://img.shields.io/static/v1?label=GitHub&message=iydon&color=green" />\n    </a>\n    ·\n    <a href="mailto:liangiydon@gmail.com">\n      <img src="https://img.shields.io/static/v1?label=Gmail&message=liangiydon&color=yellowgreen" />\n    </a>\n    ·\n    <a href="https://steamcommunity.com/id/iydon">\n      <img src="https://img.shields.io/static/v1?label=Steam&message=iydon&color=yellow" />\n    </a>\n    ·\n    <img src="https://visitor-badge.glitch.me/badge?page_id=iydon&right_color=orange&left_text=Visitors" />\n    ·\n    <img src="https://img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red" />\n  </p>\n</div>\n\n\n\n<details>\n  <summary><strong>GitHub Statistics</strong></summary>\n  <img src="https://github-readme-stats.vercel.app/api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite" />\n</details>\n\n\n\n<details>\n  <summary><strong>Code Statistics</strong></summary>\n  <pre><code>\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Language            Files        Lines         Code     Comments       Blanks\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Autoconf                9           45           36            0            9\n BASH                   32           98           34           32           32\n Batch                   7          343          289            3           51\n C                      35        4,264        2,477        1,053          734\n C Header               46        3,370        2,351          485          534\n C++                    13          611          462           40          109\n CSS                     6          493          480           12            1\n Cython                  1           16            7            5            4\n Dockerfile              3          215           95          100           20\n Forge Config            2           38           38            0            0\n FORTRAN Modern          2          201          164            0           37\n Go                      2          140          118            0           22\n INI                     1            6            6            0            0\n JavaScript              2            4            4            0            0\n JSON                   79       21,919       21,917            0            2\n Julia                   2          120          105            0           15\n M4                      2        1,069          927            0          142\n MATLAB                155        6,266        4,650        1,017          599\n Makefile               70        1,301          910           79          312\n Python                831       87,567       75,254        2,112       10,201\n R                       5          256          215            6           35\n ReStructuredText       21        1,046          705            0          341\n Rust                  144        9,551        8,301          259          991\n Shell                   9          158           91           38           29\n SQL                    22        8,027        7,823          118           86\n SVG                     6          968          883            1           84\n TeX Class              26       14,091       10,548        2,413        1,130\n TeX Definition          3          207          195           12            0\n TeX                   676      328,270      178,952        3,421      145,897\n Plain Text             66      181,661            0      179,586        2,075\n TOML                   15          435          376            7           52\n XML                     1            7            7            0            0\n YAML                   93       37,661       35,816        1,147          698\n───────────────────────────────────────────────────────────────────────────────\n HTML                   32        2,626        2,231          322           73\n |- CSS                  6          123          122            0            1\n |- JavaScript          10          530          457           11           62\n (Total)                          3,279        2,810          333          136\n───────────────────────────────────────────────────────────────────────────────\n Jupyter Notebooks      11          658          324          270           64\n |- Markdown             7          288            0          259           29\n |- Python              10          370          324           11           35\n (Total)                          1,316          648          540          128\n───────────────────────────────────────────────────────────────────────────────\n Markdown              375       27,397            0       20,914        6,483\n |- C                    1            7            6            0            1\n |- C++                  2           78           63            2           13\n |- HTML                 2           66           66            0            0\n |- JSON                 2        1,096        1,096            0            0\n |- MATLAB               1           62           28           29            5\n |- Markdown             1           51            0           50            1\n |- Python              36        2,017        1,621           82          314\n |- R                    2          214          178           36            0\n |- Rust                 2          269          237            6           26\n |- Shell               23        1,027          979            0           48\n |- SQL                  1            2            2            0            0\n |- TeX                  2           42           35            0            7\n |- TOML                 1           13           11            0            2\n |- XML                  1            8            8            0            0\n |- YAML                 7          263          234           17           12\n (Total)                         32,612        4,564       21,136        6,912\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Total               2,805      747,631      362,258      213,955      171,418\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n  </code></pre>\n</details>\n',
-    'author': 'Iydon Liang',
-    'author_email': 'liangiydon@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/iydon/iydon',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,98 +1,106 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['iydon',
-'iydon.base', 'iydon.rust', 'iydon.rust.std', 'iydon.test', 'iydon.test.rust']
-package_data = \ {'': ['*']} extras_require = \ {'full': ['typing-
-extensions>=4.5.0,<5.0.0'], 'type': ['typing-extensions>=4.5.0,<5.0.0']}
-setup_kwargs = { 'name': 'iydon', 'version': '2023.3.1', 'description':
-"Iydon's common tools", 'long_description': '
-                           \n \n_ðµâ¬ð¦â¬ð¦
-                             \n_â¬â¬ð¦â¬ð¦
-                            \n_ð¦â¬ð¦ð¦ð¦
-                             \n_ð¦â¬â¬â¬ð¦
-                            \n_ð¦â¬ð¦ð¦ð¦
-                                    \n\n\n
+Metadata-Version: 2.1 Name: iydon Version: 2023.3.2 Summary: Iydon's common
+tools Home-page: https://github.com/iydon/iydon License: GPL-3.0-only Keywords:
+utilities Author: Iydon Liang Author-email: liangiydon@gmail.com Requires-
+Python: >=3.7,<4.0 Classifier: Environment :: Console Classifier: License ::
+OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
+Language :: Chinese (Simplified) Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Topic :: Software Development :: User Interfaces Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Provides-Extra: full Provides-Extra: type Requires-
+Dist: typing-extensions (>=4.5.0,<5.0.0); extra == "type" or extra == "full"
+Project-URL: Bug Tracker, https://github.com/iydon/iydon/issues Project-URL:
+Repository, https://github.com/iydon/iydon Description-Content-Type: text/
+markdown
+                              ðµâ¬ð¦â¬ð¦
+                               â¬â¬ð¦â¬ð¦
+                              ð¦â¬ð¦ð¦ð¦
+                               ð¦â¬â¬â¬ð¦
+                              ð¦â¬ð¦ð¦ð¦
                     **** Iydon (æ¢é°æ  in Chinese) ****
-                                     \n\n
-                     \n \n_[https://img.shields.io/static/
-   v1?label=Blog&message=iydon.top&color=brightgreen]\n\n Â·\n \n_[https://
- img.shields.io/static/v1?label=GitHub&message=iydon&color=green]\n\n Â·\n \n_
                         [https://img.shields.io/static/
-  v1?label=Gmail&message=liangiydon&color=yellowgreen]\n\n Â·\n \n_[https://
-  img.shields.io/static/v1?label=Steam&message=iydon&color=yellow]\n\n Â·\n
-                       [https://visitor-badge.glitch.me/
-  badge?page_id=iydon&right_color=orange&left_text=Visitors]\n Â·\n [https://
-     img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red]\n
-                                      \n
-\n\n\n\n\n GitHub Statistics\n [https://github-readme-stats.vercel.app/
-api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite]\n\n\n\n\n\n
-Code Statistics\n
-\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Language            Files        Lines         Code     Comments
-Blanks\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Autoconf                9           45           36            0            9\n
-BASH                   32           98           34           32           32\n
-Batch                   7          343          289            3           51\n
-C                      35        4,264        2,477        1,053          734\n
-C Header               46        3,370        2,351          485          534\n
-C++                    13          611          462           40          109\n
-CSS                     6          493          480           12            1\n
-Cython                  1           16            7            5            4\n
-Dockerfile              3          215           95          100           20\n
-Forge Config            2           38           38            0            0\n
-FORTRAN Modern          2          201          164            0           37\n
-Go                      2          140          118            0           22\n
-INI                     1            6            6            0            0\n
-JavaScript              2            4            4            0            0\n
-JSON                   79       21,919       21,917            0            2\n
-Julia                   2          120          105            0           15\n
-M4                      2        1,069          927            0          142\n
-MATLAB                155        6,266        4,650        1,017          599\n
-Makefile               70        1,301          910           79          312\n
-Python                831       87,567       75,254        2,112       10,201\n
-R                       5          256          215            6           35\n
-ReStructuredText       21        1,046          705            0          341\n
-Rust                  144        9,551        8,301          259          991\n
-Shell                   9          158           91           38           29\n
-SQL                    22        8,027        7,823          118           86\n
-SVG                     6          968          883            1           84\n
-TeX Class              26       14,091       10,548        2,413        1,130\n
-TeX Definition          3          207          195           12            0\n
-TeX                   676      328,270      178,952        3,421      145,897\n
-Plain Text             66      181,661            0      179,586        2,075\n
-TOML                   15          435          376            7           52\n
-XML                     1            7            7            0            0\n
-YAML                   93       37,661       35,816        1,147
-698\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-HTML                   32        2,626        2,231          322           73\n
-|- CSS                  6          123          122            0            1\n
-|- JavaScript          10          530          457           11           62\n
-(Total)                          3,279        2,810          333
-136\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Jupyter Notebooks      11          658          324          270           64\n
-|- Markdown             7          288            0          259           29\n
-|- Python              10          370          324           11           35\n
-(Total)                          1,316          648          540
-128\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Markdown              375       27,397            0       20,914        6,483\n
-|- C                    1            7            6            0            1\n
-|- C++                  2           78           63            2           13\n
-|- HTML                 2           66           66            0            0\n
-|- JSON                 2        1,096        1,096            0            0\n
-|- MATLAB               1           62           28           29            5\n
-|- Markdown             1           51            0           50            1\n
-|- Python              36        2,017        1,621           82          314\n
-|- R                    2          214          178           36            0\n
-|- Rust                 2          269          237            6           26\n
-|- Shell               23        1,027          979            0           48\n
-|- SQL                  1            2            2            0            0\n
-|- TeX                  2           42           35            0            7\n
-|- TOML                 1           13           11            0            2\n
-|- XML                  1            8            8            0            0\n
-|- YAML                 7          263          234           17           12\n
-(Total)                         32,612        4,564       21,136
-6,912\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Total               2,805      747,631      362,258      213,955
-171,418\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-\n\n', 'author': 'Iydon Liang', 'author_email': 'liangiydon@gmail.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/iydon/
-iydon', 'packages': packages, 'package_data': package_data, 'extras_require':
-extras_require, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+v1?label=Blog&message=iydon.top&color=brightgreen] Â· [https://img.shields.io/
+ static/v1?label=GitHub&message=iydon&color=green] Â· [https://img.shields.io/
+   static/v1?label=Gmail&message=liangiydon&color=yellowgreen] Â· [https://
+ img.shields.io/static/v1?label=Steam&message=iydon&color=yellow] Â· [https://
+                           visitor-badge.glitch.me/
+    badge?page_id=iydon&right_color=orange&left_text=Visitors] Â· [https://
+      img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red]
+ GitHub Statistics [https://github-readme-stats.vercel.app/
+api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite]
+Code Statistics
+
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Language            Files        Lines         Code     Comments       Blanks
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Autoconf                9           45           36            0            9
+ BASH                   32           98           34           32           32
+ Batch                   7          343          289            3           51
+ C                      35        4,264        2,477        1,053          734
+ C Header               46        3,370        2,351          485          534
+ C++                    13          611          462           40          109
+ CSS                     6          493          480           12            1
+ Cython                  1           16            7            5            4
+ Dockerfile              3          215           95          100           20
+ Forge Config            2           38           38            0            0
+ FORTRAN Modern          2          201          164            0           37
+ Go                      2          140          118            0           22
+ INI                     1            6            6            0            0
+ JavaScript              2            4            4            0            0
+ JSON                   79       21,932       21,930            0            2
+ Julia                   2          120          105            0           15
+ M4                      2        1,069          927            0          142
+ MATLAB                155        6,266        4,650        1,017          599
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
+ R                       5          256          215            6           35
+ ReStructuredText       21        1,046          705            0          341
+ Shell                   9          158           91           38           29
+ SQL                    22        8,027        7,823          118           86
+ SVG                     6          968          883            1           84
+ TeX Class              26       14,091       10,548        2,413        1,130
+ TeX Definition          3          207          195           12            0
+ TeX                   676      328,270      178,952        3,421      145,897
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
+ XML                     1            7            7            0            0
+ YAML                   93       37,661       35,816        1,147          698
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ HTML                   32        2,626        2,231          322           73
+ |- CSS                  6          123          122            0            1
+ |- JavaScript          10          530          457           11           62
+ (Total)                          3,279        2,810          333          136
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Jupyter Notebooks      11          658          324          270           64
+ |- Markdown             7          288            0          259           29
+ |- Python              10          370          324           11           35
+ (Total)                          1,316          648          540          128
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Markdown              377       27,448            0       20,957        6,491
+ |- C                    1            7            6            0            1
+ |- C++                  2           78           63            2           13
+ |- HTML                 2           66           66            0            0
+ |- JSON                 2        1,096        1,096            0            0
+ |- MATLAB               1           62           28           29            5
+ |- Markdown             1           51            0           50            1
+ |- Python              36        2,017        1,621           82          314
+ |- R                    2          214          178           36            0
+ |- Rust                 2          269          237            6           26
+ |- Shell               23        1,027          979            0           48
+ |- SQL                  1            2            2            0            0
+ |- TeX                  2           42           35            0            7
+ |- TOML                 1           13           11            0            2
+ |- XML                  1            8            8            0            0
+ |- YAML                 7          263          234           17           12
+ (Total)                         32,663        4,564       21,179        6,920
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Total               2,822      754,196      364,792      216,825      172,579
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+
+
```

