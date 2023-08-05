# Comparing `tmp/pybmd-2023.2.0.tar.gz` & `tmp/pybmd-2023.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybmd-2023.2.0.tar", last modified: Wed Apr 19 09:35:47 2023, max compression
+gzip compressed data, was "pybmd-2023.3.0.tar", last modified: Sat Aug  5 04:15:48 2023, max compression
```

## Comparing `pybmd-2023.2.0.tar` & `pybmd-2023.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-19 09:35:34.000000 pybmd-2023.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 09:35:47.206812 pybmd-2023.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 09:35:34.000000 pybmd-2023.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/pybmd/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/bmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/fusion_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery_still.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery_still_album.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_pool_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/project_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/timeline_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/toolkits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/pybmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:35:47.206812 pybmd-2023.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-19 09:35:34.000000 pybmd-2023.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:15:48.513981 pybmd-2023.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-05 04:15:38.000000 pybmd-2023.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-05 04:15:48.513981 pybmd-2023.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-05 04:15:38.000000 pybmd-2023.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:15:48.513981 pybmd-2023.3.0/pybmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/bmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/fusion_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/gallery_still.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/gallery_still_album.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/media_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/media_pool_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/media_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/timeline_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-05 04:15:38.000000 pybmd-2023.3.0/pybmd/toolkits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:15:48.513981 pybmd-2023.3.0/pybmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-05 04:15:48.000000 pybmd-2023.3.0/pybmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-05 04:15:48.000000 pybmd-2023.3.0/pybmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:15:48.000000 pybmd-2023.3.0/pybmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 04:15:48.000000 pybmd-2023.3.0/pybmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 04:15:48.513981 pybmd-2023.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-05 04:15:38.000000 pybmd-2023.3.0/setup.py
```

### Comparing `pybmd-2023.2.0/LICENSE` & `pybmd-2023.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/PKG-INFO` & `pybmd-2023.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2023.2.0
+Version: 2023.3.0
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pybmd-2023.2.0/README.md` & `pybmd-2023.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/pybmd/bmd.py` & `pybmd-2023.3.0/pybmd/bmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
         self.EXPORT_TEXT_CSV = self.local_davinci.EXPORT_TEXT_CSV
         self.EXPORT_TEXT_TAB = self.local_davinci.EXPORT_TEXT_TAB
         self.EXPORT_DOLBY_VISION_VER_2_9 = self.local_davinci.EXPORT_DOLBY_VISION_VER_2_9
         self.EXPORT_DOLBY_VISION_VER_4_0 = self.local_davinci.EXPORT_DOLBY_VISION_VER_4_0
         
         #Add at DR 18.1.3
         self.EXPORT_DOLBY_VISION_VER_5_1 = self.local_davinci.EXPORT_DOLBY_VISION_VER_5_1
+        
+        #Add at DR 18.5.0
+        self.EXPORT_OTIO=self.local_davinci.EXPORT_OTIO
 
         # timeline exportSubtype can be one of the following enums:
         # for exportType is EXPORT_AAF:
         self.EXPORT_AAF_NEW = self.local_davinci.EXPORT_AAF_NEW
         self.EXPORT_AAF_EXISTING = self.local_davinci.EXPORT_AAF_EXISTING
         # for exportType is EXPORT_EDL:
         self.EXPORT_NONE = self.local_davinci.EXPORT_NONE
```

### Comparing `pybmd-2023.2.0/pybmd/folder.py` & `pybmd-2023.3.0/pybmd/folder.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/pybmd/gallery.py` & `pybmd-2023.3.0/pybmd/gallery.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/pybmd/gallery_still_album.py` & `pybmd-2023.3.0/pybmd/gallery_still_album.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/pybmd/media_pool.py` & `pybmd-2023.3.0/pybmd/media_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from pybmd.media_pool_item import MediaPoolItem
 from pybmd.timeline import Timeline
 from pybmd.timeline_item import TimelineItem
 
 from dataclasses import dataclass
 from dataclasses import asdict
 
