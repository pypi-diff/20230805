# Comparing `tmp/e2D-1.0.6.tar.gz` & `tmp/e2D-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-1.0.6.tar", last modified: Tue Aug  1 12:37:38 2023, max compression
+gzip compressed data, was "e2D-1.1.0.tar", last modified: Fri Aug  4 23:05:03 2023, max compression
```

## Comparing `e2D-1.0.6.tar` & `e2D-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:37:38.099961 e2D-1.0.6/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3977 2023-08-01 12:37:38.100988 e2D-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3384 2023-07-31 18:33:31.000000 e2D-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 12:37:38.077224 e2D-1.0.6/e2D/
--rw-rw-rw-   0        0        0    41254 2023-08-01 12:32:54.000000 e2D-1.0.6/e2D/__init__.py
--rw-rw-rw-   0        0        0    10487 2023-08-01 12:36:44.000000 e2D-1.0.6/e2D/envs.py
--rw-rw-rw-   0        0        0     3964 2023-07-31 18:29:22.000000 e2D-1.0.6/e2D/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 12:37:38.098949 e2D-1.0.6/e2D.egg-info/
--rw-rw-rw-   0        0        0     3977 2023-08-01 12:37:38.000000 e2D-1.0.6/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-08-01 12:37:38.000000 e2D-1.0.6/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:37:38.000000 e2D-1.0.6/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 12:37:38.000000 e2D-1.0.6/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-01 12:37:38.000000 e2D-1.0.6/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-08-01 12:37:38.102147 e2D-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.032089 e2D-1.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9505 2023-08-04 23:05:03.033086 e2D-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8910 2023-08-04 22:06:56.000000 e2D-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.011880 e2D-1.1.0/e2D/
+-rw-rw-rw-   0        0        0    59067 2023-08-04 22:09:11.000000 e2D-1.1.0/e2D/__init__.py
+-rw-rw-rw-   0        0        0    10261 2023-08-04 22:54:26.000000 e2D-1.1.0/e2D/envs.py
+-rw-rw-rw-   0        0        0     5306 2023-08-04 22:26:19.000000 e2D-1.1.0/e2D/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.031094 e2D-1.1.0/e2D.egg-info/
+-rw-rw-rw-   0        0        0     9505 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-08-04 23:05:03.034083 e2D-1.1.0/setup.cfg
```

### Comparing `e2D-1.0.6/LICENSE` & `e2D-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-1.0.6/e2D/envs.py` & `e2D-1.1.0/e2D/envs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
         for event in pg.event.get():
             if event.type == pg.QUIT or (event.type == pg.KEYDOWN and event.key == pg.K_x):
                 self.quit = True
 
 ################################################################################################################################################################################################################################
 ################################################################################################################################################################################################################################
