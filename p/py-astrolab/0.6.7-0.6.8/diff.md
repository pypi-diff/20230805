# Comparing `tmp/py_astrolab-0.6.7.tar.gz` & `tmp/py_astrolab-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.6.7.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.8.tar", max compression
```

## Comparing `py_astrolab-0.6.7.tar` & `py_astrolab-0.6.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.7/README.md
--rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.7/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.7/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.7/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80382 2023-08-03 13:54:17.011922 py_astrolab-0.6.7/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.7/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.7/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.7/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.7/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.7/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.7/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.7/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.7/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.7/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.7/py_astrolab/report.py
--rwxr-xr-x   0        0        0    18590 2023-08-02 18:39:26.606720 py_astrolab-0.6.7/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.7/py_astrolab/types.py
--rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.7/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-08-03 13:55:57.346552 py_astrolab-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.7/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.8/README.md
+-rwxr-xr-x   0        0        0     4901 2023-08-01 09:27:23.596932 py_astrolab-0.6.8/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.8/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.8/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80189 2023-08-04 16:28:34.232678 py_astrolab-0.6.8/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.8/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.8/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.8/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.8/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.8/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.8/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.8/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.8/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.8/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.8/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    18590 2023-08-02 18:39:26.606720 py_astrolab-0.6.8/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.8/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.8/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-08-05 08:58:13.186740 py_astrolab-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.8/PKG-INFO
```

### Comparing `py_astrolab-0.6.7/py_astrolab/__init__.py` & `py_astrolab-0.6.8/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/aspects.py` & `py_astrolab-0.6.8/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.8/py_astrolab/charts/charts_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,57 +152,40 @@
 
             if not hasattr(self.t_user, "sun"):
                 print(f"Generating kerykeion object for {self.t_user.name}...")
                 self.t_user.__get_all()
 
             # Make a list for the absolute degrees of the points of the graphic.
 
-            self.t_points_deg_ut = self.t_user.planets_degrees + [
-                self.t_user.houses_degree_ut[0],
-                self.t_user.houses_degree_ut[9],
-                self.t_user.houses_degree_ut[6],
-                self.t_user.houses_degree_ut[3]
-            ]
-
+            self.t_points_deg_ut = self.t_user.planets_degrees
             # Make a list of the relative degrees of the points in the graphic.
 
             self.t_points_deg = []
             for planet in self.t_user.planets_list:
                 self.t_points_deg.append(planet["position"])
 
-            self.t_points_deg = self.t_points_deg + [
-                self.t_user.houses_list[0]["position"],
-                self.t_user.houses_list[9]["position"],
-                self.t_user.houses_list[6]["position"],
-                self.t_user.houses_list[3]["position"]
-            ]
+            self.t_points_deg = self.t_points_deg
 
             # Make list of the poits sign.
 
             self.t_points_sign = []
 
             for planet in self.t_user.planets_list:
                 self.t_points_sign.append(planet["sign_num"])
 
-            self.t_points_sign = self.t_points_sign + [
-                self.t_user.houses_list[0]["sign_num"],
-                self.t_user.houses_list[9]["sign_num"],
-                self.t_user.houses_list[6]["sign_num"],
-                self.t_user.houses_list[3]["sign_num"]
-            ]
+            self.t_points_sign = self.t_points_sign
 
             # Make a list of poits if they are retrograde or not.
 
             self.t_points_retrograde = []
 
             for planet in self.t_user.planets_list:
                 self.t_points_retrograde.append(planet["retrograde"])
 
-            self.t_points_retrograde = self.t_points_retrograde + [False,
-                                                                   False, False, False]
+            self.t_points_retrograde = self.t_points_retrograde
 
             self.t_houses_sign_graph = []
             for h in self.t_user.houses_list:
                 self.t_houses_sign_graph.append(h['sign_num'])
 
         # screen size
         if self.chart_type == "Natal":