+# TODO clip info for multi version compatible
+
 
 @dataclass
 class ClipInfo():
     """ClipInfo dataclass"""
     media_pool_item: MediaPoolItem
     start_frame: int
     end_frame: int
     media_type: int
+    track_index: int
+    record_frame: int
 
 
 @dataclass
 class TimelineImportOptions():
     """TimelineImportOptions dataclass"""
     timeline_name: str
     import_source_clips: bool
@@ -46,15 +50,15 @@
 
         Args:
             folder (Folder): folder to add sub folder to 
             name (str): name of new sub folder
 
         Returns:
             Folder: folder object of new sub folder
-        """        
+        """
         return Folder(self.media_pool.AddSubFolder(folder.folder, name))
 
     # @dispatch(List[MediaPoolItem])
     # type: ignore
     def append_to_timeline(self, clips: List[MediaPoolItem]) -> List[TimelineItem]:
         """append clips to current timeline
 
@@ -65,15 +69,15 @@
             List[TimelineItem]: timeline items of appended clips at timeline
         """
         if type(clips[0]) is MediaPoolItem:
             temp_list = self.media_pool.AppendToTimeline(
                 [clip.media_pool_item for clip in clips])
         elif type(clips[0]) is ClipInfo:
             temp_list = self.media_pool.AppendToTimeline(
-                [asdict(ClipInfo) for clip in clips])
+                [asdict(clip_info) for clip_info in clips])
 
         # timeline_item_list = []
         # for timeline_item in temp_list:
         #     timeline_item_list.append(TimelineItem(timeline_item))
         return [TimelineItem(timeline_item) for timeline_item in temp_list]
 
     # @dispatch(List[ClipInfo])
@@ -167,26 +171,26 @@
         return Folder(self.media_pool.GetCurrentFolder())
 
     def get_root_folder(self) -> Folder:
         """return root folder object of media pool
 
         Returns:    
             Folder: root folder object
-        """        
+        """
         return Folder(self.media_pool.GetRootFolder())
 
     def get_timeline_matte_list(self, folder: Folder) -> List[MediaPoolItem]:
         """Get mattes in specified Folder
 
         Args:
             folder (Folder): folder to get mattes for
 
         Returns:
             List[MediaPoolItem]: list of media pool items that are mattes
-        """          
+        """
         media_pool_item_list = []
         for media_pool_item in self.media_pool.GetTimelineMatteList(folder.folder):
             media_pool_item_list.append(MediaPoolItem(media_pool_item))
         return media_pool_item_list
 
     # @dispatch(List[str])
     # type: ignore
@@ -217,32 +221,32 @@
 
         Args:
             file_path (str): timeline file path
             import_option (TimelineImportOptions): timelineimportoptions object
 
         Returns:
             Timeline: timeline object
-        """        
+        """
         return Timeline(self.media_pool.ImportTimelineFromFile(str(file_path), asdict(import_option)))
 
     def move_clips(self, clips: List[MediaPoolItem], target_folder: Folder) -> bool:
         """Moves specified clips to target Folder 
 
         Args:
             clips (List[MediaPoolItem]): list of clips to move  
             target_folder (Folder): target folder to move clips to
 
         Returns:
             bool: true if successful, false if not
-        """        
+        """
         return self.media_pool.MoveClips([clip.media_pool_item for clip in clips], target_folder.folder)
 
     def move_folders(self, folders: List[Folder], target_folder: Folder) -> bool:
         """move folders to target folder
-        
+
 
         Args:
             folders (List[Folder]): folders to move
             target_folder (Folder): target folder to move folders to
 
         Returns:
             bool: true if successful, false if not
