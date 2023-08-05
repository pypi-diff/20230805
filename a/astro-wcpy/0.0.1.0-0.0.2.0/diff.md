# Comparing `tmp/astro-wcpy-0.0.1.0.tar.gz` & `tmp/astro-wcpy-0.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-wcpy-0.0.1.0.tar", last modified: Mon Feb  6 04:35:16 2023, max compression
+gzip compressed data, was "astro-wcpy-0.0.2.0.tar", last modified: Sat Aug  5 19:07:31 2023, max compression
```

## Comparing `astro-wcpy-0.0.1.0.tar` & `astro-wcpy-0.0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-02-06 04:35:16.833889 astro-wcpy-0.0.1.0/
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)    35149 2021-11-16 09:00:35.000000 astro-wcpy-0.0.1.0/LICENSE
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      685 2023-02-06 04:35:16.833889 astro-wcpy-0.0.1.0/PKG-INFO
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      145 2023-02-06 04:28:06.000000 astro-wcpy-0.0.1.0/README.md
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)     1052 2023-02-06 04:27:32.000000 astro-wcpy-0.0.1.0/pyproject.toml
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       71 2023-02-05 12:46:19.000000 astro-wcpy-0.0.1.0/requirements.txt
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       38 2023-02-06 04:35:16.833889 astro-wcpy-0.0.1.0/setup.cfg
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       38 2023-02-05 12:52:06.000000 astro-wcpy-0.0.1.0/setup.py
-drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-02-06 04:35:16.829889 astro-wcpy-0.0.1.0/src/
-drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-02-06 04:35:16.829889 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      685 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/PKG-INFO
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      469 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/SOURCES.txt
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)        1 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/dependency_links.txt
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       65 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/entry_points.txt
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       72 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/requires.txt
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)        5 2023-02-06 04:35:16.000000 astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/top_level.txt
-drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-02-06 04:35:16.833889 astro-wcpy-0.0.1.0/src/wcpy/
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       49 2023-02-06 04:34:54.000000 astro-wcpy-0.0.1.0/src/wcpy/__init__.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)     1286 2023-02-05 13:25:18.000000 astro-wcpy-0.0.1.0/src/wcpy/command_line.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)    27265 2023-02-06 04:33:54.000000 astro-wcpy-0.0.1.0/src/wcpy/mainwindow.py
-drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-02-06 04:35:16.833889 astro-wcpy-0.0.1.0/src/wcpy/ui/
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      222 2023-02-05 11:29:16.000000 astro-wcpy-0.0.1.0/src/wcpy/ui/__init__.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      124 2023-02-05 11:29:24.000000 astro-wcpy-0.0.1.0/src/wcpy/ui/fonts.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)    42848 2023-02-04 13:42:17.000000 astro-wcpy-0.0.1.0/src/wcpy/ui/mainwindow.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)     6160 2023-02-04 11:45:21.000000 astro-wcpy-0.0.1.0/src/wcpy/ui/widgets.py
--rw-rw-r--   0 rzhao     (1000) rzhao     (1000)     4159 2023-02-06 04:33:45.000000 astro-wcpy-0.0.1.0/src/wcpy/utils.py
+drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)    35149 2021-11-16 17:00:35.000000 astro-wcpy-0.0.2.0/LICENSE
+-rw-rw-r--   0 rzhao     (1000) rzhao     (1000)      685 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/PKG-INFO
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)      145 2023-02-06 12:28:06.000000 astro-wcpy-0.0.2.0/README.md
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)     1045 2023-08-04 16:49:08.000000 astro-wcpy-0.0.2.0/pyproject.toml
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)       91 2023-08-05 18:11:48.000000 astro-wcpy-0.0.2.0/requirements.txt
+-rw-rw-r--   0 rzhao     (1000) rzhao     (1000)       38 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/setup.cfg
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)       38 2023-02-05 20:52:06.000000 astro-wcpy-0.0.2.0/setup.py
+drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-08-05 19:07:31.965662 astro-wcpy-0.0.2.0/src/
+drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)      685 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/PKG-INFO
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)      454 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)        1 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)       58 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/entry_points.txt
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)       92 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/requires.txt
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)        5 2023-08-05 19:07:31.000000 astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/top_level.txt
+drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/src/wcpy/
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)       49 2023-07-19 20:08:21.000000 astro-wcpy-0.0.2.0/src/wcpy/__init__.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)    43639 2023-08-05 19:00:33.000000 astro-wcpy-0.0.2.0/src/wcpy/core.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)     5268 2023-08-05 17:56:58.000000 astro-wcpy-0.0.2.0/src/wcpy/io.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)     2044 2023-08-04 16:45:26.000000 astro-wcpy-0.0.2.0/src/wcpy/script.py
+drwxrwxr-x   0 rzhao     (1000) rzhao     (1000)        0 2023-08-05 19:07:31.969662 astro-wcpy-0.0.2.0/src/wcpy/ui/
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)      356 2023-08-04 15:36:03.000000 astro-wcpy-0.0.2.0/src/wcpy/ui/__init__.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)      259 2023-08-04 15:35:52.000000 astro-wcpy-0.0.2.0/src/wcpy/ui/fonts.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)    44891 2023-08-05 18:28:57.000000 astro-wcpy-0.0.2.0/src/wcpy/ui/mainwindow.py
+-rwxr-xr-x   0 rzhao     (1000) rzhao     (1000)     7728 2023-08-05 16:59:09.000000 astro-wcpy-0.0.2.0/src/wcpy/ui/widgets.py
```

### Comparing `astro-wcpy-0.0.1.0/LICENSE` & `astro-wcpy-0.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-wcpy-0.0.1.0/PKG-INFO` & `astro-wcpy-0.0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-wcpy
-Version: 0.0.1.0
+Version: 0.0.2.0
 Summary: A UI for wavelength calibration.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/wcpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/wcpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-wcpy-0.0.1.0/pyproject.toml` & `astro-wcpy-0.0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3", 
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)", 
     "Operating System :: OS Independent", 
 ]
 dynamic = ["version", "dependencies"]
 
 [project.scripts]
