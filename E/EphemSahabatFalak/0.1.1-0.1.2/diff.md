# Comparing `tmp/EphemSahabatFalak-0.1.1.tar.gz` & `tmp/EphemSahabatFalak-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.1.1.tar", last modified: Wed Jul 12 02:09:02 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.1.2.tar", last modified: Thu Jul 27 15:49:03 2023, max compression
```

## Comparing `EphemSahabatFalak-0.1.1.tar` & `EphemSahabatFalak-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.870256 EphemSahabatFalak-0.1.1/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.866655 EphemSahabatFalak-0.1.1/EphemSahabatFalak/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)   224320 2023-07-12 01:45:22.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49515 2023-06-24 23:21:37.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49659 2023-06-23 14:51:37.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       82 2023-07-12 01:46:40.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/__init__.py
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.869241 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      420 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       78 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/top_level.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      152 2023-06-25 03:25:43.000000 EphemSahabatFalak-0.1.1/MANIFEST.in
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-12 02:09:02.869926 EphemSahabatFalak-0.1.1/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      876 2023-06-25 03:26:42.000000 EphemSahabatFalak-0.1.1/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-07-12 02:09:02.870396 EphemSahabatFalak-0.1.1/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1302 2023-07-12 02:08:08.000000 EphemSahabatFalak-0.1.1/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-27 15:49:03.508562 EphemSahabatFalak-0.1.2/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-27 15:49:03.506896 EphemSahabatFalak-0.1.2/EphemSahabatFalak/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)   252665 2023-07-27 15:46:41.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49515 2023-06-24 23:21:37.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49659 2023-06-23 14:51:37.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       82 2023-07-12 01:46:40.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak/__init__.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-27 15:49:03.508081 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-27 15:49:03.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      420 2023-07-27 15:49:03.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-07-27 15:49:03.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      100 2023-07-27 15:49:03.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-07-27 15:49:03.000000 EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/top_level.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      152 2023-06-25 03:25:43.000000 EphemSahabatFalak-0.1.2/MANIFEST.in
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-27 15:49:03.508376 EphemSahabatFalak-0.1.2/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      876 2023-06-25 03:26:42.000000 EphemSahabatFalak-0.1.2/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-07-27 15:49:03.508633 EphemSahabatFalak-0.1.2/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1353 2023-07-27 15:44:47.000000 EphemSahabatFalak-0.1.2/setup.py
```

### Comparing `EphemSahabatFalak-0.1.1/EphemSahabatFalak/KiraanWaktuSolat.py` & `EphemSahabatFalak-0.1.2/EphemSahabatFalak/KiraanWaktuSolat.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from skyfield.searchlib import find_discrete
 import pandas as pd
 from mpmath import degrees, acot,cot,sin, atan2, sqrt, cos, radians, atan, acos, tan, asin
 from datetime import timedelta
 from skyfield.framelib import ecliptic_frame
 import numpy as np
 import matplotlib.pyplot as plt
+from matplotlib.pyplot import cm
 from matplotlib.colors import LinearSegmentedColormap
 from timezonefinder import TimezoneFinder
 import geopandas
 from geodatasets import get_path
 
 
 class Takwim:
@@ -179,16 +180,16 @@
 
         if angle_format != 'skylib' and angle_format != 'degree':
             sun_altitude = sun_altitude.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
         
         elif angle_format == 'degree':
             sun_altitude = sun_altitude.degrees
             
-        return sun_altitude
-    
+        return sun_altitude  
+
     def sun_azimuth(self, t = None, angle_format = 'skylib'):
         """
         Returns the azimuth of the Sun.\n
 
         Parameters:\n
         t: (timen
         None -> Defaults to the current time of the class (class.current_time())\n
@@ -264,14 +265,23 @@
         else:
             if unit == 'km' or unit == 'KM':
                 sun_distance = earth.at(t).observe(sun).apparent().distance().km
             else:
                 sun_distance = earth.at(t).observe(sun).apparent().distance()
             return sun_distance 
 
+    def __sun_dec(self,t=None):
+        eph = api.load(self.ephem)
+        eph.segments = eph.segments[:14]
+        earth, sun = eph['earth'], eph['sun']
+        current_topo = earth + self.location()
+
+        s_dec= current_topo.at(t).observe(sun).radec() 
+        sun_declination = s_dec[1]
+        return sun_declination
     
     def moon_altitude(self, t = None, angle_format = 'skylib', temperature = None, pressure = None, topo = 'topo'):
         """
         Returns the altitude of the moon.
 
         Parameters:\n
         t: (time)\n
@@ -742,15 +752,15 @@
                 lag_time =  '-' + str(dt.timedelta() - lag_time)[:7]
             else:
                 lag_time = str(lag_time)[:7]
         else:
             lag_time = lag_time.total_seconds()
         return lag_time
       
-    def waktu_zawal(self, time_format = 'default'):
+    def waktu_istiwa(self, time_format = 'default'):
         eph = api.load(self.ephem)
         eph.segments = eph.segments[:14]
         earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
         
         
         transit_Sun = almanac.meridian_transits(eph, sun, self.location())
@@ -789,15 +799,15 @@
         t1 = ts.from_datetime(next_midnight)
         t, position = almanac.find_discrete(t0,t1,transit_Sun) #find the meridian & anti-meridian
         
         #calculate zuhr. We take 1 minutes and 5 seconds instead of 4 seconds since the angular radius of the
         #sun is more than 16 arcminutes during perihelion
         zuhr = t[position==1]
         zawal_skylibtime = zuhr[0]
-        zohor_datetime = zawal_skylibtime.astimezone(self.zone)+ dt.timedelta(minutes =1, seconds = 5)
+        zohor_datetime = zawal_skylibtime.astimezone(self.zone)+ dt.timedelta(minutes =1, seconds = 6)
         
         if time_format == 'datetime':
             zohor_datetime = zohor_datetime.astimezone(self.zone)
             
         elif time_format == 'string':
             zohor_datetime = str(zohor_datetime.astimezone(self.zone))[11:19]
             
@@ -853,15 +863,15 @@
         
         if altitude == 'default' or altitude == -18:
             twilight_default = almanac.dark_twilight_day(eph, self.location())
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             fajr = t2[event==1]
             subh = fajr[0].astimezone(self.zone)
             
-        elif altitude >= -24 and altitude <= -12 and altitude != -18:
+        elif altitude >= -24 and altitude < -4 and altitude != -18:
             """twilight_default = almanac.dark_twilight_day(eph, self.location())
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             fajr = t2[event==1]
             fajr_time = fajr[0].astimezone(self.zone)
             now = fajr_time - timedelta(minutes=28) #begins iteration 28 minutes before 18 degrees
             end = fajr_time + timedelta(minutes=28) #ends iteration 28 minutes after 18 degrees
             while now<end:
@@ -870,39 +880,39 @@
                 
                 if y0.degrees >= altitude:
                     subh = now
                     break
                 now += timedelta(seconds=1)
                 subh = now"""
             #starts iteration