@@ -264,33 +268,32 @@
     def set_current_folder(self, folder: Folder) -> bool:
         """set current folder"""
         return self.media_pool.SetCurrentFolder(folder.folder)
 
     def unlink_clips(self, media_pool_items: List[MediaPoolItem]) -> bool:
         """Unlink specified media pool clips"""
         return self.media_pool.UnlinkClips([clip.media_pool_item for clip in media_pool_items])
-    
+
     ##########################################################################################################################
-    #Add at DR18.0.0
+    # Add at DR18.0.0
     def refresh_folders(self) -> bool:
         """Updates the folders in collaboration mode"""
         return self.media_pool.RefreshFolders()
-    
+
     def get_unique_id(self) -> str:
         """get unique id of media pool object"""
         return self.media_pool.GetUniqueId()
-    
+
     ##########################################################################################################################
-    #Add at DR18.5.0
-    
-    def import_folder_from_file(self,file_path:str,source_clips_path:str) -> bool:
+    # Add at DR18.5.0 Beta
+
+    def import_folder_from_file(self, file_path: str, source_clips_path: str) -> bool:
         """Returns true if import from given DRB filePath is successful, false otherwise
 
         Args:
             file_path (str): file path to DRB file
             source_clips_path (str): sourceClipsPath is a string that specifies a filesystem path to search for source clips if the media is inaccessible in their original path, empty by default
 
         Returns:
             bool: Returns true if import from given DRB filePath is successful, false otherwise
-        """        
-        return self.media_pool.ImportFolderFromFile(file_path,source_clips_path)
-    
+        """
+        return self.media_pool.ImportFolderFromFile(file_path, source_clips_path)
```

### Comparing `pybmd-2023.2.0/pybmd/media_pool_item.py` & `pybmd-2023.3.0/pybmd/media_pool_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,8 +229,27 @@
     #Add at DR18.0.0
     
     #TODO Add version check
     def get_unique_id(self) -> str:
         """return unique id of the clip."""
         return self.media_pool_item.GetUniqueId()
     
-    ################################################################################
+    ##############################################################################################################################
+    # Add at DR18.5.0
+
+    def transcribe_audio(self) -> bool:
+        """Transcribes audio of the MediaPoolItem. 
+
+        Returns:
+            bool: Returns True if successful; False otherwise
+        """
+        return self.media_pool_item.TranscribeAudio()
+    
+    def clear_transcription(self) -> bool:
+        """Clears audio transcription of the MediaPoolItem. 
+
+        Returns:
+            bool: Returns True if successful; False otherwise.
+        """
+        return self.media_pool_item.ClearTranscription()
+    
+
```

### Comparing `pybmd-2023.2.0/pybmd/media_storage.py` & `pybmd-2023.3.0/pybmd/media_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 from os import path
 from typing import TYPE_CHECKING, List
 
 from pybmd.media_pool_item import MediaPoolItem
 if TYPE_CHECKING:
     from pybmd.bmd import Bmd
 
+from dataclasses import dataclass
+from dataclasses import asdict
+
+
+@dataclass
+class Item_Info():
+    """Item Info"""
+    media: str
+    start_frame: int
+    end_frame: int
+
 
 class MediaStorage:
     """MediaStorage."""
 
     media_storage = None
 
     def __init__(self, _local_davinci: 'Bmd.local_davinci'):
@@ -24,39 +35,43 @@
             stero_eye (str, optional): specifying which eye to add the matte to for stereo clips ("left" or "right"). Defaults to None.
 
         Returns:
             bool: True if success, False if fail
         """
         return self.media_storage.AddClipMattesToMediaPool(media_pool_item, paths, stero_eye)
 
