# Comparing `tmp/solidwrap-1.0.5.tar.gz` & `tmp/solidwrap-1.0.6.tar.gz`

## Comparing `solidwrap-1.0.5.tar` & `solidwrap-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 solidwrap-1.0.5/info/API Reference.rst
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/__init__.py
--rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/utilities/__init__.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/utilities/utilities.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.5/tests/test.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.5/../README.rst
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     8101 2020-02-02 00:00:00.000000 solidwrap-1.0.6/info/API Reference.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/__init__.py
+-rw-r--r--   0        0        0    15331 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/utilities/__init__.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 solidwrap-1.0.6/solidwrap/utilities/utilities.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.6/tests/test.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.6/../README.rst
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.6/PKG-INFO
```

### Comparing `solidwrap-1.0.5/info/API Reference.rst` & `solidwrap-1.0.6/info/API Reference.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 The SolidWorks API ( `SW-API <https://help.solidworks.com/2019/English/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1>`_ ) and PDM API ( `PDM-API <https://help.solidworks.com/2019/English/api/epdmapi/Welcome-epdmapi.html?id=2a67aaceb6984695a5ce8a75121853f3#Pg0>`_ ) are built on the Component Object Model ( `COM <https://learn.microsoft.com/en-us/windows/win32/com/component-object-model--com--portal>`_ ) to provide an interface with SolidWorks applications. They do not, however, have direct support for Python. SolidWrap leverages its own implementation of the COM pipeline to provide a streamlined Pythonic interface with SW-API and PDM-API.
 
 ----
 
-The core of SolidWrap relies on two objects: ``solidworks`` and ``vault``. These are treated as singletons; they come pre-instanced by the module and should not be manually created by the user. Most interactions with SolidWrap should flow through these objects.
+The core of SolidWrap relies on two classes: ``SolidWorks`` and ``Vault``. These are treated as singletons; they must be instanced by the user prior to making any SolidWrap API calls. Most interactions with SolidWrap should flow through these objects.
 
 See the Appendix for an overview of the helper classes ( ``Filepath`` & ``Model`` ) that are embedded in many of the SolidWrap class methods.
 
 **NOTE : Items labelled 'WIP' are in development and are not guaranteed to function as expected.**
 
 ----
 
-``solidworks`` ( object )
--------------------------
-The core object of the API. It serves as a representation of SolidWorks, and is responsible for handling all SolidWorks commands.
+``solidworks`` ( Class )
+------------------------
+The core class of the API. It serves as a representation of SolidWorks, and is responsible for handling all SolidWorks commands.
 
 Attributes
 ``````````
 - client ( `ISldWorks <https://help.solidworks.com/2019/english/api/sldworksapi/solidworks.interop.sldworks~solidworks.interop.sldworks.isldworks.html?verRedirect=1>`_ ) - Top level interface for SW-API
 - version ( `int <https://www.w3schools.com/python/python_datatypes.asp>`_ ) - Release year of the target SolidWorks application version ( ex. 2021 )
 
 Methods
@@ -106,15 +106,15 @@
   def stage(model: Model):
     """
     Parameters:
       - model ( Model ) - Target Model to stage.
     """
 
 
-``vault`` ( object )
+``vault`` ( Class )
 --------------------
 A representation of the PDM Vault. All PDM interactions ( state changes, checking in / out, etc. ) are handled through this object.
 
 Attributes
 ``````````
 - client ( `IEdmVault5 <https://help.solidworks.com/2019/english/api/epdmapi/epdm.interop.epdm~epdm.interop.epdm.iedmvault5.html?verRedirect=1>`_ ) - Top level interface for PDM-API
 - name ( `str <https://www.w3schools.com/python/python_datatypes.asp>`_ ) - Literal name of the PDM Vault
@@ -127,14 +127,21 @@
   # Establishes a connection to the PDM Vault.
   def connect(name: str = "VAULT_NAME_HERE"):
     """
     Parameters:
       - name ( str ) - Literal name of the target PDM Vault
     """
 
+  # Terminates the PDM Vault connection.
+  def disconnect():
+    """
+    Parameters:
+      - NONE
+    """
+
   # Authenticates login credentials for PDM Vault.
   def authenticate():
     """
     Parameters:
       - NONE
     """
 
@@ -187,25 +194,25 @@
 
 ----
 
 Appendix
 --------
 Two container classes are used to simplify the concept of a SolidWorks "document." SW-API tends to prefer the use of complete filepaths as direct references to documents. This is cumbersome, and a less verbose solution is implemented by SolidWrap to streamline file references.
 
