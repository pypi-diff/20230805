# Comparing `tmp/pmdsky_debug_py-7.0.7-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 886611 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Aug-01 04:24 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Aug-01 04:24 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   755146 b- defN 23-Aug-01 04:24 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   721145 b- defN 23-Aug-01 04:24 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   742195 b- defN 23-Aug-01 04:24 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   721145 b- defN 23-Aug-01 04:24 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   762528 b- defN 23-Aug-01 04:24 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   721156 b- defN 23-Aug-01 04:24 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   253065 b- defN 23-Aug-01 04:24 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-01 04:24 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Aug-01 04:25 pmdsky_debug_py-7.0.7.dist-info/RECORD
-14 files, 4680824 bytes uncompressed, 884713 bytes compressed:  81.1%
+Zip file size: 890237 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Aug-05 04:23 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Aug-05 04:23 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   757727 b- defN 23-Aug-05 04:23 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   723703 b- defN 23-Aug-05 04:23 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   744703 b- defN 23-Aug-05 04:23 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   723703 b- defN 23-Aug-05 04:23 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   765109 b- defN 23-Aug-05 04:23 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   723714 b- defN 23-Aug-05 04:23 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   253588 b- defN 23-Aug-05 04:23 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-05 04:23 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Aug-05 04:24 pmdsky_debug_py-7.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 04:24 pmdsky_debug_py-7.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Aug-05 04:24 pmdsky_debug_py-7.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Aug-05 04:24 pmdsky_debug_py-7.0.8.dist-info/RECORD
+14 files, 4696691 bytes uncompressed, 888339 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.7.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.8.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.7.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.7.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.7.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+8f9ddefb60"
+RELEASE = "v0.7.0+0db09d552e"
```

## pmdsky_debug_py/eu.py

```diff
@@ -771,26 +771,28 @@
         [0x2008C3C],
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         [0xC198],
         [0x200C198],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
