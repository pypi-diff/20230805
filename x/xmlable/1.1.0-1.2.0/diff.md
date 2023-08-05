# Comparing `tmp/xmlable-1.1.0.tar.gz` & `tmp/xmlable-1.2.0.tar.gz`

## Comparing `xmlable-1.1.0.tar` & `xmlable-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,47 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 xmlable-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/config_xml_template.xml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/basic_config/main.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config.xsd
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config_xml_example.xml
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/config_xml_template.xml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/complex/main.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/invalid/main.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config.xsd
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config_xml_example.xml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/config_xml_template.xml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/maps/main.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config.xsd
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config_xml_example.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/config_xml_template.xml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/namespaces/main.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config.xsd
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config_xml_example.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/config_xml_template.xml
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 xmlable-1.1.0/examples/userdefined/main.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_errors.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_io.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_lxml_helpers.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_manual.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_user.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_utils.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_xmlify.py
--rw-r--r--   0        0        0    23209 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/_xobject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.1.0/src/xmlable/py.typed
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-1.1.0/tests/test_basic.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.1.0/LICENSE
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 xmlable-1.1.0/README.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 xmlable-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xmlable-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 xmlable-1.2.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 xmlable-1.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/basic_config/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/basic_config/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/basic_config/config_xml_template.xml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/basic_config/main.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex/config.xsd
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex/config_xml_example.xml
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex/config_xml_template.xml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex/main.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex_application/config.xsd
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex_application/config_xml_example.xml
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex_application/config_xml_template.xml
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex_application/ipconn.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/complex_application/main.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/invalid/main.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/maps/config.xsd
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/maps/config_xml_example.xml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/maps/config_xml_template.xml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/maps/main.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/namespaces/config.xsd
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/namespaces/config_xml_example.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/namespaces/config_xml_template.xml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/namespaces/main.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/userdefined/config.xsd
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/userdefined/config_xml_example.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/userdefined/config_xml_template.xml
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/userdefined/main.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 xmlable-1.2.0/examples/userdefined/pgconn.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/__init__.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_errors.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_io.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_lxml_helpers.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_manual.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_user.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_utils.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_xmlify.py
+-rw-r--r--   0        0        0    20621 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/_xobject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmlable-1.2.0/src/xmlable/py.typed
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 xmlable-1.2.0/tests/test_basic.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 xmlable-1.2.0/tests/test_errors.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xmlable-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 xmlable-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 xmlable-1.2.0/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 xmlable-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 xmlable-1.2.0/PKG-INFO
```

### Comparing `xmlable-1.1.0/examples/basic_config/config.xsd` & `xmlable-1.2.0/examples/basic_config/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/basic_config/main.py` & `xmlable-1.2.0/examples/basic_config/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/complex/config.xsd` & `xmlable-1.2.0/examples/complex/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/complex/config_xml_example.xml` & `xmlable-1.2.0/examples/complex/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/complex/config_xml_template.xml` & `xmlable-1.2.0/examples/complex/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/complex/main.py` & `xmlable-1.2.0/examples/complex/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/maps/config.xsd` & `xmlable-1.2.0/examples/maps/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/maps/config_xml_example.xml` & `xmlable-1.2.0/examples/maps/config_xml_example.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/maps/config_xml_template.xml` & `xmlable-1.2.0/examples/maps/config_xml_template.xml`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/maps/main.py` & `xmlable-1.2.0/examples/maps/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/namespaces/config.xsd` & `xmlable-1.2.0/examples/namespaces/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/namespaces/main.py` & `xmlable-1.2.0/examples/namespaces/main.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/userdefined/config.xsd` & `xmlable-1.2.0/examples/userdefined/config.xsd`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/examples/userdefined/main.py` & `xmlable-1.2.0/examples/userdefined/pgconn.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 from xmlable._lxml_helpers import with_child, with_text, XMLSchema, XMLURL
 from xmlable._errors import XError, XErrorCtx
 from xmlable._xobject import XObject
 from xmlable._user import IXmlify
 from xmlable._manual import manual_xmlify
 from xmlable._utils import firstkey
 
-# public/external interface
-from xmlable import xmlify, write_file, parse_file
-
 import re
 
 CONN_STR = "postgresql://user:password@netloc:port/dbname?param1=value1&..."
 CONN_PATTERN = "postgresql:\/\/([^:]*):([^@]*)?@([^:]*):(\d+)\/([^\?]*)(\??.*)"
 
 
 @manual_xmlify
