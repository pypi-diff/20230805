# Comparing `tmp/grblhud-1.0.1.tar.gz` & `tmp/grblhud-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grblhud-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "grblhud-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `grblhud-1.0.1.tar` & `grblhud-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.0.1/LICENSE
--rw-r--r--   0        0        0     4814 2023-06-11 15:58:27.225029 grblhud-1.0.1/README.md
--rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.0.1/grblhud/README.md
--rw-r--r--   0        0        0       81 2023-06-11 15:59:48.216787 grblhud-1.0.1/grblhud/__init__.py
--rwxr-xr-x   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/__main__.py
--rw-r--r--   0        0        0    10748 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/grblbuffer.py
--rwxr-xr-x   0        0        0    30180 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/grblhudloop.py
--rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/grblmessages.py
--rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.0.1/grblhud/lineinput.py
--rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.0.1/grblhud/unblockedgetch.py
--rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 grblhud-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-10 12:49:32.174417 grblhud-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5642 2023-08-05 15:23:55.947899 grblhud-1.1.0/README.md
+-rw-r--r--   0        0        0     4801 2023-06-10 12:55:49.202815 grblhud-1.1.0/grblhud/README.md
+-rw-r--r--   0        0        0       81 2023-08-05 15:00:02.236925 grblhud-1.1.0/grblhud/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/__main__.py
+-rw-r--r--   0        0        0    14158 2023-08-05 14:52:50.818228 grblhud-1.1.0/grblhud/grblbuffer.py
+-rw-r--r--   0        0        0    33299 2023-08-05 14:54:48.460599 grblhud-1.1.0/grblhud/grblhudloop.py
+-rw-r--r--   0        0        0     6053 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/grblmessages.py
+-rw-r--r--   0        0        0     8040 2023-06-10 11:58:10.835254 grblhud-1.1.0/grblhud/lineinput.py
+-rw-r--r--   0        0        0     2994 2023-06-10 11:58:10.825254 grblhud-1.1.0/grblhud/unblockedgetch.py
+-rw-r--r--   0        0        0      645 2023-06-10 12:50:36.895883 grblhud-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6131 1970-01-01 00:00:00.000000 grblhud-1.1.0/PKG-INFO
```

### Comparing `grblhud-1.0.1/LICENSE` & `grblhud-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/README.md` & `grblhud-1.1.0/grblhud/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
 
 Note that image2gcode and svg2gcode can be used to convert images and vector graphics to gcode at the highest quality. gcode2image can be used to validate these conversions and verify the layout before using grblhud to send the code to your lasercutter or cnc machine. https://github.com/johannesnoordanus?tab=repositories
 
-### WHILE DO syntax:
+WHILE DO syntax:
 ```
     # Gcode:
     #    #100 = 1
     #    WHILE [#100 LE 5] DO1
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    #100 = #100 + 1 (Increase #100 by 1 each iteration of the loop)
     #    END1
@@ -29,40 +29,40 @@
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    ; DO <loopname>'               example: '; DO aloop123'
     #
     # Note that this is an annotation (quoted out so the grbl controller does not see it)
     # Note also that loopnames are all lowercase! And have a number (if any) at the end:
     # in regex '[a-z]+[0-9]*'
 ```
-### Installation note:
+Installation note:
 ``` 
 	- pyserial must be installed first ('pip install pyserial')
-	- inputimeout must be installed ('pip install inputimeout')
+    - inputimeout must be installed ('pip install inputimeout')
 	- pip install grblhud
 
 	To install additional tools:
 	- pip install image2gcode
 	- pip install svg2gcode
 	- pip install gcode2image 
 ```
-### Grblhud help:
+Grblhud help:
 ```
     $ ./grblhud.py --help
     usage: grblhud.py [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>]
 
     Stream g-code using grbl's serial read buffer.
 
     options:
       -h, --help            show this help message and exit
       --serialdevice /dev/<serial-tty-name>
                             serial device on linux (default: /dev/ttyUSB0 115200 baud)
       --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                             grbl status output (default: no output)
 ```
