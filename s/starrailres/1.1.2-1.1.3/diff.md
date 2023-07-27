# Comparing `tmp/starrailres-1.1.2.tar.gz` & `tmp/starrailres-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-1.1.2.tar", max compression
+gzip compressed data, was "starrailres-1.1.3.tar", max compression
```

## Comparing `starrailres-1.1.2.tar` & `starrailres-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.2/LICENSE
--rw-r--r--   0        0        0      499 2023-06-11 14:13:42.567942 starrailres-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.2/README.md
--rw-r--r--   0        0        0       22 2023-06-11 09:13:33.282915 starrailres-1.1.2/starrailres/__init__.py
--rw-r--r--   0        0        0    29710 2023-06-11 12:00:42.241192 starrailres-1.1.2/starrailres/index.py
--rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.2/starrailres/models/avatars.py
--rw-r--r--   0        0        0     1738 2023-06-10 10:42:25.990067 starrailres-1.1.2/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.2/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.2/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.2/starrailres/models/elements.py
--rw-r--r--   0        0        0     2975 2023-06-11 11:59:00.421389 starrailres-1.1.2/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.2/starrailres/models/items.py
--rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.2/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.2/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.2/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.2/starrailres/models/relics.py
--rw-r--r--   0        0        0      323 2023-06-11 09:13:35.175657 starrailres-1.1.2/starrailres/utils.py
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-1.1.3/LICENSE
+-rw-r--r--   0        0        0      499 2023-06-28 06:07:02.429053 starrailres-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-1.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 09:13:33.282915 starrailres-1.1.3/starrailres/__init__.py
+-rw-r--r--   0        0        0    30055 2023-06-28 06:06:22.684740 starrailres-1.1.3/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-1.1.3/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1738 2023-06-10 10:42:25.990067 starrailres-1.1.3/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-1.1.3/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-1.1.3/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-1.1.3/starrailres/models/elements.py
+-rw-r--r--   0        0        0     2975 2023-06-11 11:59:00.421389 starrailres-1.1.3/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-1.1.3/starrailres/models/items.py
+-rw-r--r--   0        0        0      734 2023-05-29 13:34:04.145217 starrailres-1.1.3/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-1.1.3/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-1.1.3/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-1.1.3/starrailres/models/relics.py
+-rw-r--r--   0        0        0      323 2023-06-11 09:13:35.175657 starrailres-1.1.3/starrailres/utils.py
+-rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 starrailres-1.1.3/PKG-INFO
```

### Comparing `starrailres-1.1.2/LICENSE` & `starrailres-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/README.md` & `starrailres-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/starrailres/index.py` & `starrailres-1.1.3/starrailres/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,29 +310,35 @@
             if v >= 4:
                 relic_sets.append(
                     RelicSetInfo(
                         id=k,
                         name=self.relic_sets[k].name,
                         icon=self.relic_sets[k].icon,
                         num=4,
-                        desc=self.relic_sets[k].desc[0],
+                        desc=self.relic_sets[k].desc[1]
+                        if len(self.relic_sets[k].desc) > 1
+                        else "",
                         properties=[
                             PropertyInfo(
                                 type=i.type,
                                 field=self.properties[i.type].field,
                                 name=self.properties[i.type].name,
                                 icon=self.properties[i.type].icon,
                                 value=i.value,
                                 display=self.value_display_format(
                                     i.value,
                                     self.properties[i.type].percent,
                                 ),
                                 percent=self.properties[i.type].percent,
                             )
-                            for i in self.relic_sets[k].properties[1]
+                            for i in (
+                                self.relic_sets[k].properties[1]
+                                if len(self.relic_sets[k].properties) > 1
+                                else []
+                            )
                         ],
                     )
                 )
         return relic_sets
 
     # internal methods
 
@@ -345,28 +351,27 @@
         if id not in self.characters:
             return []
         skill_info_dict = {}
         for skill_level in skill_levels:
             if skill_level.id not in self.character_skills:
                 continue
             skill = self.character_skills[skill_level.id]
+            params = skill.params[skill_level.level - 1] if skill.params else []
             skill_info = SkillInfo(
                 id=skill_level.id,
                 name=skill.name,
                 level=skill_level.level,
                 max_level=skill.max_level,
                 element=self.get_element_info(skill.element),
                 type=skill.type,
                 type_text=skill.type_text,
                 effect=skill.effect,
                 effect_text=skill.effect_text,
                 simple_desc=skill.simple_desc,
-                desc=self.format_template(
-                    skill.desc, skill.params[skill_level.level - 1]
-                ),
+                desc=self.format_template(skill.desc, params),
                 icon=skill.icon,
             )
             skill_info_dict[skill_level.id] = skill_info
         skill_info_list = []
         for skill_id in self.characters[id].skills:
             if skill_id in skill_info_dict:
                 skill_info_list.append(skill_info_dict[skill_id])
@@ -753,14 +758,16 @@
             return f"{math.floor(value)}"
 
     def format_template(self, template: str, params: List[float]) -> str:
         """
         Format string template with params.
         """
         for n in range(1, 11):
+            if len(params) < n:
+                break
             if f"#{n}[i]%" in template:
                 template = template.replace(
                     f"#{n}[i]%", f"{math.floor(params[n-1]*100)}%"
                 )
             if f"#{n}[i]" in template:
                 template = template.replace(f"#{n}[i]", f"{math.floor(params[n-1])}")
             for f in range(1, 5):
```

### Comparing `starrailres-1.1.2/starrailres/models/characters.py` & `starrailres-1.1.3/starrailres/models/characters.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/starrailres/models/info.py` & `starrailres-1.1.3/starrailres/models/info.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/starrailres/models/light_cones.py` & `starrailres-1.1.3/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/starrailres/models/relics.py` & `starrailres-1.1.3/starrailres/models/relics.py`

 * *Files identical despite different names*

### Comparing `starrailres-1.1.2/PKG-INFO` & `starrailres-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailres
-Version: 1.1.2
+Version: 1.1.3
 Summary: StarRailRes index package.
 Home-page: https://github.com/Mar-7th/StarRailRes-Python
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

