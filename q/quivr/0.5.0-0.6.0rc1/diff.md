# Comparing `tmp/quivr-0.5.0.tar.gz` & `tmp/quivr-0.6.0rc1.tar.gz`

## Comparing `quivr-0.5.0.tar` & `quivr-0.6.0rc1.tar`

### file list

```diff
@@ -1,20 +1,17 @@
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/__version__.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/attributes.py
--rw-r--r--   0        0        0    39655 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/columns.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/defragment.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/errors.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/indexing.py
--rw-r--r--   0        0        0    13144 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/linkage.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/schemagraph.py
--rw-r--r--   0        0        0    38124 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/typevars.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.5.0/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.5.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.5.0/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.5.0/README.md
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 quivr-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 quivr-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/__version__.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/attributes.py
+-rw-r--r--   0        0        0    45445 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/columns.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/defragment.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/errors.py
+-rw-r--r--   0        0        0    18327 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/schemagraph.py
+-rw-r--r--   0        0        0    39757 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/tables.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 quivr-0.6.0rc1/PKG-INFO
```

### Comparing `quivr-0.5.0/quivr/__init__.py` & `quivr-0.6.0rc1/quivr/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,28 +38,29 @@
     UInt8Column,
     UInt16Column,
     UInt32Column,
     UInt64Column,
 )
 from .concat import concatenate
 from .defragment import defragment
-from .errors import InvariantViolatedError, TableFragmentedError, ValidationError
-from .indexing import StringIndex
-from .linkage import Linkage, MultiKeyLinkage
-from .matrix import MatrixArray, MatrixExtensionType
+from .errors import (
+    InvariantViolatedError,
+    LinkageCombinationError,
+    TableFragmentedError,
+    TablesNotCompatibleError,
+    ValidationError,
+)
+from .linkage import Linkage, MultiKeyLinkage, combine_linkages, combine_multilinkages
 from .tables import AnyTable, AttributeValueType, DataSourceType, Table
 from .validators import Validator, and_, eq, ge, gt, is_in, le, lt
 
 __all__ = [
     "__version__",
     "Table",
-    "MatrixArray",
-    "MatrixExtensionType",
     "concatenate",
-    "StringIndex",
     "Column",
     "SubTableColumn",
     "Int8Column",
     "Int16Column",
     "Int32Column",
     "Int64Column",
     "UInt8Column",
@@ -110,8 +111,12 @@
     "AttributeValueType",
     "DataSourceType",
     "AnyTable",
     "MetadataDict",
     "Byteslike",
     "Linkage",
     "MultiKeyLinkage",
+    "combine_linkages",
+    "combine_multilinkages",
+    "LinkageCombinationError",
+    "TablesNotCompatibleError",
 ]
```

### Comparing `quivr-0.5.0/quivr/attributes.py` & `quivr-0.6.0rc1/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.5.0/quivr/columns.py` & `quivr-0.6.0rc1/quivr/columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,57 +8,73 @@
     from typing import TypeAlias
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
-from typing import Dict, Generic, Optional, TypeVar, Union, overload
+import datetime
+import decimal
+from typing import Any, Callable, Dict, Generic, Optional, TypeVar, Union, overload
 
 import pyarrow as pa
 
-from . import tables, validators
+from . import errors, tables, validators
 
 Byteslike: TypeAlias = Union[bytes, str]
 MetadataDict: TypeAlias = Dict[Byteslike, Byteslike]
 
 
 class Column:
     """A Column is an accessor for data in a Table, and also a
     descriptor for the Table's structure.
 
     This is a base class for all column types. It is not intended to
-    be used directly; instead, use on of its subclasses.
+    be used directly; instead, use one of its subclasses.
 
     Columns implement the descriptor protocol, so they should be used
     as class attributes on a Table subclass.
 
     :param dtype: The pyarrow data type of the column.
     :param nullable: Whether the column can contain null values.
     :param metadata: A dictionary of metadata to attach to the column.
     :param validator: A validator to use when setting the column.
+    :param default: A default value to use when setting the column.
 
     :ivar dtype: The pyarrow data type of the column.
     :ivar nullable: Whether the column can contain null values.
     :ivar metadata: A dictionary of metadata to attach to the column.
     :ivar validator: A validator to use when setting the column.
+    :ivar default: A default value to use when setting the column.
     """
 
     def __init__(
         self,
         dtype: pa.DataType,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], Any], Any] = None,
     ):
         self.dtype = dtype
         self.nullable = nullable
         self.metadata = metadata
         self.validator = validator
 