-### Example run:
+Example run:
 ```
 >
 > grblhud
 Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
 
 Status report every 0.1 seconds
```

### Comparing `grblhud-1.0.1/grblhud/README.md` & `grblhud-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Grblhub is tested on several platforms - arm64/intel - and operating systems - Linux/macosx and two grbl v1.1 devices (a lasercutter and a CNC router)
 
 Information on grbl commands: https://github.com/gnea/grbl/blob/master/doc/markdown/commands.md
 
 Note that image2gcode and svg2gcode can be used to convert images and vector graphics to gcode at the highest quality. gcode2image can be used to validate these conversions and verify the layout before using grblhud to send the code to your lasercutter or cnc machine. https://github.com/johannesnoordanus?tab=repositories
 
-WHILE DO syntax:
+### WHILE DO syntax:
 ```
     # Gcode:
     #    #100 = 1
     #    WHILE [#100 LE 5] DO1
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    #100 = #100 + 1 (Increase #100 by 1 each iteration of the loop)
     #    END1
@@ -29,65 +29,90 @@
     #    (Some G-Code Blocks Go Here to Be Repeated Each Loop)
     #    ; DO <loopname>'               example: '; DO aloop123'
     #
     # Note that this is an annotation (quoted out so the grbl controller does not see it)
     # Note also that loopnames are all lowercase! And have a number (if any) at the end:
     # in regex '[a-z]+[0-9]*'
 ```
-Installation note:
+### Installation note:
 ``` 
 	- pyserial must be installed first ('pip install pyserial')
-    - inputimeout must be installed ('pip install inputimeout')
+	- inputimeout must be installed ('pip install inputimeout')
 	- pip install grblhud
 
 	To install additional tools:
 	- pip install image2gcode
 	- pip install svg2gcode
 	- pip install gcode2image 
 ```
-Grblhud help:
+### Grblhud help:
 ```
     $ ./grblhud.py --help
     usage: grblhud.py [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>]
 
     Stream g-code using grbl's serial read buffer.
 
     options:
       -h, --help            show this help message and exit
       --serialdevice /dev/<serial-tty-name>
                             serial device on linux (default: /dev/ttyUSB0 115200 baud)
       --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                             grbl status output (default: no output)
 ```
-Example run:
+### Example run:
 ```
->
-> grblhud
+[somedir]$ grblhud --help
+usage: grblhud [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>] [-V]
+
+Stream g-code using grbl's serial read buffer.
+
+options:
+  -h, --help            show this help message and exit
+  --serialdevice /dev/<serial-tty-name>
+                        serial device on linux (default: /dev/ttyUSB0 115200 baud)
+  --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
+                        grbl status output (default: no output)
+  -V, --version         show version number and exit
+
+[somedir]$ grblhud
 Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
-
-Status report every 0.1 seconds
+okok
+okok
+Status report every 0.1 seconds (WPos coordinates)
 Start command queue
-[     XYZ:00.000,00.000,00.000 FS:0,0] grbl> Grbl 1.1h ['$' for help]
-0|[Idle XYZ:00.000,00.000,00.000 FS:0,0] grbl> help
-Type one of the following commands:
-   (<Ctrl><D>) or FSTOP                              (FULL STOP to continue: softreset)
+0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> help
+grblhud commands:
+   (<Ctrl><D>) or FSTOP                              (FULL STOP, issue softreset to continue)
 
  - cls                                               (clear screen)
  - load <filename>                                   (load file to buffer)
  - run [LOOP] <(file/loop)name> [F<eed>] [S<peed>]   (run from buffer)
  - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)
  - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)
  - softstop                                          (purge command buffer, but let machine buffer run till empty)
- - softreset                                         (Issue soft reset command)
- - hardreset                                         (Hard reset: close/open serial port)
+ - softreset                                         (issue soft reset command)
+ - hardreset                                         (hard reset: close/open serial port)
  - sleep                                             ($SLP command)
- - dryrun                                            ($C check mode)
- - Stoggle                                           (S toggle, in 'Hold' state only)
- - setting [<nr>]                                    (get setting for specific <nr>)
- - grbl/gcode (direct) command:
-     -- '!' feed hold, 
-     -- '~' start/resume, 
-     -- '?' status, 
-     -- 'ctrl-x' or 'command + x' soft reset!
-0|[Idle XYZ:00.000,00.000,00.000 FS:0,0] grbl> 
+ - Zprobe                                            (lower head until 'probe' contact is made)
+ - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)
+ - Stoggle                                           (Spindle on/off, in 'Hold' state only)
+
+grbl commands:
+ - $ (grbl help)
+     $$ (view Grbl settings)
+     $# (view # parameters)
+     $G (view parser state)
+     $I (view build info)
+     $N (view startup blocks)
+     $x=value (save Grbl setting)
+     $Nx=line (save startup block)
+     $C (check gcode mode)
+     $X (kill alarm lock)
+     $H (run homing cycle)
+     ~ (cycle start)
+     ! (feed hold)
+     ? (current status)
+     ctrl-x/command + x/softreset (reset Grbl)
+
+0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> exit
 ```