@@ -282,15 +265,15 @@
         # get color configuration
 
         # Immediately generate template.
         self.template = self.makeTemplate()
 
     # draw transit ring
     def __transitRing(self, r):
-        out = '<circle cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 36px; stroke-opacity: .4;"/>' % (
+        out = '<circle cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 36px; stroke-opacity: 1;"/>' % (
             r, r, r-18, self.colors_settings['paper_1'])
         out += '<circle cx="%s" cy="%s" r="%s" style="fill: none; stroke: %s; stroke-width: 1px; stroke-opacity: .6;"/>' % (
             r, r, r, self.colors_settings['zodiac_transit_ring_3'])
         return out
 
     # draw degree ring
     def __degreeRing(self, r):
@@ -596,17 +579,14 @@
 
                 else:
                     path = path + '<text style="fill: #00f; fill-opacity: .4; font-size: 14px"><tspan x="' + \
                         str(xtext-3)+'" y="'+str(ytext+3) + \
                         '">'+str(i+1)+'</tspan></text>'
                     path = path + '<line x1="'+str(t_x1)+'" y1="'+str(t_y1)+'" x2="'+str(t_x2)+'" y2="'+str(
                         t_y2)+'" style="stroke: '+t_linecolor+f'; stroke-width: 2px; stroke-opacity:.3;" class="house" id="{house_by_index[i+1]} House"/>'
-
-            if self.chart_type == "Transit" or self.chart_type == "Composite":
-                dropin = 84
             if i+1 == 1:
                 house_number = 'I'
             elif i+1 == 4:
                 house_number = 'IV'
             elif i+1 == 7:
                 house_number = 'VII'
             elif i+1 == 10:
@@ -642,25 +622,29 @@
         output = ""
         for i in range(len(self.zodiac)):
             output = output + self.__signDegrees(r, i, self.zodiac[i])
         return output
 
     def __signDegrees(self, r, num, sign):
         degrees = ''
+        if self.chart_type == 'Transit' or self.chart_type == 'Composite':
+            c2 = self.c2 + 35
+        else:
+            c2 = self.c2
         for i in range(num*30, (num+1)*30):
             offset_degree = i - self.houses_degree_ut[6]
             if offset_degree < 0:
                 offset_degree += 360
             elif offset_degree > 360:
                 offset_degree -= 360
             length = 5 if i % 5 == 0 else 3
-            dx1 = self.__sliceToX(0, r-self.c2, offset_degree) + self.c2
-            dy1 = self.__sliceToY(0, r-self.c2, offset_degree) + self.c2
-            dx2 = self.__sliceToX(0, r-length-self.c2, offset_degree) + length + self.c2
-            dy2 = self.__sliceToY(0, r-length-self.c2, offset_degree) + length + self.c2
+            dx1 = self.__sliceToX(0, r-c2, offset_degree) + c2
+            dy1 = self.__sliceToY(0, r-c2, offset_degree) + c2
+            dx2 = self.__sliceToX(0, r-length-c2, offset_degree) + length + c2
+            dy2 = self.__sliceToY(0, r-length-c2, offset_degree) + length + c2
             degrees += f'<line class="{sign.title()[:3]} degree" x1="{dx1}" y1="{dy1}" x2="{dx2}" y2="{dy2}" style="stroke: {self.colors_settings["paper_0"]}; stroke-width: 1px; stroke-opacity: 1;"/>'
         return degrees
 
     def __makePlanets(self, r):
 
         planets_degut = {}
 
@@ -843,17 +827,17 @@
                 int(self.planets_degree_ut[i]+planets_delta[e])
             trueoffset = (
                 int(self.houses_degree_ut[6]) / -1) + int(self.planets_degree_ut[i])
 
             planet_x = self.__sliceToX(0, (r-rplanet), offset) + rplanet
             planet_y = self.__sliceToY(0, (r-rplanet), offset) + rplanet
             if self.chart_type == "Transit" or self.chart_type == "Composite":
-                scale = 0.8
-
-            scale = 1.2
+                scale = 1.2
+            else:
+                scale = 1.2
             # output planet
             output += f''''
                 <g id="{self.planets_settings[i]["name"].title()}G" transform="translate(-{str(12*scale)}, -{str(12*scale)}) scale({str(scale)})">
                     <use x="{str(planet_x*(1/scale))}" y="{str(planet_y*(1/scale))}" xlink:href="#{self.planets_settings[i]["name"]}"/>
                 </g>'''
             if self.planets_retrograde[i]:
                 if self.planets_settings[i]["name"] == 'Mercury':
@@ -869,15 +853,21 @@
                     offset_retrograde_x = 5.5
                     offset_retrograde_y = 6.5
                 elif self.planets_settings[i]["name"] == 'Saturn':
                     offset_retrograde_x = 7 
                     offset_retrograde_y = 8.8
                 output += f'<g class="retrograde" transform="translate({planet_x + offset_retrograde_x}, {planet_y + offset_retrograde_y})"><use transform="scale(.5)" xlink:href="#retrograde" /></g>'
             # Adjust the offset degree to be within 0 to 360
-            output += self.drawTick(r, self.planets_settings[i]["name"], offset)
+            if self.chart_type == 'Transit' or self.chart_type == 'Composite':
+                c1 = self.c3 - 49
+                c2 = self.c3 + 40
+            else:
+                c1 = self.c2
+                c2 = self.c3
+            output += self.drawTick(c1, c2, r, self.planets_settings[i]["name"], offset)
 
         # make transit degut and display planets
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             group_offset = {}
             t_planets_degut = {}
             if self.chart_type == "Transit":
                 list_range = len(self.planets_settings)-4
@@ -926,39 +916,36 @@
                     group_offset[groups[i][1]] = -1.0
                     group_offset[groups[i][2]] = 1.0
                     group_offset[groups[i][3]] = 2.0
 
             switch = 0
             for e in range(len(t_keys)):
                 i = t_planets_degut[t_keys[e]]
-
                 if 22 < i < 27:
-                    rplanet = 9
+                    rplanet = 4
                 elif switch == 1:
-                    rplanet = 18
+                    rplanet = 5
                     switch = 0
                 else:
-                    rplanet = 26
+                    rplanet = 4
                     switch = 1
-
                 zeropoint = 360 - self.houses_degree_ut[6]
                 t_offset = zeropoint + self.t_planets_degree_ut[i]
                 if t_offset > 360:
                     t_offset = t_offset - 360
-                planet_x = self.__sliceToX(0, (r-rplanet), t_offset) + rplanet
-                planet_y = self.__sliceToY(0, (r-rplanet), t_offset) + rplanet
-                output = output + '<g transform="translate(-6,-6)"><g transform="scale(0.5)"><use x="' + str(
-                    planet_x*2) + '" y="' + str(planet_y*2) + '" xlink:href="#' + self.planets_settings[i]['name'] + '" /></g></g>'
+                planet_x = self.__sliceToX(0, (r+rplanet), t_offset)
+                planet_y = self.__sliceToY(0, (r+rplanet), t_offset)
+                output = output + f'<g><g id="{self.planets_settings[i]["name"].title()}GTransit" transform="scale(0.9) translate(15, 15)"><use x="' + str(planet_x) + '" y="' + str(planet_y) + '" xlink:href="#' + self.planets_settings[i]['name'] + '" /></g></g>'
                 # transit planet line
                 x1 = self.__sliceToX(0, r+3, t_offset) - 3
                 y1 = self.__sliceToY(0, r+3, t_offset) - 3
                 x2 = self.__sliceToX(0, r-3, t_offset) + 3
                 y2 = self.__sliceToY(0, r-3, t_offset) + 3
                 output = output + '<line x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
-                    y2)+'" style="stroke: '+self.planets_settings[i]['color']+'; stroke-width: 1px; stroke-opacity:.8;"/>'
+                    y2)+'" style="stroke: black'+'; stroke-width: 1px; stroke-opacity:.8;"/>'
 
                 # transit planet degree text
                 rotate = self.houses_degree_ut[0] - self.t_planets_degree_ut[i]
                 textanchor = "end"
                 t_offset += group_offset[i]
                 rtext = -3.0
 