-``Model`` ( class )
+``Model`` ( Class )
 -------------------
 A container that holds Filepath, IModelDoc2, and IEdmFile5 information.
 
 Members
 ```````
 - filepath ( `Filepath <https://github.com/SeanYeatts/QuickPathStr>`_ ) - Filepath representation
 - swobj ( `IModelDoc2 <https://help.solidworks.com/2020/English/api/sldworksapi/SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html>`_ ) - SW-API representation
 - pdmobj ( `IEdmFile5 <https://help.solidworks.com/2019/English/api/epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html?verRedirect=1>`_ ) - PDM-API representation [#f]_
 
-``Filepath`` ( class )
+``Filepath`` ( Class )
 ----------------------
 This class is a simple container that breaks up a complete filepath into its constituent components. It simplifies file references by allowing methods to pass ``Filepath`` objects instead of long, verbose strings. See the `GitHub repository <https://github.com/SeanYeatts/QuickPathStr>`_ for complete details. 
 
 .. rubric::
 -----------
 
 .. [#f] `IEdmFile5 <https://help.solidworks.com/2019/English/api/epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html?verRedirect=1>`_ data is not yet captured in this release of SolidWrap. Attempting to call this class member will throw an error.
```

### Comparing `solidwrap-1.0.5/solidwrap/solidwrap.py` & `solidwrap-1.0.6/solidwrap/solidwrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,93 +2,97 @@
 Copyright (c) 2023 Sean Yeatts. All rights reserved.
 """
 
 # ----------------------
 # I. Module Dependencies
 # ----------------------
 
-# 3rd party imports
-from quickpathstr       import Filepath     # syntax standardization helper
+# 3rd Part Imports
+from quickpathstr       import Filepath     # syntax helper
 
-# Standard imports
+# Standard Imports
 import os                                   # manipulate folders
 import win32com.client  as win              # COM object handling
 import pythoncom        as pycom            # used in conjunction with win32com.client
 import subprocess       as subproc          # quick process disconnect
 
-# Project imports
+# Project Imports
 from .utilities        import singleton     # singleton enforcement
 from .utilities        import profile       # process timing
 
 
-# ---------------------
-# II. Import Definition
-# ---------------------
+# ------------------
+# II. Import Symbols
+# ------------------
 
 __all__ = [
-    "solidworks",
-    "vault",
+    "SolidWorks",
+    "Vault",
     "SWDocument",
-    "Filepath",
-    "profile"
+    "Filepath"
 ]
 
 
 # ------------
 # III. Classes
 # ------------
 
 # Helper class
 class SWDocument:
     """
     Document
     --------
     Convenience wrapper for SolidWorks IModelDoc2 objects.
     """
-    # Special Methods
-    # ---------------
+
+    # Core Methods
     def __init__(self, swobj):
         self.filepath   = Filepath(swobj.GetPathName)   # Filepath
         self.swobj      = swobj                         # IModelDoc2
         
 
 # Core class
 @singleton
 class SolidWorks:
     """
     SolidWorks
-    ---------
+    ----------
     Wrapper for SolidWorks API. Represents the top-level application.
     """
+
     # Attributes
-    # ----------
     client  = None
     version = None
 
     # Pubic Methods
-    # -------------
-    @profile
     def connect(self, version: int=2021, visible: bool=False):
         '''Creates a connection to the SolidWorks process.'''
         print(f"Connecting to SolidWorks client...")
-
-        # Instantiate SolidWorks application via win32com dispatch (w/o concrete CLSID)
         self.version = version
-        if not self.client:                                                                     # if a client is not defined...
-            self.client = win.Dispatch("SldWorks.Application.%d" % (int(self.version)-1992))    # connect to new client  
-            self.client.Visible = visible                                                       # make application visible
-        else:                                                                                   # ...else terminal warning
-            print(f"SolidWorks client connection is already established!")
+        # Connect to application via win32com dispatch (w/o concrete CLSID)
+        if not self.client:                                                                         # if a client is not defined...
+            try:                                                                                    # ...is there an active instance?
+                win.GetActiveObject("SldWorks.Application.%d" % (int(self.version)-1992))           # check for existing client
+            except:                                                                                 # ...otherwise create new instance
+                print(f"Establishing connection...")
+                pycom.CoInitialize()
+                self.client = win.Dispatch("SldWorks.Application.%d" % (int(self.version)-1992))    # connect to new client  
+                self.client.Visible = visible                                                       # make application visible
+                return self.client
+            else:
+                print(f"Existing connection found!")
+        else:
+            print(f"Connection already established!")
 
-    @profile
     def disconnect(self):
         '''Terminates connection to the SolidWorks process.'''
         print(f"Terminating SolidWorks process...")
-        subproc.call(f"Taskkill /IM SLDWORKS.exe /F")
-        # No follow-up terminal message necessary; subproc.call() auto-responds
+        subproc.call(f"Taskkill /IM SLDWORKS.exe /F")   # no follow-up terminal message necessary; subproc.call() auto-responds
+        pycom.CoUninitialize()
+        self.client = None
 
     def open(self, filepath: Filepath) -> SWDocument:
         '''Opens a document using the specified complete path.'''
         print(f"Opening: {filepath.name}")
 
         # Define COM VARIANT arguments
         doc_type = None
@@ -147,27 +151,32 @@
         
         # Define COM VARIANT arguments
         arg1 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, False)
 
         # Execute SW-API method
         document.swobj.ForceRebuild3(arg1)
 
-    def export(self, document: SWDocument, as_type: str="PNG"):
+    def export(self, document: SWDocument, as_type: str="PNG", destination: str = None):
         '''Exports the target document as the prescribed file type.'''
 
         # Guard against incompatible types
         if document.filepath.extension == '.SLDDRW' and as_type != 'pdf':
             print(f"Drawings can only be exported as PDFs")
             return -1
 
         # Format components
-        extension   = str("." + as_type)
-        desktop     = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
-        destination = str(desktop + fr"\SolidWrap Exports")
-        file        = Filepath(f"{destination}\{document.filepath.root}{extension}")
+        extension = str("." + as_type)
+
+        if destination:
+            location = destination
+        else:
+            desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
+            location = str(desktop + fr"\SolidWrap Exports")
+
+        file = Filepath(f"{location}\{document.filepath.root}{extension}")
 
         # Make export directory
         if not os.path.exists(destination):
             os.makedirs(destination)
 
         print(f"Exporting: {file.name}")
 
@@ -232,36 +241,41 @@
 @singleton
 class Vault:
     """
     Vault
     ---------
     Wrapper for SolidWorks PDM API. Represents PDM Vault.
     """
+
     # Attributes
-    # ----------
     client      = None  # win32com application
     name        = None  # PDM Vault name (ex. "My_Vault")
     auth_state  = False # login credential authorization flag
 
     # Public Methods
-    # --------------
-    @profile
     def connect(self, name: str="My_Vault"):
         '''Creates a connection to the PDM Vault.'''
         print(f"Connecting to PDM...")
 
         # Instantiate PDM Vault via win32com dispatch (w/o concrete CLSID)
         self.name = name
         if not self.client:                                     # if a client is not defined...
+            pycom.CoInitialize()
             self.client = win.Dispatch("ConisioLib.EdmVault")   # connect to client
         else:                                                   # ...else terminal warning
             print(f"PDM connection is already established!")
         self.authenticate()
 
-    @profile
+    def disconnect(self):
+        '''Terminates connection to the PDM Vault.'''
+        print(f"Terminating PDM Vault connection...")
+        pycom.CoUninitialize()
+        self.client     = None
+        self.auth_state = False
+
     def authenticate(self):
         '''Authenticates login credentials for PDM Vault.'''
         print(f"Authentiating PDM credentials...")
 
         # Attempt login & flag authentication state
         if not self.client.IsLoggedIn:
             self.client.LoginAuto(self.name, 0)
@@ -277,61 +291,41 @@
 
         # Execute PDM-API method
         if not file.IsLocked:                       # if file is not checked out...
             file.LockFile(directory.ID, 0)          # check out file
         else:
             print(f"File is already checked out!")  # ...else terminal warning
     
-    # WIP
+    # WIP - !!! NOT THE INTENDED DEFINITION !!!
     def batch_checkout(self, files):
         '''Checks out a collection of files from the PDM Vault.'''
         for file in files:
             self.checkout(filepath=file)
-        
-        # ---
-        # WIP
-        # ---
-        # filepath = fr"C:\Goddard_Vault\Users\SYeatts\Scripts"
-        # filename = fr"C:\Goddard_Vault\Users\SYeatts\ScriptsTest_Part_01.sldprt"
-
-        # folder      = vault.client.GetFolderFromPath(filepath)  # IEdmFolder5
-        # folder_id   = folder.ID                                 # IEdmFolder5.ID (int?)
-
-        # for file in files:
-        #     item = folder.GetFile(file.name)            # IEdmFile5
-        #     file_id = item.ID                           # IEdmFile5.ID (int?)
-        #     utility = vault.client.CreateUtility(12)    # (22) IEdmBatchChangeState (12) IEdmBatchGet
-        #     # utility.AddFile(file_id, folder_id)
-        #     utility.AddSelectionEx(vault.client, file_id, folder_id, item.CurrentVersion)
-        
-        # utility.CreateTree(0, 2)    # @param2 (2) Egcf_Lock
-        # # utility.GetFiles()
-        # print(f"{utility.FileCount}")
 
     def checkin(self, filepath: Filepath, message: str="SolidWrap Automated Check In"):
         '''Checks in a file to the PDM Vault.'''
         print(f"Check In: {filepath.name}")
 
         # Get PDM-API objects
-        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = self.client.GetFolderFromPath(filepath.directory)   # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
 
         # Execute PDM-API method
         if file.IsLocked:                           # if file is not checked in...
             file.UnlockFile(0, message)             # check in file
         else:
             print(f"File is already checked in!")   # ...else terminal warning
 
-    # WIP
+    # WIP - !!! NOT THE INTENDED DEFINITION !!!
     def batch_checkin(self, files, message: str="SolidWrap Automated Check In"):
         '''Checks in a collection of files to the PDM Vault.'''
         for file in files:
             self.checkin(filepath=file)
 
-    # WIP
+    # WIP - !!! DOES NOTHING YET !!!
     def change_state(self, filepath: Filepath, state: str="WIP", message: str="SolidWrap Automated State Change"):
         '''Changes a file's PDM state to the prescribed value, if allowed.'''
         print(f"Change State: {filepath.name}")
 
         # directory   = self.client.GetFolderFromPath(filepath.directory) # IEdmFolder5
         # folder_id   = directory.ID                                      # IEdmFolder5.ID (int?)
         # file        = directory.GetFile(filepath.name)                  # IEdmFile
@@ -361,35 +355,27 @@
         '''Returns size of the target file (KB).'''
 
         # Get PDM-API objects
         directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
         file = directory.GetFile(filepath.name)                        # IEdmFile
         return int(file.GetLocalFileSize2(directory.ID)/1000)
 
-    # WIP
+    # WIP - !!! NOT THE INTENDED DEFINITION !!!
     def get_pdm_state(self, filepath: Filepath) -> str:
         '''Returns PDM state of the target file.'''
         
         # Get PDM-API objects
         directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
         return file.CurrentState.GetFirstTransitionPosition()
 
 
-# --------------
-# IV. Singletons
-# --------------
-
-vault = Vault()
-solidworks = SolidWorks()
-
-
-# ------------
-# V. Functions
-# ------------
+# -------------
+# IV. Functions
+# -------------
 
 def get_last_feature(document: SWDocument):
     '''Gets the last feature in the document's Feature Tree.'''
 
     # Get Feature Manager
     manager = document.swobj.FeatureManager
```

### Comparing `solidwrap-1.0.5/solidwrap/utilities/utilities.py` & `solidwrap-1.0.6/solidwrap/utilities/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,21 @@
     def wrapper_singleton(*args, **kwargs):                     # '*args, **kwargs' allows for infinte arguments
         if not wrapper_singleton.instance:                      # if an instance doesn't exist...
             wrapper_singleton.instance = cls(*args, **kwargs)   # ...then store instance
         return wrapper_singleton.instance                       # return instance
     wrapper_singleton.instance = None
     return wrapper_singleton
             
-
 # Used to track execution time of designated processes
 def profile(func):
     """
     Prints the runtime of the decorated function.
     """
     @functools.wraps(func)                  # helper decorator to preserve function reference
     def wrapper_profile(*args, **kwargs):   # '*args, **kwargs' allows for infinte arguments
         start_time = time.perf_counter()    # get time at start
         value = func(*args, **kwargs)
         end_time = time.perf_counter()      # get time at end
         run_time = end_time - start_time    # calculate runtime
         print(f"- {func.__name__!r} runtime: {run_time:.4f}s")
         return value
-    return wrapper_profile
+    return wrapper_profile
```

### Comparing `solidwrap-1.0.5/tests/test.py` & `solidwrap-1.0.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.5/pyproject.toml` & `solidwrap-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-1.0.5/../README.rst` & `solidwrap-1.0.6/../README.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.5/PKG-INFO` & `solidwrap-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 1.0.5
+Version: 1.0.6
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