-            twilight_default = almanac.dark_twilight_day(eph, self.location())
-            t2, event = almanac.find_discrete(t0, t1, twilight_default)
-            fajr = t2[event==1]
-            fajr_time = fajr[0].astimezone(self.zone)
-            now = fajr_time - timedelta(minutes=28) #begins iteration 28 minutes before 18 degrees
-            end = fajr_time + timedelta(minutes=28) #ends iteration 28 minutes after 18 degrees
-            t0 = ts.from_datetime(now)
-            t1 = ts.from_datetime(end)
+            # twilight_default = almanac.dark_twilight_day(eph, self.location())
+            # t2, event = almanac.find_discrete(t0, t1, twilight_default)
+            # fajr = t2[event==1]
+            # fajr_time = fajr[0].astimezone(self.zone)
+            # now = fajr_time - timedelta(minutes=28) #begins iteration 28 minutes before 18 degrees
+            # end = fajr_time + timedelta(minutes=28) #ends iteration 28 minutes after 18 degrees
+            # t0 = ts.from_datetime(now)
+            # t1 = ts.from_datetime(end)
 
 
             subh, nilai = find_discrete(t0, t1, self.__iteration_waktu_subuh)
             subh = subh[0].astimezone(self.zone)
             #ends iteration 
         
         else:
-            subh = str("altitude is below 24 degrees, or above 12 degrees")
+            subh = str("altitude is below -24 degrees, or above -4 degrees")
             
             return subh
             
             
         if time_format == 'datetime':
             subuh = subh
             
         elif time_format == 'string':
-            subuh = str(subh)[11:19]
+            subuh = subh.strftime('%H:%M:%S')
             
         else:
             subuh = ts.from_datetime(subh)
             
                     
         return subuh
     
@@ -1007,15 +1017,15 @@
             syur, nilai = almanac.find_discrete(t0,t1,f)
             syuruk = syur[3].astimezone(self.zone)
 
         if time_format == 'datetime':
             syuruk = syuruk
             
         elif time_format == 'string':
-            syuruk = str(syuruk)[11:19]
+            syuruk = syuruk.strftime('%H:%M:%S')
             
         else:
             syuruk = ts.from_datetime(syuruk)
                     
         return syuruk
     
     def __iteration_waktu_maghrib(self, t=None, alt= 'default'):
@@ -1139,26 +1149,25 @@
             magh, nilai = almanac.find_discrete(t0,t1,f)
             maghrib = magh[4].astimezone(self.zone)
 
         if time_format == 'datetime':
             maghrib = maghrib
             
         elif time_format == 'string':
-            maghrib = str(maghrib)[11:19]
+            maghrib = maghrib.strftime('%H:%M:%S')
 
         elif time_format == 'test':
             maghrib = d, horizon_depression, sun_apparent_radius
             
         else:
             maghrib = ts.from_datetime(maghrib)
                     
         return maghrib
     
     def __iteration_waktu_isya(self, t=None, alt= 'default'):
-
         
         if t is None:
             t = self.current_time()
 
         if alt == 'default':
             alt = self.altitude_isya
             
@@ -1168,15 +1177,14 @@
         return find_when_current_altitude_equals_chosen_altitude < 0
     
     __iteration_waktu_isya.step_days = 1/4
     
     def waktu_isyak(self, altitude = 'default', time_format = 'default'):
         eph = api.load(self.ephem)
         eph.segments = eph.segments[:14]
-        earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
         
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
@@ -1185,15 +1193,15 @@
         
         if altitude == 'default' or altitude == -18:
             twilight_default = almanac.dark_twilight_day(eph, self.location())
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             isya_time = t2[event==0]
             isya = isya_time[0].astimezone(self.zone)
             
-        elif altitude <= -12 and altitude >= -24 and altitude != -18:
+        elif altitude < -4 and altitude >= -24 and altitude != -18:
             """#Legacy version, using while loop.
             twilight_default = almanac.dark_twilight_day(eph, self.location())
             self.temperature = 0
             self.pressure = 0
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             isya_time = t2[event==0]
             isyak = isya_time[0].astimezone(self.zone)
@@ -1205,72 +1213,155 @@
                 
                 if y0.degrees <= altitude:
                     isya = now
                     break
                 now += timedelta(seconds=1)
                 isya = now"""
             #starts iteration
-            transit_time = self.waktu_maghrib()
-            ts = load.timescale()
+            # transit_time = self.waktu_maghrib()
+            # ts = load.timescale()
             
-            twilight_default = almanac.dark_twilight_day(eph, self.location())
+            # twilight_default = almanac.dark_twilight_day(eph, self.location())
             self.temperature = 0
             self.pressure = 0
-            t2, event = almanac.find_discrete(t0, t1, twilight_default)
-            isya_time = t2[event==0]
-            isyak = isya_time[0].astimezone(self.zone)
-
-            now = isyak - timedelta(minutes=28) #begins iteration 28 minutes before astronomical twilight
-            end = isyak + timedelta(minutes=28) #ends iteration 28 minutes after astronomical twilight
-            t0 = ts.from_datetime(now)
-            t1 = ts.from_datetime(end)
+            # t2, event = almanac.find_discrete(t0, t1, twilight_default)
+            # isya_time = t2[event==0]
+            # isyak = isya_time[0].astimezone(self.zone)
+
+            # now = isyak - timedelta(minutes=28) #begins iteration 28 minutes before astronomical twilight
+            # end = isyak + timedelta(minutes=28) #ends iteration 28 minutes after astronomical twilight
+            # t0 = ts.from_datetime(now)
+            # t1 = ts.from_datetime(end)
 
 
             isya, nilai = find_discrete(t0, t1, self.__iteration_waktu_isya)
-            isya = isya[0].astimezone(self.zone)
+            isya = isya[1].astimezone(self.zone)
             #ends iteration 
             
         
                 
         else:
-            isya = str("altitude is above -12 degrees or below 24 degrees")
+            isya = str("altitude is above -4 degrees or below 24 degrees")
             return isya
         
         if time_format == 'datetime':
             isya = isya
             
         elif time_format == 'string':
-            isya = str(isya)[11:19]
+            isya = isya.strftime('%H:%M:%S')
             
         else:
             isya = ts.from_datetime(isya)
                     
         return isya
     