@@ -124,54 +121,7 @@
                 restrict,
                 Element(f"{XMLSchema}pattern", value=CONN_PATTERN),
             ),
         )
 
     def xsd_dependencies() -> set[type]:
         return {PostgresConn}
-
-
-@xmlify
-@dataclass
-class MyConfig:
-    foos: int
-    conns: list[PostgresConn]
-
-
-write_file("config.xsd", MyConfig.xsd())
-write_file("config_xml_template.xml", MyConfig.xml())
-
-original: MyConfig = MyConfig(
-    foos=3,
-    conns=[
-        PostgresConn(
-            user="jimmy",
-            password="pass123",
-            netloc="localhost",
-            port=5432,
-            dbname="saul_db",
-            options={"secret": "10101"},
-        ),
-        PostgresConn(
-            user="bob",
-            password="username",
-            netloc="localhost",
-            port=5444,
-            dbname="other_db",
-            options={},
-        ),
-        PostgresConn(
-            user="steve",
-            password="pass1234",
-            netloc="localhost",
-            port=5444,
-            dbname="other_db",
-            options={"backdoor_key": "bingo"},
-        ),
-    ],
-)
-
-write_file("config_xml_example.xml", original.xml_value())
-
-read_config: MyConfig = parse_file(MyConfig, "config_xml_example.xml")
-
-assert read_config == original
```

### Comparing `xmlable-1.1.0/src/xmlable/_lxml_helpers.py` & `xmlable-1.2.0/src/xmlable/_lxml_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/src/xmlable/_manual.py` & `xmlable-1.2.0/src/xmlable/_manual.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,40 @@
 
 from typing import Any
 from lxml.etree import _Element, Element, _ElementTree, ElementTree
 from lxml.objectify import ObjectifiedElement
 
 from xmlable._utils import typename
 from xmlable._lxml_helpers import with_children, XMLSchema
-from xmlable._errors import XError, XErrorCtx
+from xmlable._errors import XError, XErrorCtx, ErrorTypes
 
 
 def validate_manual_class(cls: type):
-    cls_name = typename(cls)
     attrs = {"get_xobject", "xsd_forward", "xsd_dependencies"}
     for attr in attrs:
         if not hasattr(cls, attr):