+    SetDebugFlag = Symbol(
         [0xC1A0],
         [0x200C1A0],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         [0xC1A8],
         [0x200C1A8],
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -816,26 +818,28 @@
         [0x200C250, 0x200C284],
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         [0xC2BC],
         [0x200C2BC],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
+    SetDebugLogFlag = Symbol(
         [0xC2C4],
         [0x200C2C4],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         [0xC2C8],
         [0x200C2C8],
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2327,14 +2331,56 @@
     SelectWaza = Symbol(
         [0x153A4],
         [0x20153A4],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id",
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        [0x17C00],
+        [0x2017C00],
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        [0x17F0C],
+        [0x2017F0C],
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        [0x18C08],
+        [0x2018C08],
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        [0x18C44],
+        [0x2018C44],
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         [0x18F40],
         [0x2018F40],
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -14934,14 +14980,22 @@
         [0xEA94],
         [0x22EB614],
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        [0xEB30],
+        [0x22EB6B0],
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         [0xEC44],
         [0x22EB7C4],
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -22416,14 +22470,23 @@
     MONEY_STORED = Symbol(
         [0x2A5504],
         [0x22A5504],
         0x4,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        [0x2A5599],
+        [0x22A5599],
+        0x200,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         [0x2AB5A4],
         [0x22AB5A4],
         0x2,
         "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE",
     )
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -764,23 +764,28 @@
         None,
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         None,
         None,
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -806,23 +811,28 @@
         None,
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugLogFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         None,
         None,
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2257,14 +2267,56 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
     SelectWaza = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        None,
+        None,
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        None,
+        None,
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         None,
         None,
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -14493,14 +14545,22 @@
         None,
         None,
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        None,
+        None,
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -21783,14 +21843,23 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        None,
+        None,
+        None,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
     )
 
     CURSOR_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
     )
```

## pmdsky_debug_py/jp.py

```diff
@@ -771,26 +771,28 @@
         [0x2008C3C],
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         [0xC110],
         [0x200C110],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
+    SetDebugFlag = Symbol(
         [0xC118],
         [0x200C118],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         [0xC120],
         [0x200C120],
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -816,26 +818,28 @@
         [0x200C1C8, 0x200C1FC],
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         [0xC234],
         [0x200C234],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
+    SetDebugLogFlag = Symbol(
         [0xC23C],
         [0x200C23C],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         [0xC240],
         [0x200C240],
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2325,14 +2329,56 @@
     SelectWaza = Symbol(
         [0x152CC],
         [0x20152CC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id",
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        None,
+        None,
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        None,
+        None,
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         [0x18EFC],
         [0x2018EFC],
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -14737,14 +14783,22 @@
         None,
         None,
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        None,
+        None,
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         [0xEB9C],
         [0x22EC47C],
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -22047,14 +22101,23 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        None,
+        None,
+        None,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
     )
 
     CURSOR_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
     )
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -764,23 +764,28 @@
         None,
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         None,
         None,
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -806,23 +811,28 @@
         None,
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugLogFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         None,
         None,
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2257,14 +2267,56 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
     SelectWaza = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        None,
+        None,
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        None,
+        None,
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         None,
         None,
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -14493,14 +14545,22 @@
         None,
         None,
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        None,
+        None,
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -21783,14 +21843,23 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        None,
+        None,
+        None,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
     )
 
     CURSOR_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
     )
```

## pmdsky_debug_py/na.py

```diff
@@ -771,26 +771,28 @@
         [0x2008C3C],
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         [0xC110],
         [0x200C110],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
+    SetDebugFlag = Symbol(
         [0xC118],
         [0x200C118],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         [0xC120],
         [0x200C120],
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -816,26 +818,28 @@
         [0x200C1C8, 0x200C1FC],
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         [0xC234],
         [0x200C234],
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
+    SetDebugLogFlag = Symbol(
         [0xC23C],
         [0x200C23C],
         None,
-        "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value",
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         [0xC240],
         [0x200C240],
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2327,14 +2331,56 @@
     SelectWaza = Symbol(
         [0x152FC],
         [0x20152FC],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id",
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        [0x17BE0],
+        [0x2017BE0],
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        [0x17E70],
+        [0x2017E70],
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        [0x18B6C],
+        [0x2018B6C],
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        [0x18BA8],
+        [0x2018BA8],
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         [0x18EA4],
         [0x2018EA4],
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -15018,14 +15064,22 @@
         [0xEA24],
         [0x22EAC64],
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        [0xEAC0],
+        [0x22EAD00],
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         [0xEBD4],
         [0x22EAE14],
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -22503,14 +22557,23 @@
     MONEY_STORED = Symbol(
         [0x2A4BC4],
         [0x22A4BC4],
         0x4,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        [0x2A4C50],
+        [0x22A4C50],
+        0x200,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
     )
 
     CURSOR_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
     )
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -764,23 +764,28 @@
         None,
         None,
         "Loads a file from ROM by filepath into a heap-allocated buffer.\n\nr0:"
         " [output] pointer to an IO struct {ptr, len}\nr1: file path string"
         " pointer\nr2: flags",
     )
 
-    GetDebugFlag1 = Symbol(
+    GetDebugFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag1 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug flag. A no-op in the final binary.\n\nr0: flag"
+        " ID\nr1: flag value",
     )
 
     AppendProgPos = Symbol(
         None,
         None,
         None,
         "Write a base message into a string and append the file name and line number to"
@@ -806,23 +811,28 @@
         None,
         None,
         "Would log a printf format string in the debug binary.\n\nThis still constructs"
         " the string with vsprintf, but doesn't actually do anything with it in the"
         " final binary.\n\nr0: format\n...: variadic",
     )
 
-    GetDebugFlag2 = Symbol(
+    GetDebugLogFlag = Symbol(
         None,
         None,
         None,
-        "Just returns 0 in the final binary.\n\nr0: flag ID\nreturn: flag value",
+        "Should return the value of the specified debug log flag. Just returns 0 in the"
+        " final binary.\n\nr0: flag ID\nreturn: flag value",
     )
 
-    SetDebugFlag2 = Symbol(
-        None, None, None, "A no-op in the final binary.\n\nr0: flag ID\nr1: flag value"
+    SetDebugLogFlag = Symbol(
+        None,
+        None,
+        None,
+        "Should set the value of a debug log flag. A no-op in the final binary.\n\nr0:"
+        " flag ID\nr1: flag value",
     )
 
     DebugPrint = Symbol(
         None,
         None,
         None,
         "Would log a printf format string in the debug binary. A no-op in the final"
@@ -2257,14 +2267,56 @@
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
     SelectWaza = Symbol(
         None, None, None, "Note: unverified, ported from Irdkwia's notes\n\nr0: waza_id"
     )
 
+    SendAudioCommandWrapperVeneer = Symbol(
+        None,
+        None,
+        None,
+        "Likely a linker-generated veneer for SendAudioCommandWrapper.\n\nSee"
+        " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
+        " Music ID\nr1: (?) Stored on byte 8 on the struct passed to"
+        " SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    SendAudioCommandWrapper = Symbol(
+        None,
+        None,
+        None,
+        "Initializes some values and then calls SendAudioCommand.\n\nChecks for"
+        " DEBUG_FLAG_BGM_OFF. If 1, sets the volume to 0 before calling"
+        " SendAudioCommand.\n\nr0: Music ID\nr1: (?) Stored on byte 8 on the struct"
+        " passed to SendAudioCommand\nr2: Volume (0-255)",
+    )
+
+    AllocAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Searches for an entry in AUDIO_COMMANDS_BUFFER that's not currently in use"
+        " (audio_command::status == 0). Returns the first entry not in use, or null if"
+        " none was found.\n\nAlso sets the status of the found entry to the value"
+        " specified in r0.\n\nThe game doesn't bother checking if the result of the"
+        " function is null, so the buffer is not supposed to ever get filled.\n\nr0:"
+        " Status to set the found entry to\nreturn: The first unused entry, or null if"
+        " none was found",
+    )
+
+    SendAudioCommand = Symbol(
+        None,
+        None,
+        None,
+        "Used to send commands to the audio engine (seems to be used mainly to play and"
+        " stop music)\n\nThis function calls a stubbed-out one with the string 'audio"
+        " command list'\n\nr0: Command to send",
+    )
+
     ManipBgmPlayback = Symbol(
         None,
         None,
         None,
         "Uncertain. More like bgm1&2 end\n\nNote: unverified, ported from Irdkwia's"
         " notes",
     )
@@ -14493,14 +14545,22 @@
         None,
         None,
         None,
         "Sets the dungeon PRNG to use the primary LCG for subsequent random number"
         " generation.\n\nNo params.",
     )
 
+    MusicTableIdxToMusicId = Symbol(
+        None,
+        None,
+        None,
+        "Used to convert an index that refers to a MUSIC_ID_TABLE entry to a regular"
+        " music ID.\n\nr0: Music table index\nreturn: Music ID",
+    )
+
     ChangeDungeonMusic = Symbol(
         None,
         None,
         None,
         "Replace the currently playing music with the provided music\n\nr0: music ID",
     )
 
@@ -21783,14 +21843,23 @@
     MONEY_STORED = Symbol(
         None,
         None,
         None,
         "The amount of money the player currently has stored in the Duskull Bank.",
     )
 
+    AUDIO_COMMANDS_BUFFER = Symbol(
+        None,
+        None,
+        None,
+        "Buffer used to store audio commands. 16 entries in total. Seems like entries"
+        " are removed at some point (maybe after the commands are read or after they"
+        " finish executing).",
+    )
+
     CURSOR_16_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor_16.wan' sprite loaded in WAN_TABLE"
     )
 
     CURSOR_SPRITE_ID = Symbol(
         None, None, None, "Id of the 'FONT/cursor.wan' sprite loaded in WAN_TABLE"
     )
```

## pmdsky_debug_py/protocol.py

```diff
@@ -472,20 +472,20 @@
     ]
 
     LoadFileFromRom: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    GetDebugFlag1: Symbol[
+    GetDebugFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    SetDebugFlag1: Symbol[
+    SetDebugFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
     AppendProgPos: Symbol[
         Optional[List[int]],
         None,
@@ -497,20 +497,20 @@
     ]
 
     DebugPrint0: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    GetDebugFlag2: Symbol[
+    GetDebugLogFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    SetDebugFlag2: Symbol[
+    SetDebugLogFlag: Symbol[
         Optional[List[int]],
         None,
     ]
 
     DebugPrint: Symbol[
         Optional[List[int]],
         None,
@@ -1452,14 +1452,34 @@
     ]
 
     SelectWaza: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    SendAudioCommandWrapperVeneer: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SendAudioCommandWrapper: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    AllocAudioCommand: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SendAudioCommand: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ManipBgmPlayback: Symbol[
         Optional[List[int]],
         None,
     ]
 
     SoundDriverReset: Symbol[
         Optional[List[int]],
@@ -10135,14 +10155,19 @@
     ]
 
     DungeonRngSetPrimary: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    MusicTableIdxToMusicId: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     ChangeDungeonMusic: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TrySwitchPlace: Symbol[
         Optional[List[int]],
@@ -14381,14 +14406,19 @@
     ]
 
     MONEY_STORED: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    AUDIO_COMMANDS_BUFFER: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     CURSOR_16_SPRITE_ID: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     CURSOR_SPRITE_ID: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-7.0.7.dist-info/METADATA` & `pmdsky_debug_py-7.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.7
+Version: 7.0.8
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `pmdsky_debug_py-7.0.7.dist-info/RECORD` & `pmdsky_debug_py-7.0.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pmdsky_debug_py/__init__.py,sha256=xvXjdxEqeoQaaS6ssZYVI9jARzv5M4q6FNwA3Z6fOw4,1831
-pmdsky_debug_py/_release.py,sha256=PsVd5GQn9fUVLX148VsfjNdVxOlS56gso6_2lUa12T8,30
-pmdsky_debug_py/eu.py,sha256=3aHXO74NfXBnPHmKWHFnNYxJqxj8fL_yasXj8pdEFm0,755146
-pmdsky_debug_py/eu_itcm.py,sha256=klJPKVIsIziBm6o4zpZ6EhhG9krcQ923vvFsJQR5Tzc,721145
-pmdsky_debug_py/jp.py,sha256=nYs5Bb9_NJyKvTwieUh83E2mkbCfuI8OLLcd8kQDNEw,742195
-pmdsky_debug_py/jp_itcm.py,sha256=JSsYrR_IfZavqDeYbMNh1dByPK9KPIQrcfQLMOEq2KM,721145
-pmdsky_debug_py/na.py,sha256=i34tcIZrL8FNm-XRFtaMoH_FfZr3-y2yrE2vGUSym24,762528
-pmdsky_debug_py/na_itcm.py,sha256=F-2C0HDdx18sRXg45-ZUGlCKwW4CpeI0QPgDnAMnnwM,721156
-pmdsky_debug_py/protocol.py,sha256=60ssOgw2ijN0Di9wmHaK7bD8qJQL01MfBT2QTiODL8s,253065
+pmdsky_debug_py/_release.py,sha256=3h6UjBwgJfFBeEusiYKxkmfJ9ZJ4Rj6YsL9Hsltq4es,30
+pmdsky_debug_py/eu.py,sha256=aRkxSJVtw94KOKpPvc5EIO2mmV2zxYyjlu0pv90sRWk,757727
+pmdsky_debug_py/eu_itcm.py,sha256=m2A7SDqPUaylVygArgSFWjOl0cgsoIsqK9gqegDacgU,723703
+pmdsky_debug_py/jp.py,sha256=cMMeJa8CyJlWRlHLfs9Lb2Mw-UQw37oNuPod-3naaQY,744703
+pmdsky_debug_py/jp_itcm.py,sha256=0LRRzQxPCLb-KZ8S3yNEkg8YyoLt42qPuNUUj1m1afY,723703
+pmdsky_debug_py/na.py,sha256=KdgELLRqxNpbQU0yP3TgNpgq7EFNku3gTMBmkZyrI98,765109
+pmdsky_debug_py/na_itcm.py,sha256=3DkREFNEu-NZRBrANYikoigF6UGbVgJ24LngXzihggY,723714
+pmdsky_debug_py/protocol.py,sha256=o8tCp-FQwit9aUj_gx8g9xK-ALicv6QWg5EElzjijgI,253588
 pmdsky_debug_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pmdsky_debug_py-7.0.7.dist-info/METADATA,sha256=ONV-QwwYsGtXyTwabxMyAY0s5IbkX8BIOySH4f_IZc8,1320
-pmdsky_debug_py-7.0.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pmdsky_debug_py-7.0.7.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
-pmdsky_debug_py-7.0.7.dist-info/RECORD,,
+pmdsky_debug_py-7.0.8.dist-info/METADATA,sha256=5_wHZ2P5OiTSVtKT6QBhZDi-QnAqFT1HN9sRq05A_wM,1320
+pmdsky_debug_py-7.0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pmdsky_debug_py-7.0.8.dist-info/top_level.txt,sha256=cqvpcJbud2s8IyBAc1MfCySwniko_6qO5LWSSxNIoXI,16
+pmdsky_debug_py-7.0.8.dist-info/RECORD,,
```