-################################################################################################################################################################################################################################
 
 """ TODO
 from e2D import *
 import pygame as pg
 import easygui
 import uuid
```

### Comparing `e2D-1.0.6/e2D/utils.py` & `e2D-1.1.0/e2D/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 KEY_MODE_JUST_PRESSED = 1
 KEY_MODE_JUST_RELEASED = 2
 
 SCANCODES = {"":0,"backspace":8,"tab":9,"return":13,"escape":27,"space":32,"!":33,"\"":34,"#":35,"$":36,"%":37,"&":38,"'":39,"(":40,")":41,"*":42,"+":43,",":44,"-":45,".":46,"/":47,"0":48,"1":49,"2":50,"3":51,"4":52,"5":53,"6":54,"7":55,"8":56,"9":57,":":58,";":59,"<":60,"=":61,">":62,"?":63,"@":64,"[":91,"\\":92,"]":93,"^":94,"_":95,"`":96,"a":97,"b":98,"c":99,"d":100,"e":101,"f":102,"g":103,"h":104,"i":105,"j":106,"k":107,"l":108,"m":109,"n":110,"o":111,"p":112,"q":113,"r":114,"s":115,"t":116,"u":117,"v":118,"w":119,"x":120,"y":121,"z":122,"delete":127,"caps lock":1073741881,"f1":1073741882,"f2":1073741883,"f3":1073741884,"f4":1073741885,"f5":1073741886,"f6":1073741887,"f7":1073741888,"f8":1073741889,"f9":1073741890,"f10":1073741891,"f11":1073741892,"f12":1073741893,"print screen":1073741894,"scroll lock":1073741895,"break":1073741896,"insert":1073741897,"home":1073741898,"page up":1073741899,"end":1073741901,"page down":1073741902,"right":1073741903,"left":1073741904,"down":1073741905,"up":1073741906,"numlock":1073741907,"[/]":1073741908,"[*]":1073741909,"[-]":1073741910,"[+]":1073741911,"enter":1073741912,"[1]":1073741913,"[2]":1073741914,"[3]":1073741915,"[4]":1073741916,"[5]":1073741917,"[6]":1073741918,"[7]":1073741919,"[8]":1073741920,"[9]":1073741921,"[0]":1073741922,"[.]":1073741923,"power":1073741926,"equals":1073741927,"f13":1073741928,"f14":1073741929,"f15":1073741930,"help":1073741941,"menu":1073741942,"sys req":1073741978,"clear":1073741980,"euro":1073742004,"CurrencySubUnit":1073742005,"left ctrl":1073742048,"left shift":1073742049,"left alt":1073742050,"left meta":1073742051,"right ctrl":1073742052,"right shift":1073742053,"right alt":1073742054,"right meta":1073742055,"alt gr":1073742081,"AC Back":1073742094}
 SCANCODES_NUMS = [i for i in SCANCODES.values()]
 
 class Mouse:
-    """
-    # Need the pygame module to be imported as pg.
-    """
     def __init__(self, parent) -> None:
         self.parent = parent
         self.pressed :list= [False, False, False]
         self.just_pressed :list= [False, False, False]
         self.just_released :list= [False, False, False]
         self.update()
     
@@ -26,32 +23,56 @@
         self.just_pressed = [self.pressed[i] and not last_pressed[i] for i in range(3)]
         self.just_released = [not self.pressed[i] and last_pressed[i] for i in range(3)]
     
     def draw(self) -> None:
         pg.draw.circle(self.parent.screen, (110, 0, 0), self.position(), 10) # type: ignore
 
 class Keyboard:
-    """
-    # Need the pygame module to be imported as pg.
-    """
     def __init__(self, parent) -> None:
         self.parent = parent
-        self.pressed :list= [False for _ in SCANCODES_NUMS]
-        self.just_pressed :list= [False for _ in range(len(self.pressed))]
-        self.just_released :list= [False for _ in range(len(self.pressed))]
+        self.__pressed__ :list= [False for _ in SCANCODES_NUMS]
+        self.__just_pressed__ :list= [False for _ in range(len(self.__pressed__))]
+        self.__just_released__ :list= [False for _ in range(len(self.__pressed__))]
         self.update()
     
     def update(self) -> None:
-        last_pressed = self.pressed.copy()
-        self.pressed :list= [pg.key.get_pressed()[i] for i in SCANCODES_NUMS] # type: ignore
-        self.just_pressed = [self.pressed[i] and not last_pressed[i] for i in range(len(SCANCODES_NUMS))]
-        self.just_released = [not self.pressed[i] and last_pressed[i] for i in range(len(SCANCODES_NUMS))]
+        last_pressed = self.__pressed__.copy()
+        self.__pressed__ :list= [pg.key.get_pressed()[i] for i in SCANCODES_NUMS] # type: ignore
+        self.__just_pressed__ = [self.__pressed__[i] and not last_pressed[i] for i in range(len(SCANCODES_NUMS))]
+        self.__just_released__ = [not self.__pressed__[i] and last_pressed[i] for i in range(len(SCANCODES_NUMS))]
     
-    def get_key(self, scan_code, mode=KEY_MODE_PRESSED) -> bool:
-        ll = self.pressed
+    def get_key(self, scan_code:int, mode=KEY_MODE_PRESSED) -> bool:
+        """
+        # Check Key State
+
+        ## Parameters:
+            scan_code (int): The pygame code value of the key to check (e.g., pg.K_SPACE, pg.K_a, pg.K_LEFT, pg.K_RIGHT, etc.).
+            mode (int): The mode to check the key state: KEY_MODE_PRESSED, KEY_MODE_JUST_PRESSED, or KEY_MODE_JUST_RELEASED. Default is KEY_MODE_PRESSED.
+
+        ## Returns:
+            bool: True if the specified key condition is met; otherwise, False.
+
+        ## Example:
+            keyboard = Keyboard(parent_object)
+            keyboard.update()
+            if keyboard.get_key(pg.KEY_SPACE, mode=KEY_MODE_JUST_PRESSED):
+                print("Space key has just been pressed!")
+
+        ## Explanation:
+            The 'get_key' method is used to check the state of a specific key.
+
+            It takes the 'scan_code' parameter, which represents the name of the key to check (e.g., pg.K_SPACE, pg.K_a, pg.K_LEFT, pg.K_RIGHT, etc.).
+
+            The 'mode' parameter can be used to specify whether to check for 'KEY_MODE_PRESSED' (key is currently pressed), 'KEY_MODE_JUST_PRESSED' (key has just been pressed in the current frame), or 'KEY_MODE_JUST_RELEASED' (key has just been released in the current frame).
+
+            The method returns True if the specified condition is met; otherwise, it returns False.
+
+            Example usage is shown in the "Example" section above.
+        """
+        ll = self.__pressed__
         if mode == KEY_MODE_PRESSED:
-            ll = self.pressed
+            ll = self.__pressed__
         elif mode == KEY_MODE_JUST_PRESSED:
-            ll = self.just_pressed
+            ll = self.__just_pressed__
         elif mode == KEY_MODE_JUST_RELEASED:
-            ll = self.just_released
+            ll = self.__just_released__
         return ll[SCANCODES_NUMS.index(scan_code)]
```

### Comparing `e2D-1.0.6/setup.cfg` & `e2D-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 312e 302e 360d 0a61 7574 686f 7220  = 1.0.6..author 
+00000020: 3d20 312e 312e 300d 0a61 7574 686f 7220  = 1.1.0..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