-            all_attrs = ", ".join(attrs)
-            raise XError(
-                short="Missing Attribute",
-                what=f"The attribute {attr} is missing from {cls_name}",
-                why=f"To be manual_xmlified the attributes: {all_attrs} are required. Try using help(IXmlify)",
-                ctx=XErrorCtx([cls_name]),
-            )
+            raise ErrorTypes.MissingAttribute(cls, attrs, attr)
+
+
+def type_cycle(from_type: type) -> list[type]:
+    # INV: it is an xmlified type for a user define structure
+    cycle: list[type] = []
+
+    def visit_dep(curr: type) -> bool:
+        if curr == from_type or any(
+            visit_dep(dep) for dep in curr.xsd_dependencies()
+        ):
+            cycle.append(curr)
+            return True
+        else:
+            return False
+
+    assert visit_dep(from_type)
+    cycle.append(from_type)
+    return cycle
 
 
 def manual_xmlify(cls: type) -> type:
     """
     Generate the following methods:
     ```
     def xsd(
@@ -60,14 +71,16 @@
             imports: dict[str, str] = {},
         ) -> _ElementTree:
             # Get dependencies (user classes that need to be declared before)
             visited: set[type] = set()
             dec_order: list[type] = []
 
             def toposort(curr: type, visited: set[type], dec_order: list[type]):
+                if curr in visited:
+                    raise ErrorTypes.DependencyCycle(type_cycle(curr))
                 visited.add(curr)
                 deps = curr.xsd_dependencies()  # type: ignore[attr-defined]
                 for d in deps:
                     if d not in visited:
                         toposort(d, visited, dec_order)
                 dec_order.append(curr)
```

### Comparing `xmlable-1.1.0/src/xmlable/_user.py` & `xmlable-1.2.0/src/xmlable/_user.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/src/xmlable/_utils.py` & `xmlable-1.2.0/src/xmlable/_utils.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/src/xmlable/_xobject.py` & `xmlable-1.2.0/src/xmlable/_xobject.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from types import NoneType, UnionType
 from lxml.objectify import ObjectifiedElement
 from lxml.etree import Element, Comment, _Element
 from abc import ABC, abstractmethod
 from typing import Any, Callable, get_args
 
 from xmlable._utils import get, typename, firstkey
-from xmlable._errors import XErrorCtx, XError
+from xmlable._errors import XErrorCtx, ErrorTypes
 from xmlable._lxml_helpers import (
     with_text,
     with_child,
     with_children,
     XMLSchema,
     XMLURL,
     children,
@@ -99,32 +99,22 @@
             )
 
     def xml_temp(self, name: str) -> _Element:
         return with_text(Element(name), f"Fill me with an {self.type_str}")
 
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         if not self.validate_fn(val):
-            raise XError(
-                short="Invalid Data",
-                what=f"Could not validate {val} as a valid {self.type_str}",
-                why=f"Produced xml must be valid",
-                ctx=ctx,
-            )
+            raise ErrorTypes.InvalidData(ctx, val, self.type_str)
         return with_text(Element(name), self.convert_fn(val))
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> Any:
         try:
             return self.parse_fn(obj)
         except Exception as e:
-            raise XError(
-                short="Parse Failure",
-                what=f"Failed to parse {obj.text} as a {self.type_str} with error: \n {e}",
-                why=f"This error implies the xml is not validated against the current xsd, or there is a bug in this type's parser",
-                ctx=ctx,
-            )
+            raise ErrorTypes.ParseFailure(ctx, obj.text, self.type_str, e)
 
 
 @dataclass
 class ListObj(XObject):
     """
     An ordered list of objects
     """
@@ -184,19 +174,16 @@
                 Element(name), Comment(f"Empty {self.struct_name}!")
             )
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> list[Any]:
         parsed = []
         for i, child in enumerate(children(obj)):
             if child.tag != self.list_elem_name:
-                raise XError(
-                    short="Unexpected Tag",
-                    what=f"Found {self.list_elem_name} but found {child.tag}",
-                    why=f"This is a {self.struct_name} that contains 0..n elements of {self.list_elem_name} and no other elements",
-                    ctx=ctx,
+                raise ErrorTypes.UnexpectedTag(
+                    ctx, self.list_elem_name, self.struct_name, child.tag
                 )
             else:
                 parsed.append(
                     self.item_xobject.xml_in(
                         child, ctx.next(f"{self.list_elem_name}[{i}]")
                     )
                 )
@@ -236,19 +223,16 @@
             Element(name),
             [Comment(f"This is a {self.struct_name}")]
             + [xobj.xml_temp(member) for member, xobj in self.objects],
         )
 
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         if len(val) != len(self.objects):
-            raise XError(
-                short="Incorrect Type",
-                what=f"You have provided the values {len(val)} values {val} for {name}, but {name} is a {self.struct_name} that takes only {len(self.objects)} values",
-                why=f"In order to generate xml, the values provided need to be the correct types",
-                ctx=ctx,
+            raise ErrorTypes.IncorrectType(
+                ctx, len(self.objects), self.struct_name, val, name
             )
 
         return with_children(
             Element(name),
             [
                 xobj.xml_out(member, v, ctx.next(member))
                 for (member, xobj), v in zip(self.objects, val)
@@ -259,19 +243,16 @@
         self, obj: ObjectifiedElement, ctx: XErrorCtx
     ) -> list[tuple[str, Any]]:
         parsed = []
         for i, (child, (name, xobj)) in enumerate(
             zip(children(obj), self.objects)
         ):
             if child.tag != name:
-                raise XError(
-                    short="Incorrect Element Tag",
-                    what=f"While parsing {self.struct_name} {obj.tag} we expected element {i} to be {name}, but found {child.tag}",
-                    why=f"The xml representation for {self.struct_name} requires the correct names in the correct order",
-                    ctx=ctx,
+                raise ErrorTypes.IncorrectElementTag(
+                    ctx, self.struct_name, obj.tag, i, name, child.tag
                 )
             parsed.append((name, xobj.xml_in(child, ctx.next(name))))
         return parsed
 
 
 class TupleObj(XObject):
     """An anonymous struct"""
@@ -328,19 +309,16 @@
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         return self.list.xml_out(name, list(val), ctx)
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> set[Any]:
         parsed: set[Any] = set()
         for item in self.list.xml_in(obj, ctx):
             if item in parsed:
-                raise XError(
-                    short="Duplicate item in Set",
-                    what=f"In {obj.tag} the item {item} is present more than once",
-                    why=f"A set can only contain unique items",
-                    ctx=ctx,
+                raise ErrorTypes.DuplicateItem(
+                    ctx, self.struct_name, obj.tag, item
                 )
             parsed.add(item)
         return parsed
 
 
 @dataclass
 class DictObj(XObject):
@@ -424,35 +402,34 @@
             ],
         )
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> dict[Any, Any]:
         parsed = {}
         for child in children(obj):
             if child.tag != self.item_name:
-                raise XError(
-                    short="Invalid item in dictionary",
-                    what=f"An unexpected item with {child.tag} is in dictionary {obj.tag}",
-                    why=f"Each item must have tag {self.item_name} with children {self.key_name} and {self.val_name}",
-                    ctx=ctx,
+                raise ErrorTypes.InvalidDictionaryItem(
+                    ctx,
+                    self.item_name,
+                    self.key_name,
+                    self.val_name,
+                    child.tag,
+                    obj.tag,
                 )
             else:
                 child_ctx = ctx.next(self.item_name)
                 k = self.key_xobject.xml_in(
                     get(child, self.key_name), child_ctx.next(self.key_name)
                 )
                 v = self.val_xobject.xml_in(
                     get(child, self.val_name), child_ctx.next(self.val_name)
                 )
 
                 if k in parsed:
-                    raise XError(
-                        short="Duplicate key in dictionary",
-                        what=f"In dictionary {obj.tag} the key {k} is present more than once",
-                        why=f"Dictionaries must have unique keys",
-                        ctx=ctx,
+                    raise ErrorTypes.DuplicateItem(
+                        ctx, "dictionary", obj.tag, k
                     )
 
                 parsed[k] = v
                 # Check for other tags? Fail better?
         return parsed
 
 
@@ -530,45 +507,31 @@
         if t is not None and (val_xobj := self.xobjects.get(t)) is not None:
             variant_name = self.elem_gen(t)
             return with_child(
                 Element(name),
                 val_xobj.xml_out(variant_name, val, ctx.next(variant_name)),
             )
         else:
-            types = " | ".join(str(t) for t in self.xobjects.keys())
-            raise XError(
-                short=f"Datatype not in Union",
-                what=f"{name} is a union of {types}, which does not contain {t} (you provided: {val})",
-                why=f"... uuuh, its a union?",
-                ctx=ctx,
+            raise ErrorTypes.InvalidVariant(
+                ctx, name, self.xobjects.keys(), t, val
             )
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> Any:
         named = {self.elem_gen(t): xobj for t, xobj in self.xobjects.items()}
         variants = list(children(obj))
 
         if len(variants) != 1:
-            variant_names = ", ".join(v.tag for v in variants)
-            raise XError(
-                short="Multiple union variants present",
-                what=f"variants {variant_names} are present",
-                why=f"A union can only be one variant at a time",
-                ctx=ctx,
-            )
+            raise ErrorTypes.MultipleVariants(ctx, [v.tag for v in variants])
 
         variant = variants[0]
         if (xobj := named.get(variant.tag)) is not None:
             return xobj.xml_in(variant, ctx.next(variant.tag))
         else:
-            named_vars = ", ".join(named.keys())
-            raise XError(
-                short="Invalid Variant",
-                what=f"The union {obj.tag} can contain variants {named_vars}, but you have used {variant}",
-                why=f"Only valid variants can be parsed",
-                ctx=ctx,
+            raise ErrorTypes.ParseInvalidVariant(
+                ctx, obj.tag, named.keys(), variant
             )
 
 
 class NoneObj(XObject):
     """
     An object representing the python 'None' type
     - Unions of form `int | None` are used for optionals