```

### Comparing `grblhud-1.0.1/grblhud/__main__.py` & `grblhud-1.1.0/grblhud/__main__.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/grblhud/grblbuffer.py` & `grblhud-1.1.0/grblhud/grblbuffer.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import threading
 from time import sleep
 # needs pyserial!
 import serial
 from grblhud import lineinput
 from grblhud.grblmessages import grbl_errors
 from grblhud.grblmessages import grbl_alarm
+from grblhud.grblmessages import grbl_settings
 
 # subclass of Thread
 class Grblbuffer(threading.Thread):
     """
     Grblbuffer: buffering and access to serial io for grbl devices
     """
     #
@@ -54,16 +55,20 @@
         threading.Thread.__init__(self)
         self.serial = serial
         self.status_out = status_out
 
         # init
         self.grblinput = grblinput
         self.init_buffer()
+        self.WCO = {"X" : 0.0, "Y" : 0.0, "Z" : 0.0}
         self.machinestatus = { "state" : "", "X" : 0.0, "Y" : 0.0, "Z" : 0.0, "Feed" : 0, "Speed" : 0 }
 
+        # status report
+        self.status_plain = False
+
         # create and start query process
         self.grblstatus = threading.Thread(target=self.status, args=(.1,))
         self.grblstatus.start()
 
     def init_buffer(self):
         """
         init buffer
@@ -79,33 +84,71 @@
     def update_machinestatus(self, status):
         """
         set machinestatus info from grbl status (result of grbl '?' command)
         """
         if status != '':
             # Sample status report:
             #   <Idle|MPos:0.000,0.000,-10.000|FS:0,0>
-            # Note that this format should be part of the grbl specification.)
-            self.machinestatus = {"state" : "Error", "X" : -1.0, "Y" : -1.0, "Z" : -1.0, "Feed" : "-1", "Speed" : "-1" }
+            #   <Idle|MPos:-2.996,-2.996,0.000|Bf:15,126|FS:0,0|WCO:0.000,0.000,0.000>
+            # Note that 'Real-time Status Reports' are specified here:
+            # 'https://github.com/gnea/grbl/wiki/Grbl-v1.1-Interface'
+            self.machinestatus = {"state" : "Error", "X" : -1.0, "Y" : -1.0, "Z" : -1.0, "Feed" : "-1", "Speed" : "-1"}
 
             #state = re.search("^<[a-zA-Z]+",status)
             state = re.search("<[a-zA-Z]+",status)
             if state:
                 self.machinestatus["state"] = state.group(0)[1:]
 
-            mpos = re.search("MPos:[+\-]?[0-9.,+\-]+\|",status)
+            # Get WCO (Work Coordinate Offset)
+            # GRBL documentation:
+            #    GUI Developers: Simply track and retain the last WCO: vector and use the below equation to compute the
+            #    other position vector for your position readouts. If Grbl's status reports show either WPos or MPos,
+            #    just follow the equations below. It's as easy as that!
+            wco = re.search("WCO:[+\-]?[0-9.,+\-]+[\|>]",status)
+            if wco:
+                wco_X = re.search("[+-]?[0-9.+\-]+", wco.group(0))
+                if wco_X:
+                    self.WCO["X"] = float(wco_X.group(0))
+                wco_Y = re.search(",[+-]?[0-9.+\-]+", wco.group(0))
+                if wco_Y:
+                    self.WCO["Y"] = float(wco_Y.group(0)[1:])
+                wco_Z = re.search(",[+-]?[0-9.+\-]+[\|>]", wco.group(0))
+                if wco_Z:
+                    self.WCO["Z"] = float(wco_Z.group(0)[1:-1])
+
+            # always report WPos coordinates
+            mpos = re.search("MPos:[+\-]?[0-9.,+\-]+[\|>]",status)
             if mpos:
+                # * If MPos: is given, use WPos = MPos - WCO.
                 X = re.search("[+-]?[0-9.+\-]+", mpos.group(0))
                 if X:
-                    self.machinestatus["X"] = float(X.group(0))
+                    self.machinestatus["X"] = float(X.group(0)) - self.WCO["X"]
                 Y = re.search(",[+-]?[0-9.+\-]+", mpos.group(0))
                 if Y:
-                    self.machinestatus["Y"] = float(Y.group(0)[1:])
-                Z = re.search(",[+-]?[0-9.+\-]+\|", mpos.group(0))
+                    self.machinestatus["Y"] = float(Y.group(0)[1:]) - self.WCO["Y"]
+                Z = re.search(",[+-]?[0-9.+\-]+[\|>]", mpos.group(0))
                 if Z:
-                    self.machinestatus["Z"] = float(Z.group(0)[1:-1])
+                    self.machinestatus["Z"] = float(Z.group(0)[1:-1]) - self.WCO["Z"]
+            else:
+                wpos = re.search("WPos:[+\-]?[0-9.,+\-]+[\|>]",status)
+                if wpos:
+                    # always report WPos coordinates
+                    # ( * If WPos: is given, use MPos = WPos + WCO.)
+                    X = re.search("[+-]?[0-9.+\-]+", wpos.group(0))
+                    if X:
+                        # self.machinestatus["X"] = float(X.group(0)) + self.WCO["X"]
+                        self.machinestatus["X"] = float(X.group(0))
+                    Y = re.search(",[+-]?[0-9.+\-]+", wpos.group(0))
+                    if Y:
+                        # self.machinestatus["Y"] = float(Y.group(0)[1:]) + self.WCO["Y"]
+                        self.machinestatus["Y"] = float(Y.group(0)[1:])
+                    Z = re.search(",[+-]?[0-9.+\-]+[\|>]", wpos.group(0))
+                    if Z:
+                        #self.machinestatus["Z"] = float(Z.group(0)[1:-1]) + self.WCO["Z"]
+                        self.machinestatus["Z"] = float(Z.group(0)[1:-1])
 
             fs = re.search("FS:[0-9,]+",status)
             if fs:
                 F = re.search("[0-9]+", fs.group(0))
                 if F:
                     self.machinestatus["Feed"] = F.group(0)
                 S = re.search(",[0-9]+", fs.group(0))
@@ -150,26 +193,42 @@
                             color = Grblbuffer.Cyan
                         elif "Check" in self.machinestatus["state"]:
                             color = ''
 
                         prompt_length = len(str(self.buffer_not_empty()) + "|" + self.format_machinestatus() + " grbl> ")
                         self.grblinput.display_line(str(self.buffer_not_empty()) + "|" + color + self.format_machinestatus() +
                                                     Grblbuffer.EndCol + " grbl" + color + "> " + Grblbuffer.EndCol, prompt_length)
+
+                        if self.status_plain:
+                            # toggle it
+                            self.status_plain = False
+                            print(out_temp.decode('ascii'), flush=True)
+
                         if self.status_out:
                             print("\r" + lineinput.Input.ERASE_TO_EOL + out_temp.decode('ascii').strip(), file=self.status_out, end = '')
                     else:
                         # Ignore all else
                         # Note that this should not happen, but sometimes, it seems, returns on direct commands are broken off
                         otds = out_temp.decode('ascii').strip()
                         if len(otds):
                             alrm = re.search("ALARM:[1-9][0-9]?",otds)
                             if alrm and int(alrm.group()[6:]) in grbl_alarm.keys():
                                 otds += " (" + grbl_alarm[int(alrm.group()[6:])] + ")"
+                            else:
+                                # add meaning to settings
+                                # $1=25
+                                setting = re.search("^\$[0-9]+=[0-9]+(\.[0-9]+)?",otds)
+                                if setting:
+                                    setting = re.search("^\$[0-9]+",setting.group())
+                                    if setting and int(setting.group()[1:]) in grbl_settings.keys():
+
+                                        #otds += (" " * ((25 > len(otds)) ? (25 - len(otds)) : 1 )) + (" + grbl_settings[int(setting.group()[1:])] + ")"
+                                        otds += " " * ((25 - len(otds)) if len(otds) < 25 else 1)  + "(" + grbl_settings[int(setting.group()[1:])] + ")"
                             print(otds)
-                else :
+                else:
                     # Note: ignore incomming pending ok's until counting is in balance.
                     # this is needed at startup when the device is in 'Hold' state
                     if self.serial_buffer_count:            # Delete the block character count corresponding to the last 'ok'
                         self.gcode_count += 1               # update g-code counter
                         del self.serial_buffer_count[0]     # Delete the block character count corresponding to the last 'ok'
                     otds = out_temp.decode('ascii').strip()
                     if len(otds):
@@ -179,15 +238,15 @@
                                 otds += " (" + grbl_errors[int(err.group()[6:])] + ")"
                             print(otds)
 
     def status(self, delay):
         """
         write status request to grbl device and get response
         """
-        print("Status report every", delay, "seconds")
+        print("Status report every", delay, "seconds (WPos coordinates)")
         while not Grblbuffer.GRBLHUD_EXIT:
             if not Grblbuffer.STATUS_PAUZE:
                 with Grblbuffer.serialio_lock:
                     # write direct command '?'
                     self.serial.write("?".encode())
                 # read result
                 self.grbl_count_io()
```

### Comparing `grblhud-1.0.1/grblhud/grblhudloop.py` & `grblhud-1.1.0/grblhud/grblhudloop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 """
 grblhub: a command line tool to handle grbl code.