@@ -975,16 +962,16 @@
                     xo = -1
                 deg_x = self.__sliceToX(0, (r-rtext), t_offset + xo) + rtext
                 deg_y = self.__sliceToY(0, (r-rtext), t_offset + xo) + rtext
                 degree = int(t_offset)
                 output += '<g transform="translate(%s,%s)">' % (deg_x, deg_y)
                 output += '<text transform="rotate(%s)" text-anchor="%s' % (
                     rotate, textanchor)
-                output += '" style="fill: ' + \
-                    self.planets_settings[i]['color']+'; font-size: 10px;">' + \
+                output += '" style="fill: black' + \
+                    '; font-size: 10px;">' + \
                     self.__dec2deg(self.t_planets_degree[i], type="1")
                 output += '</text></g>'
 
             # check transit
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 36
             else:
@@ -1218,17 +1205,16 @@
 
     # Aspect and aspect grid functions for transit type charts.
 
     def __makeAspectsTransit(self, r, ar):
         out = ""
 
         self.aspects_list = CompositeAspects(
-            self.user, self.t_user, settings=self.settings
+            self.t_user, self.user, settings=self.settings
         ).get_relevant_aspects()
-
         for aspect_dict in self.aspects_list:
             aspect_id = f"{min(aspect_dict['p1_name'], aspect_dict['p2_name'])}{aspect_dict['aspect'].title()}{max(aspect_dict['p1_name'], aspect_dict['p2_name'])}"
             out += self.__drawAspect(r, ar, aspect_dict, aspect_id)
 
         return out
 
     def __makeAspectTransitGrid(self, r):