-wavelength-calibrator = "wcpy.command_line:main"
+wavelength-calibrator = "wcpy.script:run"
 
 [project.urls]
 "Homepage" = "https://github.com/RuiningZHAO/wcpy"
 "Tracker" = "https://github.com/RuiningZHAO/wcpy/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
```

### Comparing `astro-wcpy-0.0.1.0/src/astro_wcpy.egg-info/PKG-INFO` & `astro-wcpy-0.0.2.0/src/astro_wcpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-wcpy
-Version: 0.0.1.0
+Version: 0.0.2.0
 Summary: A UI for wavelength calibration.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/wcpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/wcpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-wcpy-0.0.1.0/src/wcpy/ui/widgets.py` & `astro-wcpy-0.0.2.0/src/wcpy/ui/widgets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,90 @@
 # -*- coding: utf-8 -*-
 # PyQt5
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
+class TableItemCompleter(QtWidgets.QStyledItemDelegate):
+
+    def createEditor(self, parent, option, index):
+
+        editor = QtWidgets.QLineEdit(parent)
+        # Positive integer or float
+        editor.setValidator(
+            QtGui.QRegExpValidator(
+                QtCore.QRegExp("^([1-9]\d*)|([1-9]\d*\.\d*)|(0\.\d*[1-9]\d*)|()$")
+            )
+        )
+        # Auto-completion
+        completion_list = index.data(QtCore.Qt.UserRole)
+        completer = QtWidgets.QCompleter(completion_list, parent)
+        editor.setCompleter(completer)
+
+        return editor
+
+
+class FormLayout(QtWidgets.QFormLayout):
+
+    def __init__(self, object_name=None):
+
+        super().__init__()
+
+        if object_name is not None:
+            self.setObjectName(object_name)
+
+        self.setSizeConstraint(QtWidgets.QLayout.SetFixedSize)
+        self.setFieldGrowthPolicy(QtWidgets.QFormLayout.AllNonFixedFieldsGrow)
+        self.setLabelAlignment(
+            QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.setFormAlignment(
+            QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
+        self.setContentsMargins(0, -1, 0, -1)
+        self.setHorizontalSpacing(10)
+
+
+class InformationBox(QtWidgets.QMessageBox):
+
+    def __init__(self, window_title=None, text=None):
+
+        super().__init__()
+
+        self.setIcon(QtWidgets.QMessageBox.Information)
+        self.setWindowTitle(window_title)
+        self.setText(text)
+
+
 class CheckBoxFileDialog(QtWidgets.QFileDialog):
-    def __init__(self, check_box_text):
+
+    def __init__(self, checkBox_text=None):
+
         super().__init__()
+
         self.setOption(QtWidgets.QFileDialog.DontUseNativeDialog)
-        self.check_box = QtWidgets.QCheckBox(text=check_box_text)
-        # Beautify
-        self.layout().addWidget(self.check_box)
+        if checkBox_text is not None:
+            self.checkBox = QtWidgets.QCheckBox(text=checkBox_text)
+            self.layout().addWidget(self.checkBox)
 
 
+# Deprecated in 0.0.2.0 (RNZ 07/20/2023)
 class RectSwitch(QtWidgets.QAbstractButton):
+
     def __init__(self, parent=None, margin=2, thumb_width=0.6, duration=150):
+
         super().__init__(parent=parent)
 
         self._margin = margin
         self._thumb_width = thumb_width
         self._duration = duration
         self.setColor()
         self.setCheckable(True)
         self.setFixedSize(self.sizeHint())
 
 
     def setColor(self):
+
         palette = self.palette()
         # Border color
         self._light_border_color = palette.light().color() # QColor
         self._dark_border_color = palette.shadow().color() # QColor
         # Face brush
         if self._margin < 0:
             self._track_brush = palette.shadow()  # QBrush
@@ -47,18 +103,20 @@
             True: QtCore.Qt.black,             # QColor
             False: palette.mid().color()       # QColor
         }
         self._text_opacity = 1
 
 
     def sizeHint(self):
+
         return QtCore.QSize(80, 20)
 
 
     def setGeometry(self):
+
         self._track_width = min(self.width(), self.width() + 2 * self._margin)
         self._track_height = min(self.height(), self.height() + 2 * self._margin)
         self._thumb_width *= self.width()
         self._thumb_height = self._track_height - 2 * self._margin
 
         if self._margin > 0:
             self._base_offset = self._margin + self._thumb_width / 2
@@ -68,36 +126,39 @@
             True: lambda: self.width() - self._base_offset,
             False: lambda: self._base_offset,
         }
         self._offset = self._base_offset
 
 
     def resizeEvent(self, event):