+(https://www.diymachining.com/downloads/GRBL_Settings_Pocket_Guide_Rev_B.pdf)
 """
 
 import os
 import sys
 import re
 from time import sleep
 # needs pyserial!
 import serial
 from inputimeout import inputimeout, TimeoutOccurred
 from grblhud import lineinput
 from grblhud.grblbuffer import Grblbuffer
 from grblhud.grblmessages import grbl_alarm
-from grblhud.grblmessages import grbl_settings
 
 def count_321():
     """
     Countdown
     """
     sleep(2)
     print("(press <enter> to abort)")
@@ -184,52 +184,52 @@
                 grblbuffer.grblstatus.join()
 		# put something to get run loop out of waiting
                 grblbuffer.put(";")
                 grblbuffer.join()
                 break
 
             if line.find("help") >= 0:
-                print("Type one of the following commands:")
-                print("   (<Ctrl><D>) or FSTOP                              (FULL STOP to continue: softreset)")
+                print("grblhud commands:")
+                print("   (<Ctrl><D>) or FSTOP                              (FULL STOP, issue softreset to continue)")
                 print()
                 print(" - cls                                               (clear screen)")
                 print(" - load <filename>                                   (load file to buffer)")
                 print(" - run [LOOP] <(file/loop)name> [F<eed>] [S<peed>]   (run from buffer)")
                 print(" - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)")
                 print(" - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)")
                 print(" - softstop                                          (purge command buffer, but let machine buffer run till empty)")
-                print(" - softreset                                         (Issue soft reset command)")
-                print(" - hardreset                                         (Hard reset: close/open serial port)")
+                print(" - softreset                                         (issue soft reset command)")
+                print(" - hardreset                                         (hard reset: close/open serial port)")
                 print(" - sleep                                             ($SLP command)")
-                print(" - dryrun                                            ($C check mode)")
-                print(" - Stoggle                                           (S toggle, in 'Hold' state only)")
-                print(" - setting [<nr>]                                    (get setting for specific <nr>)")
-                print(" - grbl/gcode (direct) command:")
-                print("     -- '!' feed hold, ")
-                print("     -- '~' start/resume, ")
-                print("     -- '?' status, ")
-                print("     -- 'ctrl-x' or 'command + x' soft reset!")
+                print(" - Zprobe                                            (lower head until 'probe' contact is made)")
+                print(" - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)")
+                print(" - Stoggle                                           (Spindle on/off, in 'Hold' state only)")
+                print()
+                print("grbl commands:")
+                print(" - $ (grbl help)")
+                print("     $$ (view Grbl settings)")
+                print("     $# (view # parameters)")
+                print("     $G (view parser state)")
+                print("     $I (view build info)")
+                print("     $N (view startup blocks)")
+                print("     $x=value (save Grbl setting)")
+                print("     $Nx=line (save startup block)")
+                print("     $C (check gcode mode)")
+                print("     $X (kill alarm lock)")
+                print("     $H (run homing cycle)")
+                print("     ~ (cycle start)")
+                print("     ! (feed hold)")
+                print("     ? (current status)")
+                print("     ctrl-x/command + x/softreset (reset Grbl)")
                 print()
                 continue
 
             if line.find("cls") >= 0:
                 os.system('cls' if os.name == 'nt' else 'clear')
                 continue
-            if line.find("setting") >= 0:
-                set_nr = re.search("[0-9]+",line)
-                if set_nr:
-                    set_nr = set_nr.group()
-                    if int(set_nr) in grbl_settings.keys():
-                        print("$" + set_nr + ": " + grbl_settings[int(set_nr)])
-                    else:
-                        print("unknown setting: $" + set_nr)
-                else:
-                    for k in grbl_settings.keys():
-                        print("$" + str(k) + ": " + grbl_settings[k])
-                continue
 
             if line == 'softstop':
                 with Grblbuffer.serialio_lock:
                     with Grblbuffer.bec:
                         print("Issued softstop (purged command buffer)")
                         # purge buffer
                         grblbuffer.init_buffer()
@@ -311,23 +311,14 @@
                     print("machinestate must be 'Idle' to be able to sleep")
                 else:
                     with Grblbuffer.serialio_lock:
                         print("Sleep 'zzzzz' ")
                         grblbuffer.serial.write("$SLP\n".encode())     # $SLP: zzzz
                 continue
 
-            if line == "dryrun":
-                with Grblbuffer.serialio_lock:
-                    if grblbuffer.machinestatus["state"] != "Check":
-                        print("Commands run Dry Run mode now (issue command again to toggle)")
-                    else:
-                        print("Commands run for REAL now (issue command again to taggle)")
-                    grblbuffer.serial.write("$C\n".encode())       # $C: G-Code Check mode
-                continue
-
             if re.search("^load +[^<>:;,*|\"]+$", line):
                 # load file: 'load <filename>'
                 if grblbuffer.machinestatus["state"] != "Idle":
                     print("machinestate must be 'Idle' to load a file")
                     continue
                 filePath = line[line.find(' ') + 1:]
                 try:
@@ -571,14 +562,18 @@
                 continue
             if line == "~":
                 with Grblbuffer.serialio_lock:
                     # write direct command '~' 'resume'
                     grblbuffer.serial.write("~".encode())
                     sleep(0.02)
                 continue
+            if line == "?":
+                # indicate 'plain' status report
+                grblbuffer.status_plain = True
+                continue
 
             # set 'realitime' Speed up down 'S+10', 'S+1', 'S-10', 'S-1' command
             if re.search("^S[\+\-](10|1)?",line):
                 # Spindle speed override
 
                 # isolate writing and response sequence
                 with Grblbuffer.serialio_lock:
@@ -633,14 +628,67 @@
                             grblbuffer.serial.write(b'\x94')
                         else:
                             # Set100%
                             grblbuffer.serial.write(b'\x90')
                     sleep(0.02)
                 continue
 
+            # G38.n Straight Probe (https://linuxcnc.org/docs/html/gcode/g-code.html)
+            if line.find("Zprobe") >= 0:
+                # direct command: soft reset
+                with Grblbuffer.serialio_lock:
+                    Grblbuffer.STATUS_PAUZE = True
+                    print("Lower head until 'probe' contact is made.")
+                    print()
+                    print("Make sure a (double) wire is conected to the 'probe' contacts on the machine board and one")
+                    print("wire - on the other end - is connected to a metal object you are setting origin Z0 to, while")
+                    print("the other is connected to the router bit (or a point that is in electric contact).")
+                    print("You can make a test run - using this command - to check if the machine halts when you connect the wires by hand.")
+                    print("After a successfull probe command, 'Zorigin <offset>' can be used to make the probe point, the new Z origin.")
+                    print()
+                    sr = input("Issue Zprobe (enter <Ctrl><D> to abort) (yes/no)? ")
+                    if sr.find("yes") >= 0:
+                        grblbuffer.serial.write("G38.2 Z-25 F24\n".encode())
+                        print("\ngrbl> G38.2 Z-25 F24\n")
+                    else:
+                        print("command aborted")
+                    Grblbuffer.STATUS_PAUZE = False
+                continue
+
+            # G92 Coordinate System Offset (https://linuxcnc.org/docs/html/gcode/g-code.html)
+            if line.find("Zorigin") >= 0:
+                # Set Z<coord> to probe point
+                offset = re.search(" [0-9]+(\.[0-9]+)?",line)
+                if offset:
+                    coord = offset.group()[1:]
+                else:
+                    coord = "0"
+                with Grblbuffer.serialio_lock:
+                    Grblbuffer.STATUS_PAUZE = True
+                    print("Set Z<coord> to probe point.")
+                    print()
+                    print("For example: to make the top of a wood 'slab' to be CNC'd, the Z origin (Z0), a probe can be run (lowered)")
+                    print("that makes contact to a thin metal plate on top of it. If the plate thickness is 2.1 mm, command 'Zorigin 2.1'")
+                    print("will make the probe point Z2.1, which is 2.1 mm above the wood 'slab'. After removing the thin metal plate,")
+                    print("command 'G1 Z0 F24' (move to Z0 with low speed, to be carefull) will make the router bit just touch the top")
+                    print("of the 'slab'. Metal objects to be CNC'd can do with command 'Zorigin' (without an argument).")
+                    print()
+                    print("Note that status report coordinates at the start of each grblhud commandline reflect the new coordinate offset")
+                    print("because it uses Work Position (WPos).")
+                    print()
+                    sr = input("Issue command 'Zorigin " + coord + "' (yes/no)? ")
+                    if sr.find("yes") >= 0:
+                        grblbuffer.serial.write(("G92 Z" + coord + "\n").encode())
+                        print("\ngrbl> G92 Z" + coord + "\n")
+                    else:
+                        print("command aborted")
+                    Grblbuffer.STATUS_PAUZE = False
+                continue
+
+
             # pauze status report
             Grblbuffer.STATUS_PAUZE = True
 
             # Need some sleep to get the command result.
             # Note that this command might be delayed
             # because other commands are pending (queued
             # in the serial buffer). In that case the
```

### Comparing `grblhud-1.0.1/grblhud/grblmessages.py` & `grblhud-1.1.0/grblhud/grblmessages.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/grblhud/lineinput.py` & `grblhud-1.1.0/grblhud/lineinput.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/grblhud/unblockedgetch.py` & `grblhud-1.1.0/grblhud/unblockedgetch.py`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/pyproject.toml` & `grblhud-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grblhud-1.0.1/PKG-INFO` & `grblhud-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grblhud
-Version: 1.0.1
+Version: 1.1.0
 Summary: grblhub: a command line tool to handle grbl code.
 Keywords: grbl,grblv1.1,hud,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: inputimeout >= 1.0.4
@@ -69,39 +69,64 @@
       --serialdevice /dev/<serial-tty-name>
                             serial device on linux (default: /dev/ttyUSB0 115200 baud)
       --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
                             grbl status output (default: no output)
 ```
 ### Example run:
 ```
->
-> grblhud
+[somedir]$ grblhud --help
+usage: grblhud [-h] [--serialdevice /dev/<serial-tty-name>] [--status /dev/<terminal-tty-name>] [-V]
+
+Stream g-code using grbl's serial read buffer.
+
+options:
+  -h, --help            show this help message and exit
+  --serialdevice /dev/<serial-tty-name>
+                        serial device on linux (default: /dev/ttyUSB0 115200 baud)
+  --status /dev/<terminal-tty-name>, -s /dev/<terminal-tty-name>
+                        grbl status output (default: no output)
+  -V, --version         show version number and exit
+
+[somedir]$ grblhud
 Opened serial port /dev/ttyUSB0 at 115200 bauds (bits/s)
 Initializing grbl...
-
-Status report every 0.1 seconds
+okok
+okok
+Status report every 0.1 seconds (WPos coordinates)
 Start command queue
-[     XYZ:00.000,00.000,00.000 FS:0,0] grbl> Grbl 1.1h ['$' for help]
-0|[Idle XYZ:00.000,00.000,00.000 FS:0,0] grbl> help
-Type one of the following commands:
-   (<Ctrl><D>) or FSTOP                              (FULL STOP to continue: softreset)
+0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> help
+grblhud commands:
+   (<Ctrl><D>) or FSTOP                              (FULL STOP, issue softreset to continue)
 
  - cls                                               (clear screen)
  - load <filename>                                   (load file to buffer)
  - run [LOOP] <(file/loop)name> [F<eed>] [S<peed>]   (run from buffer)
  - S+10, S+1, S-10, S-1                              (Speed up/down 10% 1%)
  - F+10, F+1, F-10, F-1                              (Feed up/down 10% 1%)
  - softstop                                          (purge command buffer, but let machine buffer run till empty)
- - softreset                                         (Issue soft reset command)
- - hardreset                                         (Hard reset: close/open serial port)
+ - softreset                                         (issue soft reset command)
+ - hardreset                                         (hard reset: close/open serial port)
  - sleep                                             ($SLP command)
- - dryrun                                            ($C check mode)
- - Stoggle                                           (S toggle, in 'Hold' state only)
- - setting [<nr>]                                    (get setting for specific <nr>)
- - grbl/gcode (direct) command:
-     -- '!' feed hold, 
-     -- '~' start/resume, 
-     -- '?' status, 
-     -- 'ctrl-x' or 'command + x' soft reset!
-0|[Idle XYZ:00.000,00.000,00.000 FS:0,0] grbl> 
+ - Zprobe                                            (lower head until 'probe' contact is made)
+ - Zorigin <coord>                                   (make 'probe' point the new Z<coord>)
+ - Stoggle                                           (Spindle on/off, in 'Hold' state only)
+
+grbl commands:
+ - $ (grbl help)
+     $$ (view Grbl settings)
+     $# (view # parameters)
+     $G (view parser state)
+     $I (view build info)
+     $N (view startup blocks)
+     $x=value (save Grbl setting)
+     $Nx=line (save startup block)
+     $C (check gcode mode)
+     $X (kill alarm lock)
+     $H (run homing cycle)
+     ~ (cycle start)
+     ! (feed hold)
+     ? (current status)
+     ctrl-x/command + x/softreset (reset Grbl)
+
+0|[Idle XYZ:-5.000,00.000,00.000 FS:0,0] grbl> exit
 ```
```