@@ -586,20 +549,15 @@
         )
 
     def xml_temp(self, name: str) -> _Element:
         return with_child(Element(name), Comment("This is None"))
 
     def xml_out(self, name: str, val: Any, ctx: XErrorCtx) -> _Element:
         if val != None:
-            raise XError(
-                short="None object is not None",
-                what=f"{name} contains value {val} which is not None",
-                why="A None type object can only contain none",
-                ctx=ctx,
-            )
+            raise ErrorTypes.NoneIsSome(ctx, name, val)
 
         return with_child(Element(name), Comment("This is None"))
 
     def xml_in(self, obj: ObjectifiedElement, ctx: XErrorCtx) -> Any:
         return None
 
 
@@ -661,12 +619,8 @@
             (item_type,) = get_args(data_type)
             return SetOBj(gen_xobject(item_type, forward_dec))
         else:
             if is_xmlified(data_type):
                 forward_dec.add(data_type)
                 return data_type.get_xobject()  # type: ignore[attr-defined, no-any-return]
             else:
-                raise XError(
-                    short="Non XMlified Type",
-                    what=f"You attempted to use {t_name} in an xmlified class, but {t_name} is not xmlified",
-                    why=f"All types usin in an xmlified class must be xmlified",
-                )
+                raise ErrorTypes.NonXMlifiedType(t_name)
```

### Comparing `xmlable-1.1.0/tests/test_basic.py` & `xmlable-1.2.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/LICENSE` & `xmlable-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlable-1.1.0/README.md` & `xmlable-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -118,27 +118,32 @@
 In this case an error is raised
 
 ## To Develop
 
 ```bash
 git clone # this project
 
-python3.11 -m venv ./.venv
+# Can use hatch to build, run
+hatch run check:lint
+hatch run check:test
+hatch run check:typecheck
+
+# Alternatively can just create a normal env
+python3.11 -m venv .venv
+source .venv/bin/activate # activate virtual environment
 
-source ./.venv/bin/activate # activate virtual environment
-
-pip install .      # install this project in the venv
-pip install .[dev] # install optional dev dependencies (mypy, black and pytest)
+pip install -e .      # install this project in the venv
+pip install -e .[dev] # install optional dev dependencies (mypy, black and pytest)
 
 black . # to reformat
 mypy    # type check
 pytest  # to run tests
 ```
 