+    def __iteration_tarikh_matahari_istiwa(self, t):
+
+        sun_altitude_at_meridian = self.sun_altitude(t=t)
+
+        return sun_altitude_at_meridian.radians> 1.5693418916
+    
+    __iteration_tarikh_matahari_istiwa.step_days = 1
+
+    def __tarikh_istiwa_2(self, time_format = 'string'):
+        ts = load.timescale()
+        now = self.current_time().astimezone(self.zone)
+        this_year = now.replace(year = self.year, month = 1, day = 1, hour = 0, minute = 0, second = 0, microsecond = 0)
+        next_year = this_year + dt.timedelta(days =366)
+        t0 = ts.from_datetime(this_year)
+        t1 = ts.from_datetime(next_year)
+        
+        tarikh, nilai = find_discrete(t0, t1, self.__iteration_tarikh_matahari_istiwa)
+
+        julat_tarikh = []
+        for tarikh, vi in zip(tarikh, nilai):
+            
+            if time_format == 'datetime':
+                tarikh_istiwa = tarikh.astimezone(self.zone)
+                
+            elif time_format == 'string':
+                tarikh_istiwa = tarikh.astimezone(self.zone).strftime('%Y:%m:%d %H:%M:%S')
+                
+            else:
+                tarikh_istiwa = tarikh
+
+            julat_tarikh.append(tarikh_istiwa)
+        
+        return julat_tarikh
+
+    def __iteration_matahari_istiwa(self, t=None):
+
+        return (abs(self.__sun_dec(t).radians - radians(self.latitude))<0.003)
+    
+    __iteration_matahari_istiwa.step_days = 1
+
+    def tarikh_istiwa(self, time_format = 'string'):
+        """
+        Metod ini memberikan tarikh-tarikh ketika Matahari berada tegak di atas kepala di lokasi yang dipilih. Metod
+        ini hanya akan memberikan nilai bagi kawasan yang berada pada latitud antara sekitar 23.5 Utara dan 23.5 Selatan.\n
+
+        Hasil yang diperoleh adalah sama ada sifar bagi kawasan di luar 23.5 Utara/Selatan, atau 2 tarikh bagi kawasan hampir
+        dengan 23.5 Utara/Selatan, atau 4 tarikh bagi kawasan yang berada di antara 23.3 Utara atau Selatan. \n
+
+        Metod ini melaksanakan hitungan dengan mencari tarikh yang mempunyai selisih deklinasi Matahari dan latitud tempatan
+        kurang daripada 17.18 arka minit.
+
+        """
+        ts = load.timescale()
+        now = self.current_time().astimezone(self.zone)
+        this_year = now.replace(year = self.year, month = 1, day = 1, hour = 0, minute = 0, second = 0, microsecond = 0)
+        next_year = this_year + dt.timedelta(days =366)
+        t0 = ts.from_datetime(this_year)
+        t1 = ts.from_datetime(next_year)
+        
+        tarikh, nilai = find_discrete(t0, t1, self.__iteration_matahari_istiwa)
+
+        julat_tarikh = []
+        for i, vi in zip(tarikh, nilai):
+            
+            if time_format == 'datetime':
+                tarikh_istiwa = i.astimezone(self.zone)
+                
+            elif time_format == 'string':
+                tarikh_istiwa = i.astimezone(self.zone).strftime('%Y-%m-%d')
+
+            elif time_format == 'secret':
+                tarikh_istiwa = i.astimezone(self.zone).strftime('%Y-%m-%d %H:%M:%S')
+                
+            else:
+                tarikh_istiwa = i
+
+            julat_tarikh.append(tarikh_istiwa)
+        
+        return julat_tarikh
+
     def __iteration_waktu_asar(self, t = None):
-        transit_time = self.waktu_zawal()
+        transit_time = self.waktu_istiwa()
         sun_altitude_at_meridian = self.sun_altitude(transit_time).radians
-        sun_altitude_at_asr = degrees(acot(cot(sun_altitude_at_meridian)+1))
+        if 'anafi' in self.kaedah:
+            sun_altitude_at_asr = degrees(acot(cot(sun_altitude_at_meridian)+2))    
+        else:
+            sun_altitude_at_asr = degrees(acot(cot(sun_altitude_at_meridian)+1))
         
         if t is None:
             t = self.current_time()
             current_sun_altitude = self.sun_altitude(t).degrees
-            find_when_current_altitude_equals_asr = abs(current_sun_altitude-sun_altitude_at_asr)
+            find_when_current_altitude_equals_asr = current_sun_altitude-sun_altitude_at_asr
         
         else:
             current_sun_altitude = self.sun_altitude(t).degrees
             find_when_current_altitude_equals_asr = current_sun_altitude-sun_altitude_at_asr
             
         return find_when_current_altitude_equals_asr < 0
         
     __iteration_waktu_asar.step_days = 1/4
-    def waktu_asar(self, time_format = 'default'):
-        transit_time = self.waktu_zawal()
+    def waktu_asar(self, time_format = 'default', kaedah = 'Syafie'):
+        transit_time = self.waktu_istiwa()
         ts = load.timescale()
-        
+        self.kaedah = kaedah
         
         zawal = transit_time.astimezone(self.zone)
         begins = zawal + dt.timedelta(hours = 1) #assuming that asr is more than 1 hour after zawal
         ends = zawal + dt.timedelta(hours =6) #assuming that asr is less than 6 hours after zawal
         t0 = ts.from_datetime(begins)
         t1 = ts.from_datetime(ends)
         
@@ -1281,15 +1372,15 @@
         #finding_asr = self.iteration_waktu_asar()
         #tarikh = str(asar[0].astimezone(self.zone))[:11]
         
         if time_format == 'datetime':
             asar_time  = asar[0].astimezone(self.zone)
             
         elif time_format == 'string':
-            asar_time = str(asar[0].astimezone(self.zone))[11:19]
+            asar_time = asar[0].astimezone(self.zone).strftime('%H:%M:%S')
             
         else:
             asar_time = asar[0]
         
         return asar_time
     
     def azimut_kiblat(self):
@@ -1336,14 +1427,29 @@
         else:
             current_sun_azimut = self.sun_azimuth(t, angle_format='degree')
             difference_azimut = abs(current_sun_azimut - self.azimut_kiblat())
 
         return difference_azimut < 0.3
     __iteration_bayang_searah_kiblat.step_days = 20/86400
     def bayang_searah_kiblat(self, time_format = 'default', objek = 'matahari'): #tambah tolak 0.3 darjah atau 18 arkaminit
+        """
+        Metod ini memberikan waktu mula dan waktu akhir bagi kedudukan objek samawi pilihan dari arah kiblat. Hitungan bagi
+        metod ini mengambil nilai selisih 0.3 darjah dari arah kiblat sebenar. \n
+        
+        Parameter:\n
+        time_format:\n
+        'default' -> waktu dalam format julian date\n
+        'string' -> waktu dalam format hh:mm:ss\n
+
+        objek:\n
+        'matahari'\n
+        'bulan'\n
+        'zuhrah'\n
+        """
+        
         t0 = self.waktu_syuruk()
         t1 = self.waktu_maghrib()
         self.objek = objek
         
         if objek == 'bulan':
             masa, nilai = find_discrete(t0, t0+1, self.__iteration_bayang_searah_kiblat)
         elif objek == 'venus' or objek == 'zuhrah':
@@ -1437,17 +1543,17 @@
 
         efemeris_kiblat = pd.DataFrame(az_objek_list, index=masa_list, columns=['Azimut'])
         filename = '../Efemeris_Kiblat_' + str(self.hour) + '_' + str(self.minute) + '.xlsx'
         if directory == None:
             pass
         else:
             try:
-                efemeris_kiblat_excel = efemeris_kiblat.to_excel(directory)
+                efemeris_kiblat.to_excel(directory)
             except:
-                efemeris_kiblat_excel = efemeris_kiblat.to_excel(filename)
+                efemeris_kiblat.to_excel(filename)
         return efemeris_kiblat
     
     def efemeris_hilal(self, topo = 'topo', directory = None):
         '''Returns a moon-ephemeris for a given date. The ephemeris starts at 1 hour before sunset, and ends at 1 hour after sunset.\n
         The ephemeris contains altitude and azimuth of both the moon and sun, the elongation of moon from the sun, illumination of the moon,
         width of the crescent, azimuth difference DAZ and the altitude difference ARCV.\n
         
@@ -1595,15 +1701,15 @@
         return rounded_up_waktu
     def __round_down(self,waktu):
         rounded_down_waktu = str((waktu).replace(second= 0))[11:16]
         
         return rounded_down_waktu
     
     def takwim_solat_bulanan(self, altitud_subuh ='default', altitud_syuruk ='default', 
-                             altitud_maghrib ='default', altitud_isyak ='default',kaedah_syuruk_maghrib = 'Izzat',
+                             altitud_maghrib ='default', altitud_isyak ='default', kaedah_asar = 'Syafie' ,kaedah_syuruk_maghrib = 'Izzat',
                                saat = 'tidak', directory = None):
         '''
         Returns a monthly prayer timetable. \n
         The timetable contains Subuh, Syuruk, Zohor, Asar, Maghrib and Isyak prayer. \n
         In addition, the timetable contains Bayang Searah Kiblat\n
 
         Parameters:\n
@@ -1642,25 +1748,25 @@
                     self.current_time()
                 except:
                     errormessage = "triggered"
                 
             if errormessage == "triggered":
                 continue
             print('Calculating for day: ' + str(i))
-            if altitud_subuh != 'default' and (altitud_subuh > -12 or altitud_subuh) < -24:
+            if altitud_subuh != 'default' and (altitud_subuh > -4 or altitud_subuh) < -24:
                 raise Exception ("Altitude subuh is below 24 degrees, or above 12 degrees")
 
             if altitud_syuruk != 'default' and (altitud_syuruk > 0 or altitud_subuh) < -4:
                 raise Exception ("Altitude syuruk is below -4 degrees, or above 0 degrees")
 
             if altitud_maghrib != 'default' and (altitud_maghrib > 0 or altitud_maghrib) < -4:
                 raise Exception ("Altitude maghrib is below -4 degrees, or above 0 degrees")
 
-            if altitud_isyak != 'default' and (altitud_isyak > -12 or altitud_isyak < -24):
-                raise Exception ("Altitude isyak is below 24 degrees, or above 12 degrees")
+            if altitud_isyak != 'default' and (altitud_isyak > -4 or altitud_isyak < -24):
+                raise Exception ("Altitude isyak is below -24 degrees, or above -4 degrees")
 
             
             self.day = i
 
             
             #masa
             masa = self.current_time(time_format='string')[:11]
@@ -1706,18 +1812,18 @@
                 zohor.append(self.__round_up(waktu_zohor))
             else:
                 waktu_zohor = self.waktu_zohor(time_format = 'string')
                 zohor.append(waktu_zohor)
 
             #asar
             if saat == 'tidak' or saat == 'no':
-                waktu_asar = self.waktu_asar(time_format='datetime')
+                waktu_asar = self.waktu_asar(time_format='datetime', kaedah = kaedah_asar)
                 asar.append(self.__round_up(waktu_asar))
             else:
-                waktu_asar = self.waktu_asar(time_format = 'string')
+                waktu_asar = self.waktu_asar(time_format = 'string',kaedah = kaedah_asar)
                 asar.append(waktu_asar)
 
             #maghrib
             if saat == 'tidak' or saat == 'no':
                 waktu_maghrib = self.waktu_maghrib(time_format='datetime', altitude=altitud_maghrib, kaedah = kaedah_syuruk_maghrib)
                 maghrib.append(self.__round_up(waktu_maghrib))
             else:
@@ -1745,16 +1851,16 @@
                 takwim_bulanan.to_excel(directory)
             except:
                 takwim_bulanan.to_excel(filename)
         
         return takwim_bulanan
     
     def takwim_solat_bulanan_multipoint(self, altitud_subuh ='default', altitud_syuruk ='default', 
-                             altitud_maghrib ='default', altitud_isyak ='default', saat = 'tidak', kaedah_syuruk_maghrib = 'Izzat',
-                               directory = None, **kwargs):
+                             altitud_maghrib ='default', altitud_isyak ='default', saat = 'tidak',kaedah_asar = 'Syafie',
+                               kaedah_syuruk_maghrib = 'Izzat', directory = None, **kwargs):
         
         tarikh = []
         subuh = []
         bayang_kiblat_mula = []
         bayang_kiblat_tamat = []
         syuruk = []
         zohor = []
@@ -1773,25 +1879,25 @@
                     self.current_time()
                 except:
                     errormessage = "triggered"
                 
             if errormessage == "triggered":
                 continue
             print('Calculating for day: ' + str(i))
-            if altitud_subuh != 'default' and (altitud_subuh > -12 or altitud_subuh) < -24:
+            if altitud_subuh != 'default' and (altitud_subuh > -4 or altitud_subuh) < -24:
                 raise Exception ("Altitude subuh is below 24 degrees, or above 12 degrees")
 
             if altitud_syuruk != 'default' and (altitud_syuruk > 0 or altitud_subuh) < -4:
                 raise Exception ("Altitude syuruk is below -4 degrees, or above 0 degrees")
 
             if altitud_maghrib != 'default' and (altitud_maghrib > 0 or altitud_maghrib) < -4:
                 raise Exception ("Altitude maghrib is below -4 degrees, or above 0 degrees")
 
-            if altitud_isyak != 'default' and (altitud_isyak > -12 or altitud_isyak < -24):
-                raise Exception ("Altitude isyak is below 24 degrees, or above 12 degrees")
+            if altitud_isyak != 'default' and (altitud_isyak > -4 or altitud_isyak < -24):
+                raise Exception ("Altitude isyak is below -24 degrees, or above -4 degrees")
 
             
             self.day = i
 
             #masa
             masa = self.current_time(time_format='string')[:11]
             tarikh.append(masa)
@@ -1818,20 +1924,20 @@
             compare_maghrib = []
             compare_isyak = []
             for __,location in kwargs.items():
                 try:
                     kawasan_pilihan = Takwim(latitude = location[0], longitude= location[1], elevation=location[2], 
                                              day = i, month = self.month,zone = self.zone_string, year = self.year,
                                temperature=self.temperature, pressure = self.pressure, ephem = self.ephem)