-    def add_item_list_to_meida_pool(self, item_path_list: List[str]) -> List[MediaPoolItem]:
+    def add_item_list_to_meida_pool(self, items: List[str] | List[Item_Info]) -> List[MediaPoolItem]:
         """Adds specified file/folder paths from Media Storage into current Media Pool folder. 
 
         Args:
-            item_path_list (List[str]): an array of file/folder paths
-
+            items (List[str]): an array of file/folder paths
+            items (List[Item_Info]): an array of Item_info
         Returns:
             List[MediaPoolItem]: a list of MediaPoolItem objects created from the added items
         """
         # media_pool_item_list = []
         # for media_pool_item in self.media_storage.AddItemListToMeidaPool(item_path_list):
         #     media_pool_item_list.append(MediaPoolItem(media_pool_item))
         # return media_pool_item_list
-        return [MediaPoolItem(media_pool_item) for media_pool_item in self.media_storage.AddItemListToMediaPool(item_path_list)]
+        if type(items[0]) is str:
+            return [MediaPoolItem(media_pool_item) for media_pool_item in self.media_storage.AddItemListToMediaPool(items)]
+        elif type(items[0]) is Item_Info:
+            temp_list=[asdict(item_info) for item_info in items]
+            return [MediaPoolItem(media_pool_item) for media_pool_item in self.media_storage.AddItemListToMediaPool(temp_list)]
 
     def add_timeline_mattes_to_media_pool(self, paths) -> List[MediaPoolItem]:
         """Adds specified media files as timeline mattes in current media pool folder. 
 
         Args:
             paths (_type_): one or more file/folder paths. 
 
         Returns:
             List[MediaPoolItem]:a list of created MediaPoolItem
         """
-        
+
         # media_pool_item_list = []
         # for media_pool_item in self.media_storage.AddTimelineMattesToMediaPool(paths):
         #     media_pool_item_list.append(MediaPoolItem(media_pool_item))
         # return media_pool_item_list
         return [MediaPoolItem(media_pool_item) for media_pool_item in self.media_storage.AddTimelineMattesToMediaPool(paths)]
 
     def get_file_list(self, folder_path: str) -> List[str]:
```

### Comparing `pybmd-2023.2.0/pybmd/project.py` & `pybmd-2023.3.0/pybmd/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,19 +272,34 @@
 
         Returns:
             bool: Returns True if successful, otherwise False.
         """        
         return self.project.InsertAudioToCurrentTrackAtPlayhead(media_path, start_offset_in_samples, duration_in_samples)
 
     ##############################################################################################################################
-    # Add at DR18.5.0
+    # Add at DR18.5.0 Beta
     
     def load_burn_in_preset(self,preset_name:str) -> bool:
         """Loads user defined data burn in preset for project when supplied presetName (string). 
 
         Args:
             preset_name (str): preset name
 
         Returns:
             bool: Returns true if successful.
         """        
-        return self.project.LoadBurnInPreset(preset_name)
+        return self.project.LoadBurnInPreset(preset_name)
+    ##############################################################################################################################
+    # Add at DR18.5.0 
+    
+    def export_current_frame_as_still(self,file_path:str) -> bool:
+        """Exports current frame as still to supplied filePath. 
+
+        Args:
+            file_path (str): exported still path.filePath must end in valid export file format. 
+
+        Returns:
+            bool: Returns True if succssful, False otherwise.
+        """
+        return self.project.ExportCurrentFrameAsStill(file_path)
+       
+
```

### Comparing `pybmd-2023.2.0/pybmd/project_manager.py` & `pybmd-2023.3.0/pybmd/project_manager.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.2.0/pybmd/timeline.py` & `pybmd-2023.3.0/pybmd/timeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,28 +33,63 @@
 class TrackType(Enum):
     """docstring for TrackTpye."""
     AUDIO_TRACK = 'audio'
     VIDEO_TRACK = 'video'
     SUBTITLE_TRACK = 'subtitle'
 
 
+class OptionalSubTrackType(Enum):
+    """OptionalSubTrackType is required for TrackType is AUDIO_TRACK"""
+    MONO = "mono"
+    STEREO = "stereo"
+    FP1 = "5.1"
+    FP1_FILM = "5.1film"
+    SP1 = "7.1"
+    SP1_FILM = "7.1film"
+    ADAPTIVE_1 = "adaptive1"
+    ADAPTIVE_2 = "adaptive2"
+    ADAPTIVE_3 = "adaptive3"
+    ADAPTIVE_4 = "adaptive4"
+    ADAPTIVE_5 = "adaptive5"
+    ADAPTIVE_6 = "adaptive6"
+    ADAPTIVE_7 = "adaptive7"
+    ADAPTIVE_8 = "adaptive8"
+    ADAPTIVE_9 = "adaptive9"
+    ADAPTIVE_10 = "adaptive10"
+    ADAPTIVE_11 = "adaptive11"
+    ADAPTIVE_12 = "adaptive12"
+    ADAPTIVE_13 = "adaptive13"
+    ADAPTIVE_14 = "adaptive14"
+    ADAPTIVE_15 = "adaptive15"
+    ADAPTIVE_16 = "adaptive16"
+    ADAPTIVE_17 = "adaptive17"
+    ADAPTIVE_18 = "adaptive18"
+    ADAPTIVE_19 = "adaptive19"
+    ADAPTIVE_20 = "adaptive20"
+    ADAPTIVE_21 = "adaptive21"
+    ADAPTIVE_22 = "adaptive22"
+    ADAPTIVE_23 = "adaptive23"
+    ADAPTIVE_24 = "adaptive24"
+
+
 def timeline_item_class_list_transfer(timeline_item_list: List[TimelineItem]) -> list:
     timeline_item_trans_list = []
 
     for timeline_item in timeline_item_list:
         timeline_item_trans_list.append(timeline_item.timeline_item)
 
     return timeline_item_trans_list
 
 
 class Timeline():
     """Timeline Object"""
 
     def __init__(self, timeline):
         self.timeline = timeline
+
     def __repr__(self) -> str:
         return f'Timeline:f{self.get_name()}'
 
     def add_marker(self, frame_id: str, color: str, name: str, note: str, duration: str, custom_data: str) -> bool:
         """Creates a new marker at given frameId position and with given marker information. 
 
         Args:
@@ -185,15 +220,15 @@
         """
         return self.timeline.GetMarkers()
 
     def get_name(self) -> str:
         """Returns the name of the timeline."""
         return self.timeline.GetName()
 
-    def get_setting(self, setting_name: str="") -> str:
+    def get_setting(self, setting_name: str = "") -> str:
         """Returns value of timeline setting (indicated by settingName : string)."""
         return self.timeline.GetSetting(setting_name)
 
     def get_start_frame(self) -> int:
         """Returns the frame number at the start of timeline."""
         return self.timeline.GetStartFrame()
 
@@ -207,45 +242,44 @@
         Args:
             track_type (TrackTpye): Track type.
             track_index (int):  1 <= trackIndex <= GetTrackCount(trackType)
 
         Returns:
             str: track name.
         """
-        
+
         return self.timeline.GetTrackName(track_type.value, track_index)
 
     def grab_all_stills(self, still_frame_source: int) -> List[GalleryStill]:
         """Grabs stills from all the clips of the timeline and returns a list of GalleryStill objects.
 
         Args:
             still_frame_source (int): 1 - First frame, 2 - Middle frame
 
         Returns:
             List[GalleryStill]: List of GalleryStill objects containing grabbed stills.
         """
 
         return [GalleryStill(gallery_still) for gallery_still in self.timeline.GrabAllStills(still_frame_source)]
 