+        self.default = default
+        if self.default is not None:
+            self._default_is_callable = callable(self.default)
+            if self._default_is_callable:
+                self._default_fn = self.default
+            else:
+                try:
+                    self._default_scalar = pa.scalar(self.default, self.dtype)
+                except (pa.ArrowInvalid, pa.ArrowTypeError, OverflowError) as e:
+                    raise errors.InvalidColumnDefault(self.default, self.dtype) from e
+
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Array:
         ...
@@ -78,24 +94,42 @@
     def __set__(self, obj: tables.Table, value: pa.Array) -> None:
         """
         Sets the data for this column on a Table instance.
 
         This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
         """
         idx = obj.table.schema.get_field_index(self.name)
+        value = self.fill_default(value)
         obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value])
 
     def __set_name__(self, owner: type, name: str) -> None:
         """
         Sets the name of the column.
 
         This method is part of the `descriptor protocol <https://docs.python.org/3/howto/descriptor.html>`_.
         """
         self.name = name
 
+    def fill_default(self, array: pa.Array) -> pa.Array:
+        """
+        Fills null values in the array with the Column's default value.
+        """
+        if self.default is None or array.null_count == 0:
+            return array
+        if self._default_is_callable:
+            null_count = array.null_count
+            try:
+                fill_values = pa.array([self._default_fn() for _ in range(null_count)], self.dtype)
+            except (pa.ArrowInvalid, pa.ArrowTypeError, OverflowError) as e:
+                raise errors.InvalidColumnDefault(self._default_fn, self.dtype, self.name) from e
+            null_mask = pa.compute.is_null(array)
+            return pa.compute.replace_with_mask(array, null_mask, fill_values)
+        else:
+            return array.fill_null(self._default_scalar)
+
     def pyarrow_field(self) -> pa.Field:
         """
         Returns a pyarrow Field object for this column.
         """
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
 
 
@@ -142,21 +176,26 @@
 
 
 class Int8Column(Column):
     """
     A column for storing 8-bit integers.
     """
 