+
         super().resizeEvent(event)
         self.setGeometry()
         self.offset = self._end_offset[self.isChecked()]()
 
 
     @QtCore.Property(int)
     def offset(self):
+
         return self._offset
 
 
     @offset.setter
     def offset(self, value):
+
         self._offset = value
         self.update()
 
-
     # def setChecked(self, checked):
+    # 
     #     super().setChecked(checked)
     #     self.offset = self._end_offset[checked]()
 
-
     def paintEvent(self, event):
+
         light_border_color = self._light_border_color
         dark_border_color = self._dark_border_color
         track_brush = self._track_brush
         thumb_brush = self._thumb_brush
         text_color = self._text_color[self.isEnabled()]
         track_opacity = self._track_opacity
         thumb_opacity = self._thumb_opacity
@@ -151,24 +212,27 @@
             ),
             QtCore.Qt.AlignCenter,
             self._text[self.isChecked()],
         )
 
 
     def mouseReleaseEvent(self, event):
+
         super().mouseReleaseEvent(event)
+
         if event.button() == QtCore.Qt.LeftButton:
             anim = QtCore.QPropertyAnimation(self, b'offset', self)
             anim.setDuration(self._duration)
             anim.setStartValue(self.offset)
             anim.setEndValue(self._end_offset[self.isChecked()]())
             anim.start()
 
 
     def enterEvent(self, event):
+        
         self.setCursor(QtCore.Qt.PointingHandCursor)
         super().enterEvent(event)
 
 
 if __name__ == '__main__':
 
     app = QtWidgets.QApplication([])
```