-                    waktusubuh = kawasan_pilihan.waktu_subuh(time_format = 'datetime')
-                    waktusyuruk = kawasan_pilihan.waktu_syuruk(time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
+                    waktusubuh = kawasan_pilihan.waktu_subuh(altitude=altitud_subuh, time_format = 'datetime')
+                    waktusyuruk = kawasan_pilihan.waktu_syuruk(altitude = altitud_syuruk,time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
                     waktuzohor = kawasan_pilihan.waktu_zohor(time_format = 'datetime')
-                    waktuasar = kawasan_pilihan.waktu_asar(time_format = 'datetime')
-                    waktumaghrib = kawasan_pilihan.waktu_maghrib(time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
-                    waktuisyak = kawasan_pilihan.waktu_isyak(time_format = 'datetime')
+                    waktuasar = kawasan_pilihan.waktu_asar(time_format = 'datetime',kaedah = kaedah_asar)
+                    waktumaghrib = kawasan_pilihan.waktu_maghrib(altitude = altitud_maghrib, time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
+                    waktuisyak = kawasan_pilihan.waktu_isyak(altitude = altitud_isyak,time_format = 'datetime')
 
                     compare_subuh.append(self.__round_up(waktusubuh))
                     compare_syuruk.append(self.__round_down(waktusyuruk))
                     compare_zohor.append(self.__round_up(waktuzohor))
                     compare_asar.append(self.__round_up(waktuasar))
                     compare_maghrib.append(self.__round_up(waktumaghrib))
                     compare_isyak.append(self.__round_up(waktuisyak))
@@ -1863,24 +1969,265 @@
                 takwim_bulanan.to_excel(directory)
             except:
                 takwim_bulanan.to_excel(filename)
         
         return takwim_bulanan
 
     def takwim_solat_tahunan(self, altitud_subuh ='default', altitud_syuruk ='default', 
-                             altitud_maghrib ='default', altitud_isyak ='default', saat = 'tidak'):
+                             altitud_maghrib ='default', altitud_isyak ='default', saat = 'tidak',directory = None,
+                             kaedah_syuruk_maghrib= 'Izzat', kaedah_asar = 'Syafie'):
         """
         Returns similar timetable as in takwim_solat_bulanan, but for one-year."""
-        for i in range(1,13):
-            self.month = i
-            takwim_tahunan = self.takwim_solat_bulanan( altitud_subuh = altitud_subuh, altitud_syuruk =altitud_syuruk, 
-                             altitud_maghrib =altitud_maghrib, altitud_isyak =altitud_isyak, saat =saat)
-                             
-            return takwim_tahunan
+        tarikh = []
+        subuh = []
+        bayang_kiblat_mula = []
+        bayang_kiblat_tamat = []
+        syuruk = []
+        zohor = []
+        asar = []
+        maghrib = []
+        isyak = []
+        for f in range(1,13):
+            self.month = f
+            print(f'Month: {f}')
+            for i in range (1,32):
+                errormessage = "not triggered"
+                if self.month in [2,4,6,9,11] and i >30:
+                    continue
+                elif self.month == 2 and i > 28:
+                    try:
+                        self.day = i
+                        self.current_time()
+                    except:
+                        errormessage = "triggered"
+                    
+                if errormessage == "triggered":
+                    continue
+                print('Calculating for day: ' + str(i))
+                if altitud_subuh != 'default' and (altitud_subuh > -4 or altitud_subuh) < -24:
+                    raise Exception ("Altitude subuh is below 24 degrees, or above 12 degrees")
+
+                if altitud_syuruk != 'default' and (altitud_syuruk > 0 or altitud_subuh) < -4:
+                    raise Exception ("Altitude syuruk is below -4 degrees, or above 0 degrees")
+
+                if altitud_maghrib != 'default' and (altitud_maghrib > 0 or altitud_maghrib) < -4:
+                    raise Exception ("Altitude maghrib is below -4 degrees, or above 0 degrees")
+
+                if altitud_isyak != 'default' and (altitud_isyak > -4 or altitud_isyak < -24):
+                    raise Exception ("Altitude isyak is below -24 degrees, or above -4 degrees")
+
+                
+                self.day = i
+
+                
+                #masa
+                masa = self.current_time(time_format='string')[:11]
+                tarikh.append(masa)
+
+                if saat == 'tidak' or saat == 'no':
+                    waktu_bayang_searah_kiblat = self.bayang_searah_kiblat(time_format='datetime')
+
+                    try:
+                        bayang_kiblat_mula.append(self.__round_up(waktu_bayang_searah_kiblat[0]))
+                        bayang_kiblat_tamat.append(self.__round_down(waktu_bayang_searah_kiblat[1]))
+                    except TypeError:
+                        bayang_kiblat_mula.append(waktu_bayang_searah_kiblat[0])
+                        bayang_kiblat_tamat.append(waktu_bayang_searah_kiblat[1])
+                
+                else: 
+                    waktu_bayang_searah_kiblat = self.bayang_searah_kiblat(time_format='string')
+                    bayang_kiblat_mula.append(waktu_bayang_searah_kiblat[0])
+                    bayang_kiblat_tamat.append(waktu_bayang_searah_kiblat[1])
+
+
+                #subuh
+                if saat == 'tidak' or saat == 'no':
+                    waktu_subuh = self.waktu_subuh(time_format='datetime', altitude=altitud_subuh)
+                    subuh.append(self.__round_up(waktu_subuh))
+
+                else:
+                    waktu_subuh = self.waktu_subuh(time_format='string', altitude=altitud_subuh)
+                    subuh.append(waktu_subuh)
+
+                #syuruk
+                if saat == 'tidak' or saat == 'no':
+                    waktu_syuruk = self.waktu_syuruk(time_format='datetime', altitude=altitud_syuruk,kaedah = kaedah_syuruk_maghrib)
+                    syuruk.append(self.__round_down(waktu_syuruk))
+                else:
+                    waktu_syuruk = self.waktu_syuruk(time_format = 'string', altitude=altitud_syuruk,kaedah = kaedah_syuruk_maghrib)
+                    syuruk.append(waktu_syuruk)
+                
+                #zohor
+                
+                if saat == 'tidak' or saat == 'no':
+                    waktu_zohor = self.waktu_zohor(time_format='datetime')
+                    zohor.append(self.__round_up(waktu_zohor))
+                else:
+                    waktu_zohor = self.waktu_zohor(time_format = 'string')
+                    zohor.append(waktu_zohor)
+
+                #asar
+                if saat == 'tidak' or saat == 'no':
+                    waktu_asar = self.waktu_asar(time_format='datetime',kaedah = kaedah_asar)
+                    asar.append(self.__round_up(waktu_asar))
+                else:
+                    waktu_asar = self.waktu_asar(time_format = 'string',kaedah = kaedah_asar)
+                    asar.append(waktu_asar)
+
+                #maghrib
+                if saat == 'tidak' or saat == 'no':
+                    waktu_maghrib = self.waktu_maghrib(time_format='datetime', altitude=altitud_maghrib, kaedah = kaedah_syuruk_maghrib)
+                    maghrib.append(self.__round_up(waktu_maghrib))
+                else:
+                    waktu_maghrib = self.waktu_maghrib(time_format='string', altitude=altitud_maghrib, kaedah = kaedah_syuruk_maghrib)
+                    maghrib.append(waktu_maghrib)
+                #isyak
+                if saat == 'tidak' or saat == 'no':
+                    waktu_isyak = self.waktu_isyak(time_format='datetime', altitude=altitud_isyak)
+                    isyak.append(self.__round_up(waktu_isyak))
+                else:
+                    waktu_isyak = self.waktu_isyak(time_format='string', altitude = altitud_isyak)
+                    isyak.append(waktu_isyak)
+
+            
+        takwim_tahunan = pd.DataFrame(list(zip(bayang_kiblat_mula, bayang_kiblat_tamat, 
+                                            subuh, syuruk, zohor, asar, maghrib, isyak)), index = tarikh, 
+                                            columns=["Bayang mula", "Bayang tamat", "Subuh", "Syuruk", "Zohor", "Asar", 
+                                                        "Maghrib", "Isyak"])
+            
+        filename = '../Takwim_Solat_Tahunan' + str(self.year) + '.xlsx'
+        if directory == None:
+            takwim_tahunan.to_excel(filename)
+        else:
+            try:
+                takwim_tahunan.to_excel(directory)
+            except:
+                takwim_tahunan.to_excel(filename)
+        
+        return takwim_tahunan
     
+    def takwim_solat_tahunan_multipoint(self, altitud_subuh ='default', altitud_syuruk ='default', 
+                             altitud_maghrib ='default', altitud_isyak ='default', saat = 'tidak', kaedah_syuruk_maghrib = 'Izzat',
+                               kaedah_asar = 'Syafie',directory = None, **kwargs):
+        tarikh = []
+        subuh = []
+        bayang_kiblat_mula = []
+        bayang_kiblat_tamat = []
+        syuruk = []
+        zohor = []
+        asar = []
+        maghrib = []
+        isyak = []
+        for f in range (1,13):
+            self.month = f
+            print(f'Month: {f}')
+            for i in range (1,32):
+                
+                errormessage = "not triggered"
+                if self.month in [2,4,6,9,11] and i >30:
+                    continue
+                elif self.month == 2 and i > 28:
+                    try:
+                        self.day = i
+                        self.current_time()
+                    except:
+                        errormessage = "triggered"
+                    
+                if errormessage == "triggered":
+                    continue
+                print('Calculating for day: ' + str(i))
+                if altitud_subuh != 'default' and (altitud_subuh > -4 or altitud_subuh) < -24:
+                    raise Exception ("Altitude subuh is below 24 degrees, or above 12 degrees")
+
+                if altitud_syuruk != 'default' and (altitud_syuruk > 0 or altitud_subuh) < -4:
+                    raise Exception ("Altitude syuruk is below -4 degrees, or above 0 degrees")
+
+                if altitud_maghrib != 'default' and (altitud_maghrib > 0 or altitud_maghrib) < -4:
+                    raise Exception ("Altitude maghrib is below -4 degrees, or above 0 degrees")
+
+                if altitud_isyak != 'default' and (altitud_isyak > -4 or altitud_isyak < -24):
+                    raise Exception ("Altitude isyak is below -24 degrees, or above -4 degrees")
+
+                
+                self.day = i
+
+                #masa
+                masa = self.current_time(time_format='string')[:11]
+                tarikh.append(masa)
+
+                if saat == 'tidak' or saat == 'no':
+                    waktu_bayang_searah_kiblat = self.bayang_searah_kiblat(time_format='datetime')
+
+                    try:
+                        bayang_kiblat_mula.append(self.__round_up(waktu_bayang_searah_kiblat[0]))
+                        bayang_kiblat_tamat.append(self.__round_down(waktu_bayang_searah_kiblat[1]))
+                    except TypeError:
+                        bayang_kiblat_mula.append(waktu_bayang_searah_kiblat[0])
+                        bayang_kiblat_tamat.append(waktu_bayang_searah_kiblat[1])
+                
+                else: 
+                    waktu_bayang_searah_kiblat = self.bayang_searah_kiblat(time_format='string')
+                    bayang_kiblat_mula.append(waktu_bayang_searah_kiblat[0])
+                    bayang_kiblat_tamat.append(waktu_bayang_searah_kiblat[1])
+
+                compare_subuh = []
+                compare_syuruk = []
+                compare_zohor = []
+                compare_asar = []
+                compare_maghrib = []
+                compare_isyak = []
+                for __,location in kwargs.items():
+                    try:
+                        kawasan_pilihan = Takwim(latitude = location[0], longitude= location[1], elevation=location[2], 
+                                                day = i, month = self.month,zone = self.zone_string, year = self.year,
+                                temperature=self.temperature, pressure = self.pressure, ephem = self.ephem)
+                        waktusubuh = kawasan_pilihan.waktu_subuh(time_format = 'datetime')
+                        waktusyuruk = kawasan_pilihan.waktu_syuruk(time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
+                        waktuzohor = kawasan_pilihan.waktu_zohor(time_format = 'datetime')
+                        waktuasar = kawasan_pilihan.waktu_asar(time_format = 'datetime',kaedah = kaedah_asar)
+                        waktumaghrib = kawasan_pilihan.waktu_maghrib(time_format = 'datetime', kaedah = kaedah_syuruk_maghrib)
+                        waktuisyak = kawasan_pilihan.waktu_isyak(time_format = 'datetime')
+
+                        compare_subuh.append(self.__round_up(waktusubuh))
+                        compare_syuruk.append(self.__round_down(waktusyuruk))
+                        compare_zohor.append(self.__round_up(waktuzohor))
+                        compare_asar.append(self.__round_up(waktuasar))
+                        compare_maghrib.append(self.__round_up(waktumaghrib))
+                        compare_isyak.append(self.__round_up(waktuisyak))
+                    except Exception as error:
+                        raise f'{error}: Lokasi perlu mempunyai 3 maklumat dalam format berikut (Latitud, Longitud, Ketinggian)'
+                print(f'Waktu Subuh: {compare_subuh}')
+                print(f'Waktu Syuruk: {compare_syuruk}')
+                print(f'Waktu Zohor: {compare_zohor}')
+                print(f'Waktu Asar: {compare_asar}')
+                print(f'Waktu Maghrib: {compare_maghrib}')
+                print(f'Waktu Isyak: {compare_isyak}')
+                subuh.append(max(compare_subuh))
+                syuruk.append(min(compare_syuruk))
+                zohor.append(max(compare_zohor))
+                asar.append(max(compare_asar))
+                maghrib.append(max(compare_maghrib))
+                isyak.append(max(compare_isyak))
+
+            takwim_bulanan = pd.DataFrame(list(zip(bayang_kiblat_mula, bayang_kiblat_tamat, 
+                                                subuh, syuruk, zohor, asar, maghrib, isyak)), index = tarikh, 
+                                                columns=["Bayang mula", "Bayang tamat", "Subuh", "Syuruk", "Zohor", "Asar", 
+                                                            "Maghrib", "Isyak"])
+            
+            filename = '../Takwim_Solat_multipoint_' + str(self.month) + '_' + str(self.year) + '.xlsx'
+            if directory == None:
+                takwim_bulanan.to_excel(filename)
+            else:
+                try:
+                    takwim_bulanan.to_excel(directory)
+                except:
+                    takwim_bulanan.to_excel(filename)
+            
+            return takwim_bulanan
+
     #visibility criterion
     def Yallop_criteria(self, value = 'criteria'):
         maghrib = self.waktu_maghrib()
         maghrib_datetime = maghrib.astimezone(self.zone)
         lag_time = dt.timedelta(days = 4/9 *(self.moon_set() - maghrib))
         best_time = lag_time + maghrib_datetime
         Yallop = Takwim(latitude=self.latitude, longitude=self.longitude, 
@@ -2618,14 +2965,208 @@
         else:
             try:
                 directory = directory
             except:
                 directory = f'../Gambar_Hilal_pada_{self.day}_{self.month}_{self.year}.png'
         fig.savefig(directory)
 
+    def gambar_hilal_composite(self, directory = None, criteria = 'mabims2021', waktu = 'maghrib', detail = False, **kwargs):
+        
+        #Define the positions of moon and sun at sunset
+
+        if waktu == 'syuruk' or waktu == 'pagi':
+            sun_az = self.sun_azimuth(t='syuruk', angle_format='degree')
+            sun_al = self.sun_altitude(t='syuruk', angle_format='degree', pressure = 0)
+            moon_az = self.moon_azimuth(t='syuruk', angle_format='degree')
+            moon_al = self.moon_altitude(t='syuruk', angle_format='degree', pressure = 0)
+            elon_moon_sun = self.elongation_moon_sun(t='maghrib', angle_format='degree')
+
+        else:
+            sun_az = self.sun_azimuth(t='maghrib', angle_format='degree')
+            sun_al = self.sun_altitude(t='maghrib', angle_format='degree', pressure = 0)
+            moon_az = self.moon_azimuth(t='maghrib', angle_format='degree')
+            moon_al = self.moon_altitude(t='maghrib', angle_format='degree', pressure = 0)
+            elon_moon_sun = self.elongation_moon_sun(t='maghrib', angle_format='degree')
+
+        
+        #initiate the plot
+        fig, ax = plt.subplots(figsize=[16, 9])
+
+        #Logic to draw the altitude = 3. Work it out!
+        horizon_dip = float(self.__horizon_dip_refraction_semid())
+        line_a = sun_az
+        line_b = sun_az+8+abs(sun_az-moon_az)
+        x_angle = 6.4*np.sin(np.arccos((3+horizon_dip)/6.4))
+        y_init = sun_az-abs(sun_az-moon_az)-8
+        b_y = line_b - y_init
+        first_min = (line_a-x_angle-y_init)/b_y
+        first_max = 1-(line_b-line_a-x_angle)/b_y
+        ratio_x_y = b_y/abs(moon_al-sun_al)+9
+
+        #plot the 'scatter'
+        ax.scatter(moon_az, moon_al, ratio_x_y*20, c= 'gainsboro',
+                edgecolor='black', linewidth=0.25, zorder=2)
+        ax.scatter(sun_az, sun_al, ratio_x_y*20, c= 'yellow',
+                edgecolor='black', linewidth=0.25, zorder=2)
+        
+        
+        
+        ax.axhline(y=-horizon_dip+0.25, color = 'red', linestyle = '--') #apparent horizon
+
+        #mabims 2021
+        ax.axhline(y=3, color = 'green', linestyle = ':', xmax=first_min) #3 degree. always at 3, not arcv
+        ax.axhline(y=3, color = 'green', linestyle = ':', xmin=first_max)
+
+        theta = np.linspace(np.pi/2-(np.arccos((3+horizon_dip)/6.4)),np.pi/2+(np.arccos((3+horizon_dip)/6.4)), 100)
+        # the radius of the circle
+        r = 6.4
+        # compute x1 and x2
+        x3 = r*np.cos(theta)
+        y3 = r*np.sin(theta)
+        #plot elongation
+        ax.plot(x3+sun_az, y3+sun_al, ':', color = 'green')
+        #Parameter annotate
+        moon_parameter = str(format(elon_moon_sun, '.2f'))
+        moon_age = self.moon_age()
+
+        if waktu == 'syuruk' or waktu == 'pagi':
+            ax.annotate('Jarak Lengkung: ' + moon_parameter, (moon_az, moon_al+1.5), c='black', ha='center', va='center',
+                            textcoords='offset points', xytext=(moon_az, moon_al), size=10)
+            ax.annotate('Umur Bulan: ' + moon_age, (moon_az, moon_al+0.5), c='black', ha='center', va='center',
+                            textcoords='offset points', xytext=(moon_az, moon_al), size=10)
+            moon_parameter_al = str(format(moon_al, '.2f'))
+            ax.annotate('Altitud: ' + moon_parameter_al, (moon_az, moon_al+1), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=(moon_az, moon_al), size=10)
+
+            ax.annotate('Mabims 3-6.4', ((sun_az-abs(sun_az-moon_az)-7), 3.1), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=((sun_az-abs(sun_az-moon_az)-5), 3.1), size=10)
+            ax.annotate('Ufuk Mari\'e - Wujudul Hilal Muhammadiyah', ((sun_az-abs(sun_az-moon_az)-5),-horizon_dip+0.35), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=((sun_az-abs(sun_az-moon_az)), 3.1), size=10)
+            ax.set(
+                aspect=1.0,
+                title='Kedudukan Hilal pada syuruk '+self.waktu_syuruk(time_format = 'string') +' ' + self.convert_julian_from_time() + ' di Lat: ' + str(self.latitude) + 'dan Long: '+ str(self.longitude),
+                xlabel='Azimuth (°)',
+                ylabel='Altitude (°)',
+                xlim=((sun_az-abs(sun_az-moon_az)-8), (sun_az+8+abs(sun_az-moon_az))),
+                ylim=((sun_al-2), (sun_al+abs(moon_al-sun_al)+7))
+                #xticks=np.arange((x2-abs(x2-x)-8), (x2+8+abs(x2-x)),5) ,
+                #yticks = np.arange((y2-2), (y2+abs(y-y2)+8),1)
+                
+            )
+        else:
+            # ax.annotate('Jarak Lengkung: ' + moon_parameter, (moon_az-8, moon_al+1.5), c='black', ha='center', va='center',
+            #             textcoords='offset points', xytext=(moon_az-20, moon_al), size=10)
+            # ax.annotate('Umur Bulan: ' + moon_age, (moon_az-8, moon_al+0.5), c='black', ha='center', va='center',
+            #                 textcoords='offset points', xytext=(moon_az-20, moon_al), size=10)
+            # moon_parameter_al = str(format(moon_al, '.2f'))
+            # ax.annotate('Altitud: ' + moon_parameter_al, (moon_az-8, moon_al+1), c='black', ha='center', va='center',
+            #             textcoords='offset points', xytext=(moon_az-20, moon_al), size=10)
+
+            ax.annotate('Mabims 3-6.4', ((sun_az-abs(sun_az-moon_az)-8), 3.1), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=((sun_az-abs(sun_az-moon_az)-190), 3.1), size=10)
+            ax.annotate('Ufuk Mari\'e - Wujudul Hilal Muhammadiyah', ((sun_az-abs(sun_az-moon_az)-8),-horizon_dip+0.35), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=((sun_az-abs(sun_az-moon_az)-160), 3.1), size=10)
+            ax.set(
+                aspect=1.0,
+                title='Kedudukan Hilal pada maghrib ' + self.waktu_maghrib(time_format='string') +' '+ self.convert_julian_from_time()+' di Lat: ' + str(self.latitude) + ' dan Long: ' + str(self.longitude),
+                xlabel='Azimuth (°)',
+                ylabel='Altitude (°)',
+                xlim=((sun_az-abs(sun_az-moon_az)-8), (sun_az+8+abs(sun_az-moon_az))),
+                ylim=((sun_al-2), (sun_al+abs(moon_al-sun_al)+7)),
+                #xticks=np.arange((x2-abs(x2-x)-8), (x2+8+abs(x2-x)),5) ,
+                #yticks = np.arange((y2-2), (y2+abs(y-y2)+8),1)
+                
+            )
+        
+        if 'stanbul' in criteria:
+            #istanbul 2015
+            x_angle2 = 8*np.sin(np.arccos((5+horizon_dip)/8))
+            y_init = sun_az-abs(sun_az-moon_az)-8
+            b_y = line_b - y_init
+            second_min = (line_a-x_angle2-y_init)/b_y
+            second_max = 1-(line_b-line_a-x_angle2)/b_y
+
+            ax.axhline(y=5, color = 'blue', linestyle = ':', xmax=second_min) #3 degree. always at 3, not arcv
+            ax.axhline(y=5, color = 'blue', linestyle = ':', xmin=second_max)
+            theta2 = np.linspace(np.pi/2-(np.arccos((5+horizon_dip)/8)),np.pi/2+(np.arccos((5+horizon_dip)/8)), 100)
+            # the radius of the circle
+            r2 = 8
+            # compute x1 and x2
+            x4 = r2*np.cos(theta2)
+            y4 = r2*np.sin(theta2)
+            #plot elongation
+            ax.plot(x4+sun_az, y4+sun_al, ':', color = 'blue')
+
+            
+            
+            ax.annotate('Istanbul 5-8', ((sun_az-abs(sun_az-moon_az)-8), 5.1), c='black', ha='center', va='center',
+                        textcoords='offset points', xytext=((sun_az-abs(sun_az-moon_az)-190), 3.1), size=10)
+
+
+        color = iter(cm.rainbow(np.linspace(0, 1, len(kwargs))))
+        for __,location in kwargs.items():
+                try:
+                    kawasan_pilihan = Takwim(latitude = location[0], longitude= location[1], elevation=location[2], 
+                                             day = self.day, month = self.month, year = self.year,
+                               temperature=self.temperature, pressure = self.pressure, ephem = self.ephem)
+                    
+                    #Find moon and sun position
+                    if waktu == 'syuruk' or waktu == 'pagi':
+                        sun_az2 = kawasan_pilihan.sun_azimuth(t='syuruk', angle_format='degree')
+                        sun_al2 = kawasan_pilihan.sun_altitude(t='syuruk', angle_format='degree', pressure = 0)
+                        moon_az2 = kawasan_pilihan.moon_azimuth(t='syuruk', angle_format='degree')
+                        moon_al2 = kawasan_pilihan.moon_altitude(t='syuruk', angle_format='degree', pressure = 0)
+                        elon_moon_sun2 = kawasan_pilihan.elongation_moon_sun(t='syuruk', angle_format='degree')
+
+                    else:
+                        sun_az2 = kawasan_pilihan.sun_azimuth(t='maghrib', angle_format='degree')
+                        sun_al2 = kawasan_pilihan.sun_altitude(t='maghrib', angle_format='degree', pressure = 0)
+                        moon_az2 = kawasan_pilihan.moon_azimuth(t='maghrib', angle_format='degree')
+                        moon_al2 = kawasan_pilihan.moon_altitude(t='maghrib', angle_format='degree', pressure = 0)
+                        elon_moon_sun2 = kawasan_pilihan.elongation_moon_sun(t='maghrib', angle_format='degree')
+
+                    moon_parameter2 = str(format(elon_moon_sun2, '.2f'))
+                    moon_age2 = kawasan_pilihan.moon_age()
+                    #find alt and az differences
+
+                    moon_az_diff = moon_az2 - sun_az2
+                    moon_alt_diff = moon_al2 - sun_al2
+
+                    c = next(color)
+                    ax.scatter(sun_az + moon_az_diff, sun_al + moon_alt_diff, ratio_x_y*20, c= c,
+                                edgecolor='black', linewidth=0.25, zorder=1, alpha = 0.5)
+                    
+                    if detail is True:
+                        ax.annotate('Jarak Lengkung: ' + moon_parameter2, (sun_az + moon_az_diff-8, sun_al + moon_alt_diff+1.5), c='black', ha='center', va='center',
+                                    textcoords='offset points', xytext=(sun_az + moon_az_diff-20, sun_al + moon_alt_diff), size=10)
+                        ax.annotate('Umur Bulan: ' + moon_age2, (sun_az + moon_az_diff-8, sun_al + moon_alt_diff+0.5), c='black', ha='center', va='center',
+                                        textcoords='offset points', xytext=(sun_az + moon_az_diff-20, sun_al + moon_alt_diff), size=10)
+                        moon_parameter_al2 = str(format(sun_al + moon_alt_diff, '.2f'))
+                        ax.annotate('Altitud: ' + moon_parameter_al2, (sun_az + moon_az_diff-8, sun_al + moon_alt_diff+1), c='black', ha='center', va='center',
+                                    textcoords='offset points', xytext=(sun_az + moon_az_diff-20, sun_al + moon_alt_diff), size=10)
+                        # ax.annotate( __, (sun_az + moon_az_diff-8, sun_al + moon_alt_diff+1), c='black', ha='center', va='center',
+                        #             textcoords='offset points', xytext=(sun_az + moon_az_diff-20, sun_al + moon_alt_diff), size=10)
+
+                except Exception as error:
+                    raise f'{error}: Lokasi perlu mempunyai 3 maklumat dalam format berikut (Latitud, Longitud, Ketinggian)'
+
+        sky = LinearSegmentedColormap.from_list('sky', ['white','yellow', 'orange'])
+        extent = ax.get_xlim() + ax.get_ylim()
+        ax.imshow([[0,0], [1,1]], cmap=sky, interpolation='bicubic', extent=extent)
+
+        if directory == None:
+            directory = f'../Gambar_Hilal_pada_{self.day}_{self.month}_{self.year}.png'
+        else:
+            try:
+                directory = directory
+            except:
+                directory = f'../Gambar_Hilal_pada_{self.day}_{self.month}_{self.year}.png'
+        plt.show()
+        fig.savefig(directory)        
+                       
 class Data_Hilal:
     def __init__(self, day,month,year, data = None):
         self.day = day
         self.month = month
         self.year = year
         self.data = data
     
@@ -4543,7 +5084,9 @@
             self.elevation = 945
             self.zon = zon
 
 class Selangor(Takwim):
     def __init__(self, latitude=5.41144, longitude=100.19672,zon =1, elevation=40, year=datetime.now().year, month=datetime.now().month, day=datetime.now().day, hour=datetime.now().hour, minute=datetime.now().minute, second=datetime.now().second, zone=None, temperature=27, pressure=None, ephem='de440s.bsp'):
         super().__init__(latitude, longitude, elevation, year, month, day, hour, minute, second, zone, temperature, pressure, ephem)
 
+
+
```

### Comparing `EphemSahabatFalak-0.1.1/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv` & `EphemSahabatFalak-0.1.2/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.1/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv` & `EphemSahabatFalak-0.1.2/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/PKG-INFO` & `EphemSahabatFalak-0.1.2/EphemSahabatFalak.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 Keywords: falak,solat,hilal,waktu,matahari,bulan,kiblat
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EphemSahabatFalak-0.1.1/PKG-INFO` & `EphemSahabatFalak-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 Keywords: falak,solat,hilal,waktu,matahari,bulan,kiblat
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EphemSahabatFalak-0.1.1/README.md` & `EphemSahabatFalak-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.1/setup.py` & `EphemSahabatFalak-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
     author="cartcosine (izzatzubir)",
     author_email="<cart.cosine.0x@icloud.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     include_package_data = True,
-    install_requires=['skyfield', 'pytz', 'datetime', 'DateTime', 'mpmath', 'pandas', 'timezonefinder', 'matplotlib', 'numpy'],
+    install_requires=['skyfield', 'pytz', 'datetime', 'DateTime', 'mpmath', 'pandas', 'timezonefinder',
+                       'matplotlib', 'numpy', 'geopandas', 'geodatasets'],
     keywords=['falak', 'solat', 'hilal', 'waktu', 'matahari', 'bulan', 'kiblat'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