@@ -1317,44 +1303,50 @@
                     aspect_dict = {
                         'p1_abs_pos': axis.abs_pos,
                         'p2_abs_pos': (axis.abs_pos + 180) % 360,
                         'color': axis_data['color'],
                     }
                     out += arrow_top + self.__drawAspect(r, ar, aspect_dict, axis_id, True)
                     offset = offset = (int(self.houses_degree_ut[6]) / -1) + int(aspect_dict['p1_abs_pos'])
-                    out += self.drawTick(r, axis.name, offset)
+                    if self.chart_type == 'Transit' or self.chart_type == 'Composite':
+                        c1 = self.c3 - 49
+                        c2 = self.c3 + 40
+                    else:
+                        c1 = self.c2
+                        c2 = self.c3
+                    out += self.drawTick(c1, c2, r, axis.name, offset)
         return out
 
-    def drawTick(self, r, id, offset) -> str:
+    def drawTick(self, c1, c2, r, id, offset) -> str:
         out = ''
-        for c in [self.c2, self.c3]:
+        for c in [c1, c2]:
             # Calculate the start and end points of the tick mark
             tick_start_x = self.__sliceToX(0, r-c, offset) + c
             tick_start_y = self.__sliceToY(0, r-c, offset) + c
-            if c == self.c2:
-                length = 5
+            if c == c1:
+                length = 7
                 tick_end_x = self.__sliceToX(0, r-length-c, offset) + length + c
                 tick_end_y = self.__sliceToY(0, r-length-c, offset) + length + c
                 additional_class = 'tickC2'
                 id_specification = 'C2'