-[Hatch](https://hatch.pypa.io/) is used for build.
+[Hatch](https://hatch.pypa.io/) is used for build, test and pypi publish.
 
 ## To Improve
 
 ### Fuzzing
 
 (As a fun weekend project) generate arbitrary python data types with values, and dataclasses.
 Then `@xmlify` all and validate as in the current tests
```

### Comparing `xmlable-1.1.0/pyproject.toml` & `xmlable-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xmlable"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Oliver Killane", email="oliverkillane.business@gmail.com" },
 ]
 description = "A decorator for generating xsd, xml and parsers from dataclasses"
 readme = "README.md"
 license = { file = "LICENSE"}
 keywords = ["xml", "xmlschema", "xsd", "lxml"]
```

### Comparing `xmlable-1.1.0/PKG-INFO` & `xmlable-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlable
-Version: 1.1.0
+Version: 1.2.0
 Summary: A decorator for generating xsd, xml and parsers from dataclasses
 Project-URL: Homepage, https://github.com/OliverKillane/xmlable
 Project-URL: Bug Tracker, https://github.com/OliverKillane/xmlable/issues
 Project-URL: Source, https://github.com/OliverKillane/xmlable
 Author-email: Oliver Killane <oliverkillane.business@gmail.com>
 License: MIT License
         
@@ -162,27 +162,32 @@
 In this case an error is raised
 
 ## To Develop
 
 ```bash
 git clone # this project
 
-python3.11 -m venv ./.venv
+# Can use hatch to build, run
+hatch run check:lint
+hatch run check:test
+hatch run check:typecheck
+
+# Alternatively can just create a normal env
+python3.11 -m venv .venv
+source .venv/bin/activate # activate virtual environment
 
-source ./.venv/bin/activate # activate virtual environment
-
-pip install .      # install this project in the venv
-pip install .[dev] # install optional dev dependencies (mypy, black and pytest)
+pip install -e .      # install this project in the venv
+pip install -e .[dev] # install optional dev dependencies (mypy, black and pytest)
 
 black . # to reformat
 mypy    # type check
 pytest  # to run tests
 ```
 
-[Hatch](https://hatch.pypa.io/) is used for build.
+[Hatch](https://hatch.pypa.io/) is used for build, test and pypi publish.
 
 ## To Improve
 
 ### Fuzzing
 
 (As a fun weekend project) generate arbitrary python data types with values, and dataclasses.
 Then `@xmlify` all and validate as in the current tests
```