-
     def grab_still(self) -> GalleryStill:
         """Grabs still from the current video clip. Returns a GalleryStill object."""
         return GalleryStill(self.timeline.GrabStill())
 
     # TODO test this
     def import_into_timeline(self, file_path: str, import_options: ImportOptions) -> bool:
         """Imports timeline items from an AAF file and optional importOptions dict into the timeline,
 
         Args:
             file_path (str): file path.
             import_options (ImportOptions): ImportOptions object.
 
         Returns:
             bool: true if successful, false otherwise.
-        """        
+        """
         return self.timeline.ImportIntoTimeline(file_path, asdict(import_options))
 
     def insert_fusion_generator_into_timeline(self, generator_name: str) -> TimelineItem:
         """Inserts a Fusion generator (indicated by generatorName : string) into the timeline."""
         return TimelineItem(self.timeline.InsertFusionGeneratorIntoTimeline(generator_name))
 
     def insert_fusion_title_into_timeline(self, title_name: str) -> TimelineItem:
@@ -302,25 +336,144 @@
         """Updates customData (string) for the marker at given frameId position. 
         CustomData is not exposed via UI and is useful for scripting developer to attach any user specific data to markers.
         """
         return self.timeline.UpdateMarkerCustomData(frame_id, custom_data)
 
     #######################################################################################################################
     # Add at DR18.0.0
-    
+
     def set_start_timecode(self, timecode: str) -> bool:
         """Set the start timecode of the timeline to the string 'timecode'. Returns true when the change is successful, false otherwise."""
         return self.timeline.SetStartTimecode(timecode)
 
     def get_start_timecode(self) -> str:
         """Returns the start timecode for the timeline."""
         return self.timeline.GetStartTimecode()
-    
+
     def insert_fusion_composition_into_timeline(self) -> TimelineItem:
         """Inserts a Fusion composition into the timeline.Returns a TimelineItem object."""
         return TimelineItem(self.timeline.InsertFusionCompositionIntoTimeline())
-    
+
     def get_unique_id(self) -> str:
         """Returns a unique ID for the timeline"""
         return self.timeline.GetUniqueId()
+
+    ##############################################################################################################################
+    # Add at DR18.5.0
+    def add_track(self, track_type: TrackType, optional_sub_track_type: OptionalSubTrackType) -> bool:
+        """Adds track of trackType ("video", "subtitle", "audio").
+        Second argument optionalSubTrackType is required for "audio"
+
+        Args:
+            track_type (TrackType): track type
+            optional_sub_track_type (OptionalSubTrackType): Second argument optionalSubTrackType is required for "audio"
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.AddTrack(track_type.value, optional_sub_track_type.value)
+
+    def delete_track(self, track_type: TrackType, track_index: int) -> bool:
+        """Deletes track of trackType ("video", "subtitle", "audio") and given trackIndex. 
+
+
+        Args:
+            track_type (TrackType): track type
+            track_index (int): track index.1 <= track_index <= get_track_count(track_type).
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.DeleteTrack(track_type.value, track_index)
+
+    def set_track_enable(self, track_type: TrackType, track_index: int, is_enable: bool) -> bool:
+        """Enables/Disables track with given trackType and trackIndex
+
+
+
+        Args:
+            track_type (TrackType): trackType is one of {"audio", "video", "subtitle"}
+            track_index (int): 1 <= trackIndex < GetTrackCount(trackType).
+            is_enable (bool): enable state
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.SetTrackEnable(track_type.value, track_index, is_enable)
+
+    def get_is_track_enabled(self, track_type, track_index) -> bool:
+        """
+
+        Args:
+            track_type (_type_): trackType is one of {"audio", "video", "subtitle"}
+            track_index (_type_): 1 <= trackIndex <= GetTrackCount(trackType).
+
+        Returns:
+            bool: Returns True if track with given trackType and trackIndex is enabled and False otherwise.
+        """
+        return self.timeline.GetIsTrackEnabled(track_type, track_index)
+
+    def set_track_lock(self, track_type: TrackType, track_index: int, is_locked: bool) -> bool:
+        """Locks/Unlocks track with given trackType and trackIndex
+
+        Args:
+            track_type (TrackType): trackType is one of {"audio", "video", "subtitle"}
+            track_index (int): 1 <= trackIndex <= GetTrackCount(trackType).
+            is_locked (bool):  lock state
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.SetTrackLock(track_type, track_index, is_locked)
+
+    def get_is_track_locked(self, track_type: TrackType, track_index: int) -> bool:
+        """Returns True if track with given trackType and trackIndex is locked and False otherwise.
+
+
+        Args:
+            track_type (TrackType): trackType is one of {"audio", "video", "subtitle"}
+            track_index (int): 1 <= trackIndex <= GetTrackCount(trackType).
+
+        Returns:
+            bool: Returns True if track with given trackType and trackIndex is locked and False otherwise.
+        """
+        return self.timeline.GetIsTrackLocked(track_type, track_index)
+
+    def delete_clips(self, timeline_items: List[TimelineItem], ripple_delete: bool = False) -> bool:
+        """Deletes specified TimelineItems from the timeline
+
+        Args:
+            timeline_items (List[TimelineItem]): specified TimelineItems
+            ripple_delete (bool): performing ripple delete if the second argument is True.
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.DeleteClips([timeline_item.timeline_item for timeline_item in timeline_items], ripple_delete)
+
+    def set_clips_linked(self, timeline_items: List[TimelineItem], is_linked: bool) -> bool:
+        """Links or unlinks the specified TimelineItems depending on second argument.
+
+        Args:
+            timeline_items (List[TimelineItem]): specified TimelineItems
+            is_linked (bool): Links or unlinks the specified TimelineItems
+
+        Returns:
+            bool: True if successful, False otherwise.
+        """
+        return self.timeline.SetClipsLinked([timeline_item.timeline_item for timeline_item in timeline_items], is_linked)
+
+    def create_subtitle_from_audio(self) -> bool:
+        """Creates subtitles from audio for the timeline. 
+
+        Returns:
+            bool: Returns True on success, False otherwise.
+        """
+        return self.timeline.CreateSubtitleFromAudio()
     