-            elif c == self.c3:
-                length = 10
+            elif c == c2:
+                length = 7
                 tick_end_x = self.__sliceToX(0, r+length-c, offset) - length + c
                 tick_end_y = self.__sliceToY(0, r+length-c, offset) - length + c
                 additional_class = 'tickC3'
                 id_specification = 'C3'
             # Draw the tick mark using a line element in SVG
             out += f'''
-                <g class='tick {additional_class}' id='{id}Tick{id_specification}'><line x1="{tick_start_x}" y1="{tick_start_y}" x2="{tick_end_x}" y2="{tick_end_y}" stroke="black" stroke-width="2"/>
+                <g class='tick {additional_class}' id='{id}Tick{id_specification}'><line x1="{tick_start_x}" y1="{tick_start_y}" x2="{tick_end_x}" y2="{tick_end_y}" stroke="black" stroke-width="1"/>
             '''
-            if id_specification == 'C3':
-                text_k = self.c3 + 50
-                # text_offset = offset + int(self.__degreeDiff(self.houses_degree_ut[(i+1)], self.houses_degree_ut[i]) / 6)
-                xtext = self.__sliceToX(0, (r-text_k), offset) + text_k - 5
-                ytext = self.__sliceToY(0, (r-text_k), offset) + text_k + 5
+            # if id_specification == 'C3':
+            #     text_k = self.c3 + 50
+            #     # text_offset = offset + int(self.__degreeDiff(self.houses_degree_ut[(i+1)], self.houses_degree_ut[i]) / 6)
+            #     xtext = self.__sliceToX(0, (r-text_k), offset) + text_k - 5
+            #     ytext = self.__sliceToY(0, (r-text_k), offset) + text_k + 5
                 # out += f'<text x="{xtext}" y="{ytext}" fill="white">9°22\'23\'\'</text>'
             out += '</g>'
         return out
     
     def __makePlanetGrid(self):
         out = '<g transform="translate(500,-20)">'
 
@@ -1556,32 +1548,35 @@
         self.c1 = 0
         self.c2 = 36
         self.c3 = 120
 
         # transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             td['transitRing'] = self.__transitRing(r)
-            td['degreeRing'] = self.__degreeTransitRing(r)
+            # td['degreeRing'] = self.__degreeTransitRing(r)
+            td['degreeRing'] = ''
             # circles
             td['c1'] = 'class="circle" id="c1" cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-36) + '"'
             td['c1style'] = 'fill: none; stroke: %s; stroke-width: 1px; stroke-opacity:.4;' % (
                 self.colors_settings['zodiac_transit_ring_2'])
             td['c2'] = 'class="circle" id="c2" cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-72) + '"'
             td['c2style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_1'])
             td['c3'] = 'class="circle" id="c3" cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-160) + '"'
             td['c3style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-width: 1px' % (
-                self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_0'])
-            td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
-            td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
+                self.colors_settings['paper_2'], self.colors_settings['zodiac_transit_ring_0'])
+            td['makeAspects'] = ''
+            td['makeAspectGrid'] = ''
+            # td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
+            # td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
             td['makePatterns'] = ''
-            td['makeAxis'] = ''
+            td['makeAxis'] = self.__makeAxis(r, (r-self.c1-18))
             td['chart_width'] = self.full_width
         else:
             td['transitRing'] = ""
             if self.chart_type == 'minimal':
                 td['degreeRing'] = ''
             else:
                 td['degreeRing'] = self.__degreeRing(r)
```

### Comparing `py_astrolab-0.6.7/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.8/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.8/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.8/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.8/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.8/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/kr.config.json` & `py_astrolab-0.6.8/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/main.py` & `py_astrolab-0.6.8/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/print_all_data.py` & `py_astrolab-0.6.8/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/relationship_score.py` & `py_astrolab-0.6.8/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/report.py` & `py_astrolab-0.6.8/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/transits.py` & `py_astrolab-0.6.8/py_astrolab/transits.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/types.py` & `py_astrolab-0.6.8/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/py_astrolab/utilities.py` & `py_astrolab-0.6.8/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.6.7/pyproject.toml` & `py_astrolab-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.6.7"
+version = "0.6.8"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.6.7/PKG-INFO` & `py_astrolab-0.6.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