+    primitive_dtype = pa.int8()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.int8(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.int8(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Int8Array:
@@ -169,21 +208,26 @@
 
 
 class Int16Column(Column):
     """
     A column for storing 16-bit integers.
     """
 
+    primitive_dtype = pa.int16()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.int16(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.int16(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Int16Array:
@@ -196,21 +240,26 @@
 
 
 class Int32Column(Column):
     """
     A column for storing 32-bit integers.
     """
 
+    primitive_dtype = pa.int32()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.int32(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.int32(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Int32Array:
@@ -223,21 +272,26 @@
 
 
 class Int64Column(Column):
     """
     A column for storing 64-bit integers.
     """
 
+    primitive_dtype = pa.int64()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.int64(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.int64(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Int64Array:
@@ -250,21 +304,26 @@
 
 
 class UInt8Column(Column):
     """
     A column for storing 8-bit unsigned integers.
     """
 
+    primitive_dtype = pa.uint8()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.uint8(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.uint8(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt8Array:
@@ -277,21 +336,26 @@
 
 
 class UInt16Column(Column):
     """
     A column for storing 16-bit unsigned integers.
     """
 
+    primitive_dtype = pa.uint16()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.uint16(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.uint16(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt16Array:
@@ -304,21 +368,26 @@
 
 
 class UInt32Column(Column):
     """
     A column for storing 32-bit unsigned integers.
     """
 
+    primitive_dtype = pa.uint32()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.uint32(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.uint32(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt32Array:
@@ -331,21 +400,26 @@
 
 
 class UInt64Column(Column):
     """
     A column for storing 64-bit unsigned integers.
     """
 
+    primitive_dtype = pa.uint64()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], int], int] = None,
     ):
-        super().__init__(pa.uint64(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.uint64(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.UInt64Array:
@@ -354,18 +428,31 @@
     def __get__(self, obj: Optional[tables.Table], objtype: type) -> Union[Self, pa.UInt64Array]:
         if obj is None:
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class Float16Column(Column):
-    """
-    A column for storing 16-bit floating point numbers.
+    """A column for storing 16-bit floating point numbers.
+
+    16-bit floating point arrays have limited support in Arrow, and
+    thus limited support in quivr.
+
+    In particular:
+    - They cannot be written to or read from Parquet files.
+
+    - They cannot be constructed from Python floats in a natural way
+      (one must use numpy.float16).
+
+    - They don't support quivr column default values (because they are
+      not supported by Arrow's compute functions).
     """
 
+    primitive_dtype = pa.float16()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
@@ -385,21 +472,26 @@
 
 
 class Float32Column(Column):
     """
     A column for storing 32-bit floating point numbers.
     """
 
+    primitive_dtype = pa.float32()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], float], float] = None,
     ):
-        super().__init__(pa.float32(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.float32(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.FloatArray:
@@ -412,21 +504,26 @@
 
 
 class Float64Column(Column):
     """
     A column for storing 64-bit floating point numbers.
     """
 
+    primitive_dtype = pa.float64()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], float], float] = None,
     ):
-        super().__init__(pa.float64(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.float64(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.lib.DoubleArray:
@@ -437,21 +534,26 @@
             return self
         return obj.table[self.name].combine_chunks()
 
 
 class BooleanColumn(Column):
     """A column for storing booleans."""
 
+    primitive_dtype = pa.bool_()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, Callable[[], bool], bool] = None,
     ):
-        super().__init__(pa.bool_(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.bool_(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.BooleanArray:
@@ -468,21 +570,26 @@
 
     This can be used to store strings of any length, but it is not
     recommended for storing very long strings (over 2GB, for
     example). For long strings, use LargeStringColumn instead.
 
     """
 
+    primitive_dtype = pa.string()
+
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, str, Callable[[], str]] = None,
     ):
-        super().__init__(pa.string(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.string(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.StringArray:
@@ -501,16 +608,19 @@
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
-        super().__init__(pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeBinaryArray:
@@ -529,16 +639,19 @@
     """
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, str, Callable[[], str]] = None,
     ):
-        super().__init__(pa.large_string(), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.large_string(), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.LargeStringArray:
@@ -628,25 +741,30 @@
 
     :param unit: The unit of time to use for the timestamp. Valid
         values are "s", "ms", "us", and "ns".
     :param tz: An optional timezone to associate with the timestamp.
     :param nullable: Whether the column can contain null values.
     :param metadata: Optional metadata to associate with the column.
     :param validator: An optional validator to apply to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
         tz: Optional[str] = None,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, datetime.datetime, Callable[[], datetime.datetime]] = None,
     ):
-        super().__init__(pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.TimestampArray:
@@ -668,24 +786,29 @@
 
     Internally, a time32 value is a 32-bit integer which an elapsed time since midnight.
 
     :param unit: The unit of time to use for the time. Valid values are "s" and "ms".
     :param nullable: Whether the column can contain null values.
     :param metadata: Optional metadata to associate with the column.
     :param validator: An optional validator to apply to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
-        super().__init__(pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Time32Array:
@@ -707,24 +830,29 @@
 
     Internally, a time64 value is a 64-bit integer which an elapsed time since midnight.
 
     :param unit: The unit of time to use for the time. Valid values are "us" and "ns".
     :param nullable: Whether the column can contain null values.
     :param metadata: Optional metadata to associate with the column.
     :param validator: An optional validator to apply to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
-        super().__init__(pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Time64Array:
@@ -812,16 +940,19 @@
     """A column for storing opaque binary data."""
 
     def __init__(
         self,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
-        super().__init__(pa.binary(-1), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.binary(-1), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.BinaryArray:
@@ -833,25 +964,33 @@
         return obj.table[self.name].combine_chunks()
 
 
 class FixedSizeBinaryColumn(Column):
     """A column for storing opaque fixed-size binary data.
 
     :param byte_width: The number of bytes per value.
+    :param nullable: Whether the column can contain null values.
+    :param metadata: Optional metadata to associate with the column.
+    :param validator: An optional validator to apply to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         byte_width: int,
         nullable: bool = True,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
+        default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         self.byte_width = byte_width
-        super().__init__(pa.binary(byte_width), nullable=nullable, metadata=metadata, validator=validator)
+        super().__init__(
+            pa.binary(byte_width), nullable=nullable, metadata=metadata, validator=validator, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.FixedSizeBinaryArray:
@@ -883,20 +1022,29 @@
     If you need a precision higher than 38 significant digits,
     consider using :class:`Decimal256Column`.
 
     :param precision: The number of significant digits.
     :param scale: The number of digits after the decimal point.
     :param nullable: Whether the column can contain nulls.
     :param metadata: A dictionary of metadata to attach to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
-        self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
+        self,
+        precision: int,
+        scale: int,
+        nullable: bool = True,
+        metadata: Optional[MetadataDict] = None,
+        default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
-        super().__init__(pa.decimal128(precision, scale), nullable=nullable, metadata=metadata)
+        super().__init__(
+            pa.decimal128(precision, scale), nullable=nullable, metadata=metadata, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal128Array:
@@ -918,20 +1066,29 @@
 
     Values are stored as 256-bit integers.
 
     :param precision: The number of significant digits.
     :param scale: The number of digits after the decimal point.
     :param nullable: Whether the column can contain nulls.
     :param metadata: A dictionary of metadata to attach to the column.
+    :param default: An optional default value for the column. This
+        can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
-        self, precision: int, scale: int, nullable: bool = True, metadata: Optional[MetadataDict] = None
+        self,
+        precision: int,
+        scale: int,
+        nullable: bool = True,
+        metadata: Optional[MetadataDict] = None,
+        default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
-        super().__init__(pa.decimal256(precision, scale), nullable=nullable, metadata=metadata)
+        super().__init__(
+            pa.decimal256(precision, scale), nullable=nullable, metadata=metadata, default=default
+        )
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> pa.Decimal256Array:
```

### Comparing `quivr-0.5.0/quivr/concat.py` & `quivr-0.6.0rc1/quivr/concat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 from typing import Iterator
 
 import pyarrow as pa
 
-from . import tables
+from . import errors, tables
 from .defragment import defragment
 
 
 def concatenate(values: Iterator[tables.AnyTable], defrag: bool = True) -> tables.AnyTable:
     """Concatenate a collection of Tables into a single Table.
 
-    All input Tables must have the same schema (typically, this will
-    be from being the same class).
+    All input Tables be of the same class, and have the same attribute
+    values (if any).
 
     By default, results are compacted to be contiguous in memory,
     which involves a copy. In a tight loop, this can be very
     inefficient, so you can set the 'defrag' parameter to False to
     skip this compaction step, and instead call :func:`defragment` on
     the result after the loop is complete.
 
     :param values: An iterator of :class:`Table` instances to concatenate.
     :param defrag: Whether to compact the result to be contiguous in
         memory. Defaults to True.
+
     """
     batches = []
     first = True
     for v in values:
         batches += v.table.to_batches()
         if first:
-            cls = v.__class__
+            first_cls = v.__class__
+            first_val = v
             first = False
+        else:
+            if v.__class__ != first_cls:
+                raise errors.TablesNotCompatibleError("All tables must be the same class to concatenate")
+            if not first_val._attr_equal(v):
+                raise errors.TablesNotCompatibleError(
+                    "All tables must have the same attribute values to concatenate"
+                )
+
     if len(batches) == 0:
         raise ValueError("No values to concatenate")
     table = pa.Table.from_batches(batches)
-    result = cls(table=table)
+    result = first_cls.from_pyarrow(table=table)
     if defrag:
         result = defragment(result)
     return result
```

### Comparing `quivr-0.5.0/quivr/linkage.py` & `quivr-0.6.0rc1/quivr/linkage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Any, Generic, Iterator, Optional, TypeVar
+from __future__ import annotations
+
+from typing import Any, Generic, Iterable, Iterator, List, Optional, Tuple, TypeVar
 
 import pyarrow as pa
 
-from . import tables
+from . import concat, errors, tables
 
 
 class ArrowArrayIndex:
     """
     Represents an index over the values in a PyArrow Array.
     """
 
@@ -222,21 +224,21 @@
         ... )
         >>> linkage = MultiKeyLinkage(
         ...     positions,
         ...     velocities,
         ...     {"id": positions.id, "time": positions.time},
         ...     {"id": velocities.id, "time": velocities.time},
         ... )
-        >>> for val, left, right in linkage:
+        >>> for val, left, right in sorted(linkage, key=lambda x: (x[0][1].as_py())):
         ...     print(val, left, right)
         [('id', 0), ('time', datetime.datetime(1970, 1, 1, 0, 0))] Positions(size=1) Velocities(size=1)
-        [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 4))] Positions(size=1) Velocities(size=1)
         [('id', 1), ('time', datetime.datetime(1970, 1, 1, 0, 0, 1))] Positions(size=1) Velocities(size=1)
-        [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 3))] Positions(size=1) Velocities(size=1)
         [('id', 1), ('time', datetime.datetime(1970, 1, 1, 0, 0, 2))] Positions(size=1) Velocities(size=1)
+        [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 3))] Positions(size=1) Velocities(size=1)
+        [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 4))] Positions(size=1) Velocities(size=1)
 
 
 
 
     :param left_table: The left table to link.
     :param right_table: The right table to link.
     :param left_keys: A dictionary of key names to arrays of values. The arrays
@@ -294,14 +296,32 @@
         self.scalar_type = pa.struct(self.dtypes)
 
         left_structarray = _build_struct_array(left_keys)
         right_structarray = _build_struct_array(right_keys)
 
         super().__init__(left_table, right_table, left_structarray, right_structarray)
 
+    @classmethod
+    def _from_structarray_keys(
+        cls,
+        left_table: LeftTable,
+        right_table: RightTable,
+        left_keys: pa.StructArray,
+        right_keys: pa.StructArray,
+    ) -> MultiKeyLinkage[LeftTable, RightTable]:
+        """Internal constructor used to create a MultiKeyLinkage when
+        the keys have already been converted to struct arrays.
+        """
+        self = cls.__new__(cls)
+        struct_dtype = left_keys.type
+        self.dtypes = {f.name: f.type for f in struct_dtype}
+        self.scalar_type = pa.struct(self.dtypes)
+        super().__init__(self, left_table, right_table, left_keys, right_keys)  # type: ignore
+        return self
+
     def key(self, **kwargs: Any) -> pa.Scalar:
         """
         Returns a composite key scalar for the given values.
 
         Example:
             >>> from quivr import *
             >>> class Positions(Table):
@@ -355,7 +375,114 @@
     """
     fields = []
     arrays = []
     for k, v in keys.items():
         fields.append(pa.field(k, v.type))
         arrays.append(v)
     return pa.StructArray.from_arrays(arrays, fields=fields)
+
+
+def combine_linkages(links: Iterable[Linkage[LeftTable, RightTable]]) -> Linkage[LeftTable, RightTable]:
+    """Combine a list of linkages into a single linkage.
+
+    The combined linkage will concatenate the left and right tables of
+    the source linkages, and then build an index on the combined
+    tables, using the same keys as the source linkages.
+
+    All the input linkages must have the same key names and table
+    types. All the tables that comprise the input linkages must have
+    identical attribute values, including for any nested subtables.
+
+    :param links: The linkages to concatenate.
+    :raises LinkageCombinationError: If the linkages do not have the same key names or if the
+        tables are not concatenatable.
+    :raises ValueError: If less than two linkages are provided.
+    :return: A linkage that combines the input linkages.
+    """
+    left_tables = []
+    right_tables = []
+    left_key_arrays = []
+    right_key_arrays = []
+    for next_link in links:
+        left_tables.append(next_link.left_table)
+        right_tables.append(next_link.right_table)
+        left_key_arrays.append(next_link.left_keys)
+        right_key_arrays.append(next_link.right_keys)
+
+    if len(left_tables) < 2:
+        raise ValueError("Must provide at least two linkages")
+
+    left_table, right_table, left_keys, right_keys = _concatenate_linkage_components(
+        left_tables, right_tables, left_key_arrays, right_key_arrays
+    )
+    return Linkage(left_table, right_table, left_keys, right_keys)
+
+
+def _concatenate_linkage_components(
+    left_tables: List[LeftTable],
+    right_tables: List[RightTable],
+    left_keys: List[pa.Array],
+    right_keys: List[pa.Array],
+) -> Tuple[LeftTable, RightTable, pa.Array, pa.Array]:
+    try:
+        left_table: LeftTable = concat.concatenate(left_tables)  # type: ignore
+    except errors.TablesNotCompatibleError as e:
+        raise errors.LinkageCombinationError("Left tables are not compatible") from e
+
+    try:
+        right_table: RightTable = concat.concatenate(right_tables)  # type: ignore
+    except errors.TablesNotCompatibleError as e:
+        raise errors.LinkageCombinationError("Right tables are not compatible") from e
+
+    try:
+        left_keys = pa.concat_arrays(left_keys)
+    except pa.lib.ArrowInvalid as e:
+        raise errors.LinkageCombinationError("Left keys types are not all identical") from e
+
+    try:
+        right_keys = pa.concat_arrays(right_keys)
+    except pa.lib.ArrowInvalid as e:
+        raise errors.LinkageCombinationError("Right keys types are not all identical") from e
+
+    assert len(left_table) == len(left_keys)
+    assert len(right_table) == len(right_keys)
+
+    return left_table, right_table, left_keys, right_keys
+
+
+def combine_multilinkages(
+    links: Iterable[MultiKeyLinkage[LeftTable, RightTable]]
+) -> MultiKeyLinkage[LeftTable, RightTable]:
+    """Combine a list of MultiKeyLinkages into a single MultiKeyLinkage.
+
+    The combined linkage will concatenate the left and right tables of
+    the source linkages, and then build an index on the combined
+    tables, using the same keys as the source linkages.
+
+    All the input linkages must have the same key structure (both
+    names and types), and must use the same table classes. All the
+    tables that comprise the input linkages must have identical
+    attribute values, including for any nested subtables.
+
+    :param links: The linkages to concatenate.
+    :raises LinkageCombinationError: If the linkages do not have the same key names or if the
+        tables are not concatenatable.
+    :raises ValueError: If less than two linkages are provided.
+    :return: A linkage that combines the input linkages.
+    """
+    left_tables = []
+    right_tables = []
+    left_key_arrays = []
+    right_key_arrays = []
+    for next_link in links:
+        left_tables.append(next_link.left_table)
+        right_tables.append(next_link.right_table)
+        left_key_arrays.append(next_link.left_keys)
+        right_key_arrays.append(next_link.right_keys)
+
+    if len(left_tables) < 2:
+        raise ValueError("Must provide at least two linkages")
+
+    left_table, right_table, left_keys, right_keys = _concatenate_linkage_components(
+        left_tables, right_tables, left_key_arrays, right_key_arrays
+    )
+    return MultiKeyLinkage._from_structarray_keys(left_table, right_table, left_keys, right_keys)
```

### Comparing `quivr-0.5.0/quivr/schemagraph.py` & `quivr-0.6.0rc1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.5.0/quivr/tables.py` & `quivr-0.6.0rc1/quivr/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 from io import IOBase
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
-from typing import Any, ClassVar, Iterator, Optional, Type, TypeAlias, TypeVar, Union
+from typing import (
+    Any,
+    ClassVar,
+    Iterator,
+    Optional,
+    Type,
+    TypeAlias,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
@@ -86,31 +96,61 @@
 
         # Add attributes
         cls._quivr_attributes = attributes
 
         # Add validators
         cls._column_validators = column_validators
 
-        # If the subclass has an __init__ override, it must have a
-        # with_table override as well.
-        if "__init__" in cls.__dict__ and "with_table" not in cls.__dict__:
-            raise TypeError(
-                f"{cls.__name__} has an __init__ override, but does not have a with_table "
-                + "override. You must implement both or neither."
-            )
-
         super().__init_subclass__(**kwargs)
 
     def __init__(self, table: pa.Table, **kwargs: AttributeValueType):
         self.table = table
         for name, value in kwargs.items():
             if name in self._quivr_attributes:
                 setattr(self, name, value)
             else:
                 raise AttributeError(f"{self.__class__.__name__} has no attribute {name}")
+        for name in self._quivr_attributes:
+            # Ensure all attributes are set or have a default
+            getattr(self, name)
+
+    @classmethod
+    def from_pyarrow(
+        cls,
+        table: pa.Table,
+        validate: bool = True,
+        **kwargs: AttributeValueType,
+    ) -> Self:
+        """Create a new table from a pyarrow Table.
+
+        This is a convenience method which can be used to create a
+        Table from a pyarrow Table. It can also accept keyword-style
+        arguments to set attributes on the table.
+
+        When serializing to pyarrow, the table's schema metadata
+        encodes the value of attributes. This method will use that
+        metadata to set the attributes on the table if it is
+        available. If any attributes are provided as keyword
+        arguments, they override any values in the metadata.
+
+        :param table: The pyarrow Table to create the table from.
+        :param validate: Whether to validate the table against the
+            schema, and run any column validators.
+        :param \\**kwargs: Keyword arguments to set attributes on the
+            table.
+        :type \\**kwargs: :obj:`AttributeValueType`
+        :return: A new Table instance.
+        """
+
+        schema = cls.schema.with_metadata(table.schema.metadata)
+        table = table.cast(schema)
+        instance = cls(table, **kwargs)
+        if validate:
+            instance.validate()
+        return instance
 
     @classmethod
     def from_data(
         cls,
         data: Union[pa.Table, dict[str, Any], list[Any], pd.DataFrame, None] = None,
         validate: bool = True,
         **kwargs: Union[AttributeValueType, DataSourceType],
@@ -155,15 +195,15 @@
 
         """
         if data is None:
             instance = cls.from_kwargs(**kwargs)
         else:
             attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
             if isinstance(data, pa.Table):
-                instance = cls(table=data, **attrib_kwargs)
+                instance = cls.from_pyarrow(data, False, **attrib_kwargs)
             elif isinstance(data, dict):
                 instance = cls.from_pydict(data, **attrib_kwargs)
             elif isinstance(data, list):
                 if len(data) == 0:
                     instance = cls.from_rows(data, **attrib_kwargs)
                 elif isinstance(data[0], dict):
                     instance = cls.from_rows(data, **attrib_kwargs)
@@ -241,24 +281,27 @@
         metadata: dict[bytes, bytes] = {}
         for i, field in enumerate(cls.schema):
             column_name = field.name
             value = kwargs.pop(column_name, None)
 
             if value is None:
                 if not field.nullable:
-                    raise ValueError(f"Missing non-nullable column {column_name}")
+                    column = getattr(cls, column_name)
+                    if column.default is None:
+                        raise ValueError(f"Missing non-nullable column {column_name}")
+                if size is not None:
+                    value = pa.nulls(size, type=cls.schema[i].type)
+                    arrays.append(value)
                 else:
-                    if size is not None:
-                        arrays.append(pa.nulls(size, type=cls.schema[i].type))
-                    else:
-                        # We'll have to wait until we get to a non-None column
-                        # to figure out the size.
-                        empty_columns.append(i)
-                        arrays.append(None)
-                    continue
+                    # We'll have to wait until we get to a non-None column
+                    # to figure out the size.
+                    empty_columns.append(i)
+                    arrays.append(None)
+                continue
+
             if size is None:
                 size = len(value)  # type: ignore
             elif len(value) != size:
                 raise ValueError(
                     f"Column {column_name} has wrong length {len(value)} (first column has length {size})"
                 )
 
@@ -281,14 +324,23 @@
                 raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
             arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
+
+        # Inform the type checker that we've filled all Nones
+        arrays = cast(list[pa.Array], arrays)
+
+        for i, array in enumerate(arrays):
+            if array.null_count > 0:
+                column = getattr(cls, cls.schema[i].name)
+                arrays[i] = column.fill_default(array)
+
         attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
         return cls.from_arrays(arrays, metadata=metadata, **attrib_kwargs)
 
     @classmethod
     def from_arrays(
         cls,
         arrays: list[pa.Array],
@@ -304,22 +356,22 @@
         :type \\**kwargs: :obj:`AttributeValueType`
         :return: A Table object.
         """
         if metadata is None:
             metadata = {}
         schema = cls.schema.with_metadata(metadata)
         table = pa.Table.from_arrays(arrays, schema=schema)
-        return cls(table=table, **kwargs)
+        return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
     def from_pydict(
         cls, d: dict[str, Union[pa.array, list[Any], npt.NDArray[Any]]], **kwargs: AttributeValueType
     ) -> Self:
         table = pa.Table.from_pydict(d, schema=cls.schema)
-        return cls(table=table, **kwargs)
+        return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
     def from_rows(cls, rows: list[dict[str, Any]], **kwargs: AttributeValueType) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
         :param rows: A list of values. Each value corresponds to a row in the table.
@@ -375,15 +427,15 @@
 
         :param df: A pandas DataFrame containing the data to load.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
-        return cls(table=table, **kwargs)
+        return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
     def _unflatten_table(cls, table: pa.Table) -> pa.Table:
         """Unflatten a Table.
 
         This is used when loading a flattened CSV into a nested
         Table. It takes a Table with a flat schema, and returns a
@@ -725,15 +777,15 @@
         table = cls._load_parquet_table(
             path=path,
             memory_map=memory_map,
             pq_buffer_size=pq_buffer_size,
             filters=filters,
             column_name_map=column_name_map,
         )
-        return cls(table=table, **kwargs)
+        return cls.from_pyarrow(table=table, validate=True, **kwargs)
 
     @classmethod
     def _load_parquet_table(
         cls,
         path: str,
         memory_map: bool,
         pq_buffer_size: int,
```

### Comparing `quivr-0.5.0/quivr/validators.py` & `quivr-0.6.0rc1/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.5.0/LICENSE` & `quivr-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.5.0/README.md` & `quivr-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.5.0/pyproject.toml` & `quivr-0.6.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -35,26 +35,27 @@
 include = [
   "/quivr",
 ]
 
 [tool.hatch.version]
 path = "quivr/__version__.py"
 
-[tool.hatch.envs.default]
+[tool.hatch.envs.dev]
 dependencies = [
   "black",
   "isort",
   "mypy",
   "pandas-stubs",
   "pytest",
   "pytest-benchmark",
   "ruff",
+  "ipython"
 ]
 
-[tool.hatch.envs.default.scripts]
+[tool.hatch.envs.dev.scripts]
 check = [
   "lint",
   "typecheck",
   "test",
 ]
 fix = [
   "ruff ./quivr ./test --fix"
@@ -68,27 +69,49 @@
   "black ./quivr ./test",
   "isort ./quivr ./test"
 ]
 typecheck = [
   "mypy --strict ./quivr ./examples ./test/typing_tests",
 ]
 test = [
-  "pytest --benchmark-disable ./test",
+  "pytest --benchmark-disable ./test {args}",
 ]
 doctest = [
-  "pytest --doctest-modules ./quivr"
+  "pytest --doctest-modules ./quivr {args}"
 ]
 benchmark = [
-  "pytest --benchmark-only ./test"
+  "pytest --benchmark-only ./test {args}"
+]
+
+[tool.hatch.envs.test]
+dependencies = [
+  "black",
+  "isort",
+  "mypy",
+  "pandas-stubs",
+  "pytest",
+  "pytest-benchmark",
+  "ruff",
+]
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.10", "3.11"]
+
+[tool.hatch.envs.test.scripts]
+all = [
+  "ruff ./quivr ./test",
+  "black --check ./quivr ./test",
+  "isort --check-only ./quivr ./test",
+  "mypy --strict ./quivr ./examples ./test/typing_tests",
+  "pytest --benchmark-disable ./test {args}",
+  "pytest --doctest-modules ./quivr",  
 ]
-gauntlet = [
-   "hatch run lint",
-   "hatch run typecheck",
-   "hatch run test",
-   "hatch run doctest",
+
+benchmark = [
+  "pytest --benchmark-only ./test"
 ]
 
 [tool.hatch.envs.docs]
 dependencies = [
   "sphinx==7.0.1",
   "sphinx-autodoc-typehints",
   "sphinx-copybutton",
@@ -97,23 +120,23 @@
 ]
 
 [tool.hatch.envs.docs.scripts]
 make-html = [
   "make -C docs html"
 ]
 
-open-docs = [
+open-html = [
   "open docs/build/html/index.html"
 ]
 
-clean-html = [
+clean = [
   "make -C docs clean"
 ]
 
-rebuild-html = [
+rebuild = [
   "make -C docs clean",
   "make -C docs html"
 ]
 
 [tool.black]
 line-length = 110
```

### Comparing `quivr-0.5.0/PKG-INFO` & `quivr-0.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.5.0
+Version: 0.6.0rc1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