-    #######################################################################################################################
+    def detect_scene_cuts(self) -> bool:
+        """Detects and makes scene cuts along the timeline. 
+
+        Returns:
+            bool: Returns True if successful, False otherwise.
+        """
+        return self.timeline.DetectSceneCuts()
```

### Comparing `pybmd-2023.2.0/pybmd/timeline_item.py` & `pybmd-2023.3.0/pybmd/timeline_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,28 @@
     NodeIndex: str
     Slope: str
     Offset: str
     Power: str
     Saturation: str
 
 
+@dataclass
+class MagicMask_Mode():
+    """MagicMask_Mode."""
+    Forward = "F"
+    Backward = "B"
+    Bidirection = "BI"
+
+
 class TimelineItem():
     """TimelineItem Object"""
 
     def __init__(self, timeline_item):
         self.timeline_item = timeline_item
-        
+
     def __repr__(self) -> str:
         return f'Timeline Item:f{self.get_name()}'
 
     def get_markers(self) -> dict:
         """Returns a dict (frameId -> {information}) of all markers and dicts with their information.
             Example: a value of {96.0: {'color': 'Green', 'duration': 1.0, 'note': '', 'name': 'Marker 1', 'customData': ''}, ...}
             indicates a single green marker at clip offset 96
@@ -357,58 +365,95 @@
         return self.timeline_item.UpdateSidecar()
 
     def get_unique_id(self) -> str:
         """Returns a unique ID for the timeline item"""
         return self.timeline_item.GetUniqueId()
 
     ##########################################################################################################################
-    # Add at DR18.5.0
-    
+    # Add at DR18.5.0 Beta
+
     def apply_arri_cdl_lut(self) -> bool:
         """Applies ARRI CDL and LUT.
 
         Returns:
             bool: Returns True if successful, False otherwise.
-        """        
+        """
         return self.timeline_item.ApplyArriCdlLut()
-    
-    def set_clip_enabled(self,bool_value:bool) -> bool:
+
+    def set_clip_enabled(self, bool_value: bool) -> bool:
         """Sets clip enabled based on argument.
 
         Args:
             bool_value (bool): Sets clip enabled based on argument.
 
         Returns:
             bool: True for clip is enabled
-        """        
+        """
         return self.timeline_item.SetClipEnabled(bool_value)
-    
+
     def get_clip_enabled(self) -> bool:
         """Gets clip enabled status.
 
         Returns:
             bool: clip enabled status 
-        """        
+        """
         return self.timeline_item.GetClipEnabled()
-    
-    def load_burn_in_preset(self,preset_name:str) -> bool:
+
+    def load_burn_in_preset(self, preset_name: str) -> bool:
         """Loads user defined data burn in preset for clip when supplied presetName (string). Returns true if successful.
 
         Args:
             preset_name (str): burn-in preset name
 
         Returns:
             bool: Returns true if successful
-        """        
+        """
         return self.timeline_item.LoadBurnInPreset(preset_name)
-    
-    def get_node_label(self,node_index:int) -> str:
+
+    def get_node_label(self, node_index: int) -> str:
         """Returns the label of the node at nodeIndex.
 
         Args:
             node_index (int): node index
 
         Returns:
             str: node label
-        """        
+        """
         return self.timeline_item.GetNodeLabel(node_index)
-    
+
+    ##############################################################################################################################
+    # Add at DR18.5.0
+    
+    def create_magic_mask(self, mode: MagicMask_Mode) -> bool:
+        """Returns True if magic mask was created successfully, False otherwise. 
+
+        Args:
+            mode (MagicMask_Mode): mode 
+
+        Returns:
+            bool: Returns True if magic mask was created successfully, False otherwise.
+        """
+        return self.timeline_item.CreateMagicMask(mode.value)
+    
+    def regenerate_magic_mask(self) -> bool:
+        """Returns True if magic mask was regenerated successfully, False otherwise.
+
+        Returns:
+            bool: Returns True if magic mask was regenerated successfully, False otherwise.
+        """
+        return self.timeline_item.RegenerateMagicMask()
+    
+    def stabilize(self) -> bool:
+        """Returns True if stabilization was successful, False otherwise
+
+        Returns:
+            bool: Returns True if stabilization was successful, False otherwise
+        """
+        return self.timeline_item.Stabilize()
+    
+    def smart_reframe(self) -> bool:
+        """Performs Smart Reframe. 
+
+        Returns:
+            bool: _descriReturns True if successful, False otherwise.ption_
+        """
+        return self.timeline_item.SmartReframe()
```

### Comparing `pybmd-2023.2.0/pybmd/toolkits.py` & `pybmd-2023.3.0/pybmd/toolkits.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     subfolder_list = {
         folder.get_name(): folder for folder in folder.get_sub_folder_list()}
 
     return subfolder_list.get(subfolder_name)
 
 # TODO get_folder_by_path(check path before get ,if folder not exist,create or raise error)
 
-# TODO add_subfolders (by path) MediaPool->add_subfolder
 
 
 def add_subfolders(media_pool: MediaPool, folder: Folder, subfolder_path: str) -> bool:
     """add subfolder by given path string
 
     Args:
         media_pool (MediaPool): media pool object to operate
```

### Comparing `pybmd-2023.2.0/pybmd.egg-info/PKG-INFO` & `pybmd-2023.3.0/pybmd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2023.2.0
+Version: 2023.3.0
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pybmd-2023.2.0/setup.py` & `pybmd-2023.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setuptools.setup(
     name="pybmd",
-    version="2023.2.0",
+    version="2023.3.0",
     author="wheheo",
     author_email="wheheohu@outlook.com",
     description="python library for Davinci Resolve(Repack)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WheheoHu/pybmd",
     packages=setuptools.find_packages(),
```

